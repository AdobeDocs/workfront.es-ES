---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Kanban
description: Puede crear un equipo Agile de Kanban o Scrum en [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 1%

---

# Configurar [!UICONTROL Kanban]

Puede crear un equipo Agile en [!DNL Adobe Workfront] como se describe en [Crear un equipo Agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Al crear un equipo Agile, puede elegir la metodología que utiliza el equipo para completar su trabajo. Puede elegir entre las siguientes opciones:

* Scrum
* Kanban

Este artículo describe cómo configurar los ajustes de un equipo Kanban. Después de crear un equipo Agile y elegir la metodología Kanban, puede consultar este artículo para actualizar la siguiente configuración:

* Si las historias se estiman en puntos o en horas
* Las columnas de estado del panel de historias Agile
* Campos adicionales para mostrar en tarjetas de historia en el panel de historia ágil
* Límite de trabajo en curso (WIP)
* Cómo añadir automáticamente historias del registro de pendientes
* Cuánto tiempo permanecen las tarjetas en el panel Kanban

Para obtener información sobre la configuración de un equipo de Scrum, consulte [Configurar Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p> 
   o
   <p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar acceso a Equipos</p>  </td> 
  </tr>

</tbody> 
</table>

*Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Configure si las historias se calculan en puntos o en horas

Puede configurar las historias para que se estimen mediante puntos o horas.

Para configurar cómo se calculan las historias para su equipo Agile:

{{step1-to-team}}

1. Haga clic en **[!UICONTROL Cambiar equipos]** icono ![](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en el cuadro de búsqueda.
1. Seleccione el equipo Agile que desee administrar.
1. Haga clic en **[!UICONTROL Más]** menú ![](assets/more-menu.png) , luego seleccione **[!UICONTROL Editar]**.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Agile]** , en la sección **[!UICONTROL Estimar historias en]** , seleccione si desea usar puntos u horas para estimar el tamaño (carga de trabajo) de los artículos. Si selecciona Puntos, especifique cuántas horas son iguales a 1 punto. (El valor predeterminado es 1 punto = 8 horas). Número de horas planificadas que se añaden a la historia.

   **Ejemplo:** Si ha seleccionado calcular las historias en puntos y 1 punto equivale a 8 horas, y una historia se estima en 3 puntos, se añaden 24 horas planificadas a la historia.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar columnas de estado en el panel de historias Agile

Puede definir los estados que existen en el guion gráfico para el equipo Agile. Estos son los únicos estados que se muestran en el guion gráfico.

Para definir los estados disponibles para el guion gráfico asociado con el equipo Agile:

{{step1-to-team}}

1. Haga clic en **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipos](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Agile que desee administrar.
1. Haga clic en **[!UICONTROL Más]** menú, luego seleccione **[!UICONTROL Editar]**.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Agile]** , busque la sección **[!UICONTROL Tablero de historias]** área.

1. (Opcional) Haga clic en **[!UICONTROL Agregar columna]** para agregar una columna de estado adicional al guion gráfico.
1. (Opcional) Arrastre cualquier columna de estado con el indicador de arrastrar y soltar para reordenar las columnas de estado en el guion gráfico. La primera columna no se puede mover y no se puede arrastrar otra columna delante de la primera.

   ![Arrastrar y soltar](assets/agile-story-card-drag-and-drop.png)

1. Seleccione los estados de tareas.

   >[!IMPORTANT]
   >
   >Solo se pueden seleccionar los estados bloqueados de todo el sistema. No se pueden seleccionar estados específicos de grupos. El estado de la primera columna siempre corresponde a **[!UICONTROL Nuevo]**.

   Puede añadir estados personalizados si su [!DNL Workfront] El administrador de los ha configurado. Para obtener más información, consulte [Creación o edición de un estado](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar campos adicionales para que se muestren en las tarjetas de historia en el panel de historias Agile

Cuando se agregan campos a las tarjetas de historia, los campos son de sólo lectura y sólo se muestran cuando se rellena el campo.

De forma predeterminada, los siguientes tipos de datos se muestran en la tarjeta de historia para tareas y problemas:

* Nombre de la historia con un vínculo directamente a la tarea o al problema
* El nombre del proyecto con un vínculo directamente al proyecto
* Este vínculo solo se muestra para artículos, no para subtareas
* La descripción de la tarea o el problema
* Compromisos actuales
* Vea y edite el porcentaje completado ajustando el porcentaje completado en sí o ajustando el número de puntos u horas que se han completado
* Usuarios asignados

Puede mostrar datos adicionales (incluidos datos personalizados) en tarjetas de historia. Es posible que desee mostrar campos adicionales en las tarjetas de historia por varios motivos. Por ejemplo, es posible que desee mostrar el ID de cliente si está trabajando en artículos para varios clientes dentro de la iteración, o puede que desee mostrar la Fecha de inicio del proyecto o la Fecha de finalización del proyecto.

>[!NOTE]
>
>Si utiliza un campo personalizado en una tarjeta de historia, no puede contener un punto (o punto) en el nombre.

Para configurar las tarjetas de historia asignadas al equipo de Agile para que muestren campos adicionales:

{{step1-to-team}}

1. Haga clic en **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipos](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Agile que desee administrar.
1. Haga clic en **[!UICONTROL Más]** menú, luego seleccione **[!UICONTROL Editar]**.\

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Agile]** , escriba un nombre de campo para localizarlo.

   ![Campos adicionales](assets/agile-additional-fields-kanban.png)

1. Seleccione el nombre del campo que desee añadir.
1. Escriba el **[!UICONTROL Nombre para mostrar]** para que el campo se muestre en la historia o en la tarjeta de emisión.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar el límite de trabajo en curso (WIP)

Al definir el límite de trabajo en curso de un equipo Kanban, puede controlar el número de elementos en los que está trabajando el equipo actualmente limitando el número de tareas que pueden aparecer en el [!UICONTROL Nuevo] o el [!UICONTROL En curso] en la columna [!UICONTROL Kanban] tablero.

Después de configurar el límite de WIP para un equipo Kanban, puede ver el límite de WIP y actualizarlo desde el [!UICONTROL Kanban] agile story board, tal como se describe en [Administrar el límite de trabajo en curso (WIP) en [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Para limitar WIP para el equipo Kanban:

{{step1-to-team}}

1. Haga clic en **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipos](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Kanban que desea gestionar.
1. Haga clic en **[!UICONTROL Más]** menú ![](assets/more-menu.png), luego seleccione **[!UICONTROL Editar]**.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Agile]** , en la sección **[!UICONTROL Metodología]** , asegúrese de que Kanban está seleccionado.

1. En el **[!UICONTROL Tablero de historias]** , en la sección **[!UICONTROL Límite de WIP]** , especifique el número máximo de elementos permitidos en cada columna del campo [!UICONTROL Kanban] agile story board. Puede establecer un límite diferente para cada columna. El límite máximo que puede establecer para cada columna es 100.\
   Cuando se establece, el límite de WIP muestra un mensaje de advertencia en la [!UICONTROL Kanban] agile story board cada vez que se supera el límite de cualquier columna del story board. Este mensaje de advertencia se muestra solo la primera vez que se supera el límite de trabajo en curso. Este mensaje de advertencia no se muestra en ninguna columna que tenga un estado igual a [!UICONTROL Completar].\
   El límite de trabajo en curso es simplemente una advertencia visual y no restringe a su equipo de tener más elementos en una sola columna que el límite establecido.

   ![Límite de WIP](assets/wip-limit-350x193.png)

1. Haga clic en **Guardar cambios**.

## Configurar la adición automática de historias del registro de pendientes

<!-- this functionality needs to be verified-->

Puede configurar historias del registro de pendientes para que se agreguen automáticamente a la primera columna de la [!UICONTROL Kanban] tablero inmediatamente después de mover un elemento de esa columna.

{{step1-to-team}}

1. Haga clic en **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipos](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Kanban que desea gestionar.
1. Haga clic en **[!UICONTROL Más]** menú ![](assets/more-menu.png), luego seleccione **[!UICONTROL Editar]**.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. Seleccionar **[!UICONTROL Agregar automáticamente la historia siguiente del registro de pendientes]** para configurar que el siguiente elemento del registro de pendientes se agregue automáticamente al **[!UICONTROL Nuevo]** cuando se mueve un elemento fuera de la columna **[!UICONTROL En curso]** columna.

   Los usuarios deben habilitar la variable **Mostrar registro de pendientes** configuración en la [!UICONTROL Kanban] para que esta funcionalidad surta efecto. Cuando los usuarios habilitan la variable [!UICONTROL Mostrar registro de pendientes] configuración en la [!UICONTROL Panel Kanban], se lleva a cabo la siguiente funcionalidad:

   Cada vez que una historia se mueve de la [!UICONTROL En curso] columna en una columna del guion gráfico que representa una [!UICONTROL Completar] estado (o un estado que se equipare con [!UICONTROL Completar]), un artículo de la columna Registro de pendientes pasa automáticamente al [!UICONTROL Nuevo] de la columna [!UICONTROL Panel Kanban].
Cuando se agrega desde el registro de pendientes, la historia con la prioridad más alta se agrega al guion gráfico.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Configurar cuánto tiempo permanecen las tarjetas en la [!UICONTROL Kanban] tablero

Puede elegir cuánto tiempo permanecen las tarjetas completadas en el [!UICONTROL Kanban] tablero. Tareas que no están incluidas en [!UICONTROL Kanban] se puede acceder a los tableros en su proyecto original.

{{step1-to-team}}

1. (Opcional) Haga clic en **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipos](assets/switch-team-icon.png), a continuación, seleccione un nuevo equipo Kanban en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Seleccione el equipo Kanban.
1. Haga clic en **[!UICONTROL Más]** menú ![](assets/more-menu.png) , luego seleccione **[!UICONTROL Editar]**.

   ![Editar equipo](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Número de días que las tarjetas finalizadas permanecerán en el panel Kanban]** , seleccione un valor.

   Puede elegir un número de 1 a 30 días.
1. Haga clic en **[!UICONTROL Guardar cambios]**.
