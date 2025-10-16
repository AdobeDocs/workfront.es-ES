---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Usar la lista de tarjetas
description: Puede crear una lista de tarjetas en un flujo de trabajo y añadir las tarjetas a las iteraciones.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 98%

---

# Usar la lista de tarjetas

>[!IMPORTANT]
>
>Los flujos de trabajo no están disponibles para todos los clientes.

Puede crear una lista de tarjetas en un flujo de trabajo y añadir las tarjetas a las iteraciones.

La lista de tarjetas puede funcionar como un registro de asuntos de pendientes para el flujo de trabajo.

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

## Añadir tarjetas a la lista de tarjetas

{{step1-to-boards}}

1. Para abrir una secuencia de trabajo, haga clic en [!UICONTROL **Ver secuencia de trabajo**].
1. Haga clic en la pestaña [!UICONTROL **Lista de tarjetas**].
1. Haga clic en [!UICONTROL **Añadir tarjeta**].
1. En el cuadro de diálogo [!UICONTROL **Crear/editar tarjeta**], añada la siguiente información:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>Nombre de la tarjeta.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>Descripción de la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>Número estimado de horas para completar la tarjeta. Esta entrada es solo manual.</td> 
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
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>Para asignar la tarjeta, empiece a escribir un nombre en el campo de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista. Puede añadir personas y equipos, así como asignar más de una persona o equipo a una tarjeta.</p><p>Los usuarios asignados deben ser integrantes del flujo de trabajo o no aparecerán en la lista de selección.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Haga clic en [!UICONTROL **Guardar**].
1. Continúe añadiendo tarjetas hasta que haya generado la lista de tarjetas.

## Ver tarjetas

Para ver todas las tarjetas del flujo de trabajo en una sola lista, haga clic en [!UICONTROL **Vista de lista**] en la pestaña Lista de tarjetas.

Para ver todas las tarjetas del flujo de trabajo agrupadas por iteración, haga clic en [!UICONTROL **Vista de iteración**]. Las tarjetas no planificadas se muestran en su propio grupo.

Para editar una tarjeta existente, selecciónela en la lista y haga clic en [!UICONTROL **Editar**].

Para eliminar una tarjeta, selecciónela en la lista y haga clic en [!UICONTROL **Eliminar**].

### Filtrar tarjetas

Las tarjetas solo se pueden archivar desde el tablero de iteraciones. Cuando se archiva una tarjeta, esta no se muestra en la lista de tarjetas a menos que aplique un filtro para mostrar las tarjetas archivadas. Para obtener información sobre cómo archivar una tarjeta, consulte [Eliminar o archivar una tarjeta de un tablero](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Acceda a la lista de tarjetas de la secuencia de trabajo.
1. Haga clic en [!UICONTROL **Filtro**] y seleccione [!UICONTROL **Todo**], [!UICONTROL **Tarjetas activas**] o [!UICONTROL **Tarjetas archivadas**].

   Cuando se aplica un filtro distinto del predeterminado a la lista de tarjetas, se muestra un indicador en el icono de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png).

### Buscar en la lista de tarjetas

1. Acceda a la lista de tarjetas de la secuencia de trabajo.
1. Haga clic en [!UICONTROL **Buscar**] y escriba un término de búsqueda. A continuación, presione Intro.

   Se muestran todas las tarjetas que contienen el término de búsqueda.
Haga clic en la X para borrar la búsqueda.

   ![Buscar tarjetas en un tablero](assets/boards-searchbox.png)

## Añadir tarjetas a una iteración

>[!NOTE]
>
>Primero debe crear una iteración para poder añadirle tarjetas. Para obtener más información, consulte [Crear una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Acceda a la lista de tarjetas de la secuencia de trabajo.
1. Seleccione la [!UICONTROL **Vista de iteración**] para ver qué tarjetas están asignadas a una iteración y cuáles no están planificadas.
1. Seleccione una tarjeta no planificada de la lista y haga clic en [!UICONTROL **Editar**].
1. Seleccione una iteración del campo [!UICONTROL **Iteraciones**].
1. Si va a usar puntos de caso, introduzca un valor en el campo [!UICONTROL **Estimación**].
1. Haga clic en [!UICONTROL **Guardar**].

   La tarjeta se mueve a la iteración y las métricas de iteración reflejan el número de tarjetas y puntos.

   También puede arrastrar y soltar una tarjeta desde el grupo Tarjetas no planificadas al de Iteración, o hacer clic en [!UICONTROL **Añadir tarjeta**] para añadir una nueva tarjeta a la iteración.

>[!TIP]
>
>Si ha creado un tablero de proceso de iteración, todas las tarjetas no planificadas de la lista de tarjetas aparecerán en la columna [!UICONTROL Registro de asuntos pendientes]. Cuando una tarjeta se mueve a otra columna, pasa a formar parte de la iteración activa. Las tarjetas que añada a la iteración en la lista de tarjetas se añadirán a una columna en función de su estado.
