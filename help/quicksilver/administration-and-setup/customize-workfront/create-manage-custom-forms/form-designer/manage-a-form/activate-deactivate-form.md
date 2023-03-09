---
title: Desactivar o reactivar un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede reactivar o desactivar un formulario personalizado. Se recomienda desactivar los formularios personalizados en lugar de eliminar los formularios que ya no utilice para conservar los datos históricos.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Desactivar o reactivar un formulario personalizado

Puede reactivar o desactivar un formulario personalizado. Se recomienda desactivar los formularios personalizados en lugar de eliminar los formularios que ya no utilice para conservar los datos históricos.

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
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con su administrador de Workfront.

## Desactivar un formulario personalizado

Puede desactivar los formularios personalizados que ya no utilice sin perder los datos históricos asociados. Los usuarios no pueden agregar un formulario personalizado inactivo a los objetos, pero pueden ver y agregar datos a sus campos en objetos en los que ya estaba adjunto.

Los campos de un formulario personalizado inactivo también están disponibles para su edición en línea en una vista. Si un usuario agrega un campo desde un formulario personalizado inactivo durante una edición en línea, el formulario se adjunta al objeto automáticamente, aunque el formulario personalizado esté desactivado.

Para desactivar un formulario personalizado:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, elija **Forms personalizado**.
1. En el **Forms** , seleccione el formulario personalizado que desea desactivar.
1. En la columna Is Active, elija **Falso** y haga clic en fuera de la columna. El formulario ya no está activo.

## Reactivar un formulario personalizado

Si reactiva un formulario personalizado, conservará la configuración que tenía antes y los usuarios podrán interactuar con él como si nunca se hubiera desactivado.

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, elija **Forms personalizado**.
1. En el **Forms** , seleccione el formulario personalizado que desea reactivar.
1. En la columna Is Active, elija **Verdadero** y haga clic en fuera de la columna. El formulario ahora está activo.