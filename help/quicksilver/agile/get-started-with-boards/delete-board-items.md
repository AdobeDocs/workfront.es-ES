---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Eliminar o archivar una tarjeta de un tablero
description: Al eliminar una tarjeta de un tablero, se elimina de forma permanente y no se puede restaurar. Archivar una tarjeta la envía al archivo y puede restaurarla en la placa posteriormente.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Eliminar o archivar una tarjeta de un tablero

Al eliminar una tarjeta ad hoc de un tablero, se elimina de forma permanente y no se puede restaurar. Las tarjetas conectadas se pueden volver a añadir manualmente a un tablero después de eliminarlas.

Si elimina una tarjeta conectada de un tablero dinámico, volverá a aparecer cuando actualice el tablero, ya que este tipo de tablero extrae todas las tareas y problemas de un proyecto específico. Para eliminar la tarjeta, debe eliminar la tarea o el problema conectado del proyecto de Workfront.

Cuando elimine una tarjeta conectada de cualquier otro tipo de tarjeta que tenga una columna de entrada, la tarjeta volverá a aparecer en la columna de entrada cuando actualice el tablero si la tarea o el problema conectado aún no se ha marcado como completado. Para obtener más información sobre las columnas de entrada, consulte [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Archivar una tarjeta la envía al archivo y puede restaurarla en la placa posteriormente.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

## Eliminar una tarjeta de un tablero

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Más]** menú ![Menú Más](assets/more-icon-spectrum.png) en la tarjeta y seleccione **[!UICONTROL Eliminar]**.
1. Clic **[!UICONTROL Eliminar]** en el mensaje de confirmación.

## Archivar una tarjeta de un tablero

1. Acceda al tablero.
1. Haga clic en **[!UICONTROL Más]** menú ![Menú Más](assets/more-icon-spectrum.png) en la tarjeta y seleccione **[!UICONTROL Archivar]**.

   Las tarjetas archivadas se ocultan del tablero a menos que aplique un filtro para mostrarlas. Para obtener más información, consulte [Filtrar un tablero para mostrar tarjetas archivadas](#filter-a-board-to-show-archived-cards) en este artículo.

   Un [!UICONTROL Archivar] icono ![Archivar](assets/archive-icon-spectrum-25x20.png) aparece en las tarjetas archivadas. No puede editar una tarjeta archivada, pero puede eliminarla o moverla a otra columna.

1. Para restaurar una tarjeta archivada, haga clic en **[!UICONTROL Más]** menú ![Menú Más](assets/more-icon-spectrum.png) en la tarjeta y seleccione **[!UICONTROL Restaurar]**.

## Filtrar un tablero para mostrar tarjetas archivadas {#filter-a-board-to-show-archived-cards}

De forma predeterminada, solo se muestran las tarjetas activas en un tablero. Puede filtrar el tablero para que también muestre las tarjetas archivadas.

1. Acceda al tablero.
1. Clic [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar.
1. Expandir [!UICONTROL **Tarjetas**].
1. Activar [!UICONTROL **Mostrar tarjetas archivadas en el tablero**].
1. Clic [!UICONTROL **Filtrar**], expanda el [!UICONTROL Tarjetas archivadas] y seleccione. **[!UICONTROL Tarjetas archivadas]** para mostrar cualquier tarjeta archivada.

   El filtro muestra el número de tarjetas archivadas.

   ![Filtrar tarjetas archivadas](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >El [!UICONTROL Tarjetas archivadas] La sección no está disponible en el filtro si no ha activado la configuración para mostrar tarjetas archivadas. Para obtener más información, consulte [Personalizar los campos que se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Seleccionar **[!UICONTROL Tarjetas archivadas]** de nuevo para desactivar la opción y mostrar solo las tarjetas activas.
