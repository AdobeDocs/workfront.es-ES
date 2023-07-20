---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Agregar una columna de entrada a un tablero
description: Si lo desea, puede agregar una columna de entrada al tablero que recupere automáticamente las tareas y los problemas como tarjetas conectadas cuando se añadan en Workfront, según los filtros que defina.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '975'
ht-degree: 0%

---

# Agregar una columna de entrada a un tablero

Si lo desea, puede agregar una columna de entrada al tablero que extraiga automáticamente tareas y problemas como tarjetas conectadas cuando se agreguen en [!DNL Workfront], en función de los filtros que defina. La columna de entrada puede servir como columna de registro de asuntos pendientes para un equipo de Kanban, como ubicación de entrada para que un equipo de asistencia vea los problemas a medida que se añaden a una cola de solicitudes o para cualquier otro fin que necesite.

Solo se permite una columna de entrada en un tablero, que siempre aparece como la columna situada más a la izquierda.

La columna de entrada no está disponible en un tablero dinámico.

La columna de entrada no está disponible en tableros que formen parte de un flujo de trabajo. En su lugar, puede configurar una columna de registro de pendientes para extraer las tarjetas de la lista de tarjetas. Para obtener información sobre cómo añadir una columna de registro de pendientes a un tablero de un flujo de trabajo, consulte [Configurar el registro de pendientes en una placa de flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-backlog-workstream-board.md).

La columna de admisión está limitada a 300 tareas y 300 problemas. Se ordenan por la prioridad definida en los elementos. Para obtener información sobre la prioridad, consulte [Actualizar prioridad de tareas](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) y [Actualizar prioridad del problema](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

Para obtener más información sobre las columnas, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Para obtener información sobre las tarjetas conectadas, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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
   <td> <p>[!DNL Request] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Creación de una columna de entrada mediante filtros simples

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar.
1. Expandir **[!UICONTROL Tablero]**.
1. Activar **[!UICONTROL Inserte elementos de forma dinámica en el tablero]**.

   ![Opciones de filtro simple de columna de admisión](assets/intake-column-simple-filters.png)

   La columna de entrada se añade a la izquierda del tablero. Permanece en blanco hasta que se le aplican filtros.

1. (Opcional) Busque y seleccione [!DNL Workfront] [!UICONTROL **Proyectos**].
1. (Opcional) Busque y seleccione un usuario o equipo [!UICONTROL **Asignaciones**].
1. Seleccionar [!UICONTROL **Incluir trabajo completado**] para mostrar las tareas y los problemas con un estado Completo en la columna de entrada.

   >[!NOTE]
   >
   >Si esta opción no está seleccionada, cuando las tarjetas en otros estados se marquen como completadas, se &quot;caerán&quot; del tablero y ya no se mostrarán.

1. Clic [!UICONTROL **Aplicar**].

   Todos los objetos aparecen en la columna de entrada del tablero como tarjetas conectadas.

   ![Columna de entrada](assets/intake-column-added3.png)

## Creación de una columna de entrada con filtros avanzados

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar.
1. Expandir **[!UICONTROL Tablero]**.
1. Activar **[!UICONTROL Inserte elementos de forma dinámica en el tablero]**.

   La columna de entrada se añade a la izquierda del tablero. Permanece en blanco hasta que se le aplican filtros.

1. Clic [!UICONTROL **Uso de filtros avanzados**].
1. Clic **[!UICONTROL Adición de fuentes de filtro]** y seleccione **[!UICONTROL Tareas]** o **[!UICONTROL Problemas]**.

   ![Opciones avanzadas de filtro de columna de admisión](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Puede filtrar la columna de entrada para incluir tareas y problemas, pero debe configurar los filtros por separado para cada tipo de objeto.
   >
   >Además, los filtros guardados y los filtros predeterminados del sistema están disponibles para su selección.

1. En el panel de filtro, haga clic en **[!UICONTROL Nuevo filtro]** para empezar.

   ![Haga clic en Nuevo filtro](assets/intake-filter-dialog5.png)

1. Cree el filtro y haga clic en **[!UICONTROL Guardar como nuevo]**.

   ![Generador de filtros](assets/intake-filter-dialog6.png)

   Este ejemplo muestra un filtro para tareas de un proyecto específico que se encuentran en el estado de [!UICONTROL Nuevo] o [!UICONTROL En curso], y se me asignan.

   Para obtener más información sobre la creación de un filtro, consulte la sección &quot;Creación o edición de un filtro en el generador estándar&quot; en el artículo [Creación o edición de filtros en [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Asigne un nombre al filtro y haga clic **[!UICONTROL Guardar]**.

   ![Escriba un nombre para el filtro](assets/intake-filter-dialog7.png)

   Asignar al filtro un nombre único le permite buscarlo más adelante.

1. El filtro aparece en la lista de filtros guardados y se aplica automáticamente a la columna de entrada. Haga clic en la X situada en la parte superior del panel de filtro para cerrarla.

   ![Filtro guardado](assets/intake-filter-dialog8.png)

1. (Opcional) Para compartir el filtro con otros usuarios, pase el ratón sobre el filtro guardado y haga clic en **[!UICONTROL Más]** menú ![Icono del menú Más](assets/more-icon-spectrum.png)y seleccione **[!UICONTROL Compartir]**. Elija los usuarios o equipos con los que compartir en el cuadro Compartir filtros. Para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Opcional) Para incluir tareas y problemas en la columna de entrada, haga clic en **[!UICONTROL Filtrar fuentes]** y seleccione el otro objeto para crear otro filtro.
1. Cuando termine de agregar filtros, revise la columna de entrada para comprobar que aparecen las tareas y los problemas correctos.

   ![Columna de entrada](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Puede actualizar los filtros en cualquier momento abriendo el panel Configurar y haciendo clic en **[!UICONTROL Filtrar fuentes]** y seleccionando **[!UICONTROL Tareas]** o **[!UICONTROL Problemas]**.

## Utilizar la columna de entrada

Las tarjetas de la columna de entrada no se pueden editar hasta que las mueva a otras columnas del tablero. Puede hacer clic en la tarjeta para abrirla en una vista de solo lectura o hacer clic en ![Abrir tarea o problema](assets/boards-launch-icon.png) para abrir la tarea o el problema en una nueva pestaña del explorador.


Puede reordenar manualmente los elementos de la columna de entrada.

Los iconos de la parte superior derecha de la columna de entrada muestran cuántas tarjetas hay actualmente en la columna y cuántos filtros se aplican.

1. (Opcional) Para buscar un elemento en la columna de entrada, haga clic en ![Icono de búsqueda](assets/search-icon.png) en la columna.
1. (Opcional) Para mover una tarjeta de la columna de entrada a otra columna, arrastre y suelte la tarjeta en la posición en la que desee que aparezca.

   O

   Haga clic en **[!UICONTROL Más]** menú ![Icono del menú Más](assets/more-icon-spectrum.png) en la tarjeta y seleccione **[!UICONTROL Mover]**. A continuación, en la **[!UICONTROL Mover elemento]** , elija otra columna y seleccione **[!UICONTROL Mover]**.

1. (Opcional) Para eliminar la columna de entrada, haga clic en **[!UICONTROL Más]** menú ![Icono del menú Más](assets/more-icon-spectrum.png) y seleccione **[!UICONTROL Eliminar]**.
