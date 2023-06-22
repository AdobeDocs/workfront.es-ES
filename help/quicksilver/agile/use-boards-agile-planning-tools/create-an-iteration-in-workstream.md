---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Creación de una iteración en un flujo de trabajo
description: Una iteración es una cantidad de tiempo establecida reservada para completar el trabajo. Algunos equipos Agile pueden referirse a una iteración como un sprint.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 563e0f443ecef9ee99e9f9bfb5a0d579aa50cef4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Creación de una iteración en un flujo de trabajo

{{highlighted-preview}}

Una iteración es una cantidad de tiempo establecida reservada para completar el trabajo. Algunos equipos Agile pueden referirse a una iteración como un sprint.

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

## Creación de una iteración en un flujo de trabajo

{{step1-to-boards}}

1. Abra el flujo de trabajo en el que desee añadir la iteración. Para abrir un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**].
1. Cree una iteración utilizando uno de estos métodos:

   * En la ficha Lista de tarjetas, en la vista de iteración, haga clic en [!UICONTROL **Crear iteración**].
   * En la ficha Lista de tarjetas, en la vista de lista, haga clic en [!UICONTROL **Crear iteración**].
   * En la pestaña Tableros, haga clic en [!UICONTROL **Añadir tablero**] y seleccione [!UICONTROL **Proceso de iteración**] como plantilla del tablero. A continuación, abra el panel de iteraciones y haga clic en [!UICONTROL **Configuración de iteraciones**].

1. En el cuadro de diálogo Detalles de iteración, agregue la siguiente información:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Iteration name]</strong></td> 
      <td>Nombre de la iteración; por ejemplo, "Sprint 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Longitud de iteración]</strong></td> 
      <td>La duración de la iteración, en días, semanas o meses.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Fecha de inicio]</strong></td> 
      <td>La fecha en la que comienza la iteración. La fecha de finalización se introduce automáticamente en función de la duración de la iteración.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en [!UICONTROL **Guardar**].

   La iteración ahora aparece en la vista de iteración de la lista de tarjetas y en el área de métricas del panel de iteraciones.

   Para añadir tarjetas a una iteración, consulte [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Editar una iteración existente

1. Para abrir un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**].
1. Abra la iteración utilizando uno de estos métodos:

   * En la ficha Lista de tarjetas, en la vista de iteración, haga clic en [!UICONTROL **Detalles de iteración**] icono ![Detalles de iteración](assets/iteration-details-button.png).
   * En el tablero de iteraciones, haga clic en [!UICONTROL **Detalles de iteración**] icono ![Detalles de iteración](assets/iteration-details-button.png) en el área de métricas, en la parte superior derecha.

1. En el [!UICONTROL Configuración de iteración] , edite la iteración según sea necesario.
1. Para cambiar el nombre de la iteración, expanda [!UICONTROL **Detalles de iteración**].

   Una vez iniciada una iteración, sólo se puede cambiar el nombre de la iteración y no las fechas o la longitud de la iteración.

1. <span class="preview">Para añadir metas a la iteración, expanda [!UICONTROL **Metas**].</span>
1. <span class="preview">Clic [!UICONTROL **Añadir meta**] y escriba el nombre de la meta.</span>

   <span class="preview">A medida que los objetivos se completan durante la iteración, puede seleccionar la casilla de verificación para marcarlos como completados o hacer clic en el botón **Eliminar** icono ![Icono Eliminar](assets/delete.png) para eliminar una meta. El área de métricas en la parte superior derecha de la iteración muestra cuántos objetivos existen y cuántos se han completado.</span>

<!--
<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Eliminación de una iteración

1. Haga clic en [!UICONTROL **Lista de tarjetas**] en el flujo de trabajo y abra la vista de iteración.
1. Haga clic en **Eliminar** icono ![Icono Eliminar](assets/delete.png) junto a la iteración.
1. Clic [!UICONTROL **Eliminar iteración**] en el mensaje de confirmación.
