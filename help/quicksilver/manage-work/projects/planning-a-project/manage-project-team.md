---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Administrar el equipo del proyecto
description: El equipo del proyecto está formado por usuarios asociados al proyecto. Los miembros del equipo del proyecto se muestran en la sección Personas del proyecto.
author: Alina
feature: Work Management
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

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
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Ver o acceso superior a Usuarios</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores del proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar usuarios a un equipo de proyecto

Cuando agrega usuarios al equipo del proyecto, obtiene permisos de visualización sobre el proyecto y las tareas, problemas y documentos del proyecto. Para obtener más información, consulte el artículo [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Los usuarios del equipo del proyecto no se agregan automáticamente a las herramientas de administración de recursos del proyecto.

Puede agregar usuarios al equipo del proyecto de las siguientes maneras:

* [Agregar usuarios automáticamente a un equipo de proyecto](#automatically-add-users-to-a-project-team)
* [Agregar usuarios manualmente a un equipo de proyecto](#manually-add-users-to-a-project-team)

### Agregar usuarios automáticamente a un equipo de proyecto {#automatically-add-users-to-a-project-team}

Los usuarios que cumplen las siguientes funciones en el proyecto se añaden automáticamente al equipo del proyecto y aparecen en la sección Personas cuando se crea el proyecto:

* El creador del proyecto
* El propietario del proyecto
* El patrocinador del proyecto

Los usuarios también se agregan automáticamente al equipo del proyecto cuando se les asigna lo siguiente:

* Tareas
* Problemas

### Agregar usuarios manualmente a un equipo de proyecto {#manually-add-users-to-a-project-team}

Si los usuarios que no cumplen ninguna función en el proyecto desean que se les notifique sobre ciertas actualizaciones o cambios durante la vida del proyecto, puede agregarlos manualmente al equipo del proyecto.

Para obtener más información sobre las notificaciones que se pueden habilitar para los usuarios del equipo del proyecto, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Vaya al proyecto al que desee agregar usuarios.

1. Haga clic en **People** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más** primero.

1. Haga clic en **Agregar usuarios**.

   Aparece el cuadro de diálogo Agregar usuarios al equipo del proyecto .

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. En el **Agregar usuarios** , empiece a escribir el nombre de un usuario de Workfront activo que desee agregar al equipo del proyecto y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Repita este paso para agregar varios usuarios al equipo del proyecto. Los usuarios deben pertenecer al grupo asociado al proyecto.

   >[!TIP]
   >
   >* No puede agregar usuarios agregando sus equipos, grupos, empresas o funciones de trabajo.
   >* A medida que agrega los usuarios, observe el avatar, la función principal del usuario y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función de trabajo para verla a medida que los agrega.



1. Haga clic en **Agregar**.

   Los usuarios obtienen permisos de visualización para el proyecto y reciben notificaciones sobre el proyecto como parte del equipo del proyecto.

## Eliminar usuarios de un equipo de proyecto

Cuando elimina a los usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Si elimina un usuario del equipo del proyecto y este se asigna a tareas o problemas del proyecto, el usuario no se asigna a las tareas y los problemas que no se completan. En este caso, las tareas y los problemas vuelven al área Trabajo sin asignar del equilibrador de carga de trabajo.

Los usuarios asignados a tareas completadas y problemas permanecen asignados incluso después de eliminarlos del equipo del proyecto.

Para obtener más información sobre cómo quitar usuarios del equipo del proyecto, consulte [Eliminar usuarios de proyectos](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
