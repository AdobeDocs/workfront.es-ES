---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: Comprender el diseño de la hoja de horas
description: En este artículo se describe el diseño de las partes de horas en Adobe Workfront, lo que le permite comprender mejor cómo personalizar y utilizar las partes de horas para registrar el tiempo.
author: Alina
feature: Timesheets
exl-id: 31c48a50-5235-495c-8e46-0974ed98ede1
source-git-commit: ca552b80e9d78fd09068d72479e1b2bddc596c70
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 1%

---

# Comprender el diseño de la hoja de horas

En este artículo se describe el diseño de las partes de horas en Adobe Workfront, lo que le permite comprender mejor cómo personalizar y utilizar las partes de horas para registrar el tiempo.

Las preferencias de horas y horas controlan lo que aparece en un parte de horas. Este artículo proporciona información general sobre todas las opciones disponibles. Para obtener más información, consulte [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo iniciar sesión en una hoja de tiempo, consulte [Tiempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).

![Diseño de hoja de tiempo](assets/timesheet-layout-unshimmed.png)

Las siguientes son las áreas de un parte de horas:

* [Encabezado de hoja de tiempo](#timesheet-header)
* [El panel izquierdo](#the-left-panel)
* [Elementos de trabajo](#work-items)
* [Barra de herramientas](#toolbar)
* [Pie de página de hoja de tiempo](#timesheet-footer)
* [Función del trabajo](#job-role)
* [Tipo de hora](#hour-type)
* [Área de actualizaciones del panel izquierdo](#updates-area-in-the-left-panel)
* [Panel de resumen](#summary-panel)
* [Período de tiempo y área de entrada de hora](#time-frame-and-hour-entry-area)
* [Comentarios de entrada de hora](#hour-entry-comments)
* [Horas](#hours)
* [Totales](#totals)

## Encabezado de hoja de tiempo

![](assets/timesheet-title-unshimmed-redesign.png)

El encabezado de parte de horas incluye la siguiente información:

* El lapso de tiempo del parte de horas.
* El área Acciones que incluye lo siguiente:
   * Un icono de estrella para agregar las hojas de horas a su lista de Favoritos.
   * El icono Más con una opción Eliminar desde la que puede eliminar el parte de horas.
* Nombre del propietario del parte de horas.
* Número total de horas durante las horas registradas para los elementos mostrados en el parte de horas.
* Número de horas extra. Esta es una entrada manual y solo se puede ver cuando la variable **Tiempo extra** está habilitado en un parte de horas. Para obtener más información, consulte [Editar información de hoja de horas](../create-and-manage-timesheets/edit-timesheets.md).

>[!TIP]
>
>No puede registrar un número mayor de horas extra que el total actual de horas en el parte de horas. Por ejemplo, si ha registrado 7 horas en el parte de horas hasta ahora, no puede registrar 8 horas extra.


* El estado del parte de horas.

## El panel izquierdo

![](assets/timesheet-left-panel-unshimmed-redesign.png)

Puede acceder a las siguientes secciones en el panel izquierdo:

* **Hoja de horas**: Muestra el parte de horas real.
* **Actualizaciones**: Muestra comentarios y actualizaciones del sistema para el parte de horas. Para obtener más información, consulte la [Área de actualizaciones del panel izquierdo](#updates-area-in-the-left-panel) en este artículo.

## Elementos de trabajo

![](assets/timesheet-object-names-unshimmed-redesign.png)

Los elementos de trabajo son los proyectos, tareas y problemas para los que desea registrar el tiempo. Al hacer clic en la flecha que apunta hacia abajo en la fila del encabezado, se contraen los proyectos y las tareas y problemas que aparecen debajo. Al hacer clic en la flecha que apunta hacia abajo situada al lado del nombre de un proyecto, se contraen los elementos de trabajo de ese proyecto.

Las tareas, los problemas y los proyectos en los que el tiempo se registra fuera del parte de horas o los elementos planificados durante el marco de tiempo del parte de horas aparecen aquí automáticamente.

## Barra de herramientas

![](assets/timesheet-toolbar-unshimmed-redesign.png)

La barra de herramientas incluye las siguientes opciones:

* Botón Agregar elemento desde el que puede agregar proyectos, tareas o problemas.
* El icono de filtro rápido para buscar tareas o problemas en el parte de horas.
* La variable **Mostrar comentarios** configuración que permite ver u ocultar comentarios de hora que están registrados para entradas de proyecto, tarea o hora de publicación.
* Icono de pantalla completa desde el cual puede mostrar el parte de horas en modo de pantalla completa.
* **Abrir resumen** (o **Cerrar resumen**) desde donde puede abrir o cerrar el panel Resumen para ver información adicional sobre tareas o problemas. Esto no está disponible para proyectos.

Para obtener más información, consulte [Tiempo de registro](../create-and-manage-timesheets/log-time.md).

## Pie de página de hoja de tiempo

![](assets/timesheet-footer-unshimmed-redesign.png)

Puede hacer clic en los botones Enviar para aprobación, Cerrar, Aprobar y Rechazar de esta área para cerrar o rechazar una aprobación de parte de horas.

Esta área también contiene información sobre la última vez que se guardó el parte de horas. Todos los cambios que realice en la información del parte de horas se guardan automáticamente.

## Función

![](assets/timesheet-job-role-area-unshimmed-redesign.png)

Puede seleccionar una función de trabajo diferente para asociarla con las entradas de hora. El administrador de Workfront debe habilitar manualmente la configuración Asignar funciones de trabajo a las entradas de hora. La función de trabajo especificada cuando está asignado a la tarea o el problema se muestra de forma predeterminada. Si no se le asigna una función de trabajo en la tarea o en el problema, la función principal se muestra como la predeterminada. Para obtener más información, consulte el artículo [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Puede registrar entradas de varias horas para el mismo elemento de trabajo para diferentes funciones. Para obtener más información, consulte [Tiempo de registro](../create-and-manage-timesheets/log-time.md).

## Tipo de hora

![](assets/timesheet-hour-type-unshimmed-redesign.png)

Puede seleccionar diferentes tipos de hora para asociarlos con las entradas de hora de cada artículo. Este campo solo se muestra cuando el administrador de Workfront lo habilita para su entorno. Para obtener más información, consulte el artículo [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Puede registrar entradas de varias horas para el mismo elemento de trabajo para diferentes tipos de horas. Para obtener más información, consulte [Tiempo de registro](../create-and-manage-timesheets/log-time.md).

## Área de actualizaciones del panel izquierdo

![](assets/timesheet-updates-section-unshimmed-redesign.png)

Puede realizar comentarios en un parte de horas para comunicarse con los aprobadores de parte de horas u otros usuarios en la sección Actualizaciones del panel izquierdo.

Cualquier comentario realizado en el parte de horas se muestra en esta área, en la parte inferior del parte de horas. Esta área se muestra debajo del parte de horas y encima del pie de página del parte de horas. Para obtener más información, consulte [Ver y administrar comentarios en un parte de horas](../create-and-manage-timesheets/view-and-manage-comments-timesheets.md).

## Panel de resumen

![](assets/timesheet-summary-panel-for-task-unshimmed-redesign.png)

Puede acceder al panel Resumen para realizar comentarios de tareas o problemas que se muestran en un parte de horas. Desde aquí, puede comentar sobre tareas y problemas, o actualizar su información. Para obtener más información, consulte [Resumen](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Los comentarios que introduzca para los elementos de trabajo en el panel Resumen de parte de horas se muestran en el área Actualizaciones de la tarea o en el problema. El panel Resumen no está disponible para proyectos.

## Período de tiempo y área de entrada de hora

![](assets/timesheet-time-frame-log-time-area.png)

El lapso de tiempo del parte de horas se muestra a la derecha de los elementos de trabajo.

Puede crear partes de horas para una, dos o cuatro semanas.

El lapso de tiempo se muestra en incrementos de toda la semana. Los días fuera del lapso de tiempo especificado en el parte de horas están atenuados. No puede registrar la hora de los días que están fuera del lapso de tiempo del parte de horas.

Para obtener más información, consulte [Crear hoja de horas de un solo uso](../create-and-manage-timesheets/create-tmshts.md) o [Crear, editar y asignar perfiles de parte de horas](../create-and-manage-timesheets/create-timesheet-profiles.md).

<!--drafted for the resize columns in timesheets story - make this blurb a TIP when the story is released: 
You can resize the columns that display different weeks, the time frame, or the work item areas by dragging and dropping the vertical lines that separate them.-->

## Comentarios de entrada de hora

![](assets/timesheet-hour-entry-comment-button-unshimmed-redesign.png)

Puede agregar un comentario para cada entrada de hora que agregue al parte de horas.

Los comentarios que escriba en el cuadro de comentarios de la hora se mostrarán en el parte de horas, debajo de cada elemento de trabajo en el que haya registrado la hora en la que **Mostrar comentarios** está activada en la barra de herramientas.

![](assets/hour-entry-comment-under-task-in-timesheet-unshimmed-redesign.png)

## Horas

![](assets/timesheet-hours-area-unshimmed-redesign.png)

El parte de horas proporciona campos de entrada para cada elemento de trabajo y día del rango de hojas de horas para registrar el tiempo empleado trabajando en el elemento. A medida que va registrando la hora, el elemento en el que registra la hora de resaltado en azul claro y el cuadro de la hora aparece delineado en azul oscuro.

## Totales

![](assets/timesheet-totals-column-and-header-unshimmed-redesign.png)

Revise la suma de todas las horas introducidas en el parte de horas, resumidas por día (en el encabezado del parte de horas), así como por objeto (en la última columna).
