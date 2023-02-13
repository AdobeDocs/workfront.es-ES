---
product-area: reporting
navigation-topic: text-mode-reporting
title: Información general sobre la sintaxis del modo de texto
description: Puede utilizar la interfaz del modo de texto para crear vistas, filtros, agrupaciones y mensajes personalizados más complejos en listas e informes. Mediante el modo de texto, puede acceder a los campos y sus atributos que no están disponibles en la interfaz de modo estándar.
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# Información general sobre la sintaxis del modo de texto

Puede utilizar la interfaz del modo de texto para crear vistas, filtros, agrupaciones y mensajes personalizados más complejos en listas e informes. Mediante el modo de texto, puede acceder a los campos y sus atributos que no están disponibles en la interfaz de modo estándar.

Para obtener información y consideraciones sobre el modo de texto antes de empezar, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener una lista completa de todos nuestros campos informables y sus atributos, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

## Consideraciones sobre la sintaxis del modo de texto

* Debe comprender la sintaxis de Adobe Workfront para poder empezar a crear elementos de informes en modo de texto. La sintaxis de Workfront para el modo de texto es única para esta aplicación y tiene características únicas con las que debe estar familiarizado.
* Antes de empezar a utilizar el modo de texto en los informes, le recomendamos encarecidamente que tome nuestras clases en informes avanzados para comprender mejor nuestro idioma del modo de texto. Para obtener material de capacitación sobre la presentación de informes, consulte [Rutas de aprendizaje de informes y paneles de Workfront](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* Puede personalizar vistas, filtros y agrupaciones mediante la interfaz de modo estándar. Sin embargo, puede crear mensajes personalizados solo mediante el modo de texto.

## Directrices comunes para crear elementos de informes en modo de texto

Las siguientes son directrices comunes cuando se crea cualquier informe o elemento de lista en modo de texto:

* Utilice siempre mayúsculas y minúsculas para hacer referencia a objetos o atributos en la base de datos de Workfront.
* Tenga en cuenta la jerarquía de objetos en Workfront. Existen las siguientes diferencias entre vistas, filtros y agrupaciones:

   * Puede mostrar un objeto que esté a tres objetos del informe o del objeto de lista en una vista.
   * No se puede hacer referencia a objetos que estén a más de 2 objetos del objeto principal en una agrupación, filtro o solicitud personalizada.

   **Ejemplo:** Puede mostrar el nombre o el GUID del propietario del Portfolio en una vista de tareas:

   ```
   valuefield=project:portfolio:ownerID
   ```

   No se puede agrupar, filtrar ni solicitar el propietario del Portfolio en una vista de tareas:

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   En estos ejemplos, el ID de propietario del Portfolio está a tres objetos del objeto de la lista.

   Para obtener información sobre la jerarquía de objetos en Workfront, consulte:

   * [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [Explorador de API](../../../wf-api/general/api-explorer.md)


* Utilice caracteres comodín siempre que sea posible para que los informes y listas sean más dinámicos y evite duplicarlos para distintos usuarios y líneas de tiempo similares.

## Información general del caso de camello

Al hacer referencia a campos Workfront o a sus atributos en modo de texto, Workfront requiere que escriba sus nombres en mayúsculas. En este caso, los campos de nombre único se escriben en minúsculas. Los campos compuestos se escriben según el siguiente patrón:

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>Todos los elementos de informes siguen este patrón de mayúsculas y minúsculas.

Las características del maletín de camello son:

* La primera palabra siempre comienza con una letra en minúscula.
* Las siguientes palabras siempre comienzan con una letra en mayúsculas.
* No hay espacios entre las palabras.

**Ejemplo:** Para hacer referencia a la fecha de finalización real de un proyecto, el nombre del campo que utilizaría al crear elementos de informes del modo de texto es

```
actualCompletionDate
```

.

## Sintaxis del modo de texto para varios elementos de informes

Las siguientes similitudes existen entre la sintaxis de los conjuntos de elementos de informes siguientes, al crearlos con el modo de texto:

* Las líneas de código y sintaxis son similares para vistas y agrupaciones.

   Para obtener información sobre las líneas clave de los códigos para vistas y agrupaciones al crearlos en modo de texto, consulte:

   * [Edición de una vista mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Editar el modo de texto en una agrupación](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Las líneas de código y sintaxis son similares para filtros y mensajes personalizados.

   Para obtener más información, consulte:

   * [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Sintaxis para vistas y agrupaciones

Puede observar que las líneas de código al crear vistas y agrupaciones son similares.

Para obtener información sobre la creación de vistas y agrupaciones, consulte los siguientes artículos:

* [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

La línea de código más importante para una vista o una agrupación es la línea que identifica el objeto al que se hace referencia en la columna de la vista o en la agrupación. Dependiendo de si este campo es una referencia directa a un campo de base de datos de Workfront o un cálculo entre varios campos, la línea de código puede comenzar con

```
valuefield
```

o

```
valueexpression
```

.

* [Información general sobre la sintaxis de los campos de valor para vistas y agrupaciones](#valuefield-syntax-overview-for-views-and-groupings)
* [Información general sobre la sintaxis de las expresiones de valor para vistas y agrupaciones](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* Aunque las líneas de código de los ejemplos siguientes son similares entre vistas y agrupaciones, recuerde siempre que cada línea de código de una agrupación comienza con el número de agrupación.
>
>  Para agrupar por nombre de proyecto en una lista o informe de proyecto, utilice la línea siguiente para la agrupación de primer nivel:
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

descripción general de sintaxis para vistas y agrupaciones {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

es una línea de código clave en vistas y agrupaciones que identifica el objeto al que hace referencia directamente.

La sintaxis para la referencia directa a campos es idéntica para agrupaciones y vistas.

Las siguientes reglas se aplican al hacer referencia a objetos Workfront mediante una

```
valuefield
```

línea:

* Utilice mayúsculas y minúsculas para hacer referencia a los campos directamente.

   **Ejemplo:** Para hacer referencia a la Fecha de Finalización Real de la Tarea en una vista de tareas, utilice la siguiente línea:

   ```
   valuefield=actualCompletionDate
   ```

* Utilice mayúsculas y minúsculas y dos puntos para separar los campos relacionados entre sí para el mismo objeto.

   **Ejemplo:** Para hacer referencia a la Fecha de Finalización Planificada del Proyecto en una vista de tareas, utilice la siguiente línea:

   ```
   valuefield=project:plannedCompletionDate
   ```

   Para obtener información sobre cómo los objetos se hacen referencia entre sí en la base de datos de Workfront, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

* Al hacer referencia a un campo personalizado, utilice el nombre del campo exactamente como aparece en la interfaz.

   **Ejemplo:** Para hacer referencia a un campo personalizado de proyecto etiquetado como Detalles adicionales en una vista de tareas, utilice la línea siguiente:

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

descripción general de sintaxis para vistas y agrupaciones {#valueexpression-syntax-overview-for-views-and-groupings}

Puede reemplazar la variable

```
valuefield=
```

línea de código con

```
valueexpression=
```

cuando se generan vistas y agrupaciones en modo de texto cuando se desea hacer referencia a un cálculo entre 2 o más campos.

>[!TIP]
>
>Aunque puede crear campos calculados que puede mostrar en los informes, las vistas calculadas y las agrupaciones son más dinámicas. Las vistas y agrupaciones calculadas se actualizan con nueva información cada vez que ejecuta el informe o muestra una lista.
>
>Para obtener información sobre la creación de columnas calculadas en una vista, consulte [Campos personalizados calculados vs. columnas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

La creación de una agrupación calculada es similar a la creación de una columna calculada en una vista.

Las siguientes reglas se aplican al hacer referencia a objetos Workfront mediante una

```
valueexpression
```

línea:

* Utilice mayúsculas y minúsculas para hacer referencia a los campos directamente y encierre cada campo entre llaves.

   **Ejemplo:** Visualización del campo Nombre de tarea en una columna de tarea mediante

   ```
   valueexpression
   ```

   , utilice la siguiente línea:

   ```
   valueexpression={name}
   ```

* Utilice mayúsculas y minúsculas y puntos para separar campos relacionados entre sí.

   **Ejemplo:** Para mostrar el nombre de un proyecto concatenado con el nombre de la tarea en un informe de tareas, utilice las siguientes líneas:

   * En una vista:

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * En una agrupación:

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   Para obtener información sobre cómo los objetos se hacen referencia entre sí en la base de datos de Workfront, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

* Al hacer referencia a un campo personalizado, utilice las siguientes reglas:

   * Utilice el nombre del campo exactamente como aparece en la interfaz.
   * Precediera el nombre del campo con &quot;DE:&quot;.
   * Rellene el campo entre llaves.
   * Separe los campos relacionados con el objeto por puntos.

   **Ejemplo:** Para mostrar el campo personalizado del proyecto Detalles adicionales en una vista de tarea en una línea de expresión de valor, utilice la siguiente línea:

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* Puede utilizar un comodín en una

   ```
   valueexpression
   ```

   pero no en un

   ```
   valuefield
   ```

   línea.

   Para obtener información sobre los comodines, consulte [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

información general

La segunda línea de código más importante de una vista o agrupación es la

```
valueformat=
```

línea. Esto indica a Workfront en qué formato devolver el valor especificado en la variable

```
valuefield
```

o líneas de expresión de valor. Aunque puede usar varios formatos para la variable

```
valueformat
```

líneas, se recomienda utilizar siempre el siguiente valor al utilizar

```
valueexpression
```

:

```
valueformat=HTML
```

### Sintaxis para filtros y mensajes personalizados

La sintaxis para crear filtros es similar a la utilizada para crear mensajes personalizados.

>[!TIP]
>
>Puede crear una solicitud personalizada generando primero un filtro para la instrucción que desea incluir en la solicitud. Conecte todas las líneas de código de un filtro mediante &quot;&amp;&quot; sin espacios entre las líneas y que se convierte en su mensaje personalizado.

Para obtener información sobre la creación de filtros y mensajes personalizados, consulte:

* [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Para obtener información sobre la creación de filtros en el modo de texto, consulte [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Puede utilizar los siguientes elementos para crear filtros y mensajes personalizados en el modo de texto:

* Una línea de código que hace referencia al objeto de la instrucción filter. Utilice mayúsculas y minúsculas para el objeto de filtro.
* Línea de código que hace referencia al objeto de filtro y al modificador del valor del objeto de filtro. Utilice mayúsculas y minúsculas para el objeto de filtro de esta línea.

   >[!TIP]
   >
   >Al hacer referencia a intervalos, esto requiere 2 líneas modificadoras.

* Conector de instrucciones que conecta varias instrucciones de filtro:

   * Y

      Este es el conector predeterminado entre instrucciones de filtro.

   * O

      >[!TIP]
      >
      >Los conectores de instrucciones distinguen entre mayúsculas y minúsculas. Se puede omitir &quot;AND&quot; en el modo de texto.

* Comodín para hacer los filtros más dinámicos y personalizarlos para la hora actual o para el usuario que ha iniciado sesión. Para obtener información sobre los comodines, consulte [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
