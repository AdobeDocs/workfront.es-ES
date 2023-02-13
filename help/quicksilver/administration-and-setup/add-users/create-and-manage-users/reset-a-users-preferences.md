---
title: Restablecer las preferencias de un usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede restablecer o eliminar la configuración de preferencias de usuario para cualquier usuario del sistema Workfront. Los usuarios individuales también pueden restablecer su propia configuración de preferencias de usuario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# Restablecer las preferencias de un usuario

Como administrador de Adobe Workfront, puede restablecer o eliminar la configuración de preferencias de usuario para cualquier usuario del sistema Workfront.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acerca de la configuración afectada

Al restablecer las preferencias de usuario, algunas preferencias se vuelven a la configuración predeterminada del sistema y otras se borran o eliminan:

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
   <td> <p> Revertido al valor predeterminado del sistema</p> <p>Las vistas existentes no se eliminan. Puede volver a seleccionarlos.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtros</td> 
   <td> <p>Revertido al valor predeterminado del sistema</p> <p>Los filtros existentes no se eliminan. Puede volver a seleccionarlos.</p> </td> 
  </tr> 
  <tr> 
   <td>Agrupaciones</td> 
   <td> <p>Revertido al valor predeterminado del sistema</p> <p>Los agrupamientos existentes no se eliminan. Puede volver a seleccionarlos.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista Elementos recientes</td> 
   <td>Aclarado</td> 
  </tr> 
  <tr> 
   <td>Lista de favoritos</td> 
   <td>No afectado</td> 
  </tr> 
  <tr> 
   <td>Preferencias de usuario</td> 
   <td> <p>Revertido al valor predeterminado del sistema</p> <p>Las notificaciones por correo electrónico vuelven a los valores predeterminados del sistema</p> </td> 
  </tr> 
  <tr> 
   <td>Pestañas personalizadas definidas por el usuario</td> 
   <td>Eliminado</td> 
  </tr> 
  <tr> 
   <td>Opciones de navegación global definidas por el usuario</td> 
   <td>Vuelva a la definición de la plantilla de diseño o a la configuración predeterminada del sistema si no se ha asignado ninguna plantilla de diseño.</td> 
  </tr> 
 </tbody> 
</table>

## Restaurar preferencias de usuario

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Select **Iniciar sesión como**.
1. Comience a escribir el nombre del usuario cuyas preferencias desee restablecer y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. Select  **Iniciar sesión**.
1. En el campo URL de la parte superior del explorador web, agregue `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >Esto distingue entre mayúsculas y minúsculas. La U debe tener mayúsculas, y los caracteres restantes deben estar en minúsculas. Por ejemplo:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Press **Entrar**.
1. Para restablecer todas las preferencias de usuario, seleccione **Restablecer**.

   O

   Para restablecer solo las pestañas personalizadas, seleccione **Restablecer fichas**.
