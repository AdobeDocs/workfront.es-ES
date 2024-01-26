---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Administrar el registro de pendientes Agile
description: Las tareas y los problemas se pueden asignar a un equipo Agile y agregarse al registro de asuntos pendientes de ese equipo como historias, según la metodología Agile que utilice el equipo.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 3c7bdcc1dc2a3a0db62a175ec11d4d6701acbb53
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 0%

---

# Administrar el registro de pendientes Agile

Los siguientes elementos de trabajo se pueden asignar a un equipo Agile y añadirse al registro de asuntos pendientes de ese equipo como historias, según la metodología Agile que utilice el equipo:

* **[!UICONTROL Equipos de Scrum Agile]:** Las tareas y los problemas se pueden asignar al equipo Agile y se pueden agregar al registro de pendientes.
* **[!UICONTROL Equipos Agile de Kanban]:** Las tareas se pueden asignar al equipo Agile y se pueden agregar al registro de pendientes. Los usuarios pueden ver el registro de pendientes directamente desde el panel de historias Agile, tal como se describe en [[!UICONTROL Agregar el registro de pendientes] al Panel Kanban](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). El equipo utiliza este registro de pendientes para priorizar y administrar su cola de trabajos.

Las tareas o problemas se pueden asignar al equipo (y posteriormente se pueden agregar al registro de asuntos pendientes del equipo) desde cualquier lugar de [!DNL Adobe Workfront]. Por ejemplo, a un solo equipo se le podrían asignar asignaciones de trabajo de varios proyectos.

>[!NOTE]
>
>Si agrega varios equipos a un elemento de registro de asuntos pendientes, la tarea o el problema solo se mostrarán en el registro de asuntos pendientes del equipo principal. El equipo principal es el equipo asignado en primer lugar.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Worker] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] al proyecto en el que se encuentra la historia</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Crear y administrar historias en el registro de pendientes

