---
title: Crear o editar un formulario personalizado con el generador de formularios heredado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede crear o editar un nuevo formulario personalizado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Crear o editar un formulario personalizado con el generador de formularios heredado

<!--Audited: 01/2024-->

{{form-designer-default}}

Puede crear un nuevo formulario personalizado o editar un formulario existente. Ambas tareas se explican en este artículo.

Para obtener información sobre cómo crear un formulario personalizado nuevo a partir de uno existente, consulte [Copiar un formulario personalizado para crear uno nuevo con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

Este artículo describe cómo crear un formulario personalizado mediante el creador de formularios heredados. Para obtener información sobre cómo crear un formulario personalizado con el diseñador de formularios, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>Nuevo: estándar</p>
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

## Empezar a crear un formulario personalizado

{{step-1-to-setup}}

1. Haga clic en **Forms personalizado** en el panel izquierdo.

   Los formularios personalizados se muestran en una lista. Puede revisar todos los formularios y campos personalizados que se hayan creado para su organización. También puede ver quién creó cada formulario, los objetos asociados a él y si está activo.

1. Haga clic en **Nuevo formulario personalizado.**
1. Seleccione al menos un tipo de objeto que desee asociar con el formulario personalizado y, a continuación, haga clic en **Continuar**.

   ![](assets/choose-object-type.jpg)

1. En la ficha **Configuración del formulario** que se abre, escriba un **Título del formulario** y una **Descripción** opcional para el formulario personalizado.

1. (Opcional) Si desea agregar más tipos de objetos al formulario para que se pueda adjuntar a más objetos, haga clic en el signo **más** después de **Tipos de objetos** y, a continuación, seleccione el tipo de objeto que desee en el menú que aparece.

   Puede repetir esto para agregar todos los tipos de objetos que desee.

1. (Opcional) Haga clic en **X** de un tipo de objeto para eliminarlo del formulario.

   Para obtener información acerca de cómo eliminar tipos de objetos de un formulario personalizado que ya ha guardado, vea [Eliminar tipos de objetos de un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Haga clic en **Listo** en la esquina inferior izquierda de la pantalla.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras crea un formulario personalizado para guardar los cambios y mantener el formulario abierto.

1. Si desea agregar un nuevo campo personalizado al formulario, continúe con [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Reutilizar un campo o widget personalizado en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   O

   Si desea seguir creando el formulario personalizado de otras formas, consulte uno de los siguientes artículos:

   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Coloque campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar un salto de sección a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y saltar lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Empezar a editar un formulario personalizado

Puede editar un formulario personalizado en cualquier momento después de crearlo.

>[!CAUTION]
>
>Para obtener información acerca de cómo quitar campos de un formulario personalizado sin perder los datos que los usuarios han escrito en esos campos, vea la sección [Quitar un campo personalizado sin perder los datos que los usuarios han escrito](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) en el artículo [Eliminar un campo o widget personalizado del sistema](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>En general, se recomienda minimizar el número de veces que se edita un formulario personalizado que ya está en uso. No hay ningún sistema de notificación que avise a las personas que utilizan el formulario personalizado sobre sus cambios.

{{step-1-to-setup}}

1. Haga clic en **Forms personalizado** en el panel izquierdo.

   Los formularios personalizados se muestran en una lista. Puede revisar todos los formularios y campos personalizados que se hayan creado para su organización. También puede ver quién creó cada formulario, los objetos asociados a él y si está activo.

1. Seleccione el formulario personalizado que desee editar y luego haga clic en ![Editar icono](assets/edit-icon.png).
1. (Opcional) Para cambiar el título y la descripción del formulario personalizado, haga clic en la ficha **Configuración del formulario**, luego escriba un **Título del formulario** y **Descripción**.

1. (Opcional) Si desea agregar más tipos de objetos al formulario para que se pueda adjuntar a más objetos, haga clic en el signo más + después de **Tipos de objetos** y, a continuación, seleccione el tipo que desee en el menú que aparece.

   ![](assets/add-object-type-existing-form.png)

   Puede repetir esto para agregar todos los tipos de objetos que desee.

   También puede hacer clic en la X de un tipo de objeto para eliminarlo del formulario. Esto debe hacerse con precaución cuando desee eliminar un tipo de objeto de un formulario personalizado que ya haya guardado. Para obtener más información, vea [Eliminar tipos de objetos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Haga clic en **Listo**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras crea un formulario personalizado para guardar los cambios y mantener el formulario abierto.

1. Si desea agregar un nuevo campo personalizado al formulario, continúe con [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Reutilizar un campo o widget personalizado en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   O

   Si desea seguir creando el formulario personalizado de otras formas, consulte uno de los siguientes artículos:

   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Coloque campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar un salto de sección a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y saltar lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
