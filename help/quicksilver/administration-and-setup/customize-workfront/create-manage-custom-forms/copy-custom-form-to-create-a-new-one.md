---
user-type: administrator
product-area: system-administration
keywords: crear,personalizado,formulario,copiar,base,otro
navigation-topic: create-and-manage-custom-forms
title: Copiar un formulario personalizado para crear uno nuevo
description: Puede crear un nuevo formulario personalizado basado en uno existente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Copiar un formulario personalizado para crear uno nuevo

Puede crear un nuevo formulario personalizado basado en uno existente.

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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
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
1. Realice cualquier cambio en el formulario, tal como se explica en los siguientes artículos:

   * [Copiar un formulario personalizado para crear uno nuevo](#Add2)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Colocación de campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Obtener una vista previa y completar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Opcional) Después de hacer clic en **Guardar y cerrar**, adjunte el formulario al objeto en el que desea utilizarlo, tal como se describe en [Adición de un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
