---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Administrar el trabajo atrasado ágil
description: Las tareas y los problemas se pueden asignar a un equipo ágil y añadirse al trabajo acumulado de ese equipo como artículos, según la metodología ágil que utilice el equipo.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# Administrar el trabajo atrasado ágil

Los siguientes elementos de trabajo se pueden asignar a un equipo ágil y añadirse al trabajo acumulado de dicho equipo como artículos, según la metodología ágil que utilice el equipo:

* **[!UICONTROL Anular equipos ágiles]:** Las tareas y los problemas se pueden asignar al equipo ágil y agregar al trabajo acumulado.
* **[!UICONTROL Equipos móviles kanban]:** Las tareas se pueden asignar al equipo ágil y agregar al trabajo acumulado. Los usuarios pueden ver el trabajo pendiente directamente desde el tablero de artículos ágil, tal como se describe en [[!UICONTROL Añadir el trabajo atrasado] al tablero Kanban](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). El equipo utiliza este trabajo pendiente para priorizar y administrar su cola de trabajos.

Las tareas o los problemas se pueden asignar al equipo (y posteriormente se pueden agregar al trabajo acumulado del equipo) desde cualquier lugar de [!DNL Adobe Workfront]. Por ejemplo, a un solo equipo se le podrían asignar asignaciones de trabajo de varios proyectos.

>[!NOTE]
>
>Si agrega varios equipos a un elemento de trabajo pendiente, el problema o la tarea solo se muestra en el trabajo pendiente del equipo principal. El equipo principal es el equipo que se asignó por primera vez.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Administrar] al proyecto en el que se encuentra el artículo</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Crear y administrar artículos con el trabajo atrasado

