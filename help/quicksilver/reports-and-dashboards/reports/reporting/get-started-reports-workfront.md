---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Introducción a los informes en Adobe Workfront
description: Los informes proporcionan visibilidad sobre lo que sucede con los usuarios y el trabajo. Con los informes, puede mostrar información sobre los objetos en Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '3449'
ht-degree: 0%

---

# Introducción a los informes en Adobe Workfront

Los informes proporcionan visibilidad sobre lo que sucede con los usuarios y el trabajo. Con los informes, puede mostrar información sobre los objetos en Adobe Workfront.

Para obtener información sobre cómo comprender los objetos y cómo se pueden registrar en la aplicación Workfront, consulte [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Elementos de informe

Los informes son una combinación de los tres elementos siguientes en Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Vista</td> 
   <td> <li>Define las columnas del informe y qué información puede incluir en cada columna.</li> <li>Para obtener información sobre las vistas, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre las vistas en Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agrupación</td> 
   <td> <li>Clasifica la información según una información común y enumera los resultados del informe en encabezados azules.</li> <li>Para obtener información sobre las agrupaciones, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Información general sobre las agrupaciones en Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <li>Controla la cantidad de información que aparece en un informe.</li> <li>Para obtener información sobre los filtros, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Información general sobre filtros en Adobe Workfront</a>.</li> <li>Para obtener información sobre los modificadores de filtro, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</li> <li>Puede filtrar utilizando caracteres comodín, para que los filtros sean más generales y para que su uso sea más flexible.</li> <li>Para obtener información sobre el uso de caracteres comodín en los filtros, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variables de filtro comodín</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Al seleccionar un filtro, una vista o una agrupación nuevos de una lista, esa selección se conserva aunque cierre la sesión de Workfront o cierre el explorador.

Para obtener información sobre los elementos del informe, consulte el artículo [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Para mejorar los informes, puede añadir los siguientes elementos:

* Un gráfico: una representación visual de los resultados en el informe.\
   Para obtener información sobre los informes de gráficos, consulte el artículo [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Agrupación de matriz: resume la información del informe en un formato de tabla agregado.\
   Para obtener información sobre los informes de matriz, consulte el artículo [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Un mensaje: filtro abierto que se puede personalizar y aplicar de forma diferente cada vez que ejecute el informe.\
   Para obtener información sobre las solicitudes, consulte [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

Al crear un informe, puede modificar cualquiera de estos elementos individualmente en el Creador de informes.

Otra forma de mejorar la relevancia de la información incluida en los informes es aplicar formato condicional a las vistas.\
Para obtener información sobre el uso del formato condicional, consulte [Utilizar el formato condicional en las vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Informes del sistema

Workfront proporciona varios informes del sistema que se cargan en el sistema de forma predeterminada.\
Después de introducir información en su sistema, puede utilizar estos informes para mostrar la información visualmente.

Para obtener información sobre cómo acceder a los informes del sistema, consulte la sección [Uso de los informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md) en el artículo [Uso de los informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Para obtener más información sobre los informes del sistema disponibles, consulte el artículo [Uso de los informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Crear informes

Además de los informes del sistema que proporciona Workfront, puede crear sus propios informes personalizados para satisfacer las necesidades de su organización.

Para crear un informe, puede realizar una de las siguientes acciones:

* Cree un informe desde cero.
* Copie un informe existente.\
   Debe tener al menos permiso Ver para copiar un informe creado por otra persona. Para obtener más información sobre cómo copiar un informe, consulte el artículo [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Para obtener información sobre la creación de informes, consulte el artículo [Información general sobre los informes del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* [Requisitos previos para crear informes](#prerequisites-for-creating-reports)
* [Propiedad de los informes](#report-ownership)
* [Creación de informes en la interfaz del generador](#create-reports-in-the-builder-interface)
* [Crear informes en modo de texto](#create-reports-in-text-mode)

### Requisitos previos para crear informes {#prerequisites-for-creating-reports}

* Debe tener una licencia de Plan para crear sus propios informes.\
   Para obtener información sobre los tipos de licencia de Workfront, consulte el artículo [Información general sobre las licencias de Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

* El administrador de Workfront debe proporcionarle acceso a Editar informes en su nivel de acceso.\
   Para obtener información sobre la concesión de acceso a Editar informes, consulte el artículo [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* El administrador de Workfront debe permitirle acceder a Editar filtros, vistas y grupos en el nivel de acceso.

   Para obtener información sobre la concesión de acceso a Editar filtros, vistas y agrupaciones, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Debe definir un objeto sobre el que desee crear un informe. Los informes son específicos de objeto en Workfront y debe empezar seleccionando un tipo de objeto antes de poder empezar a crear el informe. Solo se pueden crear informes de los objetos disponibles en la interfaz de Workfront.

### Propiedad de los informes {#report-ownership}

Al crear un informe en Workfront, se convierte en el propietario predeterminado del informe, que se muestra en la sección Mis informes . No se puede cambiar el propietario de un informe.

Al copiar un informe, automáticamente se convierte en el propietario del informe copiado.

Para obtener información sobre cómo copiar informes, consulte el artículo [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Puede ver quién es el propietario de un informe comprobando la variable **Introducido por** campo .

![](assets/nwe-entered-by-350x218.png)

### Creación de informes en la interfaz del generador {#create-reports-in-the-builder-interface}

Se recomienda usar primero la interfaz de creación de informes para crear un nuevo informe. La interfaz ofrece un conjunto optimizado de herramientas que le guían a través de la agrupación de elementos para crear el informe que desee. Tiene objetos y campos que puede seleccionar en las listas y agregar a todos los elementos de informes.\
Para obtener más información sobre la creación de informes en la interfaz de creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener una lista de los objetos sobre los que puede crear informes, consulte la [Informar sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) sección del artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Para obtener más información sobre los campos que se pueden mostrar en los informes, consulte el artículo [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Crear informes en modo de texto {#create-reports-in-text-mode}

En ocasiones, es posible que no pueda encontrar ciertos campos en la interfaz del generador, pero estos podrían estar disponibles en la API de .\
Para obtener información sobre los campos disponibles en la API, consulte el artículo [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener información sobre cómo utilizar el Explorador de API, consulte el artículo [Uso del Explorador de API](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>No se puede crear un informe en la interfaz de Workfront sobre los objetos que no están disponibles en el Creador de informes. Sin embargo, puede generar informes sobre los campos asociados con los objetos del Creador de informes si esos campos están disponibles a través de la API. Para ello, debe utilizar la interfaz de modo de texto .

El modo de texto permite crear vistas, filtros, agrupaciones y mensajes más complejos, ya que permite utilizar campos que no están disponibles en la interfaz de modo estándar.

* [Terminología del modo de texto](#text-mode-terminology)
* [Columnas calculadas, formato condicional y otros usos del modo de texto](#calculated-columns-conditional-formatting-and-other-uses-of-text-mode)
* [Ejemplos de modo de texto](#text-mode-samples)

#### Terminología del modo de texto {#text-mode-terminology}

Debe utilizar una sintaxis específica para utilizar la interfaz del modo de texto de Workfront.

Para obtener más información sobre la sintaxis de Workfront para el modo de texto, consulte [Información general sobre la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Columnas calculadas, formato condicional y otros usos del modo de texto {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Fuera de los informes de los campos que no están disponibles en la interfaz del generador, se puede utilizar el modo de texto para mostrar cálculos o comparaciones entre determinados campos.

Para obtener una lista de los usos más comunes del modo de texto en un informe, consulte el artículo [Descripción general de los usos comunes del modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Para obtener información sobre cómo incluir datos personalizados calculados en informes, consulte la sección [Datos personalizados calculados en informes](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para obtener información sobre la comparación de campos en formato condicional, consulte el artículo [Comparar campos con formato condicional](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

También puede hacer referencia a los campos de recopilación utilizando el modo de texto en los informes.\
Para obtener información sobre el uso del modo Texto para mostrar la información de recopilación en un informe, consulte el artículo [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Ejemplos de modo de texto {#text-mode-samples}

Tenemos una biblioteca de muestras de las vistas, filtros y agrupamientos más utilizados que puede crear con el modo de texto.

Para examinar esta biblioteca y utilizar algunos de los ejemplos que ofrecemos, consulte el artículo [Ejemplos de vista, filtro y agrupamiento personalizados](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Las pestañas de un informe

Un informe puede contener varias pestañas cuando se ejecuta el informe en la interfaz.

Para obtener información sobre cómo ejecutar un informe, consulte el artículo [Ejecutar un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

En cada ficha, la información que se incluye en el informe se muestra en formatos ligeramente diferentes. Elija el formato que mejor se adapte a las necesidades de su organización.

Puede convertir cualquier pestaña en la pestaña predeterminada del informe. La ficha predeterminada es la primera ficha que se muestra al hacer clic en el nombre de un informe para abrirlo y es la ficha que se muestra al colocar el informe en un tablero.

Según los elementos que elija en el informe, el informe puede tener las siguientes pestañas:

* [Ficha Detalles](#details-tab)
* [Ficha Resumen](#summary-tab)
* [Ficha Matriz](#matrix-tab)
* [Ficha Gráfico](#chart-tab)
* [Pestaña Solicitudes](#prompts-tab)

### Ficha Detalles {#details-tab}

La ficha Detalles de un informe muestra el objeto de los informes y los atributos que elija para ese objeto en un formulario de lista. Cada informe tiene una pestaña Detalles .

>[!IMPORTANT]
>
>La información de la ficha Detalles puede mostrarse de forma diferente a la ficha Gráfico según la zona horaria.\
>Por ejemplo, un usuario de California completó una tarea a las 21:30 PST del 12 de febrero. Cuando un usuario de Nueva York ve un informe que incluye la finalización de esta tarea, la fecha de finalización real aparece como 13 de febrero en la ficha Detalles porque se completó a las 12:30 am EST el 13 de febrero. Sin embargo, en el gráfico, se incluye en la agrupación del 12 de febrero hasta que se expande el elemento de gráfico.

### Ficha Resumen {#summary-tab}

Los informes que incluyen un grupo tienen una ficha Resumen.

La misma información mostrada en formato de lista en la ficha Detalles se resume y agrega según las agrupaciones de la ficha Resumen del informe.

Para obtener información sobre los agrupamientos, consulte el artículo [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Ficha Matriz {#matrix-tab}

Los informes que incluyen un grupo de matrices tienen una ficha Matriz .

La misma información mostrada en formato de lista en la ficha Detalles se muestra en formato de tabla, agrupada por las agrupaciones en el informe de la ficha Matriz.

Cuando se agrega una agrupación Matrix a un informe, la ficha Resumen se reemplaza por la ficha Matriz.

Para obtener información sobre la creación de un grupo de matriz, consulte el artículo [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Ficha Gráfico {#chart-tab}

Los informes que incluyen un gráfico tienen una ficha Gráfico.

Considere la posibilidad de incluir un gráfico en los informes para que los tableros resulten impactantes para sus ejecutivos. Los gráficos son una forma concisa de mostrar la información en un informe. Puede expandir un elemento de gráfico haciendo clic en él para mostrar los elementos incluidos en ese elemento.

>[!IMPORTANT]
>
>Al hacer clic en un elemento de gráfico, la información expandida puede mostrarse de forma diferente al gráfico en función de la zona horaria.\
>Por ejemplo, un usuario de California completó una tarea a las 21:30 PST del 12 de febrero. Cuando un usuario de Nueva York ve un informe que incluye la finalización de esta tarea, la fecha de finalización real aparece como 13 de febrero tanto en la pestaña Detalles como en los detalles Gráfico porque se completó a las 12:30 am EST el 13 de febrero. Sin embargo, en el gráfico, se incluye en la agrupación del 12 de febrero hasta que se expande el elemento de gráfico.

Para obtener información sobre cómo crear un informe con un gráfico, consulte el artículo [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Pestaña Solicitudes {#prompts-tab}

Los informes que incluyen una solicitud de confirmación tienen una ficha Mensajes .

Una solicitud de confirmación le permite agregar un filtro a un informe cada vez que lo ejecute. Cuando se añade una solicitud al informe, la ficha Mensajes se convierte automáticamente en la ficha predeterminada del informe. No se puede cambiar a otra pestaña.

Para obtener información sobre la creación de solicitudes para un informe, consulte el artículo [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Compartir informes

Después de crear un informe, puede compartirlo con otros usuarios.

Puede compartir un informe con otros usuarios de las siguientes maneras:

* [Asignación de permisos de uso compartido a un informe](#give-sharing-permissions-to-a-report)
* [Programar el envío de informes](#schedule-a-report-delivery)
* [Exportación de los resultados de un informe](#export-the-results-of-a-report)
* [Agregar un informe a un tablero](#add-a-report-to-a-dashboard)

### Asignación de permisos de uso compartido a un informe {#give-sharing-permissions-to-a-report}

Puede otorgar permisos de uso compartido a otro usuario para ver o administrar un informe que cree. Puede otorgar a otro usuario un nivel de permisos igual o inferior al suyo. También puede convertir un informe en público mediante permisos para compartir. Para obtener información sobre cómo compartir un informe, consulte [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Programar el envío de informes {#schedule-a-report-delivery}

Puede programar el envío de un informe. Los usuarios con los que comparta el informe recibirán un correo electrónico con un adjunto de los resultados del informe. El archivo adjunto puede tener los siguientes formatos:

* HTML
* PDF
* Excel
* .TSV

Para obtener información sobre la programación de un envío de informes, consulte el artículo [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Exportación de los resultados de un informe {#export-the-results-of-a-report}

Puede exportar los resultados de un informe a los siguientes formatos de archivo

* PDF
* Excel (formatos .xls y .xlsx)
* Delimitado por tabulaciones

Para obtener información sobre la exportación de los resultados de un informe, consulte el artículo [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Una vez exportado el informe a uno de estos formatos, puede compartirlo con otros usuarios enviándolo por correo electrónico como archivo adjunto o imprimiéndolo.

### Agregar un informe a un tablero {#add-a-report-to-a-dashboard}

Puede agregar un informe a un tablero y compartirlo con otros usuarios. Para obtener información sobre cómo agregar informes a un tablero, consulte el artículo [Agregar un informe a un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Crear calendarios

Si desea mostrar los datos en formato de calendario, puede crear calendarios en lugar de informes.

Para obtener información sobre la creación de calendarios, consulte el artículo .

Para obtener información sobre el uso de los calendarios, consulte el artículo [Información general sobre los informes del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Uso de los informes

Después de crear informes y compartirlos con otros usuarios, puede realizar un seguimiento de la frecuencia con la que utilizan estos informes.\
Para obtener información sobre el uso de los informes, incluida la frecuencia con la que se ven, el usuario y los tableros en los que se muestran, consulte el artículo [Resumen del uso de los informes](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Términos comunes utilizados en referencia a los informes

Los siguientes términos se utilizan en referencia a los informes de Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Término o frase</strong> </th> 
   <th><strong>Definición</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Opciones avanzadas</td> 
   <td> <p>Se refiere al vínculo de la ficha Columnas (vista) del Creador de informes que proporciona la capacidad de hacer lo siguiente:</p> 
    <ul> 
     <li>Establezca el formato de estilo condicional de columna del texto y las imágenes según los criterios que seleccione.</li> 
     <li>Vuelva a habilitar la columna.</li> 
     <li>Dé formato a los valores de la columna .</li> 
    </ul> <p>Por ejemplo, es posible que desee mostrar todas las tareas principales en negrita o que desee mostrar la Fecha de finalización planeada en rojo si la tarea está atrasada.</p> </td> 
  </tr> 
  <tr> 
   <td>Atributo</td> 
   <td> Campo de un objeto definido en la base de datos. Se utiliza en una expresión de modo de texto. <br>Por ejemplo, el campo Estado se muestra como <em>status</em> cuando se utiliza en una expresión de modo de texto. </td> 
  </tr> 
  <tr> 
   <td>Bean o JavaBean</td> 
   <td>Un Bean representa un elemento de programación reutilizable. El término Bean identifica las relaciones entre diferentes objetos en la aplicación Workfront. Es importante estar familiarizado con estas relaciones, ya que intenta mostrar atributos adicionales sobre un objeto que no están disponibles en las herramientas básicas de creación de informes.</td> 
  </tr> 
  <tr> 
   <td>Interfaz o Report Builder del generador</td> 
   <td>La interfaz del Generador es la serie de menús desplegables que contienen campos mostrados en las pestañas Columnas (Ver), Filtro y Agrupación. Proporciona una asignación intuitiva de las relaciones Bean para ayudar a identificar las columnas de una vista, los criterios de un filtro y los atributos comunes de una agrupación.</td> 
  </tr> 
  <tr> 
   <td>Camello</td> 
   <td> <p>Camel Case hace referencia a una forma específica de escribir elementos de programación en atributos de varias palabras de cadena. Cuando se escribe un atributo en Camel Case, la primera letra de la primera palabra aparece en minúsculas, no hay espacio entre las palabras y la primera letra de cualquier palabra posterior está en mayúsculas.</p> <p>Por ejemplo, el grupo de inicio se escribiría como <em>homeGroup</em>, el grupo de recursos sería <em>resourcePool</em>, y la Fecha de inicio real sería <em>actualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Gráfico</td> 
   <td> <p>Una ficha dentro del creador de informes, una ficha de informe, después de guardar el informe, así como un elemento opcional de un informe que le permite agregar un gráfico a cualquier informe. Debe definir un grupo en el informe para poder crear un gráfico.</p> <p>Los siguientes son tipos de gráficos que se pueden agregar a cualquier informe:<br></p> 
    <ul> 
     <li>Columna</li> 
     <li>Barras</li> 
     <li>Circular</li> 
     <li>Línea de</li> 
     <li>Medidor</li> 
     <li>Burbujas</li> 
    </ul> <p>Para obtener más información sobre cómo agregar gráficos a informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Detalles</td> 
   <td>Esta es una de las pestañas de un informe, después de guardarlo. Muestra los resultados del informe, que se muestran en la vista y la agrupación que elija.</td> 
  </tr> 
  <tr> 
   <td>Expresión</td> 
   <td>Una expresión es una fórmula escrita en modo de texto que transmite información que se busca o muestra al utilizar la interfaz del modo de texto. Normalmente es una línea en una instrucción de modo de texto más grande.</td> 
  </tr> 
  <tr> 
   <td>Campos</td> 
   <td> <p>Hace referencia a los atributos de los objetos. Por ejemplo, "Estado" es un campo para Proyecto, Tarea o Problemas. "Administrador de Portfolio" es un campo para el objeto Portfolio.</p> <p>También puede tener campos personalizados que cree y agregue a Forms personalizado.<br>Para obtener información sobre la creación de Forms personalizado, consulte el artículo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Nombre de campo </td> 
   <td>El valor de un atributo que se muestra en una vista, que se utiliza en la condición de un filtro o como elemento común de un grupo. Las opciones de Nombre de campo dependen de la selección Origen de campo.</td> 
  </tr> 
  <tr> 
   <td>Origen de campo </td> 
   <td>El valor de un objeto que se muestra en una vista, que se utiliza en la condición de un filtro o como elemento común de un grupo. Las opciones de Origen de campo dependen del tipo de objeto del elemento de interfaz de usuario que se esté creando. El origen de campo permite hacer referencia a atributos de objetos que no sean el tipo de objeto del elemento de interfaz de usuario.</td> 
  </tr> 
  <tr> 
   <td>Filtro</td> 
   <td>Un elemento de informe principal que determina qué resultados se muestran en el informe.</td> 
  </tr> 
  <tr> 
   <td>Formulario </td> 
   <td>Se utiliza de forma intercambiable con "Formulario personalizado". Los campos y las secciones se agregan a los formularios, que luego se adjuntan a un objeto para ampliar el número de campos que se pueden asociar a un objeto.</td> 
  </tr> 
  <tr> 
   <td>Agrupación </td> 
   <td>Un elemento de informe principal que identifica cómo se organiza una lista de resultados. La agrupación crea barras horizontales en todo el informe para agrupar los resultados por atributos comunes definidos al crearlo. Los grupos se utilizan en los informes de matriz para agregar datos, así como en gráficos, a fin de determinar los ejes de los gráficos.</td> 
  </tr> 
  <tr> 
   <td>Objeto o tipo de objeto</td> 
   <td> Un objeto es un elemento de aplicación de Workfront (por ejemplo, proyecto, tarea, grupo, empresa, filtro). El tipo de objeto se utiliza al crear un nuevo informe, vista, filtro o grupo para identificar qué objeto es el foco del informe. Los informes solo pueden tener un tipo de objeto, que es el objeto principal del informe.<br>Se puede hacer referencia a los objetos principales en el mismo informe.<br>Para obtener más información sobre la jerarquía de objetos, consulte la sección "Explicación de la interdependencia y la jerarquía de objetos" en el artículo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>Pedir datos</td> 
   <td> <p>Un elemento de informe opcional que se puede agregar a un informe cuando necesite ejecutar un filtro diferente antes de cada vez que ejecute el informe.</p> <p>Para obtener información sobre los mensajes, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Modificadores de condición o cualificador</td> 
   <td> <p>Este campo aparece en las siguientes áreas de un informe:</p> 
    <ul> 
     <li>En la ficha Filtro</li> 
     <li>La pantalla Opciones avanzadas de la columna de la ficha Columnas (vista). Al definir un calificador, puede comparar el Nombre de campo con otro campo o valor.</li> 
     <li> En un mensaje personalizado<br>Para obtener información sobre las solicitudes personalizadas, consulte la sección "Creación de un mensaje" en el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</li> 
    </ul> <p>Por ejemplo, al crear un filtro para tareas con una Fecha de finalización planificada de Hoy, debería seleccionar <strong>Igual</strong> en el campo Cualificador y en el campo Fecha de hoy:</p> <p><em>Tarea&gt; Fecha de finalización planeada&gt;Igual&gt; (fecha de hoy)</em> </p> <p>En esta situación, el clasificador es <strong>Igual</strong>.<br>Para obtener más información sobre los calificadores, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Informe </td> 
   <td>Combinación de una vista, un filtro y (a veces) un agrupamiento. El propósito de un informe es mostrar los datos de manera consistente en toda la interfaz, distribuir la información y eliminar la necesidad de ejecutar la misma búsqueda o consulta de forma regular.</td> 
  </tr> 
  <tr> 
   <td>Declaración</td> 
   <td>Consiste en varias expresiones que se agrupan para definir qué información se muestra en un informe al utilizar el modo de texto. Se puede crear una instrucción para una vista, un filtro, un grupo o un mensaje personalizado en un informe.</td> 
  </tr> 
  <tr> 
   <td>Resumen</td> 
   <td>Esta es una de las pestañas de un informe, después de guardarlo. Esta pestaña solo se crea al definir un grupo para el informe. Resume la información en función de la agrupación definida durante la creación del informe y proporciona una visión general rápida de los objetos agregados del informe. No muestra todos los objetos del informe, solo los que se agregan.</td> 
  </tr> 
  <tr> 
   <td>Interfaz de modo de texto</td> 
   <td>Proporciona la capacidad de crear o modificar el código de vistas, filtros, agrupamientos y peticiones de datos personalizados creados originalmente mediante la interfaz del Generador. Se sugiere que los elementos del informe se creen inicialmente a través de la interfaz de Generador y luego se conviertan en el modo Texto después de haberse guardado para simplificar la codificación de las vistas, filtros, agrupamientos o solicitudes avanzados.</td> 
  </tr> 
  <tr> 
   <td>Interfaz de usuario (IU)</td> 
   <td>Se refiere a los componentes o componentes básicos de lo que se muestra en la pantalla de un usuario en un momento determinado.</td> 
  </tr> 
  <tr> 
   <td>Ver (o columnas)</td> 
   <td>Uno de los principales elementos de un informe. Identifica los encabezados de columna que se mostrarán en la lista de un informe.</td> 
  </tr> 
 </tbody> 
</table>
