---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Crear una iteración en un flujo de trabajo
description: Una iteración es una cantidad de tiempo establecida reservada para completar el trabajo. Algunos equipos Agile pueden referirse a una iteración como un sprint.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 19%

---

# Crear una iteración en un flujo de trabajo

>[!IMPORTANT]
>
>Las secuencias de trabajo solo están disponibles para un grupo específico de clientes.

Una iteración es una cantidad de tiempo establecida reservada para completar el trabajo. Algunos equipos Agile pueden referirse a una iteración como un sprint.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p>
   </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una iteración en un flujo de trabajo

{{step1-to-boards}}

1. Abra el flujo de trabajo en el que desee añadir la iteración. Para abrir una secuencia de trabajo, haga clic en [!UICONTROL **Ver secuencia de trabajo**].
1. Cree una iteración utilizando uno de estos métodos:

   * En la ficha Lista de tarjetas, en la vista de iteración, haga clic en [!UICONTROL **Crear iteración**].
   * En la ficha Lista de tarjetas, en la vista de lista, haga clic en [!UICONTROL **Crear iteración**].
   * En la ficha Tableros, haga clic en [!UICONTROL **Agregar tablero**] y seleccione [!UICONTROL **Proceso de iteración**] como plantilla del tablero. A continuación, abra el panel de iteraciones y haga clic en [!UICONTROL **Configurar iteraciones**].

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
      <td><strong>[!UICONTROL Start date]</strong></td> 
      <td>La fecha en la que comienza la iteración. La fecha de finalización se introduce automáticamente en función de la duración de la iteración.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en [!UICONTROL **Guardar**].

   La iteración ahora aparece en la vista de iteración de la lista de tarjetas y en el área de métricas del panel de iteraciones.

   Para agregar tarjetas a una iteración, vea [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Editar una iteración existente

1. Para abrir una secuencia de trabajo, haga clic en [!UICONTROL **Ver secuencia de trabajo**].
1. Abra la iteración utilizando uno de estos métodos:

   * En la ficha Lista de tarjetas, en la vista de iteración, haga clic en el icono [!UICONTROL **Detalles de iteración**] ![Detalles de iteración](assets/iteration-details-button.png).
   * En el panel de iteraciones, haga clic en el icono [!UICONTROL **Detalles de iteración**] ![Detalles de iteración](assets/iteration-details-button.png) en el área de métricas de la parte superior derecha.

1. En el panel [!UICONTROL Configuración de iteración], edite la iteración según sea necesario.
1. Para cambiar el nombre de la iteración, expanda [!UICONTROL **Detalles de iteración**].

   Una vez iniciada una iteración, sólo se puede cambiar el nombre de la iteración y no las fechas o la longitud de la iteración.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Eliminar una iteración

1. Haga clic en la ficha [!UICONTROL **Lista de tarjetas**] del flujo de trabajo y abra la vista de iteración.
1. Haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png) junto a la iteración.
1. Haga clic en [!UICONTROL **Eliminar iteración**] en el mensaje de confirmación.