* [Reordenar artículos](#reorder-stories)
* [[!UICONTROL Salto] artículos anteriores](#break-down-stories)
* [Editar artículos](#edit-stories)
* [Crear nuevos artículos con el trabajo atrasado](#create-new-stories-on-the-backlog)
* [Mover historias del trabajo pendiente a una iteración o tablero Kanban](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### Reordenar artículos {#reorder-stories}

Puede reordenar los artículos en la lista de atrasos utilizando el método de arrastrar y soltar.

1. Vaya al archivo de trabajo atrasado en el que desea reordenar los artículos.
1. En el **[!UICONTROL Ver]** menú desplegable, seleccione la **[!UICONTROL Retraso]** vista o vista personalizada que contiene la variable **[!UICONTROL Pedido]** para abrir el Navegador.

   >[!NOTE]
   >
   >Si una tarea o problema tiene asignado un equipo ágil y el proyecto no está en un estado igual a Actual, no se muestran en el registro pendiente. Sin embargo, siguen afectando al recuento de atrasos en la columna Pedido .

1. Seleccione uno o más artículos y, a continuación, arrastre los artículos hasta el orden en el que desee que aparezcan en el registro anterior.\
   ![Arrastrar y soltar elementos de registro anterior](assets/agile-backlog-drag-and-drop.png)

### Desglose de artículos {#break-down-stories}

Dado que los artículos con un retraso varían en tamaño, los usuarios pueden desglosarlos en tamaños factibles para una iteración. Desglosar un artículo crea subtareas en la tarea que representa el artículo y reemplaza la tarea original en el trabajo pendiente. Puede tener una tarea principal o sus subtareas asignadas a un equipo ágil, pero no puede tener ambas asignadas a un equipo simultáneamente.

>[!NOTE]
>
>Tenga en cuenta las siguientes limitaciones al desglosar artículos:
>
>* Solo se pueden desglosar los artículos que representan tareas. No se pueden desglosar artículos que representen problemas.
>* Los artículos solo se pueden desglosar si están asociados a un proyecto.



Para desglosar una historia:

1. Vaya al registro que contiene el artículo que desea desglosar.
1. Seleccione el artículo que desea desglosar y haga clic en **[!UICONTROL Artículo de desglose]**.\
   La variable [!UICONTROL Artículo de desglose] se muestra.\
   ![Cuadro de diálogo Desglosar artículo](assets/backlog-breakdown-dialog.png)

1. Especifique un nombre y una estimación para el artículo y seleccione si el artículo está listo.
1. Haga clic en **[!UICONTROL Agregar artículo]** para crear otra historia a partir de la historia original.
1. Haga clic en **[!UICONTROL Guardar]**.

### Editar artículos {#edit-stories}

Puede editar artículos directamente desde la [!UICONTROL Historias] o [!UICONTROL Problemas] del informe de tareas pendientes, ya que editaría todas las tareas o problemas de un proyecto de forma masiva, tal como se describe en [Editar tareas de forma masiva](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) en [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md) y [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) en [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md).

## Crear nuevos artículos con el trabajo atrasado {#create-new-stories-on-the-backlog}

Puede crear nuevos artículos sobre el trabajo pendiente creando el artículo directamente a partir del trabajo pendiente o asignando una tarea o un problema existente a un equipo ágil.

* [Crear un artículo a partir del registro de elementos pendientes](#create-a-story-from-the-backlog)
* [Asignar una tarea o un problema a un equipo ágil](#assign-a-task-or-issue-to-an-agile-team)

### Crear un artículo a partir del registro de elementos pendientes {#create-a-story-from-the-backlog}

Cuando crea un artículo a partir del trabajo pendiente, el artículo se crea como una tarea o un problema dentro de un proyecto. No se puede crear un artículo a partir del trabajo pendiente como problema.

Para crear un artículo a partir del registro acumulado:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Select **[!UICONTROL Retraso]** del panel izquierdo.
1. Realice una de las siguientes acciones, en función de si desea crear una tarea o un problema:

   * **Para crear una tarea:** Haga clic en **[!UICONTROL Historias]**.

   * **Para crear un problema:** Haga clic en **[!UICONTROL Problemas]**.

1. Haga clic en **[!UICONTROL Nueva historia]** o **[!UICONTROL Nuevo problema]**.

1. Especifique la siguiente información:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nombre de artículo]</strong></td>
      <td> Escriba un nombre para el artículo.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong></td>
      <td>(Opcional) Escriba una descripción para el artículo.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Seleccione si el artículo está listo para agregarse a una iteración. Esta configuración solo es informativa. Los artículos se pueden agregar a una iteración independientemente del estado de esta configuración.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimación]</strong></td>
      <td>Especifique una estimación por punto o por hora del artículo. Las estimaciones afectan al gráfico desglosado. El gráfico desplegable de una iteración solo es preciso si cada artículo contiene una estimación precisa. (Si proporciona una estimación de puntos, ya debe haber designado en la configuración del equipo cuántas horas representa cada punto).</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Proyecto principal]</strong></td>
      <td>Empiece a escribir el nombre del proyecto donde se creará este artículo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.<br>El estado del proyecto debe establecerse en [!UICONTROL Current]. Si el estado del proyecto es distinto de [!UICONTROL Actual], no se muestra en el menú desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarea Principal]</strong></td>
      <td>(Opcional) Empiece a escribir el nombre de la tarea principal a la que está subordinado este artículo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Forms personalizado]</strong></td>
      <td> (Opcional) Seleccione los formularios personalizados que desee agregar a este artículo.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Guardar artículo]**.

### Asignar una tarea o un problema a un equipo ágil {#assign-a-task-or-issue-to-an-agile-team}

Puede asignar una tarea o un problema a un equipo ágil. Una vez asignada, la tarea o el problema aparece como un nuevo artículo en el trabajo acumulado del equipo.

Para asignar una tarea o un problema a un equipo ágil:

1. Vaya al proyecto que contiene la tarea que desea reasignar.
1. Seleccione la tarea o el problema en la lista.
1. Haga clic en **[!UICONTROL Editar]**.
1. Haga clic en **[!UICONTROL Asignaciones]**.
1. (Opcional) Elimine los usuarios asignados existentes.
1. Haga clic en **[!UICONTROL Agregar usuario asignado]**.
1. Empiece a escribir el nombre del equipo ágil al que desea asignar la tarea o el problema y, a continuación, haga clic en el nombre del equipo cuando aparezca en la lista desplegable.
1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   La tarea o el problema ya están disponibles en el trabajo acumulado del equipo.

## Mover artículos del registro anterior a una iteración o tablero + {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Mover los artículos existentes al registro anterior](#move-existing-stories-to-the-backlog)
* [Exportar artículos del trabajo atrasado](#export-stories-from-the-backlog)

1. Vaya al trabajo atrasado del equipo ágil.
1. Seleccione los artículos que desea mover a una iteración o a un tablero Kanban y, a continuación, haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.\
   Si se mueve el artículo a un [!UICONTROL Kanban] tablero, [!UICONTROL Mover la historia a Kanban] Se muestra el tablero.\
   Si se mueve el artículo a una iteración, la variable [!UICONTROL Mover el artículo a una iteración] se muestra.\
   ![Cuadro de diálogo Mover artículo](assets/agile-backlog-addtoiteration.png)

1. Realice una de las siguientes acciones:

   * **Para equipos de Anulación de errores:** En el **[!UICONTROL Seleccionar iteración]** , seleccione la iteración donde desea mover los artículos.

   * **Para equipos kanban:** En el **[!UICONTROL Seleccionar tablero kanban]** seleccione el equipo [!UICONTROL Kanban] tablero. (Los equipos kanban solo pueden tener uno [!UICONTROL Kanban] tablero).

1. Haga clic en **[!UICONTROL Mover artículo]**.

### Mover los artículos existentes al registro anterior {#move-existing-stories-to-the-backlog}

Si decide que su equipo aún no está listo para trabajar en un artículo, puede pasar el artículo al trabajo pendiente.

Para obtener más información, consulte [Mover una historia ágil](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exportar artículos del trabajo atrasado {#export-stories-from-the-backlog}

Puede exportar uno o más artículos (incluidas tareas y problemas) directamente desde el trabajo pendiente.

Los artículos se exportan desde el registro anterior del mismo modo que se exportan otros datos en [!DNL Workfront], tal como se describe en [Exportar datos](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
