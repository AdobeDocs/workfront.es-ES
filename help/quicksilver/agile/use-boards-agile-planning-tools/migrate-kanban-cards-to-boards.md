---
content-type: reference
navigation-topic: boards
title: Migración de tarjetas Agile Team Kanban a tableros de Workfront
description: Puede migrar los elementos de trabajo de un panel Kanban de equipo Agile a un tablero de Workfront nuevo o existente.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Migración de tarjetas Agile Team Kanban a tableros de Workfront

Puede migrar los elementos de trabajo de un panel Kanban de equipo Agile a un tablero de Workfront nuevo o existente. Al ejecutar la migración, todas las tarjetas del panel Kanban se copian en el panel Workfront. No se le permite elegir tarjetas específicas.

La ubicación de las tarjetas en el tablero de Workfront se basa en las políticas de columna. (Por ejemplo, una directiva podría mover todas las tarjetas con el estado &quot;En curso&quot; a una columna específica. Para obtener más información sobre las directivas de columna, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Si no hay políticas o las tarjetas no coinciden con las políticas, las tarjetas se colocan en la columna situada más a la izquierda del tablero. En este momento, las tarjetas de la columna Registro de pendientes del tablero heredado no se añaden al tablero de Workfront.

Las tarjetas no se eliminan del panel Kanban del equipo Agile y los cambios de estado de las tarjetas se sincronizarán con ambos paneles. Puede mantener ambos tableros activos hasta que esté listo para cambiar a los tableros de Workfront.

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Migración de tarjetas Kanban a un nuevo tablero

{{step1-to-team}}

1. Acceda al panel Kanban.
1. Haga clic en [!UICONTROL **Agregar a tableros**] y seleccione [!UICONTROL **Nuevo tablero**].
1. En el cuadro de diálogo [!UICONTROL Agregar al nuevo tablero], escriba un nombre para el nuevo tablero (el nombre del tablero actual [!UICONTROL Kanban] se muestra automáticamente) y haga clic en [!UICONTROL **Agregar**].

   ![Agregar tarjetas Kanban al nuevo tablero](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Opcional) En el mensaje de éxito que aparece, haga clic en el vínculo para abrir el nuevo tablero.

## Migración de tarjetas Kanban a un tablero existente

{{step1-to-team}}

1. Acceda al panel Kanban.
1. Haga clic en [!UICONTROL **Agregar a tableros**] y seleccione [!UICONTROL **Tablero existente**].
1. En el cuadro de diálogo [!UICONTROL Agregar al tablero existente], busque y seleccione el tablero al que migrar las tarjetas. A continuación, haga clic en [!UICONTROL **Agregar**].

   ![Agregar tarjetas Kanban al tablero existente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Opcional) En el mensaje de éxito que aparece, haga clic en el vínculo para abrir el tablero.
