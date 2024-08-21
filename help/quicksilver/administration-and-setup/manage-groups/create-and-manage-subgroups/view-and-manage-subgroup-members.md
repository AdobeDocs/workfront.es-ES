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
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Ver y administrar miembros de subgrupos

Cuando visualiza un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a los usuarios con la opción Administración de usuarios (todos los usuarios) seleccionada</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

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
