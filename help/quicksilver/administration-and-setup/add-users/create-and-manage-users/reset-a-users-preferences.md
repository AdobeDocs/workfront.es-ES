---
title: Restablecer preferencias de usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede restablecer o quitar la configuración de preferencias de usuario de cualquier usuario del sistema de Workfront. Los usuarios individuales también pueden restablecer su propia configuración de preferencias de usuario.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 7dd278fdf07824edd3336597d20209e25cad88d8
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 89%

---

# Restablecer preferencias de usuario

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Como administrador de Adobe Workfront, puede restablecer o quitar la configuración de preferencias de usuario de cualquier usuario del sistema de Workfront. 

Los usuarios individuales también pueden restablecer su propia configuración de preferencias de usuario.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acerca de la configuración afectada

Al restablecer las preferencias de usuario, algunas se revierten al valor predeterminado del sistema y otras se borran o quitan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preferencia</strong> </th> 
   <th><strong>Estado después del restablecimiento</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Vistas</td> 
   <td> <p> Revertido al valor predeterminado del sistema</p> <p>Las vistas existentes no se eliminan. Se pueden volver a seleccionar.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtros</td> 
   <td> <p>Revertido al valor predeterminado del sistema</p> <p>Los filtros existentes no se eliminan. Se pueden volver a seleccionar.</p> </td> 
  </tr> 
  <tr> 
   <td>Agrupaciones</td> 
   <td> <p>Revertido al valor predeterminado del sistema</p> <p>Las agrupaciones existentes no se eliminan. Se pueden volver a seleccionar.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista de elementos recientes</td> 
   <td>Borrado</td> 
  </tr> 
  <tr> 
   <td>Lista de favoritos</td> 
   <td>No afectado</td> 
  </tr> 
  <tr> 
   <td>Preferencias de usuario</td> 
   <td> <p>Revertido al valor predeterminado del sistema</p> <p>Las notificaciones por correo electrónico se revierten a los valores predeterminados del sistema. Las notificaciones predeterminadas se enumeran en <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Notificaciones de eventos disponibles en Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Pestañas personalizadas definidas por el usuario</td> 
   <td>Eliminado</td> 
  </tr> 
  <tr> 
   <td>Opciones de navegación global definidas por el usuario</td> 
   <td>Se recupera la definición de la plantilla de diseño o el valor predeterminado del sistema si no se ha asignado ninguna plantilla de diseño.</td> 
  </tr> 
 </tbody> 
</table>

<!-- Display this table and hide the HTML table above, when the unshim is released.
| Preference | Status after the reset |
| --- | --- |
| Views | Reverted to the system default <p>Existing views are not deleted. You can select them again.</p> |
| Filters | Reverted to the system default <p>Existing filters are not deleted. You can select them again.</p> |
| Groupings | Reverted to the system default <p>Existing groupings are not deleted. You can select them again.</p> |
| Recent items list | Cleared |
| Favorites list | Unaffected |
| User Preferences | Reverted to the system default <p>Email notifications revert to the system defaults. The default notifications are listed in [Event notifications available in Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |
-->

## Restablecer preferencias de usuario

{{step-1-to-setup}}

1. Seleccione **Iniciar sesión como**.
1. Empiece a escribir el nombre del usuario cuyas preferencias desee restablecer y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. Seleccione **Iniciar sesión**.
1. Si su organización no se ha incorporado a la experiencia unificada de Adobe, siga este paso:

   * En el campo URL de la parte superior del explorador web, añada `/resetUser` detrás de `workfront.com`.

     >[!NOTE]
     >
     >Distingue entre mayúsculas y minúsculas. La U debe escribirse en mayúscula y los caracteres restantes deben escribirse en minúscula. Por ejemplo:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Si su organización se ha incorporado a la experiencia unificada de Adobe, siga este paso:

   * En el campo URL en la parte superior del navegador web, agregue y agregue `/resetUser` después de `workfront`.

     >[!NOTE]
     >
     >Distingue entre mayúsculas y minúsculas. La U debe escribirse en mayúscula y los caracteres restantes deben escribirse en minúscula. Por ejemplo:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Presione **Intro**.
1. Para restablecer todas las preferencias de usuario, seleccione **Restablecer**.

   <!--When this is unshimmed, adjust the comment tags to hide these last two lines, because the Reset Tabs button is going away.-->
O

   Para restablecer solamente las pestañas personalizadas, seleccione **Restablecer pestañas**.
