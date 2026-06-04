---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminar un campo o widget personalizado del sistema
description: Para mejorar el rendimiento del sistema y facilitar el uso de los formularios por parte de los usuarios, es posible que desee eliminar los campos y widgets personalizados del sistema cuando ya no se utilicen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
TQID: https://experienceleague.adobe.com/ArUsDbsxOsdzpdmBGFxs0PcRqBG3HstsZmde--rkQbA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 557
ht-degree: 90%

---

# Eliminar un campo o widget personalizado del sistema

Para mejorar el rendimiento del sistema y facilitar el uso de los formularios por parte de los usuarios, es posible que desee eliminar los campos y widgets personalizados del sistema cuando ya no se utilicen.

>[!CAUTION]
>
>Al eliminar un campo personalizado, también se eliminan todos los datos personalizados que los usuarios han introducido en el campo al rellenar formularios personalizados adjuntos a los objetos. Los datos eliminados no se pueden recuperar. Además, no hay ningún sistema de notificación que avise a las personas que utilizan el formulario personalizado de que se ha eliminado.
>
>Puede ver todos los formularios e informes personalizados que utilizan un campo personalizado que desee eliminar para evaluar cuáles podrían ser las repercusiones. Para obtener más información, consulte [Ver todos los formularios personalizados que usan un campo o widget personalizado en particular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) y [Ver todos los informes que usan un campo o widget personalizado en particular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>O bien, para obtener una solución que puede utilizar para evitar la pérdida de datos en campos que ya no se utilizan, consulte [Quitar un campo personalizado sin perder los datos introducidos por los usuarios](#remove-a-custom-field-without-losing-data-that-users-have-entered) en este artículo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar un campo o widget personalizado del sistema

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Haga clic en **Campos** para abrir el área Campos.
1. Seleccione el campo o widget personalizado y, a continuación, haga clic en **Eliminar**.
1. Si está seguro de que desea eliminar permanentemente el elemento y (en el caso de un campo personalizado) todos los datos asociados en los objetos donde se adjuntó, haga clic en **Sí, eliminarlo**.

## Quitar un campo personalizado sin perder los datos introducidos por los usuarios {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>La eliminación de un campo personalizado de un formulario personalizado que tiene más de 500 campos y widgets no se puede deshacer. Si elimina el campo, no podrá volver a añadirlo hasta que el formulario tenga menos de 500 campos y widgets.

1. Determine qué campos personalizados desea eliminar del formulario personalizado original, pero no los elimine en este momento.
1. Crear un nuevo formulario personalizado:

   1. Añada los campos personalizados al nuevo formulario que desee quitar del formulario personalizado original.

      Para obtener más información, consulte la sección [Agregar campos nuevos o existentes al formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) en [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   1. Guarde el nuevo formulario personalizado.

1. Limite el acceso al formulario personalizado únicamente a los usuarios con acceso administrativo, tal como se describe en [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Aplique el nuevo formulario personalizado a los objetos donde ya se aplicó el formulario personalizado original, tal como se describe en [Añadir un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   La aplicación del nuevo formulario personalizado a estos objetos garantiza que los datos del historial de informes no se vean afectados.

1. Modifique el formulario personalizado original y quite los campos personalizados que añadió al nuevo formulario (en el paso 2).

   Los campos que ha eliminado del formulario personalizado original ahora solo están disponibles en el nuevo formulario personalizado que ha creado. Los usuarios pueden ver el formulario personalizado en el objeto, pero los usuarios sin acceso administrativo no pueden modificar el formulario personalizado.
