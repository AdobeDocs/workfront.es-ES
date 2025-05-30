---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Adición de una columna de admisión a un tablero
description: Si lo desea, puede añadir una columna de entrada al tablero que recupere automáticamente las tareas y los problemas como tarjetas conectadas cuando se añadan a Workfront, según los filtros que defina.
author: Courtney
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 68%

---

# Añadir una columna de aceptación a un tablero

<!-- Audited: 5/2025 -->

Si lo desea, puede agregar una columna de entrada al tablero que recupere automáticamente las tareas y los problemas como tarjetas conectadas cuando se agreguen en [!DNL Workfront] según los filtros que defina. La columna de entrada puede servir de registro de asuntos pendientes para un equipo de Kanban, como ubicación de entrada para que un equipo de soporte vea los problemas a medida que se añaden a la cola de solicitudes o para cualquier otro fin.

Solo se permite una columna de entrada en un tablero, que siempre aparece como la columna situada más a la izquierda.

La columna de entrada no está disponible en un tablero dinámico. Sin embargo, puede actualizar los filtros que definen qué tarjetas se llevan a un tablero dinámico. Cuando cambia estos filtros en un tablero dinámico, se restablece la configuración de la tarjeta que no forma parte de la tarea o del problema de Workfront (por ejemplo, las etiquetas).

>[!NOTE]
>
>Por motivos de seguridad, solo el propietario de un tablero puede cambiar los filtros de tablero en el panel Configurar.

La columna de entrada está limitada a 300 tareas y 300 problemas. El orden predeterminado de los elementos de la columna de entrada es el siguiente:

Tareas:

* Orden principal: nombre del proyecto
* Orden secundario: estructura del desglose de trabajo

Problemas:

* Orden principal: nombre del proyecto
* Orden secundario: número de referencia

>[!IMPORTANT]
>
>Se recomienda actualizar el tablero con frecuencia si varios usuarios trabajan en el tablero al mismo tiempo. Actualizar la página mantiene actualizados los cambios visuales en el tablero y evita que problemas como las tarjetas duplicadas se muevan al tablero desde la columna de entrada.
>
>Para sincronizar con Workfront e incluir nuevas tareas y problemas en el tablero o en la columna de entrada, haga clic en el menú Más ![[!UICONTROL menú Más]](assets/more-menu.png) junto al nombre del tablero y seleccione Sincronizar elementos conectados.

Para obtener más información sobre las columnas, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Para obtener información sobre las tarjetas conectadas, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una columna de entrada mediante filtros simples

{{step1-to-boards}}

1. En el tablero de mandos, seleccione un tablero.
1. Haga clic en **Configurar** a la derecha del tablero para abrir el panel **Configurar**.
1. Seleccione la sección **Board**. Aparecerán nuevos campos.
1. Activar **introducir elementos de forma dinámica en el tablero**. La columna de entrada en blanco aparece en el lado izquierdo del tablero.

   ![Opciones de filtro simple de columna de entrada](assets/intake-column-simple-filters.png)

1. (Opcional) Busque y seleccione [!DNL Workfront] [!UICONTROL **Proyectos**].
1. (Opcional) Busque y seleccione el usuario o equipo [!UICONTROL **asignaciones**].
1. Seleccione [!UICONTROL **Incluir el trabajo completado**] para mostrar las tareas y los problemas con el estado Completado en la columna de entrada.

   >[!NOTE]
   >
   >Si esta opción no está seleccionada, cuando las tarjetas en otros estados se marquen como completadas, no se mostrarán en el tablero.

1. Haga clic en **Aplicar**. Los objetos aparecen en la columna de entrada del tablero como tarjetas conectadas.

   ![Columna de entrada](assets/intake-column-added3.png)

## Creación de una columna de entrada con filtros avanzados

{{step1-to-boards}}

1. En el tablero de mandos, seleccione un tablero.
1. Haga clic en **Configurar** a la derecha del tablero para abrir el panel **Configurar**.
1. Seleccione la sección **Board**. Aparecerán nuevos campos.
1. Activar **introducir elementos de forma dinámica en el tablero**. La columna de entrada en blanco aparece en el lado izquierdo del tablero.

1. Haga clic en [!UICONTROL **Utilizar filtros avanzados**].

