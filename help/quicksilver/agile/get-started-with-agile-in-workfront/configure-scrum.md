---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar la anulación
description: Puede configurar las siguientes opciones para Anular equipos ágiles durante o después de crear el equipo.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# Configurar [!UICONTROL Anulación]

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

>[!NOTE]
>
>Esta configuración no se puede cambiar si el equipo tiene alguna iteración que esté actualmente en curso.

Los artículos se pueden configurar para que se estimen mediante puntos u horas.

Para configurar cómo se calculan los artículos para su equipo ágil:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!UICONTROL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** , seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.\
   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** en la sección **[!UICONTROL Calcular artículos en]** , seleccione si desea utilizar puntos u horas para estimar el tamaño (carga de trabajo) de los artículos. Si selecciona Puntos, especifique cuántas horas son iguales a 1 punto. (El valor predeterminado es 1 punto = 8 horas). Este es el número de horas planificadas que se agregan al artículo.

   **Ejemplo:** Si ha elegido estimar los artículos en puntos y 1 punto es igual a 8 horas, y se estima que un artículo es de 3 puntos, se añaden 24 horas planificadas al artículo.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar columnas de estado en el tablero de artículos ágil

Puede configurar qué columnas se muestran en el tablero de artículos ágil para todas las iteraciones asignadas a su equipo o para un proyecto determinado.

