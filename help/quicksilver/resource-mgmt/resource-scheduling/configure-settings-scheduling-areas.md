---
product-area: resource-management;setup
navigation-topic: resource-scheduling
title: Configuración de las áreas de programación
description: Se pueden configurar varias opciones para personalizar el modo y la información que se muestra en la cronología de la programación.
author: Alina
feature: Resource Management
exl-id: d76b59c0-d0fd-4698-8017-fa0778f61dc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2280'
ht-degree: 1%

---

# Configuración de las áreas de programación

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.</span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Se pueden configurar varias opciones para personalizar el modo y la información que se muestra en la cronología de la programación.

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a Proyectos, tareas y problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superior para proyectos, tareas y problemas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configuración de problemas para mostrar en la cronología de programación

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALL THE SECTIONS BELOW ARE LINKED TO PRODUCT. DO NOT CHANGE TITLES) </p>
-->

Puede configurar los problemas que se mostrarán además de las tareas en la cronología de la programación.\
Al programar recursos en la sección Programación de un equipo , los problemas se muestran de forma predeterminada, además de las tareas. Al programar recursos para proyectos, solo se muestran las tareas de forma predeterminada.

1. Vaya a la cronología de programación de varios proyectos, de un proyecto individual o de un equipo:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un equipo**: Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.

1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración de programación de recursos, active la variable **Mostrar problemas** .\
   ![RS_scheduling_tab_all_settings__1_.png](assets/rs-scheduling-tab-all-settings--1--350x417.png)

1. Haga clic en **Volver a la programación**. 

## Configurar el trabajo completado para que se muestre en la cronología de programación

Puede configurar la cronología de programación para mostrar el trabajo que ya se ha marcado como Completado. De forma predeterminada, el trabajo completado no se muestra en la cronología de la programación. 

1. Vaya a la cronología de programación de varios proyectos, de un proyecto individual o de un equipo:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un equipo**: Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.

1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración de programación de recursos, active la variable **Mostrar trabajo completado** .\
   ![RSS_show_completed_work_disabled__1_.png](assets/rss-show-completed-work-disabled--1--350x336.png)

1. Haga clic en **Volver a la programación**.\
   El trabajo completado se muestra con una marca de verificación en la esquina superior derecha del elemento de trabajo.

## Configurar nombres de proyectos para que aparezcan en la cronología de programación 

Puede configurar el nombre del proyecto para que se muestre en cada tarea y problema en la cronología de programación. Esto permite a los usuarios que ven la cronología de la programación ver rápidamente el nombre del proyecto en el que reside la tarea o el problema.

Cuando se habilitan los nombres de los proyectos para que se muestren, cada tarea y problema consume más espacio vertical en la cronología de programación, lo que da como resultado que se muestren menos tareas y problemas en una sola vista.

De forma predeterminada, los nombres de los proyectos no se muestran en las tareas ni en los problemas de la cronología de la programación.

Para mostrar los nombres de los proyectos en las tareas y los problemas en la cronología de la programación:

1. Vaya a la cronología de programación de varios proyectos o de un equipo:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un equipo**: Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.

1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración de programación de recursos, active la opción, **Mostrar nombres de proyecto**.\
   ![RS_scheduling_tab_all_settings__2_.png](assets/rs-scheduling-tab-all-settings--2--350x348.png)

1. Haga clic en **Volver a la programación**.\
   Cada tarea y problema de la cronología de la programación muestra el nombre del proyecto en el que reside la tarea o el problema.\
   ![resourcescheduling_projectnames.png](assets/resourcescheduling-projectnames-350x200.png)

## Configurar fechas proyectadas para que se muestren en la cronología de programación

De forma predeterminada, las fechas previstas se utilizan en la cronología de programación. Como alternativa, puede configurar la cronología de programación para utilizar Fechas proyectadas.

Tenga en cuenta la siguiente información sobre fechas planificadas y previstas:

