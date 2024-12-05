---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Hacer referencia a un formulario personalizado en un informe
description: Puede hacer referencia a los formularios personalizados de un objeto en las vistas, filtros y agrupaciones de un informe para ese objeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 394eb1aed6508399b6459430acec7c0729036edc
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 96%

---

# Hacer referencia a un formulario personalizado en un informe

<!-- Audited: 11/2024 -->

Puede hacer referencia a los formularios personalizados de un objeto en las vistas, filtros y agrupaciones de un informe para ese objeto.

Puede hacer referencia al contenido de los formularios personalizados para incluirlo en un informe o puede hacer referencia a la información sobre los propios formularios personalizados que se van a incluir en un informe.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
      <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a informes, paneles y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

El formulario personalizado debe existir antes de poder hacer referencia al mismo en un informe.

Para obtener más información sobre la creación de formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Hacer referencia al contenido de los formularios personalizados

Puede hacer referencia a campos dentro de formularios personalizados. Después de aplicar un formulario personalizado a un objeto, todos los campos asociados a ese formulario personalizado están disponibles para que se les haga referencia en un informe como lo estaría cualquier otro campo del objeto.

>[!NOTE]
>
>En el caso de los campos que tienen varias opciones, todas las opciones están disponibles en los filtros y los indicadores del informe, incluidas las que están ocultas.\
>Para obtener más información sobre cómo ocultar las opciones de un campo personalizado con varias opciones, consulte el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Al crear el informe, simplemente utilice el tipo de objeto del formulario como origen del campo y utilice el nombre del campo personalizado como nombre del campo.

Por ejemplo, es posible que tenga un formulario personalizado aplicado a todos los proyectos que incluya el campo personalizado **Consultor**. Para crear un informe que enumere todos los proyectos en los que Olivia Kim sea la consultora, use el tipo de objeto **Proyecto** como origen de campo y use **Consultor** como nombre de campo. Establezca el calificador de filtro en **Equal** y, a continuación, escriba Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Para obtener más información acerca de cómo crear un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Información de referencia sobre formularios personalizados

Puede hacer referencia a información sobre formularios personalizados, como el nombre de cualquier formulario personalizado asociado a un objeto.

Según el elemento (Vista, Filtro o Agrupación), puede hacer referencia a:

* El formulario personalizado principal aplicado a un objeto:

  Este es el formulario que aparece primero en la página Detalles del objeto.

* Todos los formularios personalizados (si se aplica más de un formulario personalizado a un objeto)

Puede hacer referencia a formularios personalizados en Vistas, Filtros y Agrupaciones:

* [Hacer referencia a formularios personalizados en una vista de informe (columna)](#reference-custom-forms-in-a-report-view-column)
* [Hacer referencia a formularios personalizados en un filtro de informe](#reference-custom-forms-in-a-report-filter)
* [Hacer referencia a formularios personalizados en una agrupación de informes](#reference-custom-forms-in-a-report-grouping)

### Hacer referencia a formularios personalizados en una vista de informe (columna) {#reference-custom-forms-in-a-report-view-column}

Para mostrar todos los formularios personalizados asociados a un objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la ficha **Columnas**, expanda el tipo de objeto al que se aplica el formulario personalizado al que desea hacer referencia y, a continuación, haga clic en **Nombre de categoría**.\
   Por ejemplo, para mostrar todos los formularios personalizados asociados a una tarea, expanda el origen del campo **Tarea** y, a continuación, haga clic en el nombre de campo **Nombre de categoría**.\
   ![](assets/qs-category-name-column-350x267.png)

Para mostrar solo el formulario personalizado principal asociado al objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la pestaña **Columnas**, expanda el origen del campo **Categoría** y, a continuación, haga clic en el nombre del campo **Nombre**.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Hacer referencia a los formularios personalizados en el filtro de un informe {#reference-custom-forms-in-a-report-filter}

Para filtrar todos los formularios personalizados asociados al tipo de objeto:

1. Comience a crear un informe tal como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la pestaña **Filtros**, expanda **Categorías** y, a continuación, haga clic en **Nombre**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Seleccione el calificador de condición que desee utilizar:

   * En blanco
   * No en blanco
   * Contiene
   * No contiene
   * Igual (no distingue mayúsculas y minúsculas)
   * No es igual

   Para obtener más información acerca de cada calificador, vea el artículo [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Si el campo para el que está filtrando tiene varias opciones y usa los calificadores **No es igual** o **No contiene**, se filtrarán los resultados que contengan solamente la opción que especifique. Si el campo contiene opciones adicionales, incluida la especificada, esos resultados no se filtran del informe. Esto incluye el filtrado para varios formularios personalizados si se han adjuntado al mismo objeto.

1. Empiece a escribir el nombre del formulario personalizado por el que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Haga clic en **Añadir otra regla de filtro** y, a continuación, repita los pasos 2-4 para crear reglas de filtro adicionales.
1. Haga clic en **Guardar + Cerrar**.

Para filtrar únicamente en el formulario personalizado principal asociado al tipo de objeto:

1. Comience a crear un informe tal como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la pestaña **Filtros**, expanda el origen del campo **Categoría** y, a continuación, haga clic en el nombre del campo **Nombre**.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Seleccione el calificador de condición que desee utilizar:

   * En blanco
   * No en blanco
   * Contiene
   * No contiene
   * Igual (no distingue mayúsculas y minúsculas)
   * No es igual

   Para obtener más información acerca de cada calificador, vea el artículo [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Empiece a escribir el nombre del formulario personalizado por el que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Haga clic en **Añadir otra regla de filtro** y, a continuación, repita los pasos 2-4 para crear reglas de filtro adicionales.
1. Haga clic en **Guardar + Cerrar**.

### Hacer referencia a formularios personalizados en una agrupación de informes {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Solo puede añadir elementos por el formulario personalizado principal asociado al objeto; no puede agrupar elementos según todos los formularios que haya asociados al objeto.

1. Comience a crear un informe tal como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la pestaña **Agrupaciones**, expanda **Categoría** y, a continuación, haga clic en **Nombre**.\
   ![](assets/qs-category-name-grouping-350x373.png)
