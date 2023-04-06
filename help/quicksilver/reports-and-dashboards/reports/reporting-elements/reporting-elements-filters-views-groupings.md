---
product-area: reporting
navigation-topic: reporting-elements
title: '''Elementos de informes: filtros, vistas y agrupaciones'
description: Los elementos principales que debe tener cada lista e informe en Workfront son un filtro, una vista y una agrupación. Cada elemento proporciona información diferente dentro de cualquier informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Elementos de informes: filtros, vistas y agrupaciones

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Existen varios elementos que hacen posible una lista o un informe en Adobe Workfront. Los elementos principales que debe tener cada lista e informe son un filtro, una vista y una agrupación. Cada elemento proporciona información diferente dentro de cualquier informe.

## Consideraciones sobre los elementos de informes

Tenga en cuenta lo siguiente cuando trabaje con filtros, vistas y agrupaciones:

* Los elementos de informes funcionan como componentes básicos de los informes. Definen el aspecto de un informe o una lista, así como la información que contiene el informe o la lista.
* Los informes de Workfront son específicos de un objeto. Debe definir el objeto principal de un informe para poder crearlo. Por lo tanto, todos los elementos de informes son específicos del objeto.
* El administrador de Workfront debe otorgarle acceso a filtros, vistas y agrupaciones en el nivel de acceso para poder visualizarlos o editarlos en listas e informes.

   Para obtener información sobre la concesión de acceso a filtros, vistas y agrupaciones, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* El administrador de Workfront debe permitirle acceder a informes, tableros y calendarios en el nivel de acceso para poder ver o editar informes.

   Para obtener información sobre la concesión de acceso a informes, tableros y calendarios, consulte [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Si selecciona un filtro, una vista o una agrupación en un informe o lista, Workfront conserva esta selección para las listas de ese objeto incluso después de cerrar la sesión o cerrar el explorador. Por ejemplo, si selecciona una vista específica para un informe de tareas, aparecerá esa selección para otras listas de tareas, como la lista de tareas de un proyecto.

## Filtros

El filtro controla los resultados que aparecen en un informe, generalmente reduciendo los resultados de general a específico. Funciona como un tamiz que solo toma la información que necesita y trae esa información de vuelta al informe.

Por ejemplo, si solo desea ver las tareas asignadas al usuario que ha iniciado sesión, puede crear un filtro llamado &quot;Mis tareas&quot;, definir los criterios que deben cumplirse para el filtro y ejecutar el informe para ver solo las tareas asignadas al usuario que ha iniciado sesión.

Algunos atributos de los filtros son:

* Workfront proporciona varios filtros para varios objetos de forma predeterminada.
* Puede personalizar los filtros que posee o administra.

   Para obtener más información sobre los filtros, consulte el artículo [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![Icono de filtro](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## Vistas

Al definir la vista de un informe, se define qué información se incluye en él. Al igual que todos los elementos de informes, las vistas se basan en un tipo de objeto.\
Por ejemplo, una vista para un informe de tareas podría mostrar Fechas de Vencimiento, incluir detalles financieros clave como Coste, o utilizarse para mostrar Detalles de Asignaciones y Fecha de Entrega. Las vistas se pueden utilizar para ofrecer una variedad de detalles sobre los datos del informe.

Algunos atributos de las vistas son:

* Puede usar una vista predeterminada de Workfront o crear la suya propia.
* Puede aplicar vistas adicionales desde el campo desplegable Ver después de ejecutar un informe.
* Las vistas adicionales sustituyen temporalmente la vista que se define al crear el informe; sin embargo, la vista predeterminada se muestra la próxima vez que vuelva al informe.

   Para obtener más información sobre las vistas, consulte el artículo [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Agrupaciones

Una agrupación controla cómo se organizan los datos, lo que facilita su lectura y comprensión. Los grupos crean barras horizontales en todo un informe que muestran los resultados enumerados juntos mediante atributos comunes. Puede definir los criterios para agrupar los resultados del informe al crear la agrupación.

Por ejemplo, si agrupa una lista de tareas que abarcan varios proyectos por su nombre, se organizarán todas las tareas correspondientes que pertenezcan a un solo proyecto con ese nombre.

Algunos atributos de las agrupaciones son:

* Los agrupamientos son un elemento de informes obligatorio si desea agregar más adelante un gráfico al informe.
* Los grupos muestran un valor agregado en los resultados. &#x200B;
* Los grupos determinan el eje en los gráficos.
* Los grupos determinan la identificación del encabezado en los informes de matriz.\
   Para obtener más información sobre los informes de matriz, consulte el artículo [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Los agrupamientos ayudan a crear la pestaña Resumen de un informe, proporcionando los valores agregados del informe.
* Workfront proporciona una serie de agrupaciones para diferentes objetos de forma predeterminada.
* Puede personalizar las agrupaciones que posea o administre.

   Para obtener más información sobre las agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Otros elementos de información

Además de los filtros, las vistas y las agrupaciones, también puede añadir los siguientes elementos a un informe:

* **Preguntar**: Filtro abierto que se puede personalizar y aplicar de forma diferente cada vez que ejecute un informe.\
   Para obtener más información sobre los mensajes, consulte el artículo [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Gráfico**: Puede mejorar los informes agregándoles un gráfico y mostrando la información de forma visual.\
   Para obtener más información sobre los gráficos de los informes, consulte el artículo [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
