---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Reutilizar un campo personalizado o un widget de recurso en un formulario personalizado con el generador de formularios heredado
description: Al crear o editar un formulario personalizado, puede agregar un campo personalizado o un widget que ya se haya agregado a otro formulario personalizado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Reutilizar un campo personalizado o un widget de recurso en un formulario personalizado con el generador de formularios heredado

{{form-designer-default}}

Al crear o editar un formulario personalizado, puede agregar un campo personalizado o un widget de recurso que ya se haya agregado a otro formulario personalizado.

También puede reutilizar un campo personalizado calculado existente en un formulario personalizado. Para obtener instrucciones, consulte [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md).

Para obtener información sobre los campos personalizados y los widgets de recursos en los formularios personalizados, consulte [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan Adobe Workfront*</p> </td> 
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

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con su administrador de Workfront.

## Reutilizar un campo o widget personalizado ya utilizado en otro formulario personalizado

1. Comience a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Con **Añadir un campo** seleccionado, haga clic en **Biblioteca de campos**.

1. Arrastre el campo o widget donde desee en el formulario personalizado.
1. (Opcional) Repita los dos pasos anteriores para agregar otros campos o widgets.

   >[!NOTE]
   >
   >Puede agregar hasta 500 campos y widgets en un solo formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existen más de 100 en un formulario, según su complejidad.
   >
   >
   >Algunos ejemplos de formularios complejos son formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un único campo.

1. Si desea seguir creando el formulario personalizado de otras formas, consulte uno de los siguientes artículos:

   * [Agregar un campo personalizado a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Agregar un salto de sección a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Agregar o editar un widget de recursos en un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Agregar datos calculados a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Coloque los campos y widgets personalizados en un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar lógica de visualización y saltar lógica a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Previsualizar y completar un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
