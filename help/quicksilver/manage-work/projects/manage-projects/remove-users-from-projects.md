---
product-area: projects;user-management
navigation-topic: manage-projects
title: Quitar usuarios de proyectos
description: Puede quitar usuarios de un proyecto cuando ya no estén implicados en completar el trabajo del proyecto.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 12%

---

# Quitar usuarios de proyectos

Puede quitar usuarios de un proyecto cuando ya no estén implicados en completar el trabajo del proyecto. La eliminación de usuarios de los proyectos tiene implicaciones en las asignaciones de tareas y problemas, así como en las funciones de proyecto. Los usuarios eliminados dejan de recibir notificaciones destinadas al equipo del proyecto. Para obtener más información sobre las notificaciones para los equipos del proyecto, vea [Tipos de notificación de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Los usuarios asociados a un proyecto se enumeran en el área Personas de un proyecto. Representan al equipo del proyecto. Para obtener más información sobre el equipo del proyecto, vea [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Cómo eliminar un usuario afecta a las tareas, problemas y proyectos existentes

Cuando se quita un usuario de un proyecto, cualquier tarea o problema asignado a él puede verse afectado, dependiendo de si la tarea o el problema se completaron cuando se eliminó el usuario:

* **Si el elemento no se completa cuando se quita el usuario:** El elemento se reasigna a un rol si ya se ha asignado un rol o si se asigna al rol que el usuario estaba cumpliendo en el elemento. Si el artículo o el usuario no tienen un rol asignado, debe volver a asignarlo manualmente.
* **Si el elemento se completa cuando se quita el usuario:** El nombre del usuario quitado permanece en el elemento.
* **Si el usuario eliminado también es el creador de un proyecto:** El proyecto no se ha eliminado de su lista **Proyectos en los que participo** en el área de Proyectos. El proyecto se eliminará de las listas de todos los demás usuarios que filtren para ese proyecto por el campo Ingresado por.
* **Si el usuario es el propietario o patrocinador del proyecto:** El usuario permanece en sus roles como patrocinador o propietario del proyecto.

## Quitar usuarios de un proyecto y de un equipo del proyecto

Puede quitar usuarios de un proyecto si los quita del equipo del proyecto.

Cuando los usuarios cumplen funciones en un proyecto, pasan a formar parte del equipo del proyecto.

Al quitar usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Para obtener información acerca de las funciones de los usuarios en un proyecto, vea [Administrar el equipo del proyecto](../planning-a-project/manage-project-team.md).

Para quitar usuarios del equipo del proyecto:

1. Vaya al proyecto en el que desea eliminar a los usuarios.

1. Haga clic en **Personas** en el panel izquierdo y, a continuación, seleccione los usuarios que desee eliminar.

1. Haga clic en el icono **Quitar** ![Quitar elemento](assets/remove-icon---x-in-circle.png) que se encuentra en la parte superior de la lista de usuarios.

1. Haga clic en **Sí, eliminar usuarios seleccionados** para confirmar la eliminación.

   Los usuarios se eliminarán del equipo del proyecto y de cualquier tarea o problema incompleto al que estén asignados. Ya no reciben notificaciones destinadas al equipo del proyecto.
