---
product-area: projects;user-management
navigation-topic: manage-projects
title: Quitar usuarios de proyectos
description: Puede quitar usuarios de un proyecto cuando ya no estén implicados en completar el trabajo del proyecto.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Quitar usuarios de proyectos

Puede quitar usuarios de un proyecto cuando ya no estén implicados en completar el trabajo del proyecto. La eliminación de usuarios de los proyectos tiene implicaciones en las asignaciones de tareas y problemas, así como en las funciones de proyecto. Los usuarios eliminados dejan de recibir notificaciones destinadas al equipo del proyecto. Para obtener más información sobre las notificaciones para los equipos del proyecto, consulte [Tipos de notificación de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Los usuarios asociados a un proyecto se enumeran en el área Personas de un proyecto. Representan al equipo del proyecto. Para obtener más información sobre el equipo del proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Cómo eliminar un usuario afecta a las tareas, problemas y proyectos existentes

Cuando se quita un usuario de un proyecto, cualquier tarea o problema asignado a él puede verse afectado, dependiendo de si la tarea o el problema se completaron cuando se eliminó el usuario:

* **Si el elemento no se completa cuando se quita el usuario:** El elemento se reasigna a un rol si ya se ha asignado un rol o si se asigna al rol que el usuario estaba cumpliendo en el elemento. Si el artículo o el usuario no tienen un rol asignado, debe volver a asignarlo manualmente.
* **Si el elemento se completa cuando se quita el usuario:** El nombre del usuario eliminado permanece en el elemento.
* **Si el usuario eliminado también es el creador de un proyecto:** El proyecto no se ha eliminado de sus **Proyectos en los que trabajo** en el área Proyectos. El proyecto se eliminará de las listas de todos los demás usuarios que filtren para ese proyecto por el campo Ingresado por.
* **Si el usuario es el propietario o patrocinador del proyecto:** El usuario mantiene sus funciones como patrocinador o propietario del proyecto.

## Quitar usuarios de un proyecto y de un equipo del proyecto

Puede quitar usuarios de un proyecto si los quita del equipo del proyecto.

Cuando los usuarios cumplen funciones en un proyecto, pasan a formar parte del equipo del proyecto.

Cuando elimina usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Para obtener información sobre las funciones de los usuarios en un proyecto, consulte [Administrar el equipo del proyecto](../planning-a-project/manage-project-team.md).

Para quitar usuarios del equipo del proyecto:

1. Vaya al proyecto en el que desea eliminar a los usuarios.

1. Clic **People** en el panel izquierdo, seleccione los usuarios que desee eliminar. Es posible que tenga que hacer clic en **Mostrar más**, entonces **People**.

1. Haga clic en **Eliminar** icono  ![Quitar elemento](assets/remove-icon---x-in-circle.png) en la parte superior de la lista de usuarios.

1. Clic **Sí, quitar usuarios seleccionados** para confirmar la eliminación.

   Los usuarios se eliminarán del equipo del proyecto y de cualquier tarea o problema incompleto al que estén asignados. Ya no reciben notificaciones destinadas al equipo del proyecto.
