---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Scrum
description: Puede configurar las siguientes opciones para los equipos de Scrum Agile durante o después de la creación del equipo.
author: Jenny
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1725'
ht-degree: 76%

---

# Configurar [!UICONTROL Scrum]

Puede crear un equipo Agile en [!DNL Adobe Workfront] tal como se describe en [Crear un equipo Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Al crear un equipo Agile, puede elegir la metodología que utiliza el equipo para completar su trabajo. Puede elegir entre las siguientes opciones:

* Scrum
* Kanban

Este artículo describe cómo configurar los ajustes de un equipo de Scrum. Después de crear un equipo Agile y elegir la metodología Scrum, puede consultar este artículo para actualizar la siguiente configuración:

* Si las historias se estiman en puntos o en horas
* Las columnas de estado del panel de historias de Agile para iteraciones y proyectos
* Campos adicionales para mostrar en tarjetas de historia en el panel de historia de Agile
* Cómo se utilizan los indicadores de color para las historias en el panel de historias de Agile
* Aplicación de las fechas al añadir elementos de trabajo a una iteración

Para obtener información sobre cómo configurar un equipo Kanban, consulte [Configurar Kanban](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Equipos</p>  </td> 
  </tr>

</tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure si las historias se calculan en puntos o en horas

>[!NOTE]
>
>Esta configuración no se puede cambiar si el equipo tiene iteraciones en curso.

Puede configurar las historias para que se estimen mediante puntos o horas.

Para configurar cómo se calculan las historias para su equipo de Agile:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar de equipo]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Seleccione el equipo de Agile que desee gestionar.
1. Haga clic en el menú **[!UICONTROL Más]** y, a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los miembros del equipo con una licencia de [!UICONTROL Standard], [!UICONTROL Plan] o [!UICONTROL Trabajo] ven esta opción.
   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En la sección **[!UICONTROL Agile]**, en el área **[!UICONTROL Estimar historias en]**, seleccione si desea usar puntos u horas para estimar el tamaño (carga de trabajo) de las historias. Si selecciona Puntos, especifique cuántas horas son iguales a 1 punto. (El valor predeterminado es 1 punto = 8 horas). Número de horas planificadas que se añaden a la historia.

   **Ejemplo:** Si ha seleccionado calcular historias en puntos y 1 punto equivale a 8 horas, y una historia se estima en 3 puntos, se agregan 24 horas planificadas a la historia.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar columnas de estado en el panel de historias de Agile

Puede configurar qué columnas se muestran en el panel de historia de Agile para todas las iteraciones asignadas a su equipo o para un proyecto determinado.

* [Configuración de columnas de estado para iteraciones](#configure-status-columns-for-iterations)
* [Configurar columnas de estado para proyectos](#configure-status-columns-for-projects)

### Configuración de columnas de estado para iteraciones {#configure-status-columns-for-iterations}

Puede definir los estados que existen en el guion gráfico del equipo de Agile. Estos son los únicos estados que se muestran en el panel de historias.

Para definir los estados disponibles para el guion gráfico asociado con el equipo de Agile:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo de Agile que desee gestionar.
1. Haga clic en el menú **[!UICONTROL Más]** y, a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una licencia de [!UICONTROL Plan] o [!UICONTROL Trabajo] ven esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En la sección **[!UICONTROL Agile]**, busque el área **[!UICONTROL Tablero de historias]**.

1. (Opcional) Haga clic en **[!UICONTROL Añadir columna]** para añadir una columna de estado adicional al tablero de historia.
1. (Opcional) Arrastre cualquier columna de estado con el indicador de arrastrar y soltar para reordenar las columnas de estado en el tablero de historias. La primera columna no se puede mover y no se puede arrastrar otra columna delante de la primera.

   ![Arrastrar y soltar](assets/agile-story-card-drag-and-drop.png)

1. Seleccione los estados de tarea y problema. Los estados de la tarea se muestran como el título de columna de cada columna en el tablero de historia. Los estados del problema que seleccione se asignan a los estados de tarea. Esto significa que cuando mueve un problema a otra columna del tablero de historia, el estado del problema cambia a los estados del problema que se muestran aquí y no al nombre de la columna en el tablero de historias (que refleja el estado de la tarea).

   >[!IMPORTANT]
   >
   >Solo se pueden seleccionar estados bloqueados en todo el sistema; no se pueden seleccionar estados específicos del grupo. Además, el estado de la primera columna siempre corresponde a **[!UICONTROL Nuevo]**.

   Puede añadir estados personalizados si el administrador de [!DNL Workfront] los ha configurado; los estados personalizados se pueden configurar tal como se describe en [Crear o editar un estado](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Al seleccionar estados del problema, la tercera columna siempre tiene el valor predeterminado [!UICONTROL Cerrado]. Si tiene más de tres columnas, asegúrese de actualizar manualmente las columnas para reflejar los estados adecuados.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

### Configurar columnas de estado para proyectos {#configure-status-columns-for-projects}

Para obtener información acerca de cómo configurar las columnas de estado de un proyecto, consulte la sección [Crear o personalizar una vista [!UICONTROL Agile]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) en el artículo [Crear o editar vistas en [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Configurar campos adicionales para que se muestren en tarjetas de historia en el panel de historia de Agile

Cuando se añaden campos a las tarjetas de historia, los campos son de solo vista y de solo visualización cuando se rellenan.

De forma predeterminada, los siguientes tipos de datos se muestran en la tarjeta de la historia para tareas y problemas:

* Nombre de la historia con un vínculo directamente a la tarea o al problema
* El nombre del proyecto con un vínculo directamente al proyecto
* Este vínculo solo se muestra para artículos, no para subtareas
* La descripción de la tarea o el problema
* Compromiso actual
* Vea y edite el porcentaje completado ajustando el porcentaje completado en sí o ajustando el número de puntos u horas que se han completado
* Usuarios asignados

Se pueden mostrar datos adicionales (incluidos datos personalizados) en las tarjetas de historias. Es posible que desee mostrar campos adicionales en las tarjetas de historias por varios motivos. Por ejemplo, es posible que desee mostrar el ID de cliente si está trabajando en artículos para varios clientes dentro de la iteración o puede que desee mostrar la Fecha de inicio o de finalización del proyecto.

>[!NOTE]
>
>Si utiliza un campo personalizado en una tarjeta de historias, no puede contener un punto en el nombre.

Para configurar las tarjetas de historia asignadas al equipo de Agile para que muestren campos adicionales:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo de Agile que desee gestionar.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.
Solo los integrantes del equipo con una licencia de [!UICONTROL Plan] o [!UICONTROL Trabajo] ven esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En la sección **[!UICONTROL Agile]**, busque el nombre de un campo para localizarlo.

   ![Campos adicionales](assets/agile-additional-fields-scrum.png)

1. Seleccione el nombre del campo que desee añadir.
1. Escriba **[!UICONTROL Nombre para mostrar]** para que el campo se muestre en la historia o en la tarjeta de emisión.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar cómo se utilizan los indicadores de color para las historias en el panel de historias de Agile

De forma predeterminada, los mosaicos del guion gráfico de una iteración de Agile se codifican con colores según el proyecto con el que esté asociado el artículo. A cada proyecto se le asigna arbitrariamente un color en el tablero de historias. Puede cambiar este comportamiento predeterminado para cada equipo Agile. Los colores de las historias de Agile se pueden asociar a la prioridad de la historia, el propietario, etc.

Para cambiar el comportamiento de cómo se asignan los colores a las historias para un equipo Agile:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo de Agile que desee gestionar.
1. Haga clic en el menú **[!UICONTROL Más]** y, a continuación, seleccione **[!UICONTROL Editar]**.

   Solo los integrantes del equipo con una licencia de [!UICONTROL Plan] o [!UICONTROL Trabajo] ven esta opción.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En la sección [!UICONTROL Agile], en el área [!UICONTROL Asociar color de tarjeta con], seleccione entre las siguientes opciones:

   * **[!UICONTROL Proyecto]**: los colores están asociados con el proyecto al que está asociada la historia. (Cuando se crea una historia, debe asociarse con un proyecto, como se describe en [Crear una historia Agile](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Todas las tareas del mismo proyecto se muestran con el mismo color.
   * **[!UICONTROL Forma libre]**: todas las tarjetas se muestran en azul de forma predeterminada hasta que un usuario cambie el color manualmente, tal como se describe en [[!UICONTROL Categorizar historias por color] en el tablero Scrum](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Prioridad]**: los colores están asociados con la prioridad de la historia, de la siguiente manera:

      * Alta = Rojo
      * Media = Amarillo
      * Baja = Verde

        Si el administrador del sistema ha configurado prioridades personalizadas para su sistema [!DNL Workfront], la prioridad más alta es de color rojo, la segunda más alta es de color amarillo y la tercera más alta es de color verde.
   * **[!UICONTROL Propietario de la tarea]**: todas las historias con el mismo usuario principal asignado son del mismo color. El usuario asignado principal es el usuario que se asignó por primera vez a la tarea.


1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar cómo se aplican las fechas al añadir elementos de trabajo a una iteración

De forma predeterminada, cuando se añade un elemento de trabajo a una iteración de Scrum, las Fechas de inicio planificada y la de finalización del elemento de trabajo se modifican para que coincidan con las de inicio y de finalización de la iteración. Puede optar por mantener las fechas originales de todos los elementos de trabajo del equipo.

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.
Solo los integrantes del equipo con una licencia de [!UICONTROL Plan] o [!UICONTROL Trabajo] ven esta opción.
1. En la sección [!UICONTROL Agile], en el área [!UICONTROL Cuando se añade un elemento de trabajo a una iteración], seleccione entre las siguientes opciones:

   * **[!UICONTROL Modifique la Fecha planificada de inicio y Fecha planificada de finalización para que coincidan con las fechas de inicio y finalización de la iteración]**: Cuando se agregan elementos de trabajo a una iteración, las fechas de los elementos de trabajo se cambian a las fechas de iteración.

     Para obtener más información sobre cómo se modifican las fechas, consulte la sección [Comprender cómo afecta la adición de historias a las fechas de las tareas](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understand-how-adding-stories-affects-task-dates) en el artículo [Añadir historias a una iteración existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL No modificar la fecha de inicio planificada ni la fecha planificada de finalización para que coincidan con las fechas de inicio y de finalización de la iteración]**: cuando se añaden elementos de trabajo a una iteración, los elementos de trabajo conservan sus fechas originales.

   Si cambia la opción de fecha, las fechas de los elementos de trabajo que ya se encuentran en la iteración no se ajustan.

   Estas opciones pueden afectar a las fechas en las que los equipos asignan elementos de trabajo a las iteraciones de los demás. Por ejemplo, el equipo A modifica las fechas de los elementos de trabajo a las fechas de la iteración y el equipo B no modifica las fechas de los elementos de trabajo. Si el equipo B asigna un elemento de trabajo a la iteración del equipo A, las fechas del elemento de trabajo cambiarán. Sin embargo, si el equipo A asigna un elemento de trabajo a la iteración del equipo B, las fechas no cambiarán.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