* [Reordenar historias](#reorder-stories)
* [[!UICONTROL Desglose] historias](#break-down-stories)
* [Editar historias](#edit-stories)

### Reordenar historias {#reorder-stories}

Puede reordenar las historias en la lista de trabajos pendientes mediante el método de arrastrar y soltar.

1. Vaya al registro de pendientes Agile donde desee reordenar las historias.
1. En el **[!UICONTROL Ver]** menú desplegable, seleccione la opción **[!UICONTROL Registro Pendiente]** vista o una vista personalizada que contenga la variable **[!UICONTROL Pedido]** columna.

   >[!NOTE]
   >
   >Si una tarea o un problema tiene un equipo Agile asignado y el proyecto no está en un estado equivalente a Actual, no se muestran en el registro de pendientes. Sin embargo, sí afectan al recuento de trabajos pendientes en la columna Pedido.

1. Seleccione uno o varios artículos y, a continuación, arrastre los artículos al orden en que desee que aparezcan en el registro de pendientes.\
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
1. Seleccione la historia que desea desglosar y haga clic en **[!UICONTROL Desglose de historia]**.\
   El [!UICONTROL Desglose de historia] Cuadro de diálogo.\
   ![Cuadro de diálogo Desglose de historia](assets/backlog-breakdown-dialog.png)

1. Especifique un nombre y una estimación para la historia y seleccione si la historia está lista.
1. Clic **[!UICONTROL Agregar historia]** para crear otra historia a partir de la historia original.
1. Haga clic en **[!UICONTROL Guardar]**.

### Editar historias {#edit-stories}

Puede editar historias directamente desde el [!UICONTROL Historias] o [!UICONTROL Problemas] Fichas del registro de pendientes como editaría las tareas o problemas de un proyecto de forma masiva, tal como se describe en [Editar tareas de forma masiva](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) in [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md), y [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md).

## Crear nuevas historias en el registro de pendientes {#create-new-stories-on-the-backlog}

Puede crear nuevas historias en el registro de pendientes creando la historia directamente a partir del registro de pendientes o asignando una tarea o problema existente a un equipo Agile.

* [Crear una historia a partir del registro de pendientes](#create-a-story-from-the-backlog)
* [Asignar una tarea o un problema a un equipo Agile](#assign-a-task-or-issue-to-an-agile-team)

### Crear una historia a partir del registro de pendientes {#create-a-story-from-the-backlog}

Cuando crea una historia a partir del registro de pendientes, la historia se crea como una tarea o un problema dentro de un proyecto. No puede crear una historia a partir del registro de pendientes como un problema.

Para crear una historia a partir del registro de pendientes:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda y selecciónelo cuando aparezca.

1. Seleccionar **[!UICONTROL Registro Pendiente]** en el panel izquierdo.
1. Realice una de las siguientes acciones, en función de si desea crear una tarea o un problema:

   * **Para crear una tarea:** Clic **[!UICONTROL Historias]**.

   * **Para crear una incidencia:** Clic **[!UICONTROL Problemas]**.

1. Clic **[!UICONTROL Nueva historia]** o **[!UICONTROL Nuevo problema]**.

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
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong></td>
      <td>(Opcional) Escriba una descripción para la historia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Seleccione si el artículo está listo para añadirse a una iteración. Esta configuración es solo informativa. Las historias se pueden agregar a una iteración independientemente del estado de esta configuración.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimar]</strong></td>
      <td>Especifique un punto o una estimación horaria para la historia. Las estimaciones afectan al gráfico de evolución. El gráfico de evolución de una iteración sólo es preciso si cada artículo contiene una estimación precisa. (Si proporciona una estimación de puntos, ya debe haber designado en la configuración del equipo cuántas horas representa cada punto).</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Proyecto principal]</strong></td>
      <td>Empiece a escribir el nombre del proyecto donde se creará esta historia y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.<br>El estado del proyecto debe establecerse en [!UICONTROL Actual]. Si el estado del proyecto es cualquier cosa excepto [!UICONTROL Actual], no se muestra en el menú desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarea principal]</strong></td>
      <td>(Opcional) Comience a escribir el nombre de la tarea principal a la que está subordinada esta historia y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Opcional) Seleccione los formularios personalizados que desee agregar a este artículo.</td>
     </tr>
    </tbody>
   </table>

1. Clic **[!UICONTROL Guardar historia]**.

### Asignar una tarea o un problema a un equipo Agile {#assign-a-task-or-issue-to-an-agile-team}

Puede asignar una tarea o un problema a un equipo Agile. Una vez asignada, la tarea o el problema aparecen como una nueva historia en el registro de asuntos pendientes del equipo.

Para asignar una tarea o un problema a un equipo Agile:

1. Vaya al proyecto que contiene la tarea que desea asignar.
1. Seleccione la tarea o el problema en la lista.
1. Clic **[!UICONTROL Editar]**.
1. Clic **[!UICONTROL Asignaciones]**.
1. (Opcional) Elimine los usuarios asignados existentes.
1. Clic **[!UICONTROL Agregar usuario asignado]**.
1. Comience a escribir el nombre del equipo Agile que desea que se le asigne a la tarea o al problema y, a continuación, haga clic en el nombre del equipo cuando aparezca en la lista desplegable.
1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   La tarea o el problema ya están disponibles en el registro de pendientes del equipo.

## Mover historias dentro o fuera del registro de pendientes

{#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Mover historias del registro de pendientes a una iteración o tablero +](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Mover las historias existentes al registro de pendientes](#move-existing-stories-to-the-backlog)
* [Exportar historias del registro de pendientes](#export-stories-from-the-backlog)

### Mover historias del registro de pendientes a una iteración o tablero +

1. Vaya al registro de pendientes del equipo Agile.
1. Seleccione las historias que desea mover a una iteración o panel Kanban y, a continuación, haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.\
   Si se mueve la historia a un [!UICONTROL Kanban] tablero, el [!UICONTROL Mover historia al Kanban] Se muestra el tablero.\
   Si mueve la historia a una iteración, la variable [!UICONTROL Mover historia a iteración] Cuadro de diálogo.\
   ![Cuadro de diálogo Mover historia](assets/agile-backlog-addtoiteration.png)

1. Realice una de las acciones siguientes:

   * **Para equipos de Scrum:** En el **[!UICONTROL Seleccionar iteración]** , seleccione la iteración a la que desee mover los artículos.

   * **Para equipos Kanban:** En el **[!UICONTROL Seleccionar Panel Kanban]** , seleccione su equipo [!UICONTROL Kanban] tablero. (Los equipos de Kanban solo pueden tener uno [!UICONTROL Kanban] tablero.)

1. Clic **[!UICONTROL Mover historia]**.

### Mover las historias existentes al registro de pendientes {#move-existing-stories-to-the-backlog}

Si decide que su equipo aún no está listo para trabajar en una historia, puede mover la historia al registro de pendientes.

Para obtener más información, consulte [Mover una historia ágil](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exportar historias del registro de pendientes {#export-stories-from-the-backlog}

Puede exportar uno o más artículos (incluidas las tareas y los problemas) directamente desde el registro de pendientes.

Las historias del registro de pendientes se exportan del mismo modo que se exportan otros datos en [!DNL Workfront], tal como se describe en [Exportación de datos](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