1. Haga clic en **[!UICONTROL Agregar orígenes de filtro]** y, a continuación, seleccione **[!UICONTROL Tareas]** o **[!UICONTROL Problemas]**.

   ![Opciones de filtro avanzadas de columna de entrada](assets/add-filter-sources-options.png)

   >[!NOTE]
   >
   >Se puede filtrar la columna de entrada para incluir tareas y problemas, pero los filtros se deben configurar por separado para cada tipo de objeto.
   >
   >Además, los filtros guardados y los filtros predeterminados del sistema están disponibles para su selección.

1. En el panel de filtros, haga clic en **[!UICONTROL Nuevo filtro]**.

1. Genere el filtro y luego haga clic en **[!UICONTROL Guardar como nuevo]**.

   ![Generador de filtros](assets/intake-filter-dialog6.png)

   El ejemplo anterior muestra un filtro para tareas de un proyecto específico que están en estado de [!UICONTROL Nuevo] o [!UICONTROL En curso].

   >[!NOTE]
   >
   >Se recomienda no utilizar el comodín “Yo” (usuario que ha iniciado sesión) en un filtro de tablero, ya que no se garantiza que siempre se muestren tareas o problemas para dicho usuario. Una vez configurado el tablero con las tareas y los problemas correspondientes, se puede filtrar el tablero para mostrar los elementos de un asignado específico. Para obtener más información, consulte [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   Para obtener más información acerca de cómo crear un filtro, vea la sección Crear o editar un filtro en el generador estándar en el artículo [Crear o editar filtros en [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Asigne un nombre al filtro y haga clic en **[!UICONTROL Guardar]**. El filtro aparece en la lista de filtros guardados y se aplica automáticamente a la columna de entrada.

   ![Escribiendo un nuevo nombre de filtro](assets/save-as-modal.png)

1. Haga clic en la X de la parte superior derecha del panel de filtro para cerrarlo.

1. (Opcional) Para compartir el filtro, pase el puntero por encima del filtro guardado, haga clic en el **[!UICONTROL icono de menú]** Más![del menú Más](assets/more-menu.png) y seleccione **[!UICONTROL Compartir]**. Elija los usuarios o equipos con los que compartir en el cuadro **Uso compartido de filtros**. Para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Opcional) Para incluir tareas y problemas en la columna de entrada, haga clic en **[!UICONTROL Fuentes de filtro]** y seleccione el otro objeto para crear otro filtro.
1. Cuando haya terminado de añadir filtros, revise la columna de entrada para comprobar que aparecen las tareas y los problemas correctos.

   ![Columna de entrada](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Puede actualizar los filtros en cualquier momento desde el panel Configurar, haciendo clic en **[!UICONTROL Fuentes de filtro]** y seleccionando **[!UICONTROL Tareas]** o **[!UICONTROL Problemas]**.

## Utilizar la columna de entrada

Para poder editar las tarjetas de la columna de entrada, debe moverlas a otras columnas del tablero. Haga clic en la tarjeta para abrirla en una vista de solo lectura, o bien haga clic en ![Abrir tarea o problema](assets/boards-launch-icon.png) para abrir la tarea o el problema en una nueva pestaña del explorador.

Los elementos de la columna de entrada se pueden reordenar manualmente.

En la parte superior derecha de la columna de entrada, los iconos muestran cuántas tarjetas hay en la columna y cuántos filtros se aplican.

1. (Opcional) Para buscar un elemento en la columna de entrada, haga clic en ![Buscar icono](assets/search-icon.png).
1. (Opcional) Para mover una tarjeta de la columna de entrada a otra columna, arrastre y suelte la tarjeta en la posición en la que desee que aparezca.

   O

   Haga clic en el **[!UICONTROL icono de menú]** Más ![del menú Más](assets/more-menu.png) de la tarjeta y seleccione **[!UICONTROL Mover]**. A continuación, en el cuadro **Mover [ELEMENTO]**, elija otra columna y seleccione **[!UICONTROL Mover]**.

1. (Opcional) Para eliminar la columna de entrada, haga clic en el **[!UICONTROL icono de menú Más]** del menú ![Más](assets/more-menu.png) y seleccione **[!UICONTROL Eliminar]**.
