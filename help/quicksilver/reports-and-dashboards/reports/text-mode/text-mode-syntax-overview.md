---
product-area: reporting
navigation-topic: text-mode-reporting
title: Resumen de sintaxis de modo de texto
description: Puede utilizar la interfaz de modo de texto para crear vistas, filtros, agrupaciones y peticiones de datos personalizadas más complejos en listas e informes. Con el modo de texto, puede acceder a campos y sus atributos que no están disponibles en la interfaz del modo estándar.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 6279106f56fa0d128e0dd03cd13b63a71d4c2952
workflow-type: tm+mt
source-wordcount: '1865'
ht-degree: 0%

---

# Resumen de sintaxis de modo de texto

Puede utilizar la interfaz de modo de texto para crear vistas, filtros, agrupaciones y peticiones de datos personalizadas más complejos en listas e informes. Con el modo de texto, puede acceder a campos y sus atributos que no están disponibles en la interfaz del modo estándar.

Para obtener información y consideraciones sobre el modo de texto antes de comenzar, consulte [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener una lista completa de todos los campos de los que se puede realizar informes y sus atributos, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener más información sobre la creación de informes con el modo de texto, incluidas clases, vídeos y tutoriales, visite la sección Más información en el sitio de Adobe Experience League.

## Consideraciones sobre la sintaxis del modo de texto

* Debe comprender la sintaxis de Adobe Workfront antes de poder empezar a crear elementos de informes en modo de texto. La sintaxis de Workfront para el modo de texto es única para esta aplicación y tiene características únicas con las que debe estar familiarizado.
* Antes de empezar a usar el modo de texto en los informes, le recomendamos encarecidamente que tome nuestras clases sobre informes avanzados para comprender mejor nuestro lenguaje del modo de texto. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* Puede personalizar vistas, filtros y agrupaciones mediante la interfaz de modo estándar. Sin embargo, puede crear indicadores personalizados solo con el modo de texto.

## Directrices comunes para crear elementos de informes en modo de texto

Las siguientes son directrices comunes al crear cualquier elemento de lista o informe en modo de texto:

* Utilice siempre mayúsculas y minúsculas al hacer referencia a objetos o atributos en la base de datos de Workfront.
* Tenga en cuenta la jerarquía de objetos en Workfront. Existen las siguientes diferencias entre vistas, filtros y agrupaciones:

   * Puede mostrar en una vista un objeto que esté a tres objetos del objeto de informe o lista.
   * No se puede hacer referencia a objetos que estén más de 2 objetos lejos del objeto principal en una agrupación, filtro o petición de datos personalizada.

  **Ejemplo:** Puede mostrar el nombre o el GUID del Propietario del Portfolio en una vista de tareas:


  `valuefield=project:portfolio:ownerID`

  No se puede agrupar, filtrar ni preguntar al Propietario del Portfolio en una vista de tareas:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  En estos ejemplos, el ID de propietario del Portfolio está a tres objetos del objeto de la lista.

  Para obtener información sobre la jerarquía de objetos en Workfront, consulte:

   * [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [Explorador de API](../../../wf-api/general/api-explorer.md)

* Utilice caracteres comodín siempre que sea posible para que los informes y las listas sean más dinámicos y evitar duplicarlos para distintos usuarios y líneas de tiempo similares.

## Descripción general de Camel Case

Cuando se hace referencia a campos de Workfront o a sus atributos en el modo de texto, Workfront requiere que escriba sus nombres en minúscula. En este caso, los campos de un solo nombre se escriben en minúsculas. Los campos compuestos se escriben según el siguiente patrón:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Todos los elementos de informes siguen este patrón de mayúsculas y minúsculas.

Las características de la caja de camello son:

* La primera palabra siempre empieza con una letra minúscula.
* Las siguientes palabras siempre comienzan con una letra mayúscula.
* No hay espacios entre las palabras.

**Ejemplo:** Para hacer referencia a la fecha real de finalización de un proyecto, el nombre del campo que utilizaría al crear elementos de informes de modo de texto es

`actualCompletionDate`

## Sintaxis del modo de texto para varios elementos de informes

Existen las siguientes similitudes entre la sintaxis de los conjuntos de elementos de informes siguientes al crearlos con el modo de texto:

* Las líneas de código y sintaxis son similares para vistas y agrupaciones.

  Para obtener información sobre las líneas clave de los códigos para vistas y agrupaciones al crearlos en modo texto, consulte:

   * [Edición de una vista mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Editar modo de texto en una agrupación](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Las líneas de código y sintaxis son similares para los filtros y las peticiones de datos personalizadas.

  Para obtener más información, consulte:

   * [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Sintaxis para vistas y agrupaciones

Las líneas de código al crear vistas y agrupaciones son similares.

Para obtener información sobre la creación de vistas y agrupaciones, consulte los siguientes artículos:

* [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

La línea de código más importante para una vista o una agrupación es la línea que identifica el objeto al que se hace referencia en la columna de la vista o en la agrupación. Esta línea de código puede comenzar con `valuefield` o `valueexpression` en función de si este campo es una referencia directa a un campo de base de datos de Workfront o un cálculo entre varios campos.

En la tabla siguiente se enumeran las líneas de códigos más comunes de una vista o agrupación:

| Línea de código | Descripción |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifica el objeto al que se hace referencia en la columna de la vista o en la agrupación. Es una referencia directa al objeto al que se hace referencia. |
| `valueexpression` | Identifica el objeto al que se hace referencia en la columna de la vista o en la agrupación. Es un cálculo entre varios campos. |
| `valueformat` | Identifica el formato en el que Workfront devuelve el valor especificado en el campo de valor o en las líneas de expresión de valor. |
| `width` | Identifica el ancho de una columna en píxeles. |
| `stretch` | Identifica qué columnas ocupan espacio adicional que la vista no necesita. |

>[!TIP]
>
>* Aunque las líneas de código de los ejemplos siguientes son similares entre vistas y agrupaciones, recuerde siempre que cada línea de código de una agrupación comienza con el número de agrupación.
>
>  Para agrupar por nombre de proyecto en una lista de proyectos o un informe, utilice la línea siguiente para la agrupación de primer nivel:
>
>  `group.0.valuefield=name`
>  
>* Si edita varias columnas en una vista de la misma columna (como en el caso de las columnas compartidas), recuerde que cada línea de código de cada columna comienza con el número de columna.
>
>  Utilice el siguiente formato para identificar la primera columna de una vista:
>
>  `column.0.valuefield=name`
>  
>  Para obtener información sobre cómo compartir columnas, consulte [Ver: combinar información de varias columnas en una columna compartida](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` información general sobre sintaxis para vistas y agrupaciones

`Valuefield=` es una línea clave de código en vistas y agrupaciones que identifica el objeto al que hace referencia directamente.

La sintaxis para hacer referencia directamente a los campos es idéntica para las agrupaciones y las vistas.

Al hacer referencia a objetos de Workfront mediante una etiqueta, se aplican las siguientes reglas `valuefield` línea:

* Utilice camel case para hacer referencia directamente a los campos.

  **Ejemplo:** Para hacer referencia a la fecha real de finalización de la tarea en una vista de tareas, utilice la línea siguiente:

  `valuefield=actualCompletionDate`

* Utilice mayúsculas y minúsculas y dos puntos para separar campos relacionados entre sí para el mismo objeto.

  **Ejemplo:** Para hacer referencia a la fecha planificada de finalización del proyecto en una vista de tareas, utilice la línea siguiente:

  `valuefield=project:plannedCompletionDate`

  Para obtener información sobre cómo se hacen referencia los objetos entre sí en la base de datos de Workfront, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

* Al hacer referencia a un campo personalizado, utilice el nombre del campo exactamente como aparece en la interfaz.

  **Ejemplo:** Para hacer referencia a un campo personalizado de proyecto denominado Detalles adicionales en una vista de tareas, utilice la línea siguiente:

  `valuefield=project:Additional Details`

#### `Valueexpression` información general sobre sintaxis para vistas y agrupaciones

Puede reemplazar el `valuefield=` línea de código con `valueexpression=` al crear vistas y agrupaciones en modo de texto cuando desea hacer referencia a un cálculo entre 2 o más campos.

>[!TIP]
>
>Aunque puede generar campos calculados que se pueden mostrar en los informes, las vistas calculadas y las agrupaciones son más dinámicas. Las vistas calculadas y las agrupaciones se actualizan con información nueva cada vez que se ejecuta el informe o se muestra una lista.
>
>Para obtener información sobre la creación de columnas calculadas en una vista, consulte [Campos personalizados calculados frente a columnas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Crear una agrupación calculada es similar a crear una columna calculada en una vista.

Al hacer referencia a objetos de Workfront mediante una etiqueta, se aplican las siguientes reglas `valueexpression` línea:

* Utilice camel case para hacer referencia a los campos directamente y encerrar cada campo entre llaves.

  **Ejemplo:** Para mostrar el campo Nombre de tarea en una columna de tarea con `valueexpression`, utilice la línea siguiente:

  `valueexpression={name}`


* Utilice mayúsculas y minúsculas y puntos para separar campos relacionados entre sí.

  **Ejemplo:** Para mostrar el nombre de un proyecto concatenado con el nombre de la tarea en un informe de tareas, utilice las siguientes líneas:

   * En una vista:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * En una agrupación:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Para obtener información sobre cómo se hacen referencia los objetos entre sí en la base de datos de Workfront, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

* Al hacer referencia a un campo personalizado, utilice las siguientes reglas:

   * Utilice el nombre del campo exactamente como aparece en la interfaz.
   * Escriba &quot;DE:&quot; antes del nombre del campo.
   * Escriba el campo entre llaves.
   * Separe los campos relacionados con el objeto por puntos.

  **Ejemplo:** Para mostrar el campo personalizado del proyecto Detalles adicionales en una vista de tareas en una línea de expresión de valor, utilice la línea siguiente:

  `valueexpression={project}.{DE:Additional Details}`

* Puede utilizar un comodín en una `valueexpression` pero no en un `valuefield` línea.

  Para obtener información sobre los caracteres comodín, consulte [Resumen de variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` información general sobre vistas y agrupaciones

La segunda línea de código más importante de una vista o agrupación es la siguiente `valueformat=` línea. Esto indica a Workfront en qué formato debe devolver el valor especificado en la variable `valuefield` o `valueexpression` líneas. Aunque puede utilizar varios formatos para `valueformat` líneas, recomendamos que siempre utilice el siguiente valor al utilizar `valueexpression`:

`valueformat=HTML`

Para obtener información adicional `valueformat` Consulte también los artículos siguientes:

* [Formato de fechas en informes de modo de texto](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Formato de números, moneda y valores de porcentaje en los informes de modo de texto](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` información general sobre vistas

`width=` es la línea de código donde se puede especificar el ancho de cada columna en píxeles. Workfront proporciona una anchura sugerida para cada campo, aunque según el tipo de campo y el formato, puede que desee realizar ajustes.

Debe utilizar el adicional `usewidths=true` línea de código para exigir el ancho especificado para la columna.

**Ejemplo:** Para mostrar una columna con una anchura de 80 píxeles, utilice las líneas siguientes:

`width=80`

`usewidths=true`

#### `stretch` información general sobre vistas

El `stretch` se utiliza para identificar qué columnas ocupan espacio adicional que la vista no necesita. La anchura de la interfaz de usuario del espacio de trabajo de un usuario típico es de unos 850 píxeles. Esto significa que si tiene una vista con cuatro columnas (150 píxeles cada una), esa vista ocupará 600 de 850 píxeles. Hay 250 píxeles adicionales en la interfaz de usuario que se añadirán a las columnas que tengan un porcentaje de ampliación proporcionado.

La ampliación de una columna se impone cuando se utiliza la línea de código adicional: `usewidths=true` para al menos una de las columnas de la vista.

**Ejemplo:** Para indicar que una columna podría utilizar un 70% del espacio vacío en una vista, utilice las líneas siguientes:

`stretch=70`

`usewidths=true`

### Sintaxis para filtros y peticiones de datos personalizadas

La sintaxis para crear filtros es similar a la para crear peticiones de datos personalizadas.

>[!TIP]
>
>Puede crear una petición de datos personalizada generando primero un filtro para la sentencia que desea incluir en la petición de datos. Conecte todas las líneas de código de un filtro con &quot;&amp;&quot; sin ningún espacio entre las líneas, lo que se convertirá en el mensaje personalizado.

Para obtener información sobre la creación de filtros y mensajes personalizados, consulte:

* [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Para obtener información sobre la creación de filtros en modo de texto, consulte [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Puede utilizar los siguientes elementos para crear filtros y mensajes personalizados en modo de texto:

* Una línea de código que hace referencia al objeto de la instrucción de filtro. Utilice mayúsculas y minúsculas para el objeto de filtro.
* Línea de código que hace referencia al objeto de filtro y al modificador del valor del objeto de filtro. Utilice mayúsculas y minúsculas para el objeto de filtro de esta línea.

  >[!TIP]
  >
  >Cuando se hace referencia a rangos, esto requiere 2 líneas de modificador.

* Un conector de instrucciones que conecta varias instrucciones de filtro:

   * Y

     Este es el conector predeterminado entre instrucciones de filtro.

   * O

     >[!TIP]
     >
     >Los conectores de instrucciones distinguen entre mayúsculas y minúsculas y siempre están en mayúsculas. &quot;AND&quot; se puede omitir en el modo de texto.

* Comodines para hacer que los filtros sean más dinámicos y personalizarlos para el momento actual o para el usuario que ha iniciado sesión. Para obtener información sobre los caracteres comodín, consulte [Resumen de variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
