---
title: Restablecer preferencias de usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede restablecer o quitar la configuración de preferencias de usuario de cualquier usuario del sistema de Workfront. Los usuarios individuales también pueden restablecer su propia configuración de preferencias de usuario.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
TQID: https://experienceleague.adobe.com/rcmVwp5wZgG0cmtmUclkBUnTcOT9OaW7LDHIt373AjM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 85%

---

# Restablecer preferencias de usuario

<!-- Audited: 12/2023 -->

Como administrador de Adobe Workfront, puede restablecer o quitar la configuración de preferencias de usuario de cualquier usuario del sistema de Workfront.

Los usuarios individuales también pueden restablecer su propia configuración de preferencias de usuario.

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
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acerca de la configuración afectada

Al restablecer las preferencias de usuario, algunas se revierten al valor predeterminado del sistema y otras se borran o quitan:

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

| Preferencia | Estado tras el restablecimiento |
| --- | --- |
| Vistas | Revertido al valor predeterminado del sistema <p>Las vistas existentes no se eliminan. Se pueden volver a seleccionar.</p> |
| Filtros | Revertido al valor predeterminado del sistema <p>Los filtros existentes no se eliminan. Se pueden volver a seleccionar.</p> |
| Agrupaciones | Revertido al valor predeterminado del sistema <p>Las agrupaciones existentes no se eliminan. Se pueden volver a seleccionar.</p> |
| Lista de elementos recientes | Borrado |
| Lista de favoritos | No afectado |
| Preferencias de usuario | Revertido al valor predeterminado del sistema <p>Las notificaciones por correo electrónico se revierten a los valores predeterminados del sistema. Las notificaciones predeterminadas se enumeran en [Notificaciones de eventos disponibles en Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

## Restablecer preferencias de usuario

{{step-1-to-setup}}

1. Seleccione **Iniciar sesión como**.
1. Empiece a escribir el nombre del usuario cuyas preferencias desee restablecer y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. Seleccione **Iniciar sesión**.
1. En el campo URL en la parte superior del navegador web, agregue y agregue `/resetUser` después de `workfront`.

   >[!NOTE]
   >
   >Distingue entre mayúsculas y minúsculas. La U debe escribirse en mayúscula y los caracteres restantes deben escribirse en minúscula. Por ejemplo:
   >
   >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Presione **Intro**.

1. Para restablecer todas las preferencias de usuario, haga clic en **Restablecer**.

   O

   Para restablecer la navegación izquierda del usuario a la configuración original de la plantilla de diseño, haga clic en **Restablecer navegación izquierda**.
