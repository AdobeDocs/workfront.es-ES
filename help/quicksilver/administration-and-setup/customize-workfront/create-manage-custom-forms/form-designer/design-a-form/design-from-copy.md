---
title: Crear un formulario a partir de una copia
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede crear un formulario personalizado a partir de una copia con el diseñador de formularios.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Creación de un formulario a partir de una copia

<!--add preview tags and see below in comment out-->

Puede diseñar un nuevo formulario personalizado basado en uno existente. Puede adjuntar formularios personalizados a diferentes objetos de Workfront para capturar datos sobre esos objetos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Copiar un formulario personalizado para crear uno nuevo

{{step-1-to-setup}}

1. Haga clic en **Forms personalizado.**
1. Seleccione el formulario personalizado que desee usar como base para un nuevo formulario personalizado y luego haga clic en ![Icono de copiar](assets/copy-icon.png).
1. En el cuadro **Copia de formulario personalizado** que aparece, escriba la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de formulario</td> 
      <td>Escriba un nombre para el formulario copiado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Tipos de formularios </p> </td> 
      <td> <p>En el cuadro <b>Tipo de formulario</b>, seleccione los tipos de objeto con los que desea que funcione el formulario personalizado y haga clic en la X situada junto a los tipos que desee quitar. Los tipos que ya están asociados con el formulario se deshabilitan en la lista.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>El formulario debe estar asociado al menos a un tipo de objeto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Copiar**.

   En el formulario original, si los campos calculados hacen referencia a campos incompatibles con un tipo de objeto que agregue al nuevo formulario, un mensaje le pedirá que cambie los cálculos en esos campos.

   Del mismo modo, si una opción de acceso para un salto de sección en el formulario original no es compatible con un tipo de objeto que agregue al nuevo, aparecerá un mensaje en el que se le pedirá que ajuste la opción.

1. Seleccione el formulario que acaba de copiar y haga clic en ![Editar icono](assets/edit-icon.png).
1. Realice cambios en el formulario, tal como se explica en las siguientes secciones del artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md):

   * [Reutilizar un campo o widget existente ya utilizado en otro formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Añadir campos de texto](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Añadir campos calculados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Agregar botones de opción, grupos de casillas de verificación y menús desplegables](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adición de campos de fecha y tipo anticipado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [Agregar imágenes, PDF y vídeos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Agregar archivos de Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
     <!--* [Add Planning connection fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)-->

1. (Opcional) Después de hacer clic en **Guardar y cerrar**, adjunte el formulario al objeto donde desea utilizarlo, tal como se describe en [Agregar un formulario personalizado a un objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
