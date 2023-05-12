---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Agregar una columna de admisión a un tablero
description: Si lo desea, puede agregar una columna de admisión al tablero que extraiga automáticamente tareas y problemas como tarjetas conectadas cuando se agregan en Workfront, en función de los filtros definidos.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 5e73603b695ff7456216ca7a4e15ce527b01559d
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Agregar una columna de admisión a un tablero

Si lo desea, puede agregar una columna de admisión al tablero que extraiga automáticamente tareas y problemas como tarjetas conectadas cuando se agregan [!DNL Workfront], en función de los filtros definidos. La columna de admisión puede servir como columna de trabajo pendiente para un equipo de Kanban, ubicación de admisión para un equipo de asistencia para ver los problemas a medida que se añaden a una cola de solicitudes o cualquier otro propósito que necesite.

En un tablero solo se permite una columna de admisión y siempre aparece como la columna situada más a la izquierda.

La columna de admisión no está disponible en un panel dinámico.

La columna de admisión está limitada a 300 tareas y 300 problemas. Se ordenan por la prioridad definida en los elementos. Para obtener información sobre la prioridad, consulte [Actualizar prioridad de tareas](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) y [Actualizar prioridad del problema](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

Para obtener más información sobre las columnas, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Para obtener información sobre tarjetas conectadas, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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

## Creación de una columna de admisión mediante filtros simples

>[!NOTE]
>
>Los filtros simples solo están disponibles a través de la opción de inclusión de las funciones iniciales para los tableros de Adobe Workfront.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar .
1. Expandir **[!UICONTROL Consejo]**.
1. Activar **[!UICONTROL Ingesta dinámica de elementos a bordo]**.

   ![Opciones de filtro simple de la columna de entrada](assets/intake-column-simple-filters.png)

   La columna de admisión se añade a la izquierda del tablero. Permanecerá en blanco hasta que se le apliquen filtros.

1. (Opcional) Busque y seleccione [!DNL Workfront] [!UICONTROL **Proyectos**].
1. (Opcional) Busque y seleccione un usuario o equipo [!UICONTROL **Asignaciones**].
1. Select [!UICONTROL **Incluir trabajo completado**] para mostrar las tareas y los problemas con un estado de finalización en la columna de admisión.

   >[!NOTE]
   >
   >Si esta opción no está seleccionada, cuando las tarjetas de otros estados se marquen como completas, se &quot;quitarán&quot; el tablero y ya no se mostrarán.

1. Haga clic en [!UICONTROL **Aplicar**].

   Todos los objetos aparecen como tarjetas conectadas en la columna de admisión del tablero.

   ![Columna de entrada](assets/intake-column-added3.png)

## Creación de una columna de admisión mediante filtros avanzados

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar .
1. Expandir **[!UICONTROL Consejo]**.
1. Activar **[!UICONTROL Ingesta dinámica de elementos a bordo]**.

   La columna de admisión se añade a la izquierda del tablero. Permanecerá en blanco hasta que se le apliquen filtros.

1. Haga clic en [!UICONTROL **Usar filtros avanzados**].
1. Haga clic en **[!UICONTROL Fuentes de filtro]** y seleccione **[!UICONTROL Tareas]** o **[!UICONTROL Problemas]**.

   ![Opciones de filtro avanzado de la columna de entrada](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Puede filtrar la columna de admisión para incluir tareas y problemas, pero debe configurar los filtros por separado para cada tipo de objeto.
   >
   >Además, los filtros guardados y los filtros predeterminados del sistema están disponibles para su selección.

1. En el panel de filtro, haga clic en **[!UICONTROL Nuevo filtro]** para empezar.

   ![Haga clic en Nuevo filtro](assets/intake-filter-dialog5.png)

1. Cree el filtro y haga clic en **[!UICONTROL Guardar como nuevo]**.

   ![Generador de filtros](assets/intake-filter-dialog6.png)

   Este ejemplo muestra un filtro para tareas de un proyecto específico que se encuentran en el estado de [!UICONTROL Nuevo] o [!UICONTROL En curso], y se me asignan.

   Para obtener más información sobre la creación de filtros, consulte la sección &quot;Creación o edición de filtros en el generador estándar&quot; en el artículo [Crear o editar filtros en [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Asigne un nombre al filtro y haga clic en **[!UICONTROL Guardar]**.

   ![Escriba un nombre para el filtro](assets/intake-filter-dialog7.png)

   Asignar al filtro un nombre único le permite buscarlo más adelante.

1. El filtro aparece en la lista de filtros guardados y se aplica automáticamente a la columna de admisión. Haga clic en la X en la parte superior del panel de filtro para cerrarla.

   ![Filtro guardado](assets/intake-filter-dialog8.png)

1. (Opcional) Para compartir el filtro con otros usuarios, pase el ratón sobre el filtro guardado y haga clic en el botón **[!UICONTROL Más]** menú ![Más icono de menú](assets/more-icon-spectrum.png)y seleccione **[!UICONTROL Compartir]**. Elija los usuarios o equipos con los que desea compartir en el cuadro Compartir filtros . Para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Opcional) Para incluir tareas y problemas en la columna de admisión, haga clic en **[!UICONTROL Fuentes de filtro]** y seleccione el otro objeto para crear otro filtro.
1. Cuando haya terminado de añadir filtros, revise la columna de admisión para comprobar que aparecen las tareas y los problemas correctos.

   ![Columna de entrada](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Puede actualizar los filtros en cualquier momento abriendo el panel Configurar , haciendo clic en **[!UICONTROL Fuentes de filtro]** y seleccionando **[!UICONTROL Tareas]** o **[!UICONTROL Problemas]**.

## Utilice la columna de admisión

Las tarjetas de la columna de admisión no se pueden editar hasta que se mueven a otras columnas de la placa. Puede hacer clic en la tarjeta para abrirla en una vista de solo lectura o hacer clic en ![Abrir tarea o problema](assets/boards-launch-icon.png) para abrir la tarea o el problema en una nueva pestaña del navegador.


Puede reordenar manualmente los elementos de la columna de admisión.

Los iconos de la parte superior derecha de la columna de admisión muestran cuántas tarjetas hay actualmente en la columna y cuántos filtros se aplican.

1. (Opcional) Para buscar un elemento en la columna de admisión, haga clic en ![Icono de búsqueda](assets/search-icon.png) en la columna .
1. (Opcional) Para mover una tarjeta de la columna de admisión a otra columna, arrastre y suelte la tarjeta en la posición en la que desea que aparezca.

   O

   Haga clic en el **[!UICONTROL Más]** menú ![Más icono de menú](assets/more-icon-spectrum.png) en la tarjeta y seleccione **[!UICONTROL Mover]**. A continuación, en el **[!UICONTROL Mover elemento]** , elija otra columna y seleccione **[!UICONTROL Mover]**.

1. (Opcional) Para eliminar la columna de admisión, haga clic en el botón **[!UICONTROL Más]** menú ![Más icono de menú](assets/more-icon-spectrum.png) y seleccione **[!UICONTROL Eliminar]**.
