---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Hacer referencia a un formulario personalizado en un informe
description: Puede hacer referencia a los formularios personalizados de un objeto en las vistas, filtros y agrupamientos de un informe para ese objeto.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# Hacer referencia a un formulario personalizado en un informe

Puede hacer referencia a los formularios personalizados de un objeto en las vistas, filtros y agrupamientos de un informe para ese objeto.

Puede hacer referencia al contenido de los formularios personalizados para incluirlos en un informe o puede hacer referencia a la información sobre los propios formularios personalizados para incluirlos en un informe.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

El formulario personalizado debe existir para poder hacer referencia a él en un informe.

Para obtener más información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Referencia al contenido de formularios personalizados

Puede hacer referencia a campos dentro de formularios personalizados. Después de aplicar un formulario personalizado a un objeto, todos los campos asociados con ese formulario personalizado están disponibles para ser referenciados en un informe como cualquier otro campo del objeto.

>[!NOTE]
>
>En los campos que tienen varias opciones, todas las opciones están disponibles en los filtros y las solicitudes del informe, incluidas las que están ocultas.\
>Para obtener más información sobre cómo ocultar opciones de un campo personalizado con varias opciones, consulte el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Al crear el informe, simplemente utilice el tipo de objeto del formulario como origen de campo y el nombre del campo personalizado como nombre de campo.

Por ejemplo, puede tener un formulario personalizado aplicado a todos los proyectos que incluyan el campo personalizado **Consultor**. Para crear un informe que enumere todos los proyectos en los que Olivia Kim es la consultora, utilice la variable **Proyecto** tipo de objeto como origen de campo y utilice **Consultor** como nombre del campo. Establezca el calificador de filtro en **Igual** y luego escriba Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Información de referencia sobre formularios personalizados

Puede hacer referencia a información sobre los formularios personalizados, como el nombre de cualquier formulario personalizado asociado a un objeto.

&#x200B; En función del elemento (Ver, Filtrar o Agrupar), puede hacer referencia a:

* El formulario personalizado principal aplicado a un objeto:

   Este es el formulario que aparece primero en la página Detalles del objeto.

* Todos los formularios personalizados (si se aplica más de un formulario personalizado a un objeto)

Puede hacer referencia a formularios personalizados en Vistas, Filtros y Agrupaciones:

* [Hacer referencia a formularios personalizados en una vista de informe (columna)](#reference-custom-forms-in-a-report-view-column)
* [Hacer referencia a formularios personalizados en un filtro de informe](#reference-custom-forms-in-a-report-filter)
* [Hacer referencia a formularios personalizados en un grupo de informes](#reference-custom-forms-in-a-report-grouping)

### Hacer referencia a formularios personalizados en una vista de informe (columna) {#reference-custom-forms-in-a-report-view-column}

Para mostrar todos los formularios personalizados asociados a un objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En el **Columnas** , expanda el tipo de objeto al que se aplica el formulario personalizado al que desea hacer referencia y, a continuación, haga clic en **Nombre de la categoría**.\
   Por ejemplo, para mostrar todos los formularios personalizados asociados a una tarea, expanda el **Tarea** fuente del campo y, a continuación, haga clic en el botón **Nombre de la categoría** nombre del campo.\
   ![](assets/qs-category-name-column-350x267.png)

Para mostrar solo el formulario personalizado principal asociado al objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En el **Columnas** expanda la pestaña **Categoría** fuente del campo y, a continuación, haga clic en el botón **Nombre** nombre del campo.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Hacer referencia a formularios personalizados en un filtro de informe {#reference-custom-forms-in-a-report-filter}

Para filtrar todos los formularios personalizados asociados al tipo de objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En el **Filtros** pestaña, expandir **Categorías** y haga clic en **Nombre**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Seleccione el calificador de condición que desee utilizar:

   * En blanco
   * No en blanco
   * Contiene
   * No contiene
   * Igual (no distingue mayúsculas y minúsculas)
   * no es igual

   Para obtener más información sobre cada calificador, consulte el artículo [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Si el campo que está filtrando tiene varias opciones y usa la variable **Distinto a** o **No contiene** cualificadores, esto filtra los resultados que contienen solo la opción especificada. Si el campo contiene opciones adicionales, incluida la especificada, esos resultados no se filtran del informe. Esto incluye el filtrado de varias Forms personalizadas si están conectadas al mismo objeto.

1. Comience a escribir el nombre del formulario personalizado que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Haga clic en **Añadir otra regla de filtro**, repita los pasos del 2 al 4 para crear reglas de filtro adicionales.
1. Haga clic en **Guardar y cerrar**.

Para filtrar solo el formulario personalizado principal asociado al tipo de objeto:

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En el **Filtros** expanda la pestaña **Categoría** fuente del campo y, a continuación, haga clic en el botón **Nombre** nombre del campo.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Seleccione el calificador de condición que desee utilizar:

   * En blanco
   * No en blanco
   * Contiene
   * No contiene
   * Igual (no distingue mayúsculas y minúsculas)
   * no es igual

   Para obtener más información sobre cada calificador, consulte el artículo [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Comience a escribir el nombre del formulario personalizado que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Haga clic en **Añadir otra regla de filtro**, repita los pasos del 2 al 4 para crear reglas de filtro adicionales.
1. Haga clic en **Guardar y cerrar**.

### Hacer referencia a formularios personalizados en un grupo de informes {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Los elementos solo se pueden agrupar mediante el formulario personalizado principal asociado al objeto; no se pueden agrupar elementos por todos los formularios asociados al objeto.

1. Comience a crear un informe como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. En el **Agrupaciones** pestaña, expandir **Categoría** y haga clic en **Nombre**.\
   ![](assets/qs-category-name-grouping-350x373.png)
