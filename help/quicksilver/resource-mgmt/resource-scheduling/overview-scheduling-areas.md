---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Descripción general de las áreas de programación
description: Las secciones siguientes describen dónde puede acceder al área de programación dentro de Adobe Workfront, así como la funcionalidad disponible en el área de programación.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Descripción general de las áreas de programación

>[!IMPORTANT]
>  
><span class="preview">La funcionalidad Programación descrita en este artículo se ha desaprobado y eliminado de Adobe Workfront a partir de la versión 23.1 de enero de 2023.   </span>
>  
> <span class="preview"> Este artículo también se eliminará poco después de la versión 23.1, a principios de 2023. En este momento, le recomendamos que actualice los marcadores según corresponda. </span>
> 
><span class="preview"> Ahora puede utilizar el equilibrador de carga de trabajo para programar el trabajo para sus recursos. </span>
>  
> <span class="preview">Para obtener información sobre la programación de recursos mediante el equilibrador de carga de trabajo, consulte la sección [El equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--  

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


Las secciones siguientes describen dónde puede acceder al área de programación dentro de Adobe Workfront, así como la funcionalidad disponible en el área de programación.

## Áreas de Workfront que le permiten programar recursos

Puede programar recursos en las siguientes áreas de Workfront:

* **Para cualquier proyecto para el que sea el gestor de recursos** (desde el **Programación** ) El área Programación de Workfront permite a los administradores de recursos realizar asignaciones de recursos en varios proyectos.

* **Para un proyecto individual cuando es miembro del equipo del proyecto** (desde el **Programación** área de un proyecto):

   El área Programación de un proyecto permite a los miembros del equipo del proyecto asignar el trabajo del proyecto a los usuarios del equipo del proyecto.

* **Para un equipo individual, usted es miembro de** (desde el **Programación** sección del equipo) La sección Programación de un equipo permite que los integrantes del equipo asignen el trabajo ya asignado al equipo desde varios proyectos a integrantes individuales del equipo.

## Funcionalidad disponible en el área Programación

El área de programación muestra tareas y problemas y asignaciones de recursos actuales.\
![resource_scheduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Herramientas de filtrado e intercambio](#filter-and-swap-tools)
* [Selección de fecha](#date-selection)
* [Área no asignada](#unassigned-area)
* [Usuarios y funciones](#users-and-roles)
* [Calendario de programación](#scheduling-timeline)

### Herramientas de filtrado e intercambio {#filter-and-swap-tools}

* **Herramienta Filtro:** Permite filtrar el contenido que se muestra en la cronología de programación. Para obtener más información sobre el uso de la herramienta Filtro, consulte [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Intercambiar herramienta:** (Disponible solo cuando se programan recursos para proyectos desde la pestaña Programación o Plantilla ) Permite asignar, intercambiar o desasignar rápidamente usuarios a tareas en varios proyectos. Para obtener más información, consulte [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Selección de fecha {#date-selection}

Puede ajustar el intervalo de fechas para el cual se muestran los datos en la cronología de la programación. De forma predeterminada, el intervalo de fechas es de 2 semanas (14 días consecutivos, incluidos los fines de semana) a partir del día actual.

### Área no asignada {#unassigned-area}

* [Al programar recursos como administrador de recursos (para varios proyectos en el área Programación)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Al programar recursos como miembro del equipo del proyecto (de un proyecto)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Al programar recursos como miembro del equipo (de un equipo)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Al programar recursos como administrador de recursos (para varios proyectos en el área Programación) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

La variable **No asignado** en la cronología de programación solo se muestran las tareas y los problemas que cumplen todos los criterios siguientes:

* No está asignado a un usuario.
* No está asignado a un equipo.\
   Si la tarea o el problema está asignado a un equipo, se seguirá mostrando en la **No asignado** área si la tarea o el problema también está asignado a una función además de la asignación de equipo.\
   Si las tareas o los problemas tienen asignaciones de funciones adicionales que un usuario no está cumpliendo, también se muestran.\
   Por ejemplo, una tarea se asigna a 3 funciones de trabajo: Designer, Product Manager y Developer. Asigne esta tarea al usuario A que tiene una función de trabajo de Designer y al usuario B que tiene una función de trabajo de Product Manager. En este escenario, la tarea sigue visible en el área No asignado de la cronología de programación, ya que la función de trabajo de desarrollador no está asignada a un usuario.

#### Al programar recursos como miembro del equipo del proyecto (de un proyecto) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

La variable **No asignado** en la parte superior de la cronología de programación, se muestran las tareas y los problemas que cumplen los siguientes criterios:

* Se asocia al proyecto pero no se asigna a ningún usuario del equipo del proyecto.\
   Las tareas asociadas al proyecto y asignadas a un usuario del equipo del proyecto se muestran en la fila del usuario al que se asignan las tareas.
* Se asocia al proyecto pero se asigna a un miembro que no está en el equipo del proyecto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **Al programar recursos como miembro del equipo (de un equipo)** {#when-scheduling-resources-as-a-team-member-from-a-team}

La variable **No asignado** en la parte superior de la cronología de programación, se muestran las tareas y los problemas que cumplen los siguientes criterios:

* Se asigna al equipo y a ningún otro usuario del equipo.\
   Las tareas asignadas tanto al equipo como a un usuario del equipo se muestran en la fila del usuario al que se asignan las tareas.
* Se asigna tanto al equipo como a un usuario que no es miembro del equipo.

### Usuarios y funciones {#users-and-roles}

* [Al programar recursos como administrador de recursos (para varios proyectos en el área Programación)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Al programar recursos como miembro del equipo del proyecto (de un proyecto)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Al programar recursos como miembro del equipo (de un equipo)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Al programar recursos como administrador de recursos (para varios proyectos en el área Programación) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Todos los usuarios que cumplen los requisitos para que se les asigne una de las tareas no asignadas se encuentran debajo de la variable **No asignado** . Los usuarios están disponibles en la cronología de programación para que se les asigne una tarea o un problema en las siguientes circunstancias:

* De forma predeterminada, los usuarios se muestran en la cronología de la programación solo cuando tienen una función de trabajo definida en el sistema (la función de trabajo principal o una función de trabajo secundaria) y esa función de trabajo coincide con la función de trabajo asignada a una tarea o problema que actualmente está visible en la **No asignado** en la línea de tiempo de programación. Puede deshabilitar esta funcionalidad para permitir que se asignen tareas y problemas a cualquier usuario, independientemente de si ese usuario tiene una función definida en su perfil de usuario que coincida con la asignación de funciones de la tarea o el problema que se les está asignando. Para obtener más información, consulte [Permitir asignaciones de usuarios independientemente de la función y la pertenencia a grupos en las áreas de programación](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   Un usuario y las tareas asignadas al usuario pueden aparecer varias veces en la cronología de la programación si el usuario tiene varias funciones de trabajo designadas en el sistema Workfront.\
   Los usuarios permanecen en la cronología de programación después de que se les asigne una tarea o un problema, incluso si no quedan tareas o problemas que tengan una asignación de función coincidente. Esto le permite realizar los cambios necesarios una vez asignados.\
   Si la tarea no está asignada a una función de trabajo, se muestran todos los usuarios que cumplen los requisitos del filtro. Para obtener más información sobre el filtro, consulte [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* Se han designado en el **Usuarios** en el campo **Filtro** pestaña .\
   Para obtener más información sobre el filtro, consulte [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   Al programar recursos para un equipo (en la ficha Trabajar en ), también se muestra la asignación de equipo.

Cualquier otra tarea o problema asignado a esos usuarios también se muestra en la cronología.

Puede ver el nivel en el que se asignan los usuarios en un día determinado, tal como se describe en [Administrar asignaciones de usuario en las áreas de programación](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Las tareas que no tienen al menos permisos de Contribute se muestran como una barra gris en la cronología de programación.

#### Al programar recursos como miembro del equipo del proyecto (de un proyecto) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Cada miembro del equipo se muestra siempre en la cronología de la programación, independientemente de las asignaciones de funciones de los usuarios y las asignaciones de funciones de las tareas en el área No asignado.

Si un usuario tiene varias funciones de trabajo definidas en el sistema, el usuario aparece varias veces en la cronología de programación cuando se cumple cualquiera de los siguientes criterios:

* Hay tareas o problemas que se muestran en la sección **No asignado** que están asignadas a las funciones de trabajo asociadas al usuario.
* Hay tareas o problemas en el proyecto que tienen asignadas funciones de trabajo, y esas tareas o problemas se asignan a un usuario que tiene esa función de trabajo definida en el sistema.

#### Al programar recursos como miembro del equipo (de un equipo) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Cada miembro del equipo se muestra siempre en la cronología de la programación, independientemente de las asignaciones de funciones de los usuarios y las asignaciones de funciones de las tareas en el área No asignado.

Puede ver el nivel en el que se asignan los usuarios en un día determinado, tal como se describe en [Administrar asignaciones de usuario en las áreas de programación](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Tareas que no tienen al menos permisos de Contribute para mostrarse como una barra gris en la cronología de programación.

### Calendario de programación {#scheduling-timeline}

* **Contenido predeterminado:** De forma predeterminada, todas las tareas que cumplan los requisitos definidos en la sección [Requisitos previos de tarea y problema](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) en el [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) en todos los proyectos con el estado actual se muestran en la cronología de la programación.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Para personalizar lo que se muestra en la cronología de la programación, incluida la visualización de problemas y proyectos con un estado diferente, utilice el filtro descrito en [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Se muestran un máximo de 10 tareas por día para un usuario determinado. Puede ampliar la lista para ver todas las tareas asignadas actualmente a ese usuario.

* **Tareas principales:** Si las tareas principales se muestran en la cronología depende de varias configuraciones. Para obtener más información, consulte la sección &quot;Configurar si las tareas principales se muestran en la cronología de programación&quot; en la [Configuración de las áreas de programación](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artículo.

* **Codificación de color:** Las tareas y los problemas de la cronología de la programación están codificados por colores según el proyecto al que pertenezcan. No se puede personalizar el color asociado a un proyecto específico.

   Al programar el trabajo para los equipos (en la pestaña Dotación de personal), los colores solo se utilizan si se usa la variable **Mostrar todas las tareas del usuario** está activada. Para obtener más información, consulte la sección &quot;Configurar si las tareas principales se muestran en la cronología de programación&quot; en la sección [Configuración de las áreas de programación](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artículo.

* **Duraciones de las tareas:** Las duraciones de la tarea se representan en la cronología de cada tarea (la tarea abarca físicamente el número de días igual a la duración). No se puede ajustar la duración de la tarea desde la cronología de programación.

* **Tiempo de espera:** El tiempo de espera se representa en la cronología de la programación mediante un indicador gris claro en la columna del día en el que el tiempo de espera está programado para un usuario determinado.\
   El tiempo de espera se configura para cada usuario en función de la siguiente información:

   Calendario personal del usuario. Para obtener más información sobre el calendario de tiempo de espera personal, consulte [Configuración del tiempo de espera personal en Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   La programación asignada al usuario. Puede ser la programación predeterminada o una programación personalizada. Para obtener más información sobre las programaciones, consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Fines de semana:** Los fines de semana se representan en la cronología de programación como sombreado gris claro los sábados y domingos. Los días de la semana que se establecen como fines de semana en la cronología de programación no se pueden configurar. Puede programar usuarios para que trabajen los fines de semana.
