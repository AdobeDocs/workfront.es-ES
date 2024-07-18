---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Hacer referencia a un formulario personalizado en un informe
description: Puede hacer referencia a los formularios personalizados de un objeto en las vistas, filtros y agrupaciones de un informe para ese objeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 2%

---

# Hacer referencia a un formulario personalizado en un informe

Puede hacer referencia a los formularios personalizados de un objeto en las vistas, filtros y agrupaciones de un informe para ese objeto.

Puede hacer referencia al contenido de los formularios personalizados para incluirlo en un informe o puede hacer referencia a la información sobre los propios formularios personalizados que se van a incluir en un informe.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

El formulario personalizado debe existir antes de poder hacer referencia a él en un informe.

Para obtener más información sobre la creación de formularios personalizados, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Hacer referencia al contenido de los formularios personalizados

Puede hacer referencia a campos dentro de formularios personalizados. Después de aplicar un formulario personalizado a un objeto, todos los campos asociados a ese formulario personalizado están disponibles para que se haga referencia en un informe como lo estaría cualquier otro campo del objeto.

>[!NOTE]
>
>En el caso de los campos que tienen varias opciones, todas las opciones están disponibles en los filtros y los indicadores del informe, incluidas las que están ocultas.\
>Para obtener más información sobre cómo ocultar las opciones de un campo personalizado con varias opciones, vea el artículo [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Al crear el informe, simplemente utilice el tipo de objeto del formulario como origen del campo y utilice el nombre del campo personalizado como nombre del campo.

Por ejemplo, es posible que tenga un formulario personalizado aplicado a todos los proyectos que incluya el campo personalizado **Consultor**. Para crear un informe que enumere todos los proyectos en los que Olivia Kim sea la consultora, use el tipo de objeto **Proyecto** como origen de campo y use **Consultor** como nombre de campo. Establezca el calificador de filtro en **Equal** y, a continuación, escriba Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Para obtener más información acerca de cómo crear un informe, vea el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Información de referencia sobre formularios personalizados

Puede hacer referencia a información sobre formularios personalizados, como el nombre de cualquier formulario personalizado asociado a un objeto.

&#x200B;Según el elemento (Ver, Filtro o Agrupación), puede hacer referencia a:

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
1. En la ficha **Columnas**, expanda el origen del campo **Categoría** y, a continuación, haga clic en el nombre del campo **Nombre**.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Hacer referencia a formularios personalizados en un filtro de informe {#reference-custom-forms-in-a-report-filter}

Para filtrar todos los formularios personalizados asociados al tipo de objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la ficha **Filtros**, expanda **Categorías** y, a continuación, haga clic en **Nombre**.\
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
   >Si el campo para el que está filtrando tiene varias opciones y usa los calificadores **No es igual** o **No contiene**, se filtrarán los resultados que contengan solamente la opción que especifique. Si el campo contiene opciones adicionales, incluida la especificada, esos resultados no se filtran del informe. Esto incluye el filtrado para varios Forms personalizados si están adjuntos al mismo objeto.

1. Empiece a escribir el nombre del formulario personalizado por el que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Haga clic en **Agregar otra regla de filtro** y, a continuación, repita los pasos 2-4 para crear reglas de filtro adicionales.
1. Haga clic en **Guardar+Cerrar**.

Para filtrar únicamente en el formulario personalizado principal asociado al tipo de objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la ficha **Filtros**, expanda el origen del campo **Categoría** y, a continuación, haga clic en el nombre del campo **Nombre**.\
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
1. (Opcional) Haga clic en **Agregar otra regla de filtro** y, a continuación, repita los pasos 2-4 para crear reglas de filtro adicionales.
1. Haga clic en **Guardar+Cerrar**.

### Hacer referencia a formularios personalizados en una agrupación de informes {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Solo puede agrupar elementos por el formulario personalizado principal asociado al objeto; no puede agrupar elementos por todos los formularios asociados al objeto.

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En la ficha **Agrupaciones**, expanda **Categoría** y, a continuación, haga clic en **Nombre**.\
   ![](assets/qs-category-name-grouping-350x373.png)
