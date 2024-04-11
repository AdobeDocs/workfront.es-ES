---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminar tipos de objetos en un formulario personalizado
description: En un formulario personalizado existente, puede eliminar los tipos de objetos asociados al formulario. Una vez hecho esto, los usuarios ya no podrán adjuntar el formulario a objetos de ese tipo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Eliminar tipos de objetos en un formulario personalizado

En un formulario personalizado existente, puede eliminar los tipos de objetos asociados al formulario. Una vez hecho esto, los usuarios ya no podrán adjuntar el formulario a objetos de ese tipo.

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

## Eliminar tipos de objetos en un formulario personalizado

Puede eliminar tipos de objetos de un formulario personalizado existente.

Un formulario personalizado debe tener al menos un tipo de objeto.

>[!CAUTION]
>
>Si las personas ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y le han agregado datos, esos datos se eliminan de forma permanente al eliminar ese tipo de objeto en el formulario. Puede incluir información histórica que los usuarios necesitarán más adelante.
>
>En general, se recomienda minimizar el número de veces que se edita un formulario personalizado que ya está en uso. No hay ningún sistema de notificación que avise a las personas que utilizan el formulario personalizado sobre sus cambios.

{{step-1-to-setup}}

1. Clic **Forms personalizado** en el panel izquierdo.
1. Seleccione el formulario personalizado que desee editar y haga clic en ![Icono Editar](assets/edit-icon.png).
1. Haga clic en la X de cualquiera de las **Tipos de objetos** que desee eliminar del formulario y, a continuación, haga clic en **Eliminar** en el mensaje de advertencia que se muestra.

   ![](assets/click-x-object-types.jpg)

1. (Opcional) Repita el paso anterior para cualquier otro tipo de objeto que desee quitar del formulario.
1. Clic **Listo**, luego haga clic en **Guardar y cerrar**.
