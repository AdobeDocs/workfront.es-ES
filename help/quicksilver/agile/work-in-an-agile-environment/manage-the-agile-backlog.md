---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Administrar el registro de pendientes de Agile
description: Las tareas y los problemas se pueden asignar a un equipo Agile y agregarse al registro de asuntos pendientes de ese equipo como historias, según la metodología Agile que utilice el equipo.
author: Jenny
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 7%

---

# Administrar el registro de asuntos pendientes Agile

Los siguientes elementos de trabajo se pueden asignar a un equipo Agile y añadirse al registro de asuntos pendientes de ese equipo como historias, según la metodología Agile que utilice el equipo:

* **[!UICONTROL Equipos Agile de Scrum]:** Las tareas y problemas se pueden asignar al equipo Agile y agregarse al registro de pendientes.
* **[!UICONTROL Equipos Agile Kanban]:** Se pueden asignar tareas al equipo Agile y agregarlas al registro de pendientes. Los usuarios pueden ver el registro de pendientes directamente desde el panel de historias Agile, tal como se describe en [[!UICONTROL Agregar el registro de pendientes] al panel Kanban](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). El equipo utiliza este registro de pendientes para priorizar y administrar su cola de trabajos.

Las tareas o problemas se pueden asignar al equipo (y posteriormente se agregarán al registro de asuntos pendientes del equipo) desde cualquier lugar de [!DNL Adobe Workfront]. Por ejemplo, a un solo equipo se le podrían asignar asignaciones de trabajo de varios proyectos.

>[!NOTE]
>
>Si añade varios equipos a un elemento de registro de asuntos pendientes, la tarea o el problema solo se mostrarán en el registro de asuntos pendientes del equipo principal. El equipo principal es el equipo que se ha asignado en primer lugar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso al proyecto en el que se encuentra la historia </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear y administrar historias en el registro de pendientes

