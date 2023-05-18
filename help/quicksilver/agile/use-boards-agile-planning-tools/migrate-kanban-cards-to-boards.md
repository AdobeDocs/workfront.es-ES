---
content-type: reference
navigation-topic: boards
title: Migración de tarjetas Kanban de equipos ágiles a tableros de Workfront
description: Puede migrar los elementos de trabajo de un tablero Kanban de equipo ágil a un tablero Workfront nuevo o existente.
author: Lisa
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: a788a8d39c714463f7ea9aa32f0c5a0f050eabdc
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Migración de tarjetas Kanban de equipos ágiles a tableros de Workfront

Puede migrar los elementos de trabajo de un tablero Kanban de equipo ágil a un tablero Workfront nuevo o existente. Al ejecutar la migración, todas las tarjetas del tablero Kanban se copian en el tablero Workfront. No se le permite elegir tarjetas específicas.

La colocación de tarjetas en el tablero de Workfront se basa en políticas de columna. (Por ejemplo, una directiva podría mover todas las tarjetas con el estado &quot;En curso&quot; a una columna específica. Para obtener más información sobre las directivas de columna, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Si no hay directivas o las tarjetas no coinciden con las directivas, las tarjetas se colocan en la columna situada más a la izquierda del tablero. En este momento, las tarjetas de la columna Backlog en el tablero preexistente no se agregan al tablero de Workfront.

Las tarjetas no se eliminan del tablero Kanban del equipo ágil y los cambios de estado de las tarjetas se sincronizarán con ambos tableros. Puede mantener ambos tableros activos hasta que esté preparado para cambiar a los tableros de Workfront.

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
   <td> <p>[!UICONTROL Request] o superior</p> </td>
  </tr>
 </tbody>
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Migración de tarjetas Kanban a un tablero nuevo

{{step1-to-team}}

1. Acceda a un tablero Kanban.
1. Haga clic en [!UICONTROL **Agregar a tableros**] y seleccione [!UICONTROL **Nuevo tablero**].
1. En el [!UICONTROL Agregar a tablero nuevo] , escriba un nombre para el tablero nuevo (el nombre del tablero actual) [!UICONTROL Kanban] el tablero se muestra automáticamente) y haga clic en [!UICONTROL **Agregar**].

   ![Agregar tarjetas Kanban a un tablero nuevo](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Opcional) En el mensaje de éxito que aparece, haga clic en el vínculo para abrir el tablero nuevo.

## Migración de tarjetas Kanban a un tablero existente

{{step1-to-team}}

1. Acceda a un tablero Kanban.
1. Haga clic en [!UICONTROL **Agregar a tableros**] y seleccione [!UICONTROL **Tablero existente**].
1. En el [!UICONTROL Agregar a tablero existente] , busque y seleccione el tablero al que desea migrar las tarjetas. A continuación, haga clic en [!UICONTROL **Agregar**].

   ![Agregar tarjetas Kanban a un tablero existente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Opcional) En el mensaje de éxito que aparece, haga clic en el vínculo para abrir el tablero.
