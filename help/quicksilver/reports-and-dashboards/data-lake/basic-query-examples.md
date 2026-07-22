---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Ejemplos de consultas de Data Connect
description: Consultas de ejemplo que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
ht-degree: 1%

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

La consulta utiliza las funciones de seguimiento de eventos de cambio de Data Connect. Determina la fecha en la que se activó un evento que tenía un nuevo valor de estado diferente del evento anterior. 

Examinando la consulta de adentro hacia afuera: 

1. Calcular registros en los que el estado anterior es diferente: 
   * Para cada evento de cambio, utilice la función lag() para identificar el valor anterior de estado. 

2. Filtre solo por los registros que han cambiado: 

   * Seleccione los registros del cálculo en el paso 1, donde el estado anterior != el estado actual. 

3. Calcule la marca de tiempo efectiva de inicio/fin y la duración en días: 

   * `<status_begin_effective_timestamp>`: se calcula en el paso 2. 

   * `<status_end_effective_timestamp>`: se calcula según el siguiente (posible cliente). `<status_begin_effective_timestamp>`: mostrar solo el estado si `<status_begin_effective_timestamp>` NO es NULO. 
   * `<status_duration_days>`: diferencia de datos entre `<status_begin_effective_timestamp>` y `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Se recomienda usar esta consulta como su propia &quot;vista&quot; en Power BI o Tableau. Si desea traer otros campos de `<object>_event view`, una el resultado de esta consulta de nuevo a `<object>_event view`. Los campos combinados serían los siguientes: <br>
>Para projects_event: 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planning: consulta de tipo de registro único

En este ejemplo se muestra cómo consultar los datos de Workfront Planning para un único tipo de registro almacenado en el lago de datos de Data Connect.

### Escenario

Su organización utiliza Workfront Planning para realizar el seguimiento de campañas. Cada registro de campaña incluye un nombre, un estado, una fecha de inicio, una fecha de finalización y un propietario. Desea extraer una lista de todas las campañas activas y sus detalles clave para utilizarla en un panel.

* Los datos del tipo de registro de planificación se almacenan en la vista PLANNINGRECORD_CURRENT.
* Cada fila representa un único registro y todos los valores de campo se almacenan en una columna JSON denominada FIELD_VALUES.
* El tipo de registro se identifica mediante la columna RECORDTYPEID.
* El espacio de trabajo del registro se identifica mediante la columna WORKSPACEID (o la columna WORKSPACENAME para un filtro legible en lenguaje natural).

### Consulta

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### Respuesta

La consulta anterior devuelve los siguientes datos:

* **recordid**: ID de registro de Planning único para la campaña.
* **campaign_name**: El nombre de la campaña, extraído del objeto JSON FIELD_VALUES.
* **campaign_status**: El estado actual de la campaña.
* **start_date**: la fecha de inicio de la campaña, convertida a un tipo de datos de fecha.
* **end_date**: la fecha de finalización de la campaña, convertida a un tipo de datos de fecha.
* **propietario**: El nombre del usuario o equipo asignado como propietario de la campaña.

### Explicación

Los registros de Planning en Data Connect comparten una sola estructura de tabla independientemente del tipo de registro. La columna RECORDTYPEID se utiliza para asignar el ámbito de la consulta a un tipo de registro específico; en este caso, Campaigns. Reemplace `<your_campaign_record_type_id>` por el identificador del tipo de registro que desea consultar, que se puede encontrar en la configuración del tipo de registro de Workfront Planning o consultando RECORDTYPE_CURRENT.

Los valores de campo se almacenan como un objeto JSON en la columna FIELD_VALUES y se accede a ellos utilizando la misma sintaxis de notación de dos puntos utilizada para los datos de formulario personalizados:

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

Las referencias del nombre de campo deben coincidir exactamente con el nombre de campo definido en la configuración del campo de tipo de registro de Planning, incluidas las mayúsculas, el espaciado y los emoji.

>[!NOTE]
>
>Los ID de tipo de registro de Planning se pueden encontrar en la dirección URL cuando se visualiza un tipo de registro en Workfront Planning. Es la ruta de la dirección URL que comienza con &quot;Rt...&quot;. Los tipos de registro también se pueden encontrar con la siguiente llamada SQL en Data Connect:
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning: consulta de tipos de registros conectados

En este ejemplo se muestra cómo consultar datos en dos tipos de registros conectados de Planning: un tipo de registro principal y un tipo de registro al que está conectado.

### Escenario

Su organización conecta registros de Campaign con registros tácticos en Workfront Planning. Desea producir un informe que muestre cada campaña junto con los detalles clave de sus tácticas asociadas. Específicamente, quieren mostrar el nombre de la táctica, la prioridad estratégica y la asignación de presupuesto para que el liderazgo pueda revisar la actividad de la campaña organizada por táctica.

En Data Connect, las conexiones entre los tipos de registros nativos de Planning se almacenan directamente en la columna FIELD_VALUES_RAW de PLANNINGRECORD_CURRENT. Para un campo de referencia denominado &quot;Tácticas&quot;, el valor es una matriz JSON de objetos de registro conectados, cada uno de los cuales contiene una propiedad id con el RECORDID del registro conectado. Utilice LATERAL FLATTEN de Snowflake para expandir esta matriz en filas y unirla al tipo de registro conectado.

### Consulta

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### Respuesta

La consulta anterior devuelve los siguientes datos:

* **campaign_id**: ID de registro de Planning único para la campaña.
* **campaign_name**: Nombre del registro de campaña.
* **campaign_status**: El estado actual de la campaña.
* **tactic_name**: Nombre del registro táctico conectado.
* **priority_estratégica**: Valor del campo Prioridad estratégica del registro táctico conectado.
* **budget_allocation**: El valor del campo Asignación de presupuesto del registro táctico conectado, convertido en flotante.

### Explicación - KP modificado

Las conexiones entre tipos de registros de Planning nativos se almacenan en una tabla de combinación REFERENCE_CURRENT.  La tabla de combinación REFERENCE_CURRENT se utiliza para las uniones entre RecordType.   Al unir entre RecordType, se debe utilizar el campo TO_RECORDID.

La columna REFERENCE_ID de la vista PLANNINGRECORD contiene una lista de todos los campos REFERENCEID aplicables a ese registro de planificación. Puede acceder al ID utilizando la misma notación JSON como field_value.

```
<reference_ids>:"<reference_name>"::text
```

La vista REFERENCE_CURRENT contiene uno o más registros donde TO_RECORDID apunta a otros campos de `recordId` de planificación en las vistas de PLANNINGRECORD_*.

Para unir otro campo REFERENCE a registros de planificación adicionales, se agregarían a la consulta anterior las vistas REFERENCE_CURRENT y PLANNINGRECORD_* del mismo modo.


## Planning: tipo de registro unido a la consulta de datos del flujo de trabajo de Workfront

En este ejemplo se muestra cómo unir un tipo de registro de Workfront Planning a un objeto de flujo de trabajo de Workfront nativo (en este caso, un proyecto) mediante la función de conexión nativa de Planning, que almacena referencias de objetos externos en la vista REFERENCE_CURRENT.

### Escenario

Su organización conecta registros de Campaign en Workfront Planning a Workfront Projects mediante la función de conexión nativa de Planning. Desea producir un informe combinado que muestre los detalles de la campaña junto con los datos de la ejecución en directo del proyecto vinculado, específicamente el porcentaje completado actual del proyecto, la fecha planificada de finalización y el propietario del proyecto asignado, de modo que los administradores de campaña puedan realizar un seguimiento del progreso de entrega sin salir del contexto de Planning Workspace.

### Consulta

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### Respuesta

La consulta anterior devuelve los siguientes datos:

* **campaign_id**: ID de registro de Planning único para la campaña.
* **campaign_name**: Nombre del registro de campaña.
* **campaign_status**: El estado actual de la campaña, de Planning.
* **linked_project_id**: El identificador de proyecto de Workfront de REFERENCE_CURRENT.TO_EXTERNALID, que identifica el proyecto de Workfront conectado.
* **project_name**: El nombre de proyecto nativo de Workfront de PROJECTS_CURRENT.
* **project_percent_complete**: el valor de porcentaje completado actual del proyecto.
* **project_planning_completion**: La fecha planificada de finalización del proyecto de Workfront vinculado.
* **project_owner_id**: el identificador de usuario de Workfront del propietario del proyecto.
* **nombre_propietario_proyecto**: El nombre para mostrar del propietario del proyecto, resuelto uniéndose a USERS_CURRENT.

### Explicación

Las conexiones de un tipo de registro de Planning a un objeto de flujo de trabajo de Workfront nativo se almacenan en REFERENCE_CURRENT. Cada fila de esta vista representa un vínculo direccional: TO_EXTERNALID contiene el ID. del objeto de Workfront conectado. Las filas que representan conexiones de Workfront se identifican mediante `TO_EXTERNALCONNECTIONNAME = 'workfront'` y un valor TO_EXTERNALOBJECTNAME que corresponde al código de API del tipo de objeto de Workfront; por ejemplo, PROJ for Projects.

La columna REFERENCE_ID de las tablas de PLANNINGRECORD contiene una lista de todos los campos REFERENCEID aplicables a ese registro.  Puede acceder al ID utilizando la misma notación JSON como field_value.\
Un solo REFERENCE_ID en PLANNINGRECORD_CURRENT puede contener uno o más enlaces de referencia en la tabla REFERENCE_CURRENT que enlacen a objetos de un tipo de objeto específico en la tabla de Workfront.

```
<reference_ids>:"<reference_name>"::text
```

Tenga en cuenta que las vistas de Planning (PLANNINGRECORD_CURRENT, REFERENCE_CURRENT) residen en el esquema WORKFRONT.PLANNING, mientras que las vistas nativas de flujo de trabajo de Workfront (PROJECTS_CURRENT, USERS_CURRENT, etc.) residen en el esquema WORKFRONT.WF. Las uniones entre esquemas requieren nombres de tabla completos.

La consulta realiza tres combinaciones:

1. **Planning registra la tabla de referencias:** REFERENCE_CURRENT se unió el `TO_RECORDID = c.RECORDID` para buscar todas las conexiones que se originan de cada registro de Campaign. Los filtros de `TO_EXTERNALCONNECTIONNAME = 'workfront'` y `TO_EXTERNALOBJECTNAME = 'PROJ'` limitan los resultados a filas que representan específicamente conexiones a proyectos de Workfront.
1. **Referencias de tabla a proyectos de Workfront:** TO_EXTERNALID contiene el ID de proyecto nativo de Workfront para el proyecto conectado. Se ha unido directamente a `PROJECTS_CURRENT.projectid` para recuperar los datos del proyecto activo.
1. **Proyectos para usuarios:** Un LEFT JOIN to USERS_CURRENT resuelve la clave externa del identificador de propietario del proyecto en un nombre legible en lenguaje natural. Aquí se utiliza LEFT JOIN para que los proyectos sin propietario asignado se incluyan en los resultados.

>[!NOTE]
>
>Al combinar con tablas externas a Planning, NO utilice el campo TO_RECORDID en la consulta.  No es necesario cuando se unen a tablas externas.
>
>Este patrón se puede aplicar a cualquier objeto de flujo de trabajo de Workfront al que Planning admita la conexión, como Proyectos, Portafolios o Programas, cambiando el filtro TO_EXTERNALOBJECTNAME por el código de API de objeto adecuado (por ejemplo, PUERTO para Portafolios o PRGM para Programas) y uniéndolo a la tabla WORKFRONT.WF correspondiente. Consulte el diccionario de datos de Workfront Data Connect para obtener los nombres de tabla y columna de ID correctos para cada tipo de objeto.

Para unir otro campo REFERENCE a registros externos adicionales, se agregaría a la consulta anterior el mismo patrón de unión a REFERENCE_CURRENT y las vistas de flujo de trabajo de Workfront.

Los valores de registros externos y planificados se pueden unir en la misma consulta uniendo varias veces a la tabla REFERENCE_CURRENT y utilizando el patrón de unión adecuado.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
