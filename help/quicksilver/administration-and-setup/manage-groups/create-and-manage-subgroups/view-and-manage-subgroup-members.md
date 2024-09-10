---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Ver y administrar miembros del subgrupo
description: Cuando visualiza un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 63c2206905f4ebbc35cb162ae6e895b98b5d20eb
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Ver y administrar miembros de subgrupos

Cuando visualiza un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Editar</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-settings.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y administrar los miembros de los subgrupos de un grupo

{{step-1-to-setup}}

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo para el que desea ver o administrar los miembros del subgrupo.
1. En el panel izquierdo, haga clic en **Miembros del subgrupo**.

   Este elemento del panel izquierdo solo está disponible si el grupo tiene subgrupos.

1. Realice una de las siguientes acciones:

   * Seleccione un miembro de la lista y, a continuación, haga clic en Editar ![](assets/edit-icon.png) para modificar el perfil de usuario de esa persona.

     Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) o [Editar perfiles de usuario de forma masiva](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Seleccione cualquier número de miembros de la lista y, a continuación, haga clic en Actualizar ![](assets/comment-icon.png) para agregar un comentario a sus perfiles de usuario.

     El usuario o los usuarios reciben una notificación en la aplicación, así como una notificación por correo electrónico con su comentario. El comentario se muestra en el área de Actualizaciones del perfil del usuario.

   * Seleccione cualquier número de miembros de la lista y, a continuación, haga clic en Desactivar ![](assets/deactivate-user.png) o Activar ![](assets/activate-user.png).

     Para obtener más información, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportar ![](assets/export.png) la lista de miembros.
