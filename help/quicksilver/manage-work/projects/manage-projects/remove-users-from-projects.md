---
product-area: projects;user-management
navigation-topic: manage-projects
title: Eliminar usuarios de proyectos
description: Puede eliminar usuarios de un proyecto cuando ya no estén involucrados en completarlo.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 301c86152340a184345bd39cec77fdcf28258196
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Eliminar usuarios de proyectos

Puede eliminar usuarios de un proyecto cuando ya no estén involucrados en completarlo. La eliminación de usuarios de los proyectos tiene implicaciones en las asignaciones de tareas y problemas, así como en las funciones de los proyectos. Los usuarios eliminados dejan de recibir notificaciones destinadas al equipo del proyecto. Para obtener más información sobre las notificaciones para los equipos de proyecto, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Los usuarios asociados a un proyecto se enumeran en el área Personas de un proyecto. Representan al equipo del proyecto. Para obtener más información acerca del equipo del proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acceso

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
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Cómo afecta la eliminación de un usuario a las tareas, los problemas y los proyectos existentes

Cuando se elimina a un usuario de un proyecto, cualquier tarea o problema asignado a él podría verse afectado, dependiendo de si la tarea o el problema se completaron cuando se eliminó al usuario:

* **Si el elemento no se completa cuando se elimina el usuario:** El artículo se vuelve a asignar a una función de trabajo si ya se ha asignado una función de trabajo o si se ha asignado a la función de trabajo que el usuario estaba cumpliendo en el artículo. Si el artículo o el usuario no tenían una función de trabajo asignada, debe volver a asignarlo manualmente.
* **Si el elemento se completa cuando se elimina el usuario:** El nombre del usuario eliminado permanece en el elemento.
* **Si el usuario eliminado también es el creador de un proyecto:** El proyecto no se elimina de sus **Proyectos en los que estoy** en el área Proyectos . El proyecto se elimina de las listas de todos los demás usuarios que filtran para ese proyecto mediante el campo Introducido por .
* **Si el usuario es el propietario o el patrocinador del proyecto:** El usuario permanece en sus funciones como patrocinador o propietario del proyecto.

## Eliminar usuarios de un proyecto y del equipo del proyecto

Puede quitar usuarios de un proyecto eliminándolos del equipo del proyecto.

Cuando los usuarios cumplen funciones en un proyecto, pasan a formar parte del equipo del proyecto.

Cuando elimina a los usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Para obtener información sobre las funciones de los usuarios en un proyecto, consulte [Administrar el equipo del proyecto](../planning-a-project/manage-project-team.md).

Para eliminar usuarios del equipo del proyecto:

1. Vaya al proyecto donde desee eliminar a los usuarios.

1. Haga clic en **People** en el panel izquierdo, seleccione los usuarios que desee eliminar. Es posible que tenga que hacer clic en **Mostrar más**, luego **People**.

1. Haga clic en el **Eliminar** icono  ![Quitar elemento](assets/remove-icon---x-in-circle.png) en la parte superior de la lista de usuarios.

1. Haga clic en **Sí, Eliminar usuarios seleccionados** para confirmar la eliminación.

   Los usuarios se eliminan del equipo del proyecto y de cualquier tarea o problema incompleto al que puedan asignarse. Ya no reciben notificaciones destinadas al equipo del proyecto.
