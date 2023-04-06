---
title: Diseño de un formulario a partir de una copia con el diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado desde una copia con el diseñador de formularios.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---


# Diseño de un formulario a partir de una copia con el diseñador de formularios

Puede diseñar un nuevo formulario personalizado basado en uno existente. Puede adjuntar formularios personalizados a distintos objetos de Workfront para capturar datos sobre dichos objetos.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>
   <p>Plan actual: Estándar</p>
   <p>o</p>
   <p>Plan heredado: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Copiar un formulario personalizado para crear uno nuevo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado.**
1. Seleccione el formulario personalizado que desee utilizar como base para un nuevo formulario personalizado y haga clic en **Copiar**.
1. En el **Copia de formulario personalizada** que aparece, escriba la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de formulario</td> 
      <td>Escriba un nombre para el formulario copiado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Tipos de formulario </p> </td> 
      <td> <p>En el <b>Tipo de formulario</b> , seleccione los tipos de objeto con los que desea que funcione el formulario personalizado y haga clic en la X junto a cualquier tipo que desee quitar. Los tipos que ya están asociados al formulario se desactivan en la lista.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>El formulario debe estar asociado al menos a un tipo de objeto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Copiar formulario**.

   En el formulario original, si los campos calculados hacen referencia a campos que son incompatibles con un tipo de objeto que se agrega al nuevo formulario, un mensaje le pedirá que cambie los cálculos en esos campos.

   Del mismo modo, si una opción de acceso para un salto de sección en el formulario original no es compatible con un tipo de objeto que agregue al nuevo, un mensaje le pedirá que ajuste la opción.

1. Seleccione el formulario que acaba de copiar y haga clic en **Editar**.
1. Realice cualquier cambio en el formulario, tal como se explica en las siguientes secciones de la sección [Diseño de un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) artículo:

* [Reutilizar un campo o widget existente que ya se haya utilizado en otro formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Adición de campos de texto](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Añadir campos calculados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Agregar botones de opción, grupo de casillas de verificación y desplegables](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adición de campos de fecha y de avance](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [Añadir imágenes, PDF y vídeos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Añadir archivos Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Opcional) Después de hacer clic en **Guardar y cerrar**, adjunte el formulario al objeto en el que desea utilizarlo, tal como se describe en [Adición de un formulario personalizado a un objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).