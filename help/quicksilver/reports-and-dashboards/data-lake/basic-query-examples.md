---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Ejemplos de consultas de Data Connect
description: Consultas de ejemplo que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Ejemplos de consultas de Workfront Data Connect

Para ayudarle a utilizar mejor los datos de Workfront Data Connect, esta página contiene consultas de ejemplo básicas que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.

## Consulta de datos personalizados

En este ejemplo se muestra cómo crear una consulta para devolver los datos personalizados en Workfront, como formularios y campos personalizados.

### Escenario

Su organización utiliza un formulario personalizado denominado Integración financiera. El formulario se adjunta a cada proyecto y contiene los campos siguientes:

* **Unidad de negocio**: Campo personalizado que contiene una cadena.
* **ProjectID**: Campo personalizado que contiene una cadena numérica.
* **Nombre de proyecto expandido**: Campo de datos personalizados calculados que concatena los valores de unidad de negocio, identificador de proyecto y el nombre de proyecto nativo de Workfront en una sola cadena.

Debe incluir esta información en la respuesta para una consulta contra Data Connect. Los valores de datos personalizados para un registro del lago de datos se encuentran en una columna denominada `parametervalues`. Esta columna se almacena como un objeto JSON.

### Consulta

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Respuesta

La consulta anterior devuelve los siguientes datos:

* `projectid`: ID de proyecto nativo de Workfront.
* `parametervalues`: una columna que almacena un objeto JSON.
* `name`: nombre nativo del proyecto de Workfront.
* `Business Unit`: un valor de datos personalizados que está incluido en el objeto `parametervalues`.
* `Project ID`: un valor de datos personalizados que está incluido en el objeto `parametervalues`.
* `Expanded Project Name`: un valor de datos personalizados que está incluido en el objeto `parametervalues`.

### Explicación

Al consultar el objeto JSON `parametervalues`, se puede acceder a cada campo de datos personalizado como una columna mediante lo siguiente:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` es el nombre del objeto JSON en la tabla que se está consultando. En el caso de los datos personalizados, siempre será `parametervalues`.
* `<parameter_name>` es la cadena `parametername` que se encuentra en la herramienta de configuración de formularios, aunque no siempre coincide con este valor.

>[!NOTE]
>
>Si el nombre del parámetro se cambia en la herramienta de configuración de formularios de Workfront, se representará como una nueva columna en el objeto JSON. Por lo tanto, se recomienda no cambiar el nombre de una columna una vez que se haya creado en la herramienta de configuración de formularios. Sin embargo, la etiqueta se puede cambiar sin afectar al objeto JSON.
>
>Si la cadena de texto del nombre del parámetro es incorrecta, la columna devolverá un valor NULL, en lugar de un error.

* `<data_type>` convierte el valor devuelto por el objeto JSON en un tipo de datos apropiado para el campo. Si se elige un tipo de datos incompatible para el valor que se devuelve, se producirá un error de no coincidencia de tipos de datos. Los tipos de datos posibles incluyen:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (por ejemplo, `Number(32,4)` devolvería 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` es la etiqueta que crea para cada columna de datos personalizada.

>[!NOTE]
>
>Solo se incluirán en el objeto JSON los parámetros que tengan valores asignados en el formulario. Si un campo de datos personalizados está vacío en el formulario, no aparecerá.

## Tiempo en la consulta de estado

En este ejemplo se muestra cómo medir el tiempo que un proyecto ha invertido en estados asignados anteriormente. Se puede adaptar fácilmente para medir el tiempo de las tareas o los problemas en un estado, o para medir cuánto tiempo se le ha aplicado a un objeto cualquier otro atributo (incluidos los valores de datos personalizados).

### Escenario

El liderazgo de su organización cree que está pasando demasiado tiempo en cada fase del ciclo de vida de su trabajo. Antes de realizar recomendaciones para mejorar el proceso, desea crear una medición de línea de base de la frecuencia con la que cambia el estado de un proyecto con el paso del tiempo y de los días que un proyecto permanece en un estado determinado.

Va a utilizar la vista de datos PROJECTS_EVENT para extraer una lista de cada cambio de estado con respecto al objeto del proyecto. Comparará el nuevo estado con el estado anterior, obtendrá el intervalo de tiempo efectivo para el estado asignado anteriormente y, a continuación, calculará los días empleados en ese estado.

Con este resultado sin procesar del tiempo empleado en cada estado por proyecto, puede empezar a crear visualizaciones o agregar los datos más adelante para generar promedios de duración de estado por estado, tipo de proyecto o época del año. Esta línea de base se utiliza para establecer un punto de referencia que puede medir para satisfacer las expectativas de su liderazgo.

La siguiente consulta utiliza la vista de datos Data Connect PROJECTS_EVENTS para comparar cada evento de cambio de estado del proyecto y mostrar el tiempo en estado.

### Consulta

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Respuesta

La consulta anterior devuelve los siguientes datos:

* `PROJECTID`: el ID del proyecto de Workfront asociado con el evento de cambio de estado.
* `PROJECT_NAME`: nombre del proyecto de Workfront.
* `PREVIOUS_STATUS`: el estado del proyecto inmediatamente antes del cambio.
* `STATUS`: el estado del proyecto después del cambio.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: marca de tiempo del evento de cambio cuando se estableció el estado anterior.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: marca de tiempo del evento de cambio cuando se estableció el valor de estado actualizado.
* `STATUS_DURATION_DAYS`: diferencia (en días) entre la marca de tiempo efectiva final y la marca de tiempo efectiva inicial.

### Explicación

La consulta utiliza las funciones de seguimiento de eventos de cambio de Data Connect.  Determina la fecha en la que se activó un evento que tenía un nuevo valor de estado diferente del evento anterior. 

Examinando la consulta de adentro hacia afuera: 

1. Calcular registros en los que el estado anterior es diferente: 
   * Para cada evento de cambio, utilice la función lag() para identificar el valor anterior de estado. 

2. Filtre solo por los registros que han cambiado: 

   * Seleccione los registros del cálculo en el paso 1, donde el estado anterior != estado actual. 

3. Calcule la marca de tiempo efectiva de inicio/fin y la duración en días: 

   * `<status_begin_effective_timestamp>`: se calcula en el paso 2. 

   * `<status_end_effective_timestamp>`: se calcula según el siguiente (posible cliente). `<status_begin_effective_timestamp>`: mostrar solo el estado si `<status_begin_effective_timestamp>` NO es NULO. 
   * `<status_duration_days>`: diferencia de datos entre `<status_begin_effective_timestamp>` y `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Se recomienda utilizar esta consulta como su propia &quot;Vista&quot; en Power BI o Tableau.  Si desea traer otros campos del `<object>_event view`, una el resultado de esta consulta de nuevo al `<object>_event view`.  Los campos combinados serían los siguientes: <br>
>>Para projects_event: 
>>`From projects_event p`
>>`Join <above query> c on c.projectid = p.projectid  `
>>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
