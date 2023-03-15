---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminar un campo o widget personalizado del sistema
description: Para mejorar el rendimiento del sistema y facilitar el uso de los formularios por parte de los usuarios, es posible que desee quitar los campos personalizados y las utilidades del sistema cuando ya no se utilicen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f43a0aae33b96f5a061d9134122078d73fc21e40
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Eliminar un campo o widget personalizado del sistema

Para mejorar el rendimiento del sistema y facilitar el uso de los formularios por parte de los usuarios, es posible que desee quitar los campos personalizados y las utilidades del sistema cuando ya no se utilicen.

>[!CAUTION]
>
>Al eliminar un campo personalizado, también se eliminan todos los datos personalizados que los usuarios han introducido en el campo al rellenar formularios personalizados adjuntos a objetos. Los datos eliminados no se pueden recuperar.
>
>Puede ver todos los formularios personalizados y los informes que utilizan un campo personalizado que desee eliminar para evaluar las repercusiones. Para obtener más información, consulte [Ver todos los formularios personalizados que utilizan un widget o campo personalizado en particular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) y [Ver todos los informes que utilizan un widget o campo personalizado en particular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>O bien, para una solución alternativa que puede utilizar para evitar perder datos en campos que ya no se utilizan, consulte [Eliminación de un campo personalizado sin perder los datos introducidos por los usuarios](#remove-a-custom-field-without-losing-data-that-users-have-entered) en este artículo.

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
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo conceden este acceso los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Eliminar un campo o widget personalizado del sistema

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado.**
1. Haga clic en el **Campos** pestaña .
1. Seleccione el campo o la utilidad personalizados y, a continuación, haga clic en **Eliminar**.
1. Si está seguro de que desea eliminar permanentemente el elemento y (en el caso de un campo personalizado) todos los datos asociados de los objetos adjuntos, haga clic en **Sí, Eliminarlo**.

## Eliminación de un campo personalizado sin perder los datos introducidos por los usuarios {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>No se puede deshacer la eliminación de un campo personalizado de un formulario personalizado que tenga más de 500 campos y utilidades. Si quita el campo, no puede volver a agregarlo hasta que el formulario tenga menos de 500 campos y utilidades.

1. Determine qué campos personalizados desea quitar del formulario personalizado original, pero no los elimine en este momento.
1. Cree un nuevo formulario personalizado:

   1. Agregue los campos personalizados al nuevo formulario que desee quitar del formulario personalizado original.

      * Si utiliza el creador de formularios personalizado, consulte [Reutilizar un campo o un widget personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * Si usa el diseñador de formularios, consulte [Adición de campos nuevos o existentes al formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).
   1. Guarde el nuevo formulario personalizado.


1. Limitar el acceso al formulario personalizado solo a los usuarios con acceso administrativo, tal como se describe en [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Aplique el nuevo formulario personalizado a los objetos en los que ya se haya aplicado el formulario personalizado original, tal como se describe en [Adición de un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   La aplicación del nuevo formulario personalizado a estos objetos garantiza que los datos históricos de los informes no se vean afectados.

1. Modifique el formulario personalizado original y elimine los campos personalizados que agregó al nuevo formulario (en el paso 2).

   Los campos que quitó del formulario personalizado original ahora solo están disponibles en el nuevo formulario personalizado que ha creado. Los usuarios pueden ver el formulario personalizado en el objeto, pero los usuarios sin acceso administrativo no pueden modificarlo.
