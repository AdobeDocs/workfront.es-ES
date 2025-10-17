---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Crear o editar un tablero
description: En el panel de control [!UICONTROL tableros], puede crear un nuevo tablero o editar uno existente.
author: Jenny
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 91%

---

# Crear o editar un tablero

<!-- Audited: 12/2023 -->

En el panel de control [!UICONTROL tableros], puede crear un nuevo tablero o editar uno existente.

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

## Crea un nuevo tablero

{{step1-to-boards}}

1. Haga clic en **[!UICONTROL Añadir tablero]**.

1. Seleccione una plantilla para el tablero.

   | Plantilla | Descripción |
   |---------|----------|
   | Tablero básico | Se proporcionan tres columnas predeterminadas en el tablero. Puede añadir nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas. <p>Se proporcionan tres columnas predeterminadas en el tablero. Puede añadir nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas. |
   | Tablero Kanban | Se proporcionan las siguientes columnas en el tablero: Registro de pendientes, Nuevo, En curso, Completado y En espera. Puede añadir nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas.<p>Para utilizar el registro de pendientes, debe configurar filtros para la columna de entrada. Para obtener más información, consulte [Añadir una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para revisar las políticas predeterminadas de cada columna, haga clic en el menú [!UICONTROL **Más**] de una columna y seleccione [!UICONTROL **Editar**]. Puede cambiar cualquiera de estas políticas preconfiguradas. Para obtener más información, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Tablero retrospectivo | En el tablero se proporcionan las siguientes columnas: ¿Qué ha ido bien? ¿Qué se podría mejorar? ¿A quién debemos felicitar? ¿Qué podemos hacer para avanzar más rápido? Puede añadir nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas. <p>No se aplican políticas de columna. |
   | Tablero dinámico | Se proporcionan las siguientes columnas en el tablero: Deseleccionado, Nuevo, En curso, En espera y Completado. Puede añadir nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas. (Se puede cambiar el nombre de la columna Deseleccionado, pero no eliminarla. Esta columna contiene todas las tarjetas con un estado que no coincide con ninguno de los demás estados de columna). <p>Las políticas de columna predeterminadas asignan tarjetas a las columnas en función de su estado. Para obtener más información, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Para un tablero dinámico únicamente, siga los pasos del asistente de configuración:

   1. Escriba un nombre para el tablero y haga clic en [!UICONTROL **Siguiente**].
   1. Busque y seleccione [!DNL Workfront] [!UICONTROL **Proyectos**] para incluir tareas y problemas en el tablero.
   1. Busque y seleccione [!UICONTROL **Asignaciones**] para incluir tareas y problemas en el tablero.

      Todos los objetos aparecen en el tablero como tarjetas conectadas.

      El contador de [!UICONTROL **Tarjetas añadidas**] muestra cuántas tarjetas habrá en el tablero. Por ejemplo, si selecciona un proyecto con 100 tareas y problemas, el contador mostrará 100. Si añade una asignación de usuario y a esa persona se le han asignado 5 tareas en el proyecto, el contador mostrará 5.

      >[!NOTE]
      >
      >El límite de tarjetas de los tableros dinámicos es de 700 tareas y 700 problemas, lo que hace un total de 1400 tarjetas. Un alto número de tarjetas en el tablero puede afectar el rendimiento del tablero. Todas las tarjetas archivadas, tanto ocultas como visibles, se contabilizan en este límite.

   1. (Opcional) Seleccione [!UICONTROL **No archivar las tarjetas completadas**] para llevar las tareas y los problemas completados al tablero como tarjetas visibles en la columna Completada. Cuando esta opción no está seleccionada, las tarjetas completadas en el momento de la creación del tablero se incorporan al tablero como tarjetas archivadas.

      >[!NOTE]
      >
      >De forma predeterminada, las tarjetas archivadas no se muestran en el tablero. Para mostrar las tarjetas archivadas, debe activar una configuración y filtrar el tablero para mostrar las tarjetas archivadas. Para obtener más información, consulte [Personalizar campos a mostrar en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) y [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Opcional) Haga clic en [!UICONTROL **Usar filtros avanzados**] para mostrar opciones de filtro adicionales.

      Es el mismo proceso que cuando se crea un filtro en una columna de entrada. Para obtener más información, consulte [Añadir una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Si actualizan los filtros de un panel dinámico después de crearlos, se restablecerán los ajustes de la tarjeta que no formen parte de la tarea o del problema de Workfront (como las etiquetas).

   1. Tras añadir los filtros, haga clic en [!UICONTROL **Crear tablero**].

1. Escriba un nombre para el tablero en el campo **[!UICONTROL Tablero]** y presione Intro.
1. Configure el tablero según sea necesario.

   Para obtener más información, consulte [Añadir o quitar miembros de un tablero](../../agile/get-started-with-boards/add-members-to-board.md), [Administrar columnas del tablero](../../agile/get-started-with-boards/manage-board-columns.md), [Añadir una tarjeta ad hoc a un tablero](../../agile/get-started-with-boards/add-card-to-board.md) y [Usar tarjetas conectadas en los tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Haga clic en **[!UICONTROL Todos los tableros]** para volver al panel de control de tableros.

   También puede localizar el menú desplegable etiquetado con el nombre del tablero actual y hacer clic en él para cambiar a otro tablero.

   ![Lista de tableros](assets/boards-button-list-of-boards-350x188.png)

## Editar un tablero existente

{{step1-to-boards}}

1. En el panel de control, seleccione el tablero que desea abrir.
1. Edite el tablero según sea necesario. Puede hacer clic en el nombre del tablero para cambiarle el nombre.

   Para sincronizar tarjetas conectadas con Workfront e incluir nuevas tareas y problemas en la columna de entrada o tablero, haz clic en el menú **[!UICONTROL Más]** ![[!UICONTROL Menú Más]](assets/more-icon-spectrum.png) que está junto al nombre del tablero y selecciona **[!UICONTROL Sincronizar elementos conectados]**.

   Para obtener más información, consulte [Añadir o quitar miembros de un tablero](../../agile/get-started-with-boards/add-members-to-board.md), [Administrar columnas del tablero](../../agile/get-started-with-boards/manage-board-columns.md) y [Añadir una tarjeta a un tablero](../../agile/get-started-with-boards/add-card-to-board.md).

1. Haga clic en **[!UICONTROL Todos los tableros]** para volver al panel de control de tableros.

   También puede localizar el menú desplegable etiquetado con el nombre del tablero actual y hacer clic en él para cambiar a otro tablero.

