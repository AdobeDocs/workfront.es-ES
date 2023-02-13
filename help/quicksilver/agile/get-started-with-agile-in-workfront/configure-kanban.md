---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Kanban
description: Puede configurar las siguientes opciones para los equipos móviles Kanban durante o después de crear el equipo.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Configurar [!UICONTROL Kanban]

Puede configurar las siguientes opciones para equipos ágiles durante o después de crear el equipo. Puede crear un equipo ágil (Kanban o Scrum) en [!DNL Adobe Workfront] tal como se describe en [Crear un equipo ágil](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

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
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Configurar si los artículos se estiman en puntos u horas

Los artículos se pueden configurar para que se estimen mediante puntos u horas.

Para configurar cómo se calculan los artículos para su equipo ágil:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** , seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.\
   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** en la sección **[!UICONTROL Calcular artículos en]** , seleccione si desea utilizar puntos u horas para estimar el tamaño (carga de trabajo) de los artículos. Si selecciona Puntos, especifique cuántas horas son iguales a 1 punto. (El valor predeterminado es 1 punto = 8 horas). Este es el número de horas planificadas que se agregan al artículo.

   **Ejemplo:** Si ha elegido estimar los artículos en puntos y 1 punto es igual a 8 horas, y se estima que un artículo es de 3 puntos, se añaden 24 horas planificadas al artículo.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar columnas de estado en el tablero de artículos ágil

Puede definir los estados que existen en el tablero de artículos para el equipo ágil. Estos son los únicos estados que se muestran en el tablero de artículos.

Para definir los estados disponibles para el tablero de artículos asociado al equipo ágil:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!UICONTROL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** , ubique la sección **[!UICONTROL Tablero de historias]** .

1. (Opcional) Haga clic en **[!UICONTROL Agregar columna]** para agregar una columna de estado adicional al tablero de artículos.
1. (Opcional) Arrastre cualquier columna de estado utilizando el indicador de arrastrar y soltar para reordenar las columnas de estado en el tablero de artículos. La primera columna no se puede mover y no se puede arrastrar otra columna delante de la primera columna.

   ![Arrastrar y soltar](assets/agile-story-card-drag-and-drop.png)

1. Seleccione los estados de las tareas.

   >[!IMPORTANT]
   >
   >Solo se pueden seleccionar estados bloqueados de todo el sistema; no se pueden seleccionar estados específicos de grupo. Además, el estado de la primera columna siempre corresponde a **[!UICONTROL Nuevo]**.

   Puede agregar estados personalizados si su [!DNL Workfront] administrador los ha configurado; los estados personalizados se pueden configurar como se describe en [Crear o editar un estado](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configure campos adicionales para mostrarlos en tarjetas de historia en el tablero de artículos ágiles

Cuando se añaden campos a tarjetas de artículo, los campos son de solo vista y solo se muestran cuando se rellena el campo.

De forma predeterminada, los siguientes tipos de datos se muestran en la tarjeta de artículo para tareas y problemas:

* Nombre del artículo con un vínculo directamente a la tarea o problema
* El nombre del proyecto con un vínculo directo al proyecto
* Este vínculo solo se muestra para los artículos, no para las subtareas
* La descripción de la tarea o del problema
* Compromiso actual
* Ver y editar el porcentaje completado ajustando el porcentaje completado por sí mismo o ajustando el número de puntos u horas completadas
* Usuarios asignados

Puede mostrar datos adicionales (incluidos datos personalizados) en tarjetas de artículos. Es posible que desee mostrar campos adicionales en las tarjetas de artículo por varios motivos. Por ejemplo, es posible que desee mostrar el ID de cliente si está trabajando en artículos para varios clientes dentro de la iteración o que desee mostrar la fecha de inicio del proyecto o la fecha de finalización del proyecto.

>[!NOTE]
>
>Si utiliza un campo personalizado en una tarjeta de artículo, no puede contener un punto/punto en el nombre.

Para configurar las tarjetas de artículo asignadas al equipo ágil para que muestren campos adicionales:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.\
   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** , escriba un nombre de campo para localizarlo.

   ![Campos adicionales](assets/agile-additional-fields-kanban.png)

1. Seleccione el nombre del campo que desee añadir.
1. Escriba la **[!UICONTROL Nombre para mostrar]** para que el campo aparezca en la historia o en la tarjeta de emisión.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configuración del límite de trabajo en curso (WIP)

Kanban en [!DNL Workfront] le permite controlar la cantidad de trabajo en la que está trabajando el equipo limitando el número de tareas que pueden aparecer en la variable [!UICONTROL En curso] en la columna [!UICONTROL Kanban] tablero.

Cuando se configura el límite de trabajo en curso, puede ver el límite de trabajo en curso o incluso actualizarlo desde el [!UICONTROL Kanban] tablero de historia ágil, tal como se describe en [Administre el límite de trabajo en curso (WIP) en el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Para limitar el trabajo en curso para su equipo kanban:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Kanban que desee administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** en la sección **[!UICONTROL Metodología]** compruebe que Kanban está seleccionado.

1. En el **[!UICONTROL Tablero de historias]** en la sección **[!UICONTROL LÍMITE DE WIP]** especifique el número máximo de elementos permitidos en cada columna del [!UICONTROL Kanban] tablero de historia ágil. Puede establecer un límite diferente para cada columna. El límite máximo que puede establecer para cada columna es de 100.\
   Cuando se configura, el límite de WIP muestra un mensaje de advertencia en la variable [!UICONTROL Kanban] tablero de artículos ágil en cualquier momento en que se supere el límite para cualquier columna del tablero de artículos. Este mensaje de advertencia se muestra sólo la primera vez que se supera el límite de WIP. Este mensaje de advertencia no se muestra en ninguna columna que tenga un estado igual a [!UICONTROL Completar].\
   El límite de WIP es simplemente una advertencia visual y no restringe que su equipo tenga más artículos en una sola columna que el límite establecido.

   ![Límite de trabajo en curso](assets/wip-limit-350x193.png)

1. Haga clic en **Guardar cambios**.

## Configurar artículos para que se agreguen automáticamente desde el registro acumulado

Puede configurar los artículos del registro anterior para que se agreguen automáticamente a la primera columna de la columna [!UICONTROL Kanban] tablero inmediatamente después de mover un elemento de esa columna.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Kanban que desee administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. Select **[!UICONTROL Agregar automáticamente el siguiente artículo desde el registro acumulado]** para configurar los artículos que se añadirán automáticamente del registro acumulado a la primera columna de la [!UICONTROL Kanban] tablero de historia.

   Esto ocurre cada vez que se mueve un artículo a una columna del tablero de artículos que representa un estado de Finalización (un estado que coincide con Completar). Cuando se agrega desde el registro de artículo, el artículo con la prioridad más alta se agrega al tablero de artículos. seleccione esta opción para configurar el siguiente elemento del registro de artículo para que se agregue automáticamente al **[!UICONTROL En curso]** cuando un elemento se mueve fuera de la columna **[!UICONTROL En curso]** para abrir el Navegador.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configure cuánto tiempo permanecen las tarjetas en la variable [!UICONTROL Kanban] tablero

Puede elegir cuánto tiempo permanecen las tarjetas completadas en el [!UICONTROL Kanban] tablero. Tareas que caen del [!UICONTROL Kanban] aún se puede acceder al tablero en su proyecto original.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo Kanban en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Seleccione el equipo Kanban.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **Edit**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Número de días Las tarjetas completadas permanecen en el tablero Kanban]** menú desplegable, seleccione un valor.
1. Haga clic en **[!UICONTROL Guardar cambios]**.
