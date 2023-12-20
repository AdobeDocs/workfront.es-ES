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
source-git-commit: ae063189eebb17a3341aabb978ee0f0e03d1e299
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# Restablecer preferencias de usuario

<!-- Audited: 12/2023 -->

Como administrador de Adobe Workfront, puede restablecer o quitar la configuración de preferencias de usuario de cualquier usuario del sistema de Workfront.

Los usuarios individuales también pueden restablecer su propia configuración de preferencias de usuario.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acerca de la configuración afectada

Al restablecer las preferencias de usuario, algunas se revierten al valor predeterminado del sistema y otras se borran o eliminan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preferencia</strong> </th> 
   <th><strong>Estado tras el restablecimiento</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Vistas</td> 
   <td> <p> Revertido al sistema predeterminado</p> <p>Las vistas existentes no se eliminan. Puede seleccionarlos de nuevo.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtros</td> 
   <td> <p>Revertido al sistema predeterminado</p> <p>Los filtros existentes no se eliminan. Puede seleccionarlos de nuevo.</p> </td> 
  </tr> 
  <tr> 
   <td>Agrupaciones</td> 
   <td> <p>Revertido al sistema predeterminado</p> <p>Las agrupaciones existentes no se eliminan. Puede seleccionarlos de nuevo.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista de elementos recientes</td> 
   <td>Borrado</td> 
  </tr> 
  <tr> 
   <td>Lista de favoritos</td> 
   <td>Inafectado</td> 
  </tr> 
  <tr> 
   <td>Preferencias de usuario</td> 
   <td> <p>Revertido al sistema predeterminado</p> <p>Las notificaciones por correo electrónico vuelven a los valores predeterminados del sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Fichas personalizadas definidas por el usuario</td> 
   <td>Eliminado</td> 
  </tr> 
  <tr> 
   <td>Opciones de navegación global definidas por el usuario</td> 
   <td>Volver a la definición de la plantilla de diseño o establecer el valor predeterminado del sistema si no se asigna ninguna plantilla de diseño.</td> 
  </tr> 
 </tbody> 
</table>

## Restablecer preferencias de usuario

{{step-1-to-setup}}

1. Seleccionar **Iniciar sesión como**.
1. Empiece a escribir el nombre del usuario cuyas preferencias desee restablecer y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. Seleccionar  **Iniciar sesión**.
1. En el campo URL de la parte superior del explorador web, añada `/resetUser` después `workfront.com`.

   >[!NOTE]
   >
   >Distingue entre mayúsculas y minúsculas. La U debe escribirse en mayúsculas y los caracteres restantes deben escribirse en minúsculas. Por ejemplo:
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. Prensa **Entrar**.
1. Para restablecer todas las preferencias de usuario, seleccione **Restablecer**.

   O

   Para restablecer solo las pestañas personalizadas, seleccione **Restablecer fichas**.