* [Configuración de columnas de estado para iteraciones](#configure-status-columns-for-iterations)
* [Configuración de columnas de estado para proyectos](#configure-status-columns-for-projects)

### Configuración de columnas de estado para iteraciones {#configure-status-columns-for-iterations}

Puede definir los estados que existen en el tablero de artículos para el equipo ágil. Estos son los únicos estados que se muestran en el tablero de artículos.

Para definir los estados disponibles para el tablero de artículos asociado al equipo ágil:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** , ubique la sección **[!UICONTROL Tablero de historias]** .

1. (Opcional) Haga clic en **[!UICONTROL Agregar columna]** para agregar una columna de estado adicional al tablero de artículos.
1. (Opcional) Arrastre cualquier columna de estado utilizando el indicador de arrastrar y soltar para reordenar las columnas de estado en el tablero de artículos. La primera columna no se puede mover y no se puede arrastrar otra columna delante de la primera columna.

   ![Arrastrar y soltar](assets/agile-story-card-drag-and-drop.png)

1. Seleccione los estados de tarea y problema. Los estados de tareas se muestran como el título de columna de cada columna en el tablero de artículos. Los estados del problema que seleccione corresponden a los estados de las tareas. Esto significa que, cuando se mueve un problema a otra columna del tablero de artículos, el estado del problema cambia a los estados de problema que se muestran aquí y no al nombre de la columna del tablero de artículos (que refleja el estado de la tarea).

   >[!IMPORTANT]
   >
   >Solo se pueden seleccionar estados bloqueados de todo el sistema; no se pueden seleccionar estados específicos de grupo. Además, el estado de la primera columna siempre corresponde a **[!UICONTROL Nuevo]**.

   Puede agregar estados personalizados si su [!DNL Workfront] administrador los ha configurado; los estados personalizados se pueden configurar como se describe en [Crear o editar un estado](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Al seleccionar los estados de los problemas, la tercera columna siempre establece de forma predeterminada [!UICONTROL Cerrado]. Si tiene más de tres columnas, asegúrese de actualizar manualmente las columnas para que reflejen los estados adecuados.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

### Configuración de columnas de estado para proyectos {#configure-status-columns-for-projects}

Para obtener información sobre cómo configurar las columnas de estado de un proyecto, consulte la sección [Crear o personalizar un [!UICONTROL Águila] ver](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) en el artículo [Crear o editar vistas en [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

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

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!UICONTROL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.\
   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** , escriba un nombre de campo para localizarlo.

   ![Campos adicionales](assets/agile-additional-fields-scrum.png)

1. Seleccione el nombre del campo que desee añadir.
1. Escriba la **[!UICONTROL Nombre para mostrar]** para que el campo aparezca en la historia o en la tarjeta de emisión.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar cómo se utilizan los indicadores de color para los artículos en el tablero de artículos ágil

De forma predeterminada, los mosaicos del tablero de historia en una iteración ágil se codifican con colores según el proyecto al que esté asociada la historia. A cada proyecto se le asigna arbitrariamente un color en el tablero de la historia. Puede cambiar este comportamiento predeterminado para cada equipo ágil. Los colores de las historias ágiles se pueden asociar a la prioridad de la historia, al propietario, etc.

Para cambiar el comportamiento de cómo se asignan los colores a artículos para un equipo ágil:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo ágil que desea administrar.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el [!UICONTROL Águila] en la sección [!UICONTROL Asociar color de tarjeta a] , seleccione entre las siguientes opciones:

   * **[!UICONTROL Proyecto]**: Los colores están asociados al proyecto al que está vinculado el artículo. (Cuando se crea un artículo, debe asociarse a un proyecto, tal como se describe en [Crear una historia ágil](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Todas las tareas del mismo proyecto se muestran con el mismo color.
   * **[!UICONTROL Forma libre]**: Todas las tarjetas se muestran de forma predeterminada como azules hasta que un usuario cambia el color manualmente, tal como se describe en [[!UICONTROL Categorizar artículos por color] en el tablero de mandos](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Prioridad]**: Los colores están asociados a la prioridad del artículo de la siguiente manera:

      * Alto = Rojo
      * Medio = Amarillo
      * Bajo = Verde\

         Si el administrador del sistema ha configurado prioridades personalizadas para su [!DNL Workfront] sistema, la prioridad más alta es roja, la segunda más alta es amarilla y la tercera más alta es verde.
   * **[!UICONTROL Propietario de la tarea]**: Todos los artículos con el mismo usuario asignado principal son del mismo color. El usuario asignado principal es el usuario que se asignó primero a la tarea.


1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración

De forma predeterminada, cuando se agrega un elemento de trabajo a una iteración de Anulación, se modifican la Fecha de Inicio Planificado y la Fecha de Finalización Planificada del elemento de trabajo para que coincidan con las fechas de inicio y finalización de la iteración. Puede elegir mantener las fechas originales en todos los elementos de trabajo del equipo.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Equipos]**.
1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.\
   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.
1. En el [!UICONTROL Águila] en la sección [!UICONTROL Cuando se agrega un elemento de trabajo a una iteración] , seleccione entre las siguientes opciones:

   * **[!UICONTROL Modifique la Fecha de Inicio Planificado y la Fecha de Finalización Planificada para que coincidan con las fechas de inicio y finalización de la iteración]**: Cuando se agregan elementos de trabajo a una iteración, las fechas del elemento de trabajo se cambian a las fechas de iteración.\

      Para obtener más información sobre cómo se modifican las fechas, consulte la sección [Comprender cómo la adición de artículos afecta a las fechas de las tareas](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) en el artículo [Añadir artículos a una iteración existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL No modifique la Fecha de inicio planificada ni la Fecha de finalización planificada para que coincidan con las fechas de inicio y finalización de la iteración]**: Cuando se agregan elementos de trabajo a una iteración, los elementos de trabajo conservan sus fechas originales.

   Si cambia la opción de fecha, las fechas de los elementos de trabajo que ya están en la iteración no se ajustan.

   Estas opciones pueden afectar a las fechas en las que los equipos asignan elementos de trabajo a las iteraciones de los demás. Por ejemplo, el equipo A modifica las fechas de los elementos de trabajo a las fechas de iteración y el equipo B no modifica las fechas de los elementos de trabajo. Si el equipo B asigna un elemento de trabajo a la iteración del equipo A, las fechas del elemento de trabajo cambiarán. Sin embargo, si el equipo A asigna un elemento de trabajo a la iteración del equipo B, las fechas no cambiarán.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