* [Reordenar historias](#reorder-stories)
* [[!UICONTROL Desglosar] historias](#break-down-stories)
* [Editar historias](#edit-stories)

### Reordenar historias {#reorder-stories}

Puede reordenar las historias en la lista de trabajos pendientes mediante el método de arrastrar y soltar.

1. Vaya al registro de pendientes Agile donde desee reordenar las historias.
1. En el menú desplegable **[!UICONTROL Vista]**, seleccione la vista **[!UICONTROL Registro de pendientes]** o una vista personalizada que contenga la columna **[!UICONTROL Pedido]**.

   >[!NOTE]
   >
   >Si una tarea o un problema tiene un equipo Agile asignado y el proyecto no está en un estado equivalente a Actual, no se muestran en el registro de pendientes. Sin embargo, sí afectan al recuento de trabajos pendientes en la columna Pedido.

1. Seleccione uno o varios artículos y, a continuación, arrastre los artículos al orden en que desee que aparezcan en el registro de pendientes.
   ![Arrastrar y soltar elementos de registro de pendientes](assets/agile-backlog-drag-and-drop.png)

### Desglose de historias {#break-down-stories}

Dado que las historias de un registro de pendientes varían en tamaño, los usuarios pueden desglosarlas en tamaños viables para una iteración. Desglosar un artículo crea subtareas en la tarea que representa el artículo y reemplaza la tarea original en el registro de pendientes. Puede asignar una tarea principal o sus subtareas a un equipo Agile, pero no puede asignar ambas a un equipo simultáneamente.

>[!NOTE]
>
>Tenga en cuenta las siguientes limitaciones al desglosar las historias:
>
>* Solo se pueden desglosar las historias que representan tareas. No puede desglosar historias que representen problemas.
>* Las historias solo se pueden desglosar si están asociadas a un proyecto.


Para desglosar una historia:

1. Vaya al registro de pendientes que contiene la historia que desea desglosar.
1. Seleccione la historia que desee desglosar y, a continuación, haga clic en **[!UICONTROL Desglose de historia]**.
Se muestra el cuadro de diálogo [!UICONTROL Desglose de historia].
   ![Cuadro de diálogo Desglose de historia](assets/backlog-breakdown-dialog.png)

1. Especifique un nombre y una estimación para la historia y seleccione si la historia está lista.
1. Haz clic en **[!UICONTROL Agregar historia]** para crear otra historia a partir de la historia original.
1. Haga clic en **[!UICONTROL Guardar]**.

### Editar historias {#edit-stories}

Puede editar historias directamente desde las pestañas [!UICONTROL Historias] o [!UICONTROL Problemas] del registro de pendientes de la misma manera que editaría cualquier tarea o problema de un proyecto por lotes, tal como se describe en [Editar tareas por lotes](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) en [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md) y [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md).

## Crear nuevas historias en el registro de pendientes {#create-new-stories-on-the-backlog}

Puede crear nuevas historias en el registro de pendientes creando la historia directamente a partir del registro de pendientes o asignando una tarea o problema existente a un equipo Agile.

* [Crear una historia a partir del registro de pendientes](#create-a-story-from-the-backlog)
* [Asignar una tarea o un problema a un equipo Agile](#assign-a-task-or-issue-to-an-agile-team)

### Crear una historia a partir del registro de pendientes {#create-a-story-from-the-backlog}

Cuando crea una historia a partir del registro de pendientes, la historia se crea como una tarea o un problema dentro de un proyecto.

Para crear una historia a partir del registro de pendientes:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda y selecciónelo cuando aparezca.

1. Seleccione **[!UICONTROL Registro de pendientes]** en el panel izquierdo.
1. Realice una de las siguientes acciones, en función de si desea crear una tarea o un problema:

   * **Para crear una tarea:** Haga clic en **[!UICONTROL Historias]**.

   * **Para crear un problema:** Haga clic en **[!UICONTROL Problemas]**.

1. Haga clic en **[!UICONTROL Nueva historia]** o en **[!UICONTROL Nuevo problema]**.

1. Especifique la siguiente información:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nombre de artículo]</strong></td>
      <td> Escriba un nombre para la historia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>(Opcional) Escriba una descripción para la historia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Seleccione si el artículo está listo para añadirse a una iteración. Esta configuración es solo informativa. Las historias se pueden agregar a una iteración independientemente del estado de esta configuración.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Especifique un punto o una estimación horaria para la historia. Las estimaciones afectan al gráfico de evolución. El gráfico de evolución de una iteración sólo es preciso si cada artículo contiene una estimación precisa. (Si proporciona una estimación de puntos, ya debe haber designado en la configuración del equipo cuántas horas representa cada punto).</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Empiece a escribir el nombre del proyecto donde se creará esta historia y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.<br>El estado del proyecto debe establecerse en [!UICONTROL Actual]. Si el estado del proyecto es cualquier cosa excepto [!UICONTROL Actual], no se muestra en el menú desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>(Opcional) Comience a escribir el nombre de la tarea principal a la que está subordinada esta historia y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Opcional) Seleccione los formularios personalizados que desee agregar a este artículo.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Guardar historia]**.

### Asignar una tarea o un problema a un equipo Agile {#assign-a-task-or-issue-to-an-agile-team}

Puede asignar una tarea o un problema a un equipo Agile. Una vez asignada, la tarea o el problema aparecen como una nueva historia en el registro de asuntos pendientes del equipo.

Para asignar una tarea o un problema a un equipo Agile:

1. Vaya al proyecto que contiene la tarea que desea asignar.
1. Seleccione la tarea o el problema en la lista.
1. Haga clic en **[!UICONTROL Editar]**.
1. Haga clic en **[!UICONTROL Asignaciones]**.
1. (Opcional) Elimine los usuarios asignados existentes.
1. Haga clic en **[!UICONTROL Agregar usuario asignado]**.
1. Comience a escribir el nombre del equipo Agile que desea que se le asigne a la tarea o al problema y, a continuación, haga clic en el nombre del equipo cuando aparezca en la lista desplegable.
1. Haga clic en **[!UICONTROL Guardar cambios]**.
La tarea o el problema ya están disponibles en el registro de pendientes del equipo.

## Mover historias dentro o fuera del registro de pendientes

* [Mover historias del registro de pendientes a una iteración o tablero](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Mover las historias existentes al registro de pendientes](#move-existing-stories-to-the-backlog)
* [Exportar historias del registro de pendientes](#export-stories-from-the-backlog)

### Mover historias del registro de pendientes a una iteración o tablero

1. Vaya al registro de pendientes del equipo Agile.
1. Seleccione las historias que desee mover a una iteración o panel Kanban y, a continuación, haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.
Si se mueve la historia al tablero [!UICONTROL Kanban], se mostrará la historia [!UICONTROL Mover historia al tablero Kanban].
Si se mueve la historia a una iteración, aparecerá el cuadro de diálogo [!UICONTROL Mover historia a una iteración].
   ![Cuadro de diálogo Mover historia](assets/agile-backlog-addtoiteration.png)

1. Realice una de las siguientes acciones:

   * **Para equipos de Scrum:** En el campo **[!UICONTROL Seleccionar iteración]**, seleccione la iteración a la que desea mover las historias.

   * **Para equipos Kanban:** En el campo **[!UICONTROL Seleccionar Panel Kanban]**, seleccione el tablero [!UICONTROL Kanban] de su equipo. (Los equipos Kanban solo pueden tener un tablero [!UICONTROL Kanban]).

1. Haga clic en **[!UICONTROL Mover historia]**.

### Mover las historias existentes al registro de pendientes {#move-existing-stories-to-the-backlog}

Si decide que su equipo aún no está listo para trabajar en una historia, puede mover la historia al registro de pendientes.

Para obtener más información, consulte [Mover una historia Agile](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exportar historias del registro de pendientes {#export-stories-from-the-backlog}

Puede exportar uno o más artículos (incluidas las tareas y los problemas) directamente desde el registro de pendientes.

Exporta historias del registro de pendientes de la misma manera que exporta otros datos de [!DNL Workfront], tal como se describe en [Exportar datos](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
