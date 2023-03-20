---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Usar la lista de tarjetas
description: Puede crear una lista de tarjetas en un flujo de trabajo y agregarlas a iteraciones.
author: Lisa
feature: Agile
source-git-commit: 96819e5d81a063ad623350a0a75428629d6f7b6d
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Usar la lista de tarjetas

{{highlighted-preview-article-level}}

Puede crear una lista de tarjetas en un flujo de trabajo y agregarlas a iteraciones.

La lista de tarjetas puede funcionar como un trabajo atrasado para el flujo de trabajo.

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

## Agregar tarjetas a la lista de tarjetas

{{step1-to-boards}}

1. Para abrir un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**].
1. Haga clic en el [!UICONTROL **Lista de tarjetas**] pestaña .
1. Haga clic en [!UICONTROL **Agregar tarjeta**].
1. En el [!UICONTROL **Crear/editar tarjeta**] , añada la siguiente información:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>El nombre de la tarjeta.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Descripción]</strong></td> 
      <td>Descripción de la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimación]</strong></td> 
      <td>El número estimado de horas para completar la tarjeta. Esta es una entrada manual solamente.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Seleccione un estado para la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Seleccione una iteración a la que asignar la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Asignados]</strong></td> 
      <td><p>Para asignar la tarjeta, empiece a escribir un nombre en el campo de búsqueda y selecciónelo cuando aparezca en la lista. Puede agregar personas y equipos, y puede asignar más de una persona o equipo a una tarjeta.</p><p>Los destinatarios asignados deben ser miembros del flujo de trabajo o no aparecerán en la lista de selección.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Haga clic en [!UICONTROL **Guardar**].
1. Siga agregando tarjetas hasta que haya creado la lista de tarjetas.

## Ver tarjetas

Para ver todas las tarjetas del flujo de trabajo en una sola lista, haga clic en [!UICONTROL **Vista de lista**] en la ficha Lista de tarjetas.

Para ver todas las tarjetas del flujo de trabajo agrupadas por iteración, haga clic en [!UICONTROL **Vista iteración**]. Las tarjetas no planificadas se muestran en su propio grupo.

Para editar una tarjeta existente, selecciónela en la lista y haga clic en [!UICONTROL **Editar**].

Para eliminar una tarjeta, selecciónela en la lista y haga clic en [!UICONTROL **Eliminar**].

### Filtrar tarjetas

Las tarjetas solo se pueden archivar desde el panel de iteración. Cuando se archiva una tarjeta, esta no se muestra en la lista de tarjetas a menos que filtre para mostrar tarjetas archivadas. Para obtener información sobre cómo archivar una tarjeta, consulte [Eliminar o archivar una tarjeta de un tablero](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Acceda a la lista de tarjetas para el flujo de trabajo.
1. Haga clic en [!UICONTROL **Filtro**] y seleccione [!UICONTROL **Todo**], [!UICONTROL **Tarjetas activas**] o [!UICONTROL **Tarjetas archivadas**].

   Cuando se aplica un filtro que no sea el predeterminado en la lista de tarjetas, se muestra un indicador en el icono de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png).

### Buscar en la lista de tarjetas

1. Acceda a la lista de tarjetas para el flujo de trabajo.
1. Haga clic en [!UICONTROL **Buscar**] y escriba un término de búsqueda. A continuación, pulse Intro.

   Se muestran todas las tarjetas que contienen el término de búsqueda.
Haga clic en la X para borrar la búsqueda.

   ![Buscar tarjetas en un tablero](assets/boards-searchbox.png)

## Añadir tarjetas a una iteración

>[!NOTE]
>
>Debe crear una iteración para poder añadir tarjetas a ella. Para obtener más información, consulte [Creación de una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Acceda a la lista de tarjetas para el flujo de trabajo.
1. Seleccione el [!UICONTROL **Vista iteración**] para ver qué tarjetas se asignan a una iteración y cuáles no están planificadas.
1. Seleccione una tarjeta no planificada en la lista y haga clic en [!UICONTROL **Editar**].
1. Seleccione una iteración en el [!UICONTROL **Iteraciones**] campo .
1. Si utiliza puntos de artículo, introduzca un valor en la variable [!UICONTROL **Estimación**] campo .
1. Haga clic en [!UICONTROL **Guardar**].

   La tarjeta se mueve a la iteración y las métricas de iteración reflejan el número de tarjetas y puntos.

   También puede arrastrar y soltar una tarjeta del grupo Tarjetas no planificadas en la iteración o hacer clic en [!UICONTROL **Agregar tarjeta**] para agregar una tarjeta nueva a la iteración.

>[!TIP]
>
>Si ha creado un tablero de proceso de iteración, todas las tarjetas no planificadas de la lista de tarjetas aparecerán en el [!UICONTROL Retraso] para abrir el Navegador. Cuando una tarjeta se mueve a otra columna, pasa a formar parte de la iteración activa. Las tarjetas que agregue a la iteración en la lista de tarjetas se agregan a una columna en función de su estado.