* Las fechas planificadas para las tareas se pueden configurar manualmente o automáticamente, según la restricción de tarea y el tipo de duración. Para obtener más información, consulte los artículos [Información general sobre la restricción de tareas](../../manage-work/tasks/task-constraints/task-constraint-overview.md) y  [Información general sobre la duración y el tipo de duración de la tarea](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

   Las fechas planificadas para problemas se establecen manualmente en los problemas por parte de los usuarios. Sin embargo, el administrador del sistema puede impedir que los usuarios ajusten las fechas planeadas para solucionar problemas.

* Las fechas proyectadas para las tareas y los problemas se establecen automáticamente. Para obtener más información sobre las fechas proyectadas, consulte los artículos [Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas](../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

>[!NOTE]
>
>Al utilizar Fechas proyectadas en la cronología de programación, no se puede mostrar la información de asignación de usuarios. Para obtener más información sobre las asignaciones de usuarios, consulte el artículo [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

Para configurar la cronología de programación de modo que muestre las tareas y los problemas según las Fechas proyectadas: 

1. Vaya a la cronología de programación de varios proyectos, de un proyecto individual o de un equipo:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un equipo**: Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.

1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración de programación de recursos, desactive la **Usar fechas planificadas en lugar de fechas proyectadas** .
1. Haga clic en **Volver a la programación**.

## Configurar cómo se muestran los usuarios en la cronología de programación

>[!NOTE]
>
>Esta sección solo se aplica cuando se programan recursos para equipos (en la sección Programación de un equipo ). Cuando se programan recursos para varios proyectos (en la ficha Programación) o para un solo proyecto (en la ficha Dotación de personal), los usuarios no se pueden mostrar alfabéticamente; siempre están organizados por rol.

Al programar recursos para un equipo, puede configurar los usuarios para que se muestren en la cronología de la programación alfabéticamente o por función. De forma predeterminada, los usuarios se muestran alfabéticamente (las funciones no se muestran).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en Equipos. Un equipo está seleccionado de forma predeterminada.

1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración, seleccione si desea habilitar la variable **Agrupar por función** .\
   Cuando se deshabilita esta opción, los usuarios se muestran en orden alfabético y las funciones no se muestran en la cronología de programación.\
   Cuando esta opción está habilitada, las funciones se muestran en la cronología de la programación y los usuarios se agrupan dentro de su función respectiva. Si un usuario determinado tiene varias funciones definidas en el sistema, ese usuario aparece varias veces en la cronología de programación, debajo de cada función adecuada.\
   ![RS_working_on_team_scheduling_full_settings__1_.png](assets/rs-working-on-team-scheduling-full-settings--1--350x348.png)

1. Haga clic en **Volver a la programación**.

## Configure si las tareas principales se muestran en la cronología de programación

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!! - Resource Scheduling (People> Scheduling>Settings>Show Parent Tasks tooltip)</p>
-->

Las tareas principales se muestran de forma diferente en función de la cronología de programación a la que acceda. 

* [Mostrar tareas principales para varios proyectos](#display-parent-tasks-for-multiple-projects)
* [Mostrar las tareas principales de un proyecto o equipo](#display-parent-tasks-for-a-project-or-a-team)

### Mostrar tareas principales para varios proyectos {#display-parent-tasks-for-multiple-projects}

Al programar recursos para varios proyectos en la sección Programación , si las tareas principales se muestran o no depende de la siguiente configuración:

* Modo de finalización del proyecto.
* Modo de finalización de resumen del proyecto.
* La configuración Mostrar tareas principales de la ficha Programación.

La siguiente tabla describe cuándo se muestran las tareas principales en la ficha Programación y cuándo solo se muestran las subtareas. 

| **Mostrar configuración de tareas principales** | **Modo de finalización del proyecto** | **Modo de finalización de resumen del proyecto** | **Tipo de tareas mostradas en la línea de tiempo de programación** |
|---|---|---|---|
| Deshabilitado | Manual | Automático | Solo subtareas |
| Deshabilitado | Manual | Manual | Solo subtareas |
| Deshabilitado | Automático | Automático | Solo subtareas |
| Deshabilitado | Automático | Manual | Solo subtareas |
| Habilitado | Automático | Manual | Subtareas y tareas principales |
| Habilitado | Automático | Automático | Solo subtareas |
| Habilitado | Manual | Manual | Subtareas y tareas principales |
| Habilitado | Manual | Automático | Solo subtareas |

Para obtener información sobre cómo configurar la variable **Modo de finalización** y **Modo de finalización de resumen** para cada proyecto, consulte la sección &quot;Configuración&quot; en el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

Puede configurar manualmente la configuración Mostrar tareas principales en la sección Programación de varios proyectos. 

Para configurar la configuración Mostrar tareas principales : 

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración de programación de recursos, seleccione si desea habilitar la opción, **Mostrar tareas principales.**
Cuando esta opción está habilitada, las tareas principales de todos los proyectos se muestran según la configuración del modo de finalización del resumen y del modo de finalización de los proyectos, como se describe en la tabla anterior. Esta opción está activada de forma predeterminada.
\
   ![RS_scheduling_tab_all_settings__3_.png](assets/rs-scheduling-tab-all-settings--3--350x348.png)

1. Haga clic en **Volver a la programación** en la esquina inferior izquierda.

### Mostrar las tareas principales de un proyecto o equipo {#display-parent-tasks-for-a-project-or-a-team}

Al programar los recursos en la sección Dotación de personal de un proyecto o en la sección Programación , si se muestran o no las Tareas principales depende de la siguiente configuración:

* Modo de finalización del proyecto.
* Modo de finalización de resumen del proyecto.

Para obtener información sobre cómo configurar la variable **Modo de finalización** y **Modo de finalización de resumen** para cada proyecto, consulte la sección &quot;Configuración&quot; en el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

La siguiente tabla describe cuándo se muestran las tareas principales en la sección Personal de un proyecto o en la sección Programación y cuándo solo se muestran las subtareas. 

| Modo de finalización del proyecto | Modo de finalización de resumen del proyecto | Tipo de tareas que se muestran en la sección Programación | Tipo de tareas mostradas en la sección Programación de equipos |
|---|---|---|---|
| Manual | Automático | Solo subtareas | Solo subtareas |
| Manual | Manual | Subtareas y tareas principales | Solo subtareas |
| Automático | Automático | Solo subtareas | Solo subtareas |
| Automático | Manual | Subtareas y tareas principales | Solo subtareas |
| Automático | Manual | Subtareas y tareas principales | Solo subtareas |
| Automático | Automático | Solo subtareas | Solo subtareas |
| Manual | Manual | Subtareas y tareas principales | Solo subtareas |
| Manual | Automático | Solo subtareas | Solo subtareas |

## Configure si las horas planificadas diarias se muestran en la cronología de programación

Para configurar la cronología de programación de modo que muestre los totales diarios de las horas planificadas para cada usuario: 

1. Vaya a la cronología de programación de varios proyectos, de un proyecto individual o de un equipo:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un equipo**: Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.

1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el cuadro de diálogo Configuración, habilite las siguientes opciones:

   *  **Mostrar totales por horas planificadas diarias**: Muestra el total de las horas planificadas diarias para cada usuario.
   * **Mostrar resaltado de asignación de recursos**: Destaca la asignación del usuario para tareas y problemas, así como los días en los que los usuarios están sobreasignados.\
      Estas opciones están desactivadas de forma predeterminada.\
      ![RS_all_settings__1_.png](assets/rs-all-settings--1--350x358.png)

1. Haga clic en **Volver a la programación**.\
   El total de horas planificadas asignadas al usuario se muestra para cada día.\
   Las horas planificadas para los días en los que el usuario está sobreasignado se resaltan en rojo.\
   Para obtener más información sobre las asignaciones de usuarios, consulte el artículo [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Configure si todas las tareas del usuario se muestran en la cronología de programación

>[!NOTE]
>
>Esta opción solo se aplica cuando se programan recursos para proyectos individuales (en la sección Programación del proyecto ). Esta opción no está disponible al programar recursos para varios proyectos (en la sección Programación ) o para equipos (en la sección Programación de un equipo ).

Para configurar si todas las tareas asignadas a cada usuario (no solo las tareas asociadas con el proyecto que está viendo) se muestran en la cronología de programación:

1. Vaya al proyecto en el que desea configurar la cronología de programación para mostrar todas las tareas asignadas a cada usuario.
1. Haga clic en el **Equilibrador de carga de trabajo** en el panel izquierdo (puede que se encuentre debajo de **Mostrar más**) y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en el **Configuración** en la cronología de la programación.

1. En el área Configuración , seleccione si desea habilitar la opción, **Mostrar todas las tareas del usuario**.\
   Cuando esta opción está habilitada, todas las tareas asignadas a cada usuario se muestran en la cronología de programación, independientemente del proyecto donde se encuentren las tareas.\
   Esta opción está desactivada de forma predeterminada.\
   ![RS_project_scheduling_area__1_.png](assets/rs-project-scheduling-area--1--350x340.png)

1. Haga clic en **Volver a la programación**.
