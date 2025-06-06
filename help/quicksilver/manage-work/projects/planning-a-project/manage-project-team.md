---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Administrar el equipo del proyecto
description: El equipo del proyecto está formado por usuarios asociados al proyecto. Los miembros del equipo del proyecto se muestran en la sección Personas del proyecto.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 99%

---

# Administrar el equipo del proyecto

El equipo del proyecto está formado por usuarios asociados al proyecto. Los miembros del equipo del proyecto se muestran en la sección Personas del proyecto.

## Requisitos de acceso

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a proyectos</p> <p>Acceso de visualización o superior a los usuarios</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores para el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Agregar usuarios al equipo del proyecto

Cuando agregue usuarios al equipo del proyecto, esos usuarios recibirán permisos de visualización en el proyecto y en las tareas, problemas y documentos del proyecto. Para obtener más información, consulte el artículo [Infomación general sobre el equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Los usuarios del equipo del proyecto no se agregan automáticamente a las herramientas de administración de recursos del proyecto.

Puede agregar usuarios al equipo del proyecto de las siguientes maneras:

* [Agregar usuarios automáticamente a un equipo del proyecto](#automatically-add-users-to-a-project-team)
* [Agregar usuarios manualmente a un equipo del proyecto](#manually-add-users-to-a-project-team)

### Agregar usuarios automáticamente a un equipo del proyecto {#automatically-add-users-to-a-project-team}

Los usuarios que cumplen las siguientes funciones en el proyecto se agregan automáticamente al equipo del proyecto y aparecen en la sección Personas cuando se crea el proyecto:

* El creador del proyecto
* El propietario del proyecto
* El patrocinador del proyecto

Los usuarios también se agregan automáticamente al equipo del proyecto cuando se les asigna lo siguiente:

* Tareas
* Problemas

### Agregar usuarios manualmente a un equipo del proyecto {#manually-add-users-to-a-project-team}

Si los usuarios que no cumplen ninguna función en el proyecto desean que se les notifiquen determinadas actualizaciones o cambios durante la duración del proyecto, puede agregarlos manualmente al equipo del proyecto.

Para obtener más información sobre las notificaciones que se pueden habilitar para los usuarios del equipo del proyecto, consulte [Tipos de notificaciones de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Vaya al proyecto al que desee agregar usuarios.

1. Haga clic en **Personas** en el panel izquierdo.

1. Haga clic en **Agregar usuarios**.

   Aparece el cuadro de diálogo Agregar usuarios al equipo del proyecto.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. En el cuadro **Agregar usuarios**, empiece a escribir el nombre de un usuario activo de Workfront que desee agregar al equipo del proyecto y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Repita este paso para agregar varios usuarios al equipo del proyecto. Los usuarios deben pertenecer al grupo asociado al proyecto.

   >[!TIP]
   >
   >* No puede agregar usuarios agregando sus equipos, grupos, compañías o funciones.
   >* A medida que añada usuarios, fíjese en su avatar, su función principal y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
   >
   >  Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Haga clic en **Añadir**.

   Los usuarios obtienen permisos de visualización del proyecto y reciben notificaciones sobre el proyecto como parte del equipo del proyecto.

## Quitar usuarios del equipo del proyecto

Al quitar usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Si quita un usuario del equipo del proyecto y el usuario está asignado a tareas o problemas del proyecto, se le quita la asignación de las tareas y problemas que no se hayan completado. En este caso, las tareas y los problemas vuelven al área Trabajo no asignado del Distribuidor de cargas de trabajo.

Los usuarios asignados a tareas y problemas completados permanecen asignados incluso después de quitarlos del equipo del proyecto.

Para obtener más información sobre cómo quitar usuarios del equipo del proyecto, consulte [Quitar usuarios de los proyectos](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
