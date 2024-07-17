---
user-type: administrator
product-area: system-administration
keywords: crear,personalizado,formulario,copiar,base,otro
navigation-topic: create-and-manage-custom-forms
title: Copiar un formulario personalizado para crear uno nuevo con el generador heredado
description: Puede crear un nuevo formulario personalizado basado en uno existente.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Copiar un formulario personalizado para crear uno nuevo con el generador heredado

{{form-designer-default}}

Puede crear un nuevo formulario personalizado basado en uno existente.

## Requisitos de acceso

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

1. Seleccione el formulario que acaba de copiar y haga clic en **Editar**.
1. Realice cambios en el formulario, tal como se explica en los siguientes artículos:

   * [Copie un formulario personalizado para crear uno nuevo con el generador de formularios heredados](#Add2)
   * [Agregar datos calculados a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Coloque campos y widgets personalizados en un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregue o edite un widget de recursos en un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregue lógica de visualización y omita la lógica a un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Previsualizar y completar un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Opcional) Después de hacer clic en **Guardar+Cerrar**, adjunte el formulario al objeto donde desea utilizarlo, tal como se describe en [Agregar un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
