---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminación o desactivación de un formulario personalizado
description: Puede eliminar o desactivar un formulario personalizado del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Eliminación o desactivación de un formulario personalizado

Puede eliminar o desactivar un formulario personalizado del sistema.

>[!CAUTION]
>
>Al eliminar un formulario personalizado también se eliminan todos los datos personalizados de los objetos asociados al formulario. Los datos eliminados no se pueden recuperar. Considere desactivar un formulario personalizado en su lugar; cuando desactive un formulario personalizado que ya no utilice, conservará todos los datos históricos asociados.

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

## Eliminación de un formulario personalizado

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado.**
1. Seleccione el formulario personalizado y haga clic en **Eliminar**.
1. Si está seguro de que desea eliminar permanentemente el formulario personalizado y todos los datos asociados de los objetos adjuntos, haga clic en **Sí, Eliminarlo**.

## Desactivar un formulario personalizado

Puede desactivar los formularios personalizados que ya no utilice sin perder los datos históricos asociados. Los usuarios no pueden agregar un formulario personalizado inactivo a los objetos, pero sí pueden ver y agregar datos a sus campos en objetos que ya estaban adjuntos.

Los campos de un formulario personalizado inactivo también están disponibles para su edición en línea en una vista. Si un usuario agrega un campo de un formulario personalizado inactivo durante una edición en línea, el formulario se adjunta automáticamente al objeto, aunque el formulario personalizado esté desactivado.

Si vuelve a activar un formulario personalizado, conserva la configuración que tenía antes y los usuarios pueden interactuar con él como si nunca se hubiera desactivado.

Para desactivar un formulario personalizado:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en el nombre del formulario personalizado que desee desactivar.
1. Haga clic en el **Configuración de formulario** pestaña .
1. Desactive el **Está activo** .
1. Haga clic en **Guardar + Cerrar**.
