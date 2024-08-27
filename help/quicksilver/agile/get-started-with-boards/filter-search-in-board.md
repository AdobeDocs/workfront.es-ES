---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtrar y buscar en un tablero
description: Puede filtrar un tablero para mostrar solo determinadas tarjetas.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Filtrar y buscar en un tablero

Puede filtrar un tablero para mostrar:

* Tarjetas asignadas a determinadas personas
* Tarjetas con ciertas etiquetas
* Tarjetas con un estado específico
* Tarjetas con vencimiento en un intervalo de tiempo determinado
* Tarjetas archivadas
* Tarjetas conectadas a un proyecto específico

Al ordenar el tablero, se ordenan todas las tarjetas de las columnas. No puede ordenar una sola columna y la columna de registro de pendientes o de entrada no está ordenada.

La búsqueda también le ayuda a localizar una tarjeta específica en el tablero.

Cuando se aplican filtros, se muestra un indicador en el panel ![Filtro aplicado al panel](assets/boards-filterapplied-30x30.png). Haga clic en **[!UICONTROL Borrar todo]** para eliminar todos los filtros del tablero y, a continuación, haga clic en el icono contraer para cerrar el panel de filtros.

![Panel de filtro](assets/boards-all-filters-collapsed-0823.png)

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

## Filtrar un tablero por personas asignadas

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en [!UICONTROL **Filtro**], expanda la sección [!UICONTROL Miembros] y seleccione la persona o personas cuyas tarjetas desee ver. También puede mostrar las tarjetas sin asignar.

   ![Filtrar por miembro](assets/boards-filter-by-assignees-0822.png)

## Filtrado de tableros por etiquetas

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Filtro**], expanda la sección [!UICONTROL Etiquetas] y seleccione las etiquetas que desee ver.

   ![Filtrar por etiqueta](assets/boards-filter-by-tags-0822.png)

## Filtrar un tablero por estado

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Filtro**], expanda la sección [!UICONTROL Estados] y seleccione los tipos de estado que desee ver.

   También puede ocultar las tarjetas completadas.

   ![Filtrar por estado](assets/boards-filter-by-status-0822.png)

## Filtrar un tablero por fecha de vencimiento

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Filtro**], expanda la sección [!UICONTROL Fecha de vencimiento] y seleccione las opciones de fecha que desee ver.

   Solo se muestran las tarjetas en los intervalos de fechas seleccionados.

   ![Filtrar por fecha de vencimiento](assets/boards-filter-by-due-date-0822.png)

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

## Filtrar un tablero por conexión

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Filtro**], expanda la sección [!UICONTROL Conexión] y seleccione los [!DNL Workfront] proyectos de las tarjetas conectadas que desee ver.

   También puede mostrar tarjetas que no estén conectadas a un proyecto.

   ![Filtrar por conexión](assets/boards-filter-by-connection.png)

## Ordenar en un tablero

Al seleccionar una opción para ordenar, se ordenan todas las columnas. No puede ordenar una sola columna y la columna de registro de pendientes o de entrada no está ordenada.

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Ordenar por**] y seleccione [!UICONTROL **Nombre**], [!UICONTROL **Fecha de vencimiento**], [!UICONTROL **Estimación**], [!UICONTROL **Estado**] o [!UICONTROL **Conexión**].

   La conexión (nombre de proyecto) se aplica solo a tarjetas conectadas y las demás opciones ordenarán tarjetas conectadas y ad hoc en las columnas.

   La opción &quot;orden del usuario&quot; devuelve las tarjetas en el orden en que se establecieron manualmente, antes de que se aplicaran otras opciones de ordenación. Este es el orden predeterminado para las columnas.

1. Seleccione [!UICONTROL **Orden inverso**] para ordenar las columnas en orden inverso a la opción de ordenación.

   La flecha del icono de ordenación indica si las columnas se ordenan en orden ascendente o descendente.

   Cuando se aplica una ordenación distinta de la predeterminada, se muestra un indicador en el icono de ordenación ![Ordenar aplicado](assets/sort-applied-boards.png).

   ![Ordenar por columnas en un tablero](assets/sort-by-columns-in-board.png)

## Buscar en un tablero

1. Acceda al tablero.
1. Haga clic en [!UICONTROL **Buscar**] y escriba un término de búsqueda. A continuación, pulse Intro.

   Se muestran todas las tarjetas que contienen el término de búsqueda.

   Haga clic en la X para borrar la búsqueda.

   ![Buscar tarjetas en un tablero](assets/boards-searchbox.png)
