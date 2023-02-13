---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Asignación manual de tareas y problemas no asignados en las áreas de programación
description: Con la cronología de programación, puede administrar las asignaciones de usuario, además de especificar cuánto tiempo se asigna a cada usuario para un elemento de trabajo.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Asignación manual de tareas y problemas no asignados en las áreas de programación

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Con la cronología de programación, puede administrar las asignaciones de usuario, además de especificar cuánto tiempo se asigna a cada usuario para un elemento de trabajo.

## Requisitos de acceso

Debe tener lo siguiente:

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver o tener más acceso a Proyectos, Tareas y Problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute para proyectos, tareas y problemas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos para asignar tareas y problemas en la cronología de programación

Antes de empezar a administrar las asignaciones de usuarios como se describe en esta sección, familiarícese con el funcionamiento de la programación de recursos en Workfront, tal como se describe en [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Para administrar correctamente las asignaciones de usuario como se describe en esta sección, primero debe asegurarse de que usted, sus proyectos y sus tareas y problemas cumplan los requisitos previos descritos en la sección [Requisitos previos para utilizar las herramientas de programación en Workfront](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) sección del artículo [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Las secciones siguientes describen cómo modificar las asignaciones de usuario de forma manual, automática o mediante el intercambio de asignaciones por usuario o función.

## Asignación manual de tareas o problemas no asignados a usuarios

La cronología de programación proporciona la visibilidad necesaria sobre qué usuarios son capaces de completar la tarea o el problema.\
Para obtener más información sobre la cronología de programación, consulte [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Puede asignar tareas y problemas individuales a los usuarios en la cronología de programación desde las siguientes áreas de Workfront:

* La sección Programación en Recursos (al programar recursos para varios proyectos).
* La sección Programación de un proyecto (al programar recursos para un solo proyecto).
* La sección Programar de un equipo (al programar recursos para un equipo).

La información mostrada en el área No asignado en la parte superior de la cronología de programación difiere según el área de Workfront donde esté utilizando la programación de recursos (ya sea en la sección Programación (al programar recursos para varios proyectos), en la sección Programación (al programar recursos para un único proyecto) o en la sección Programación (al programar recursos para un equipo). Para obtener más información, consulte la sección [Funcionalidad disponible en el área Programación](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) en el artículo [Descripción general de las áreas de programación](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Según el área de Workfront en la que esté viendo la cronología de la programación, solo algunos usuarios pueden ser asignados al trabajo. Para obtener más información, consulte [Descripción general de las áreas de programación](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Para asignar tareas o problemas no asignados a usuarios en la cronología de programación:

1. Vaya a la cronología de programación de varios proyectos, de un proyecto individual o de un equipo:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un equipo**: Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. (Opcional) Cree un filtro para personalizar qué contenido se muestra en la cronología de programación, tal como se describe en [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). Por ejemplo, para que los problemas se muestren en la cronología de programación, debe crear un filtro.

1. (Opcional) Modifique el intervalo de fechas que se muestra en la cronología de programación, tal como se describe en [Ajustar el intervalo de fechas de las áreas de programación](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) en [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. Haga lo siguiente para asignar una tarea o problema sin asignar:

   * Arrastre la tarea o el problema a la fila del usuario que desee asignar.\
      Se muestran un máximo de 10 tareas por día para un usuario determinado. Puede ampliar la lista para ver todas las tareas asignadas actualmente a ese usuario. (Después de realizar asignaciones en la cronología de programación, es posible que se muestren más de 10 tareas de forma temporal).\
      Al arrastrar un elemento, se muestra la siguiente información antes de soltar la tarea o el problema y de completar la asignación:

   * Si las asignaciones de usuario están habilitadas en la cronología de programación, se muestran los indicadores rojos de sobreasignación si se completa la asignación, lo que hace que el usuario esté sobreasignado.\
      Para obtener más información sobre los indicadores de sobreasignación, consulte la sección [Indicadores de asignación](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) en el artículo [Administrar asignaciones de usuario en las áreas de programación](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      Si la variable **Limitar asignaciones a usuarios con una función coincidente** está activada en el área Configuración , los usuarios que no cumplen los requisitos para recibir la asignación aparecen atenuados. Si esta opción está desactivada, todos los usuarios están disponibles para recibir la asignación. La opción está activada de forma predeterminada.\
      Para obtener más información sobre esta opción, consulte [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) en [Permitir asignaciones de usuarios independientemente de la función y la pertenencia a grupos en las áreas de programación](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      Se muestra un indicador de colocación en la fila del usuario. Esto permite ver dónde se asigna un elemento antes de realizar la asignación.

      Expanda la tarea o el problema que desee asignar, haga clic en la flecha desplegable en la **Asignaciones** , empiece a escribir el nombre del usuario que desea asignar y, a continuación, haga clic en el nombre del usuario en la lista desplegable.\
      ![schedule_task_expand.png](assets/schedule-task-expanded-350x170.png)

1. (Condicional) Después de asignar una tarea o un problema no asignado a un usuario, es posible que desee ajustar las asignaciones existentes para tareas y problemas entre los usuarios en la cronología de programación. Al programar recursos para proyectos (ya sea en la ficha Programación o en la pestaña Dotación de personal), solo los usuarios que tengan la misma función de trabajo pueden recibir la asignación.\
   Para volver a asignar una tarea o un problema a otro usuario, arrastre la tarea desde la fila de un usuario a la fila de otro usuario.
1. (Opcional) Configure el número de horas que cada usuario asignado se asigna a la tarea o problema, tal como se describe en [Administrar asignaciones de usuario en las áreas de programación](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
