---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminar tipos de objetos en un formulario personalizado
description: En un formulario personalizado existente, puede eliminar tipos de objeto asociados al formulario. Una vez hecho esto, los usuarios ya no podrán adjuntar el formulario a los objetos de ese tipo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Eliminar tipos de objetos en un formulario personalizado

En un formulario personalizado existente, puede eliminar tipos de objeto asociados al formulario. Una vez hecho esto, los usuarios ya no podrán adjuntar el formulario a los objetos de ese tipo.

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

## Eliminar tipos de objetos en un formulario personalizado

Puede eliminar tipos de objetos de un formulario personalizado existente.

Un formulario personalizado debe tener al menos un tipo de objeto.

>[!CAUTION]
>
>Si hay personas que ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y que le han agregado datos, esos datos se eliminarán de forma permanente cuando elimine ese tipo de objeto en el formulario. Puede incluir información histórica que los usuarios necesitarán más adelante.
>
>En general, se recomienda minimizar el número de veces que se edita un formulario personalizado que ya está en uso. No hay ningún sistema de notificación para avisar a las personas que usen el formulario personalizado sobre sus cambios.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado** en el panel izquierdo.
1. Seleccione el formulario personalizado que desee editar y haga clic en **Editar**.
1. Haga clic en la X de cualquiera de las **Tipos de objetos** que desea eliminar del formulario y, a continuación, haga clic en **Eliminar** en el mensaje de advertencia que aparece.

   ![](assets/click-x-object-types.jpg)

1. (Opcional) Repita el paso anterior con cualquier otro tipo de objeto que desee quitar del formulario.
1. Haga clic en **Listo** y haga clic en **Cerrar y guardar**.
