---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Introducción a los informes
description: Los informes proporcionan visibilidad de lo que está pasando con los usuarios y el trabajo. Con los informes, puede mostrar información sobre los objetos de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: f30bed961b339e20c0693a8b5e485f872375b688
workflow-type: tm+mt
source-wordcount: '3296'
ht-degree: 0%

---

# Introducción a los informes

<!-- Audited: 12/2023 -->

Los informes proporcionan visibilidad de lo que está pasando con los usuarios y el trabajo. Con los informes, puede mostrar información sobre los objetos de Adobe Workfront.

Para obtener información sobre los objetos y cómo se pueden incluir en los informes en la aplicación Workfront, consulte [Descripción general de los objetos Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Elementos de informe

Los informes son una combinación de los tres elementos siguientes en Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ver</td> 
   <td> <li>Define las columnas del informe y qué información puede incluir en cada columna.</li> <li>Para obtener información acerca de las vistas, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre vistas en Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agrupación</td> 
   <td> <li>Clasifica la información en función de un fragmento común de información y enumera los resultados del informe en encabezados.</li> <li>Para obtener información acerca de las agrupaciones, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Información general sobre agrupaciones en Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <li>Controla la cantidad de información que aparece en un informe.</li> <li>Para obtener información acerca de los filtros, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Resumen de filtros</a>.</li> <li>Para obtener información acerca de los modificadores de filtro, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</li> <li>Puede filtrar mediante caracteres comodín para que los filtros sean más generales y les proporcionen más flexibilidad de uso.</li> <li>Para obtener información acerca del uso de caracteres comodín en los filtros, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variables de filtro comodín</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Al seleccionar un nuevo filtro, vista o agrupación de una lista, esa selección se conserva aunque cierre la sesión de Workfront o del explorador.

Para obtener información acerca de los elementos de informe, vea [Elementos de informe: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Para mejorar los informes, puede añadir los siguientes elementos:

* Un gráfico: una representación visual de los resultados del informe.\
  Para obtener información acerca de los informes de gráficos, vea [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* A matrix grouping: resume la información del informe en un formato de tabla agregado.\
  Para obtener información sobre los informes de matriz, consulte [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Una solicitud: un filtro abierto que se puede personalizar y aplicar de forma diferente cada vez que se ejecuta el informe.\
  Para obtener información acerca de las solicitudes, vea [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

Al crear un informe, puede modificar cualquiera de estos elementos de forma individual en Report Builder.

Otra forma de mejorar la relevancia de la información incluida en los informes es aplicar formato condicional a las vistas. Para obtener información acerca del uso del formato condicional, vea [Usar formato condicional en las vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Informes del sistema

Workfront proporciona varios informes del sistema que se cargan en el sistema de forma predeterminada.\
Después de introducir la información en el sistema, puede utilizar estos informes para mostrarla visualmente.

Para obtener más información sobre cómo obtener acceso a los informes del sistema y qué informes del sistema están disponibles, consulte [Usar informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Creación de informes

Además de los informes del sistema que proporciona Workfront, puede crear sus propios informes personalizados para satisfacer las necesidades de su organización.

Para crear un informe, puede realizar una de las siguientes acciones:

* Cree un informe desde cero.
* Copie un informe existente.

  Debe tener al menos permiso de visualización para copiar un informe creado por otra persona. Para obtener más información sobre cómo copiar un informe, vea [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Para obtener información sobre cómo crear informes, consulte [Crear un informe personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Requisitos previos para crear informes {#prerequisites-for-creating-reports}

* Debe tener una licencia de planificación (licencias actuales) o una licencia estándar (nuevas licencias) para crear sus propios informes.

  Para obtener información sobre los tipos de licencia de Workfront, consulte [Resumen de licencias](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) para las licencias actuales y [Resumen de licencias nuevas](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) para las licencias nuevas.

* El administrador de Workfront debe darle acceso a Editar informes en su nivel de acceso.

  Para obtener información acerca de cómo conceder acceso a Editar informes, vea [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* El administrador de Workfront debe darle acceso a Editar filtros, vistas y agrupaciones en su nivel de acceso.

  Para obtener información sobre cómo conceder acceso a Editar filtros, vistas y agrupaciones, vea [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Debe definir un objeto sobre el que desee crear un informe. Los informes son específicos de objetos en Workfront y debe empezar por seleccionar un tipo de objeto antes de poder empezar a crear el informe. Solo puede crear informes sobre los objetos disponibles en la interfaz de Workfront.

### Propiedad del informe {#report-ownership}

Cuando crea un informe en Workfront, se convierte en el propietario predeterminado del informe y se muestra en la sección Mis informes. No se puede cambiar el propietario de un informe.

Al copiar un informe, se convierte automáticamente en el propietario del informe copiado.
Para obtener información sobre cómo copiar informes, consulte [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Puede ver a quién pertenece un informe revisando el campo **Ingresado por**.

![Ingresado por campo](assets/unshimmed-entered-by.png)

### Creación de informes en la interfaz del generador {#create-reports-in-the-builder-interface}

Le recomendamos que utilice primero la interfaz de generación de informes para generar un nuevo informe. La interfaz ofrece un conjunto optimizado de herramientas que le guían a través de la recopilación de elementos para crear el informe que desee. Tiene objetos y campos que puede seleccionar en las listas y añadir a todos los elementos de informes.\
Para obtener más información sobre la creación de informes en la interfaz de generación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener una lista de los objetos sobre los que puede generar informes, consulte la sección [Informar sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects) en el artículo [Información general sobre objetos de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Para obtener más información sobre los campos que se pueden mostrar en los informes, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Creación de informes en modo texto {#create-reports-in-text-mode}

A veces, es posible que no encuentre ciertos campos en la interfaz del generador, pero podrían estar disponibles en la API.\
Para obtener información sobre los campos que están disponibles en la API, consulte el artículo [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener información sobre cómo usar el Explorador de API, consulte el artículo [Uso del Explorador de API](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>En la interfaz de Workfront no se pueden crear informes de objetos que no estén disponibles en Report Builder. Sin embargo, se puede crear informes sobre los campos asociados con los objetos en Report Builder si dichos campos están disponibles a través de la API. Para ello, debe utilizar la interfaz Text Mode.

El modo de texto permite crear vistas, filtros, agrupaciones y peticiones de datos más complejos, lo que permite utilizar campos que no están disponibles en la interfaz del modo estándar.

#### Terminología del modo de texto {#text-mode-terminology}

Debe utilizar una sintaxis específica para utilizar la interfaz de modo de texto de Workfront.

Para obtener más información acerca de la sintaxis de Workfront para el modo de texto, consulte [Descripción general de la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Columnas calculadas, formato condicional y otros usos del modo Texto {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Fuera de los informes sobre campos que no están disponibles en la interfaz del generador, puede utilizar el modo Texto para mostrar cálculos o comparaciones entre determinados campos.

Para obtener una lista de los usos más comunes del modo de texto en un informe, vea [Información general sobre los usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Para obtener información sobre cómo incluir datos personalizados calculados en los informes, consulte [Datos personalizados calculados en los informes](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para obtener información acerca de cómo comparar campos en formato condicional, vea [Comparar campos en formato condicional](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

También puede hacer referencia a los campos de colección mediante el Modo de texto en los informes.\
Para obtener información acerca del uso del modo Texto para mostrar la información de colección en un informe, vea [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Ejemplos de modo de texto {#text-mode-samples}

Tenemos una biblioteca de muestras de las vistas, filtros y agrupaciones más utilizados que puede crear con el modo de texto.

Para examinar esta biblioteca y usar algunos de los ejemplos que ofrecemos, vea el artículo [Ejemplos de vista personalizada, filtro y agrupación: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Las pestañas de un informe

Un informe puede contener varias pestañas cuando se ejecuta en la interfaz de.

Para obtener información acerca de cómo ejecutar un informe, vea el artículo [Ejecutar un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

En cada ficha, la información incluida en el informe se muestra en formatos ligeramente diferentes. Elija el formato que mejor se adapte a las necesidades de su organización.

Puede hacer que cualquier pestaña sea la pestaña predeterminada del informe. La ficha predeterminada es la primera ficha que se muestra al hacer clic en el nombre de un informe para abrirlo y es la ficha que se muestra al colocar el informe en un panel.

### Pestaña Detalles {#details-tab}

La pestaña Detalles de un informe muestra el objeto de los informes y los atributos que elija para ese objeto en forma de lista. Cada informe tiene una pestaña Detalles.

>[!IMPORTANT]
>
>La información de la pestaña Detalles puede mostrarse de forma diferente a la de la pestaña Gráfico en función de la zona horaria.\
>Por ejemplo, un usuario de California completó una tarea a las 21:30 (PST) del 12 de febrero. Cuando un usuario de Nueva York ve un informe que incluye la finalización de esta tarea, la fecha de finalización real se muestra como 13 de febrero tanto en la pestaña Detalles como en los detalles del gráfico porque se completó a las 12:30 h EST del 13 de febrero. Sin embargo, en el gráfico, se incluye en la agrupación del 12 de febrero hasta que expanda el elemento de gráfico.

### Pestaña Resumen {#summary-tab}

Los informes que incluyen una agrupación tienen una pestaña Resumen.

La misma información mostrada en formato de lista en la pestaña Detalles se resume y agrega según las agrupaciones del informe en la pestaña Resumen.

Para obtener información acerca de las agrupaciones, vea [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Pestaña Matriz {#matrix-tab}

Los informes que incluyen una agrupación de matriz tienen una pestaña Matriz.

La misma información mostrada en formato de lista en la ficha Detalles se muestra en formato de tabla, agrupada por las agrupaciones del informe en la ficha Matriz.

Cuando se agrega una agrupación de matriz a un informe, la ficha Resumen se reemplaza por la ficha Matriz.

Para obtener información acerca de cómo crear una agrupación de matriz, vea el artículo [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Pestaña Gráfico {#chart-tab}

Los informes que incluyen un gráfico tienen una pestaña Gráfico.

Considere la posibilidad de incluir un gráfico en los informes para ver paneles impactantes para los ejecutivos. Los gráficos son una forma concisa de mostrar la información de un informe. Puede expandir un elemento de gráfico haciendo clic en él para mostrar los elementos incluidos en ese elemento.

>[!IMPORTANT]
>
>Al hacer clic en un elemento del gráfico, la información expandida puede mostrarse de forma diferente a la del gráfico en función de la zona horaria.\
>Por ejemplo, un usuario de California completó una tarea a las 21:30 (PST) del 12 de febrero. Cuando un usuario de Nueva York ve un informe que incluye la finalización de esta tarea, la fecha de finalización real se muestra como 13 de febrero tanto en la pestaña Detalles como en los detalles del gráfico porque se completó a las 12:30 h EST del 13 de febrero. Sin embargo, en el gráfico, se incluye en la agrupación del 12 de febrero hasta que expanda el elemento de gráfico.

Para obtener información acerca de cómo crear un informe con un gráfico, vea el artículo [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Pestaña Indicadores {#prompts-tab}

Los informes que incluyen una solicitud tienen una ficha Peticiones de datos.

Una solicitud permite agregar un filtro a un informe cada vez que se ejecuta el informe. Cuando se agrega una solicitud al informe, la ficha Indicadores se convierte automáticamente en la ficha predeterminada del informe. No se puede cambiar a otra pestaña.

Para obtener información acerca de cómo generar una solicitud para un informe, vea el artículo [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Compartir informes

Después de crear un informe, puede compartirlo con otros usuarios.

### Conceder permisos de uso compartido a un informe {#give-sharing-permissions-to-a-report}

Puede conceder permisos de uso compartido a otro usuario para Ver o Administrar un informe que cree. Puede otorgar a otro usuario un nivel de permisos igual o inferior al suyo. También puede hacer que un informe sea público usando permisos de uso compartido. Para obtener información sobre cómo compartir un informe, vea [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Programar una entrega de informes {#schedule-a-report-delivery}

Puede programar la entrega de un informe. Los usuarios con los que comparte el informe recibirán un correo electrónico con un archivo adjunto de los resultados del informe. El archivo adjunto puede tener los siguientes formatos:

* HTML
* PDF
* Excel
* .TSV

Para obtener información sobre cómo programar la entrega de un informe, consulte [Resumen de la entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Exportación de los resultados de un informe {#export-the-results-of-a-report}

Puede exportar los resultados de un informe a los siguientes formatos de archivo:

* PDF
* Excel (formatos .xls y .xlsx)
* Delimitado por tabulaciones

Para obtener información acerca de cómo exportar los resultados de un informe, vea [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Una vez exportado el informe a uno de estos formatos, puede compartirlo con otros usuarios enviándolo por correo electrónico como datos adjuntos o imprimiéndolo.

### Agregar un informe a un tablero {#add-a-report-to-a-dashboard}

Puede agregar un informe a un tablero y compartirlo con otros usuarios. Para obtener información acerca de cómo agregar informes a un panel, vea [Agregar un informe a un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Creación de calendarios

Si desea mostrar los datos en formato de calendario, puede crear calendarios en lugar de informes.

Para obtener información acerca de cómo generar y usar calendarios, vea [Resumen de informes de calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Uso del informe

Después de crear informes y compartirlos con otros usuarios, puede realizar un seguimiento de la frecuencia con la que los usan.
Para obtener información sobre el uso de los informes, incluida la frecuencia con la que se visualizan, el usuario y los paneles en los que se muestran, consulte el artículo [Resumen del uso de los informes](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

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
   <td> <p>Hace referencia al vínculo en la ficha Columnas (Ver) de Report Builder, que permite realizar las siguientes acciones:</p> 
    <ul> 
     <li>Establezca el formato de estilo condicional de columna de texto e imágenes en función de los criterios que seleccione.</li> 
     <li>Vuelva a etiquetar la columna.</li> 
     <li>Dé formato a los valores de la columna.</li> 
    </ul> <p>Por ejemplo, es posible que desee mostrar todas las tareas principales en negrita o que desee mostrar la Fecha planificada de finalización en rojo si la tarea está atrasada.</p> </td> 
  </tr> 
  <tr> 
   <td>Atributo</td> 
   <td> Campo de un objeto tal como se define en la base de datos. Se utiliza en una expresión Text Mode. <br>Por ejemplo, el campo Estado se muestra como <em>estado</em> cuando se usa en una expresión de modo de texto. </td> 
  </tr> 
  <tr> 
   <td>Bean o JavaBean</td> 
   <td>Bean representa un elemento de programación reutilizable. El término Bean identifica las relaciones entre diferentes objetos de la aplicación de Workfront. Es importante familiarizarse con estas relaciones a medida que intenta mostrar atributos adicionales acerca de un objeto que no están disponibles en las herramientas básicas de creación de informes.</td> 
  </tr> 
  <tr> 
   <td>Interfaz de generador o Report Builder</td> 
   <td>La interfaz del generador es la serie de menús desplegables que contienen campos mostrados en las pestañas Columnas (Ver), Filtro y Agrupación. Proporciona una asignación intuitiva de las relaciones de Bean para ayudar a identificar las columnas de una vista, los criterios de un filtro y los atributos comunes de una agrupación.</td> 
  </tr> 
  <tr> 
   <td>Camel Case</td> 
   <td> <p>Camel Case hace referencia a una forma específica de escribir elementos de programación para encadenar atributos de varias palabras. Cuando se escribe un atributo en Mayúsculas y minúsculas, la primera letra de la primera palabra es minúscula, no hay espacio entre las palabras y la primera letra de cualquier palabra posterior es mayúscula.</p> <p>Por ejemplo, el grupo de inicio se escribiría como <em>homeGroup</em>, el conjunto de recursos sería <em>resourcePool</em> y la fecha de inicio real sería <em>actualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Gráfico</td> 
   <td> <p>Una pestaña dentro de Report Builder, una pestaña de informe, después de guardar el informe, así como un elemento opcional de un informe que le permite agregar un gráfico a cualquier informe. Debe definir una agrupación en el informe antes de crear un gráfico.</p> <p>Los siguientes son tipos de gráficos que se pueden agregar a cualquier informe:<br></p> 
    <ul> 
     <li>Columna</li> 
     <li>Barra</li> 
     <li>Circular</li> 
     <li>Línea de</li> 
     <li>Medidor</li> 
     <li>Burbujas</li> 
    </ul> <p>Para obtener más información sobre cómo agregar gráficos a los informes, vea el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Detalles</td> 
   <td>Esta es una de las pestañas de un informe, después de guardarlo. Muestra las conclusiones del informe, que aparecen en la vista y la agrupación que elija.</td> 
  </tr> 
  <tr> 
   <td>Expresión</td> 
   <td>Una expresión es una fórmula escrita en modo texto para transmitir información que se debe buscar o mostrar al utilizar la interfaz de modo texto. Suele ser una línea en una instrucción Text Mode más grande.</td> 
  </tr> 
  <tr> 
   <td>Campos</td> 
   <td> <p>Se refiere a los atributos de los objetos. Por ejemplo, "Estado" es un campo para Proyectos, Tareas o Problemas. "Administrador de Portfolio" es un campo para el objeto de Portfolio.</p> <p>También puede tener campos personalizados que cree usted mismo y agregue a los formularios personalizados.<br>Para obtener información acerca de cómo crear formularios personalizados, vea el artículo <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Diseñar un formulario con el diseñador de formularios</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Nombre de campo </td> 
   <td>El valor de un atributo que se muestra en una vista, o que se utiliza en la condición de un filtro, o como el elemento común de una agrupación. Las opciones del Nombre de campo dependen de la selección del Campo Source.</td> 
  </tr> 
  <tr> 
   <td>Origen de campo </td> 
   <td>El valor de un objeto que se muestra en una vista, o que se utiliza en la condición de filtro, o como elemento común de una agrupación. Las opciones de Field Source dependen del tipo de objeto del elemento de interfaz de usuario que se crea. El Source de campo permite hacer referencia a atributos de objetos que no sean el tipo de objeto del elemento de interfaz de usuario.</td> 
  </tr> 
  <tr> 
   <td>Filtro</td> 
   <td>Elemento de informe principal que determina qué resultados se muestran en el informe.</td> 
  </tr> 
  <tr> 
   <td>Formulario </td> 
   <td>Se utiliza indistintamente con "Formulario personalizado". Los campos y las secciones se agregan a los formularios, que luego se adjuntan a un objeto para ampliar el número de campos que puede asociar a un objeto.</td> 
  </tr> 
  <tr> 
   <td>Agrupación </td> 
   <td>Elemento de informe principal que identifica cómo se organiza una lista de resultados. La agrupación crea barras horizontales en todo el informe para agrupar los resultados por atributos comunes definidos al crearlo. Las agrupaciones se utilizan en los informes de matriz para acumular datos y en los gráficos para determinar los ejes de los gráficos.</td> 
  </tr> 
  <tr> 
   <td>Objeto u Tipo de objeto</td> 
   <td> Un objeto es un elemento de aplicación de Workfront (por ejemplo, proyecto, tarea, grupo, compañía, filtro). El tipo de objeto se utiliza al crear un nuevo informe, vista, filtro o agrupación para identificar qué objeto es el enfoque del informe. Los informes solo pueden tener un tipo de objeto, que es el objeto principal del informe.Se puede hacer referencia a <br>objetos principales en el mismo informe.<br>Para obtener más información acerca de la jerarquía de objetos, vea la sección "Explicación de la interdependencia y la jerarquía de objetos" en el artículo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Descripción general de los objetos de Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>Solicitud</td> 
   <td> <p>Elemento de informe opcional que se puede agregar a un informe cuando necesite utilizar un filtro diferente cada vez que ejecute el informe.</p> <p>Para obtener información acerca de las solicitudes, vea <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Agregar una solicitud a un informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Modificadores de cualificador o condición</td> 
   <td> <p>Este campo aparece en las siguientes áreas de un informe:</p> 
    <ul> 
     <li>En la pestaña Filtro</li> 
     <li>La pantalla Opciones avanzadas de la columna de la pestaña Columnas (Ver). Al definir un cualificador, puede comparar el Nombre de campo con otro campo o valor.</li> 
     <li> En un indicador personalizado<br><p>Para obtener información acerca de las solicitudes, vea <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Agregar una solicitud a un informe</a>.</p>.</li> 
    </ul> <p>Por ejemplo, al generar un filtro para tareas con una Fecha planificada de finalización de hoy, debe seleccionar <strong>Igual</strong> en el campo Calificador y la fecha de hoy en el campo Fecha:</p> <p><em>Tarea&gt; Fecha planificada de finalización&gt;Igual&gt;(fecha de hoy)</em> </p> <p>En este escenario, el calificador es <strong>Igual</strong>.<br>Para obtener más información acerca de los calificadores, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Informe </td> 
   <td>La combinación de una vista, un filtro y (a veces) una agrupación. El propósito de un informe es mostrar los datos de forma coherente en toda la interfaz, distribuir la información y eliminar la necesidad de ejecutar la misma búsqueda o consulta de forma regular.</td> 
  </tr> 
  <tr> 
   <td>Declaración</td> 
   <td>Consta de varias expresiones que se agrupan para definir qué información se muestra en un informe al utilizar el modo Texto. Se puede crear una instrucción para una vista, filtro, agrupación o para una petición de datos personalizada en un informe.</td> 
  </tr> 
  <tr> 
   <td>Resumen</td> 
   <td>Esta es una de las pestañas de un informe, después de guardarlo. Esta pestaña solo se crea al definir una agrupación para el informe. Resume la información en función de la agrupación definida durante la creación del informe y ofrece una visión general rápida de los objetos agregados del informe. No muestra todos los objetos del informe, solo los que se agregan.</td> 
  </tr> 
  <tr> 
   <td>Interfaz de modo de texto</td> 
   <td>Proporciona la capacidad de crear o modificar el código de vistas, filtros, agrupaciones y peticiones de datos personalizados creados originalmente mediante la interfaz de generación. Se recomienda que los elementos de informe se creen inicialmente mediante la interfaz de Generador y luego se conviertan al modo de texto después de haberlos guardado para simplificar la codificación de las vistas avanzadas, los filtros, las agrupaciones o las peticiones de datos.</td> 
  </tr> 
  <tr> 
   <td>Interfaz de usuario (IU)</td> 
   <td>Se refiere a los componentes o componentes básicos de lo que se muestra en la pantalla de un usuario en un momento determinado.</td> 
  </tr> 
  <tr> 
   <td>Ver (o columnas)</td> 
   <td>Uno de los elementos principales de un informe. Identifica los encabezados de columna que se mostrarán en la lista de un informe.</td> 
  </tr> 
 </tbody> 
</table>
