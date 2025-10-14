---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Eliminar o archivar una tarjeta de un tablero
description: Al eliminar una tarjeta de un tablero, se elimina de forma permanente y no se puede restaurar. Archivar una tarjeta la envía al archivo y puede restaurarla en la placa posteriormente.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 81e87793905fd925db00c7a0ac107150263a1365
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Eliminar o archivar una tarjeta de un tablero

Al eliminar una tarjeta ad hoc de un tablero, se elimina de forma permanente y no se puede restaurar. Las tarjetas conectadas se pueden volver a añadir manualmente a un tablero después de eliminarlas.

Si elimina una tarjeta conectada de un tablero dinámico, volverá a aparecer cuando actualice el tablero, ya que este tipo de tablero extrae todas las tareas y problemas de un proyecto específico. Para eliminar la tarjeta, debe eliminar la tarea o el problema conectado del proyecto de Workfront.

Cuando elimine una tarjeta conectada de cualquier otro tipo de tarjeta que tenga una columna de entrada, la tarjeta volverá a aparecer en la columna de entrada cuando actualice el tablero si la tarea o el problema conectado aún no se ha marcado como completado. Para obtener más información sobre las columnas de entrada, vea [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Archivar una tarjeta la envía al archivo y puede restaurarla en la placa posteriormente.

Las tarjetas archivadas no se sincronizan con las tareas y problemas de Workfront. Si restaura una tarjeta, se volverá a sincronizar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> 
   <p>Nuevo: [!UICONTROL Contributor] o superior</p> 
   <p>o</p>
   <p>Actual: [!UICONTROL Request] o superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar una tarjeta de un tablero

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en el menú **[!UICONTROL Más]** ![Más &#x200B;](assets/more-icon-spectrum.png) de la tarjeta y seleccione **[!UICONTROL Eliminar]**.
1. Haz clic en **[!UICONTROL Eliminar]** en el mensaje de confirmación.

## Archivar una tarjeta de un tablero

1. Acceda al tablero.
1. Haga clic en el menú **[!UICONTROL Más]** ![Más &#x200B;](assets/more-icon-spectrum.png) de la tarjeta y seleccione **[!UICONTROL Archivar]**.

   Las tarjetas archivadas se ocultan del tablero a menos que aplique un filtro para mostrarlas. Para obtener más información, consulte [Filtrar un tablero para mostrar tarjetas archivadas](#filter-a-board-to-show-archived-cards) en este artículo.

   Aparece un icono [!UICONTROL Archivo] ![Archivo](assets/archive-icon-spectrum-25x20.png) en las tarjetas archivadas. No puede editar una tarjeta archivada, pero puede eliminarla o moverla a otra columna.

1. Para restaurar una tarjeta archivada, haga clic en el menú **[!UICONTROL Más]** ![Menú más](assets/more-icon-spectrum.png) de la tarjeta y seleccione **[!UICONTROL Restaurar]**.

## Filtrar un tablero para mostrar tarjetas archivadas

De forma predeterminada, solo se muestran las tarjetas activas en un tablero. Puede filtrar el tablero para que también muestre las tarjetas archivadas.

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar.
1. Expandir [!UICONTROL **Tarjetas**].
1. Activar [!UICONTROL **Mostrar tarjetas archivadas en el tablero**].
1. Haga clic en [!UICONTROL **Filtro**], expanda la sección [!UICONTROL Tarjetas archivadas] y seleccione **[!UICONTROL Tarjetas archivadas]** para mostrar cualquier tarjeta archivada.

   El filtro muestra el número de tarjetas archivadas.

   ![Filtrar tarjetas archivadas](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >La sección [!UICONTROL Tarjetas archivadas] no está disponible en el filtro si no ha activado la opción de configuración para mostrar las tarjetas archivadas. Para obtener más información, consulte [Personalizar qué campos se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Vuelva a seleccionar **[!UICONTROL tarjetas archivadas]** para borrar la opción y mostrar solo las tarjetas activas.
