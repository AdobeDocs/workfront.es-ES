---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Usar la lista de tarjetas
description: Puede crear una lista de tarjetas en un flujo de trabajo y añadir las tarjetas a las iteraciones.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Usar la lista de tarjetas

>[!IMPORTANT]
>
>Los flujos de trabajo no están disponibles para todos los clientes.

Puede crear una lista de tarjetas en un flujo de trabajo y añadir las tarjetas a las iteraciones.

La lista de tarjetas puede funcionar como un registro de trabajo pendiente para el flujo de trabajo.

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

## Agregar tarjetas a la lista de tarjetas

{{step1-to-boards}}

1. Para abrir un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**].
1. Haga clic en la ficha [!UICONTROL **Lista de tarjetas**].
1. Haga clic en [!UICONTROL **Agregar tarjeta**].
1. En el cuadro de diálogo [!UICONTROL **Crear/editar tarjeta**], agregue la siguiente información:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Nombre]</strong></td> 
      <td>Nombre de la tarjeta.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Descripción]</strong></td> 
      <td>Una descripción de la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimación]</strong></td> 
      <td>Número estimado de horas que se completará la tarjeta. Esto es solo una entrada manual.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estado]</strong></td> 
      <td>Seleccione un estado para la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Seleccione una iteración a la que asignar la tarjeta.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Asignados]</strong></td> 
      <td><p>Para asignar la tarjeta, empiece a escribir un nombre en el campo de búsqueda y, a continuación, selecciónela cuando se muestre en la lista. Puede agregar personas y equipos, así como asignar más de una persona o equipo a una tarjeta.</p><p>Los usuarios asignados deben ser miembros del flujo de trabajo o no aparecerán en la lista de selección.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Haga clic en [!UICONTROL **Guardar**].
1. Continúe agregando tarjetas hasta que haya creado la lista de tarjetas.

## Ver tarjetas

Para ver todas las tarjetas del flujo de trabajo en una sola lista, haga clic en [!UICONTROL **Vista de lista**] en la ficha Lista de tarjetas.

Para ver todas las tarjetas del flujo de trabajo agrupadas por iteración, haga clic en [!UICONTROL **Vista de iteración**]. Las tarjetas no planificadas se muestran en su propio grupo.

Para editar una tarjeta existente, selecciónela en la lista y haga clic en [!UICONTROL **Editar**].

Para eliminar una tarjeta, selecciónela en la lista y haga clic en [!UICONTROL **Eliminar**].

### Filtrar tarjetas

Las tarjetas sólo se pueden archivar desde el tablero de iteraciones. Cuando se archiva una tarjeta, esta no se muestra en la lista de tarjetas a menos que filtre para mostrar tarjetas archivadas. Para obtener información acerca de cómo archivar una tarjeta, vea [Eliminar o archivar una tarjeta de un tablero](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Acceda a la lista de tarjetas del flujo de trabajo.
1. Haga clic en [!UICONTROL **Filtro**] y seleccione [!UICONTROL **Todas**], [!UICONTROL **Tarjetas activas**] o [!UICONTROL **Tarjetas archivadas**].

   Cuando se aplica un filtro distinto del predeterminado en la lista de tarjetas, se muestra un indicador en el icono de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png).

### Buscar en la lista de tarjetas

1. Acceda a la lista de tarjetas del flujo de trabajo.
1. Haga clic en [!UICONTROL **Buscar**] y escriba un término de búsqueda. A continuación, pulse Intro.

   Se muestran todas las tarjetas que contienen el término de búsqueda.
Haga clic en la X para borrar la búsqueda.

   ![Buscar tarjetas en un tablero](assets/boards-searchbox.png)

## Añadir tarjetas a una iteración

>[!NOTE]
>
>Debe crear una iteración para poder agregarle tarjetas. Para obtener más información, vea [Crear una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Acceda a la lista de tarjetas del flujo de trabajo.
1. Seleccione la [!UICONTROL **vista de iteración**] para ver qué tarjetas están asignadas a una iteración y cuáles no están planificadas.
1. Seleccione una tarjeta no planeada en la lista y haga clic en [!UICONTROL **Editar**].
1. Seleccione una iteración en el campo [!UICONTROL **Iteraciones**].
1. Si usa puntos de historia, escriba un valor en el campo [!UICONTROL **Estimación**].
1. Haga clic en [!UICONTROL **Guardar**].

   La tarjeta se mueve a la iteración, y las métricas de iteración reflejan el número de tarjetas y puntos.

   También puede arrastrar y soltar una tarjeta del grupo Tarjetas no planificadas en la iteración, o hacer clic en [!UICONTROL **Agregar tarjeta**] para agregar una nueva tarjeta a la iteración.

>[!TIP]
>
>Si ha creado un tablero de proceso de iteración, todas las tarjetas no planeadas de la lista de tarjetas aparecerán en la columna [!UICONTROL Registro de pendientes]. Cuando una tarjeta se mueve a otra columna, pasa a formar parte de la iteración activa. Las tarjetas que agregue a la iteración en la lista de tarjetas se agregarán a una columna en función de su estado.
