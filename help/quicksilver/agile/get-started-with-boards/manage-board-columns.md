---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Administrar columnas de tablero
description: Un tablero nuevo contiene tres columnas de forma predeterminada. Puede agregar más columnas, cambiar el orden de las columnas, cambiar el nombre de las columnas y eliminar las columnas que no necesite.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 2dfa3e7b215a8234453b2d688031c993978e02ae
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Administrar columnas de tablero

Un tablero nuevo contiene tres columnas de forma predeterminada. Puede agregar más columnas, cambiar el orden de las columnas, cambiar el nombre de las columnas y eliminar las columnas que no necesite.

La configuración de columna incluye políticas que le permiten definir las opciones para lo que sucede con una tarjeta cuando se mueve a esa columna.

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

## Agregar una columna a un tablero

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Agregar columna]** a la derecha de las columnas existentes.
1. En la nueva columna, escriba un nombre y haga clic en **[!UICONTROL Agregar columna]**.

   ![Añadir nueva columna](assets/boards-add-column.png)

>[!TIP]
>
>Para añadir una columna de admisión, consulte [Agregar una columna de admisión a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Reordenar columnas en un tablero

1. Acceda al tablero.
1. Arrastre y suelte las columnas en el orden correcto. Asegúrese de seleccionar la parte superior de la columna antes de arrastrarla a otra ubicación.

   ![Arrastrar y soltar columnas](assets/boards-dragdropcolumn.png)

## Cambiar el nombre de una columna de tablero

1. Acceda al tablero.
1. Haga clic en el nombre de la columna, escriba el nuevo nombre y pulse Intro.

   O

   Haga clic en el **[!UICONTROL Más]** menú ![Más menú](assets/more-icon-spectrum.png) en la columna y seleccione **[!UICONTROL Editar]**. En el área Configuración, escriba el nuevo nombre en la **[!UICONTROL Nombre de columna]** y haga clic en **[!UICONTROL Cerrar]**.

## Eliminar una columna de tablero

1. Acceda al tablero.
1. Haga clic en el **[!UICONTROL Más]** menú ![Más menú](assets/more-icon-spectrum.png) en la columna y seleccione **[!UICONTROL Eliminar]**.

   >[!NOTE]
   >
   >Las columnas que contienen tarjetas, incluidas las archivadas, no se pueden eliminar. Si intenta eliminar una columna que contenga tarjetas, debe elegir otra columna para esas tarjetas.

## Mostrar recuento de tarjetas

Puede utilizar una configuración para mostrar el número de tarjetas en cada columna.

Si utiliza el límite de WIP en una columna, no se agregará un contador de tarjeta independiente. Para obtener más información sobre los límites de WIP, consulte [Administre el [!UICONTROL Trabajo en curso] Límite (WIP) en un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Acceda al tablero.
1. Haga clic en **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar .
1. Expandir **[!UICONTROL Columna]**.
1. Activar **[!UICONTROL Mostrar un recuento de tarjetas de columna]**.

   ![Activar contador de tarjeta](assets/display-card-count.png)

   El contador de tarjetas aparece en la parte superior de cada columna.

1. Haga clic en **[!UICONTROL Ocultar configurar]** para cerrar el [!UICONTROL Configurar] panel.

## Definir la configuración y las políticas de la columna

1. Acceda al tablero.
1. Haga clic en el **[!UICONTROL Más]** menú ![Más menú](assets/more-icon-spectrum.png) en la columna y seleccione **[!UICONTROL Editar]**.

   La variable [!UICONTROL Configuración] aparece. La variable **[!UICONTROL Nombre de columna]** permite saber para qué columna se define la configuración.

1. Active la variable **[!UICONTROL Actualizar valores de campo automáticamente]** directiva para cambiar automáticamente ciertos valores de campo cuando se mueve una tarjeta a esta columna.

   ![Configuración y políticas de columna](assets/boards-column-policies-enabled.png)

1. (Opcional) Establezca un valor para el estado de la tarjeta:

   1. Seleccione el **[!UICONTROL Estado]** en el Navegador.

   1. Seleccione el estado que se aplicará a una tarjeta cuando se mueva a esta columna.

      ![Estado de las columnas](assets/boards-column-status.png)

      También se muestran las opciones de traducción del estado de las tarjetas conectadas. (La traducción del estado no se aplica a las tarjetas ad hoc). Estas opciones determinan el estado que se aplica a la tarea o al problema en [!DNL Workfront] cuando se mueve una tarjeta conectada a esta columna.

   1. Para cambiar las selecciones de traducción de estado predeterminadas, haga clic en el botón **[!UICONTROL Editar]** icono ![Icono Editar](assets/edit-icon-spectrum.png).
   1. Seleccione un estado para las tareas y un estado para los problemas. Solo el valor predeterminado [!DNL Workfront] los estados están disponibles, no los personalizados.

   >[!NOTE]
   >
   >Si utiliza estados personalizados en [!DNL Workfront], la primera vez que mueva una tarjeta conectada a esta columna se le pedirá que elija un estado. Por ejemplo, si el proyecto conectado tiene varios tipos de estado a los que corresponden todos [!UICONTROL Completado], debe elegir qué estado utilizar en [!DNL Workfront]. Puede establecer su opción como predeterminada para que no tenga que realizar la selección cada vez que mueva una tarjeta a la columna.
   >Para obtener más información sobre los estados, consulte [Resumen de los estados](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

1. (Opcional) Establezca un valor para los asignadores de tarjetas:

   1. Seleccione el **[!UICONTROL Destinatarios]** en el Navegador.
   1. Seleccione una acción.

      * **[!UICONTROL Agregar en usuarios asignados]:** Los usuarios asignados que seleccione se añadirán a la lista existente de usuarios asignados en una tarjeta cuando se mueva a esta columna.
      * **[!UICONTROL Anular asignaciones]:** Los usuarios asignados que seleccione anulan a todos los demás usuarios asignados y se convierten en los únicos usuarios asignados de una tarjeta cuando se mueve a esta columna.
   1. Seleccione los usuarios asignados en la lista desplegable. Solo los miembros del consejo están disponibles para elegir. Para obtener más información, consulte [Agregar o quitar miembros de un tablero](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![Asignados para la columna](assets/boards-column-assignees.png)


1. (Opcional) Establezca un valor para las etiquetas de tarjeta:

   1. Seleccione el **[!UICONTROL Tarjetas]** en el Navegador.
   1. Seleccione una acción.

      * **[!UICONTROL Añadir en etiquetas]:** Las etiquetas que seleccione se añaden a la lista existente de etiquetas en una tarjeta cuando se mueve a esta columna.
      * **[!UICONTROL Anular etiquetas]:** Las etiquetas que seleccione anulan todas las demás etiquetas y se convierten en las únicas etiquetas de una tarjeta cuando se mueve a esta columna.
   1. Seleccione las etiquetas en la lista desplegable. Solo las etiquetas que ya se hayan creado en la variable [!UICONTROL Administrador de etiquetas] están disponibles para elegir. Para obtener información sobre cómo agregar nuevas etiquetas, consulte [Agregar etiquetas](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Etiquetas para la columna](assets/boards-column-tags.png)


1. Active la variable **[!UICONTROL Límite de trabajo en curso]** directiva para limitar el número de tarjetas que se pueden agregar a la columna. A continuación, escriba el número límite en la variable **[!UICONTROL Establecer límite]** campo .

   ![Límite de trabajo en curso para columna](assets/boards-wip-limit-in-column.png)

   Para obtener más información, consulte [Administrar el límite de trabajo en curso (WIP) en un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Haga clic en **[!UICONTROL Cerrar]** para salir del área Configuración y ver la columna y sus tarjetas.
