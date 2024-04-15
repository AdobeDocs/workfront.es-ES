---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Administrar columnas de tablero
description: Un tablero nuevo contiene tres columnas de forma predeterminada. Puede agregar más columnas, cambiar el orden de las columnas, cambiar el nombre de las columnas y eliminar las columnas que no necesite.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Administrar columnas de tablero

Un tablero nuevo contiene tres columnas de forma predeterminada. Puede agregar más columnas, cambiar el orden de las columnas, cambiar el nombre de las columnas y eliminar las columnas que no necesite.

La configuración de columna incluye directivas, que le permiten definir opciones para lo que sucede con una tarjeta cuando se mueve a esa columna.

Para obtener información sobre cómo ordenar las tarjetas en las columnas, consulte [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Añadir una columna a un tablero

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic **[!UICONTROL Agregar columna]** a la derecha de las columnas existentes.
1. En la nueva columna, escriba un nombre y haga clic en **[!UICONTROL Agregar columna]**.

   ![Añadir nueva columna](assets/boards-add-column.png)

>[!TIP]
>
>Para añadir una columna de entrada, consulte [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Reordenar columnas en un tablero

1. Acceda al tablero.
1. Arrastre y suelte las columnas en el orden correcto. Asegúrese de seleccionar la parte superior de la columna antes de arrastrarla a otra ubicación.

   ![Arrastrar y soltar columna](assets/boards-dragdropcolumn.png)

## Cambiar nombre de columna de tablero

1. Acceda al tablero.
1. Haga clic en el nombre de la columna, escriba el nuevo nombre y pulse Intro.

   O

   Haga clic en **[!UICONTROL Más]** menú ![Menú Más](assets/more-icon-spectrum.png) en la columna y seleccione **[!UICONTROL Editar]**. En el área Configuración, escriba el nuevo nombre en la **[!UICONTROL Nombre de columna]** y haga clic en **[!UICONTROL Cerrar]**.

## Eliminar una columna del tablero

Cuando se elimina una columna de un tablero, no se puede recuperar.

1. Acceda al tablero.
1. Haga clic en **[!UICONTROL Más]** menú ![Menú Más](assets/more-icon-spectrum.png) en la columna y seleccione **[!UICONTROL Eliminar]**.

   >[!NOTE]
   >
   >Las columnas que contienen tarjetas, incluidas las tarjetas archivadas, no se pueden eliminar. Si intenta eliminar una columna que contiene tarjetas, debe elegir otra columna para esas tarjetas.

## Mostrar recuento de tarjetas

Puede utilizar una configuración para mostrar el número de tarjetas en cada columna.

Si utiliza el límite de trabajo en curso en una columna, no se agrega un contador de tarjetas independiente. Para obtener más información sobre los límites de WIP, consulte [Administrar el [!UICONTROL Trabajo en curso] Límite (WIP) en un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Acceda al tablero.
1. Clic **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar.
1. Expandir **[!UICONTROL Columna]**.
1. Activar **[!UICONTROL Mostrar un recuento de tarjetas de columna]**.

   ![Activar el contador de tarjetas](assets/display-card-count.png)

   El contador de tarjetas aparece en la parte superior de cada columna.

1. Clic **[!UICONTROL Ocultar configuración]** para cerrar el [!UICONTROL Configurar] panel.

## Definir la configuración y las directivas de columna

>[!NOTE]
>
>Los tableros dinámicos siempre colocan tarjetas en la columna que coincide con su estado, independientemente de si las directivas de columna están habilitadas o deshabilitadas. Las tarjetas volverán a sus columnas asignadas cuando actualice el tablero.

1. Acceda al tablero.
1. Haga clic en **[!UICONTROL Más]** menú ![Menú Más](assets/more-icon-spectrum.png) en la columna y seleccione **[!UICONTROL Editar]**.

   El [!UICONTROL Configuración] aparece el área. El **[!UICONTROL Nombre de columna]** le permite saber para qué columna está definiendo la configuración.

1. Habilite la **[!UICONTROL Actualizar valores de campo automáticamente]** directiva para cambiar automáticamente ciertos valores de campo cuando se mueva una tarjeta a esta columna.

   ![Configuración y directivas de columna](assets/boards-column-policies-enabled.png)

1. (Opcional) Establezca un valor para el estado de la tarjeta:

   1. Seleccione el **[!UICONTROL Estado]** casilla de verificación.

   1. Seleccione el estado que se aplicará a una tarjeta cuando se mueva a esta columna.

      ![Estado de las columnas](assets/boards-column-status.png)

      También se muestran las opciones de traducción de estado de las tarjetas conectadas. (La traducción de estado no se aplica a tarjetas ad hoc). Estas opciones determinan el estado personalizado aplicado a la tarea o al problema en [!DNL Workfront] cuando se mueva una tarjeta conectada a esta columna.

   1. Seleccione una [!UICONTROL **Personalizado**] estado que se aplicará a la tarjeta para tareas y problemas.

      Cuando se mueve una tarjeta a esta columna, [!DNL Workfront] intenta aplicar primero el estado personalizado (por ejemplo, Resuelto). Si el estado personalizado seleccionado no está disponible para esa tarjeta, se le pedirá que elija otro estado que corresponda al estado del sistema (del paso b anterior). Para obtener más información sobre los estados, consulte [Resumen de estados](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Además, si el estado de la tarea o del problema conectado se cambia al estado personalizado o del sistema establecido en la directiva de columnas, la tarjeta se mueve automáticamente a la columna.

1. (Opcional) Establezca un valor para las personas asignadas a la tarjeta:

   1. Seleccione el **[!UICONTROL Asignados]** casilla de verificación.
   1. Seleccione una acción.

      * **[!UICONTROL Agregar a usuarios asignados]:** Las personas asignadas que seleccione se agregarán a la lista existente de personas asignadas en una tarjeta cuando se mueva a esta columna.
      * **[!UICONTROL Anular asignados]:** Los usuarios asignados que seleccione anularán todos los demás usuarios asignados y se convertirán en los únicos usuarios asignados de una tarjeta cuando se mueva a esta columna.

   1. Clic [!UICONTROL **Agregar asignación**] y busque un usuario. Seleccione los usuarios asignados en los resultados de búsqueda. Todos los usuarios y equipos de Workfront están disponibles para elegir.

      ![Usuarios asignados para la columna](assets/boards-column-assignees.png)

1. (Opcional) Establezca un valor para las etiquetas de tarjeta:

   1. Seleccione el **[!UICONTROL Tarjetas]** casilla de verificación.
   1. Seleccione una acción.

      * **[!UICONTROL Agregar en etiquetas]:** Las etiquetas que seleccione se añadirán a la lista de etiquetas existente en una tarjeta cuando se mueva a esta columna.
      * **[!UICONTROL Anular etiquetas]:** Las etiquetas que seleccione anularán todas las demás etiquetas y se convertirán en las únicas etiquetas de una tarjeta cuando se mueva a esta columna.

   1. Seleccione las etiquetas de la lista desplegable. Solo las etiquetas ya creadas en [!UICONTROL Administrador de etiquetas] están disponibles para elegir. Para obtener información sobre cómo añadir nuevas etiquetas, consulte [Añadir etiquetas](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Etiquetas para la columna](assets/boards-column-tags.png)

1. Habilite la **[!UICONTROL Límite de trabajo en curso]** directiva para limitar el número de tarjetas que se pueden agregar a la columna. A continuación, escriba el número de límite en la **[!UICONTROL Establecer límite]** field.

   ![Límite de trabajo en curso para columna](assets/boards-wip-limit-in-column.png)

   Para obtener más información, consulte [Administrar el límite de trabajo en curso (WIP) en un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Clic **[!UICONTROL Cerrar]** para salir del área de Configuración y ver la columna y sus tarjetas.
