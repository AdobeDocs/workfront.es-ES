---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Administrar columnas de tablero
description: Un tablero nuevo contiene tres columnas de forma predeterminada. Puede añadir más columnas, cambiar el orden, cambiarles el nombre y eliminar las que no necesite. También puede definir directivas de columna.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 97b2118b1897f75dea0e45758e3d7f7c3409b234
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 96%

---

# Administrar columnas de tablero

<!-- Audited: 05/2024 -->

Un tablero nuevo contiene tres columnas de forma predeterminada. Puede añadir más columnas, cambiar el orden, cambiarles el nombre y eliminar las que no necesite.

La configuración de columna incluye directivas, las cuales le permiten definir opciones para lo que sucede con una tarjeta cuando se mueve a esa columna.

Para obtener más información sobre cómo ordenar las tarjetas en columnas, vea [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: colaborador o superior </p>
        <p>o</p> 
        <p>Actual: [!UICONTROL Request] o superior </p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una columna a un tablero

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Añadir columna]** a la derecha de las columnas existentes.
1. En la nueva columna, escriba un nombre y haga clic en **[!UICONTROL Añadir columna]**.

   ![Añadir nueva columna](assets/boards-add-column.png)

>[!TIP]
>
>Para añadir una columna de entrada, consulte [Añadir una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Reordenar columnas en un tablero

1. Acceda al tablero.
1. Arrastre y suelte las columnas en el orden correcto. Asegúrese de seleccionar la parte superior de la columna antes de arrastrarla a otra ubicación.

   ![Arrastre y suelte la columna](assets/boards-dragdropcolumn.png)

## Cambiar nombre de columna de tablero

1. Acceda al tablero.
1. Haga clic en el nombre de la columna, escriba el nuevo nombre y pulse Intro.

   O

   Haga clic en el menú **[!UICONTROL Más]** ![menú Más](assets/more-icon-spectrum.png) de la columna y seleccione **[!UICONTROL Editar]**. En el área Configuración, escriba el nuevo nombre en el campo **[!UICONTROL Nombre de la columna]** y haga clic en **[!UICONTROL Cerrar]**.

## Eliminar una columna del tablero

Cuando se elimina una columna de un tablero, no se puede recuperar.

1. Acceda al tablero.
1. Haga clic en el menú **[!UICONTROL Más]** ![menú Más](assets/more-icon-spectrum.png) de la columna y seleccione **[!UICONTROL Eliminar]**.

   >[!NOTE]
   >
   >Las columnas que contienen tarjetas, incluidas las tarjetas archivadas, no se pueden eliminar. Si quiere eliminar una columna que contiene tarjetas, deberá elegir otra columna en donde contener esas tarjetas.

## Mostrar recuento de tarjetas

Puede utilizar un ajuste de configuración para mostrar el número de tarjetas en cada columna.

Si utiliza el límite de trabajo en curso en una columna, no se añade un contador de tarjetas independiente. Para obtener más información sobre los límites de WIP, consulte [Administrar el límite de [!UICONTROL Trabajo en curso] (WIP) en un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Acceda al tablero.
1. Haga clic en **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar.
1. Expanda **[!UICONTROL Columna]**.
1. Active **[!UICONTROL Mostrar un recuento de tarjetas de columna]**.

   ![Activar el contador de tarjetas](assets/display-card-count.png)

   El contador de tarjetas aparece en la parte superior de cada columna.

1. Haga clic en **[!UICONTROL Ocultar configuración]** para cerrar el panel [!UICONTROL Configurar].

## Definición de la configuración y las directivas de columna

Las directivas de columna incluyen la actualización automática de los valores de campo y la configuración de un límite de trabajo en curso.

La directiva para actualizar el estado funciona automáticamente tanto para la tarjeta como para la columna:

* Cuando se mueve una tarjeta a una columna con una directiva, el estado de la tarjeta se actualiza al estado definido en esa directiva. Esto se aplica tanto a las tarjetas ad hoc como a las tarjetas conectadas.
* Cuando se actualiza un estado ad hoc o conectado en la tarjeta para que coincida con el estado de la columna en la directiva, o cuando se actualiza un estado conectado de tarjeta en cualquier otra parte de Workfront, la tarjeta se mueve automáticamente a esa columna. Además, si un estado personalizado de una tarjeta coincide con el estado del sistema asignado a la columna, la tarjeta se mueve a esa columna.

Una tarjeta permanecerá en la columna donde se coloque si el estado de la tarjeta no coincide con ningún estado establecido en ninguna directiva de la columna existente.

1. Acceda al tablero.
1. Haga clic en el menú **[!UICONTROL Más]** ![menú Más](assets/more-icon-spectrum.png) de la columna y seleccione **[!UICONTROL Editar]**.

   Aparecerá el área [!UICONTROL Configuración]. El **[!UICONTROL nombre de la columna]** le permite saber para qué columna está definiendo la configuración.

1. Habilite la directiva **[!UICONTROL Actualizar valores de campo automáticamente]** para cambiar automáticamente ciertos valores del campo el moverse una tarjeta a la columna.

   ![Configuración y directivas de columna](assets/boards-column-policies-enabled.png)

1. (Opcional) Establezca un valor para el estado de la tarjeta:

   1. Seleccione la casilla de verificación **[!UICONTROL Estado]**.

   1. Seleccione el estado que se aplicará a una tarjeta cuando se mueva a esta columna.

      ![Estado de las columnas](assets/boards-column-status.png)

      También se muestran las opciones de traducción de estado de las tarjetas conectadas. (La traducción de estado no se aplica a tarjetas ad hoc). Estas opciones determinan el estado personalizado aplicado a la tarea o al problema en [!DNL Workfront] cuando se mueve una tarjeta conectada a esta columna.

   1. Seleccione un estado [!UICONTROL **Personalizado**] para aplicarlo a la tarjeta en tareas y problemas.

      Cuando se mueve una tarjeta a esta columna, [!DNL Workfront] intenta aplicar primero el estado personalizado (por ejemplo, Resuelto). Si el estado personalizado seleccionado no está disponible para esa tarjeta, se le pedirá que elija otro estado que corresponda al estado del sistema (desde el paso b anterior). Para obtener más información sobre los estados, vea [Información general sobre los estados](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Además, si el estado de la tarea o del problema conectados se cambia al estado personalizado o del sistema establecidos en la directiva de columnas, la tarjeta se mueve automáticamente a la columna.

1. (Opcional) Establezca un valor para los usuarios asignados a la tarjeta:

   1. Active la casilla de verificación **[!UICONTROL Usuarios asignados]**.
   1. Seleccione una acción.

      * **[!UICONTROL Añadir a usuarios asignados]:** los usuarios asignados que seleccione se añadirán a la lista de usuarios asignados existente en una tarjeta cuando esta se mueva a esta columna.
      * **[!UICONTROL Anular usuarios asignados]:** los usuarios asignados que seleccione anularán a todos los demás usuarios asignados y se convertirán en los únicos usuarios asignados de una tarjeta cuando esta se mueva a esta columna.

   1. Haga clic en [!UICONTROL **Añadir asignación**] y busque un usuario. Seleccione los usuarios asignados en los resultados de búsqueda. Todos los usuarios y equipos de Workfront están disponibles para elegir.

      ![Usuarios asignados a la columna](assets/boards-column-assignees.png)

1. (Opcional) Establezca un valor para las etiquetas de la tarjeta:

   1. Active la casilla de verificación **[!UICONTROL Tarjetas]**.
   1. Seleccione una acción.

      * **[!UICONTROL Añadir en etiquetas]:** las etiquetas que seleccione se añadirán a la lista de etiquetas existente en una tarjeta cuando esta se mueva a esta columna.
      * **[!UICONTROL Anular etiquetas]:** las etiquetas que seleccione anularán todas las demás etiquetas y se convertirán en las únicas etiquetas de una tarjeta cuando esta se mueva a esta columna.

   1. Seleccione las etiquetas de la lista desplegable. Solo las etiquetas que ya se hayan creado en [!UICONTROL Administrador de etiquetas] están disponibles para elegir. Para obtener información sobre cómo añadir nuevas etiquetas, consulte [Añadir etiquetas](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Etiquetas para la columna](assets/boards-column-tags.png)

1. Habilite la directiva **[!UICONTROL Work in progress limit]** para limitar el número de tarjetas que se pueden añadir a la columna. A continuación, escriba el número límite en el campo **[!UICONTROL Set limit]**.

   ![WIP limit for column](assets/boards-wip-limit-in-column.png)

   Para obtener más información, consulte [Administrar el límite de trabajo en curso (WIP) en un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Haga clic en **[!UICONTROL Cerrar]** para salir del área Configuración y ver la columna y sus tarjetas.
