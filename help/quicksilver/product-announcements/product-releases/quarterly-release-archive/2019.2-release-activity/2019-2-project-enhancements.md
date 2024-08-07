---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Mejoras de proyectos en 2019.2
description: Esta página describe todas las mejoras de Project incluidas en la versión 2019.2. La funcionalidad está planificada para estar disponible en el entorno de producción la semana del 20 de mayo de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# Mejoras de proyectos en 2019.2

Esta página describe todas las mejoras de Project incluidas en la versión 2019.2. La funcionalidad está planificada para estar disponible en el entorno de producción la semana del 20 de mayo de 2019.

Para obtener una lista de todos los cambios realizados en 2019.2, consulte [Información general sobre la actividad de la versión 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Búsqueda De Grupos Más Rápida Al Personalizar Estados

El menú desplegable de la pestaña Estados del área Configuración es ahora un menú de escritura anticipada. Esto le permite buscar y encontrar rápidamente cualquier grupo en el sistema, lo que facilita la personalización de los estados.

Anteriormente, el menú desplegable mostraba un número limitado de grupos. Si el grupo deseado no se mostraba, tenía que ir a Configuración > Grupos y buscar el grupo específico para personalizar sus estados.

Para obtener más información, consulte [Crear o editar un estado](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Adjuntar procesos personalizados de Forms y aprobación predeterminados a las tareas

Ahora puede configurar formularios personalizados y procesos de aprobación predeterminados para adjuntarlos a las tareas cuando agregue tareas a un proyecto. Puede establecer la configuración predeterminada en el nivel de proyecto.

Para obtener información sobre la configuración de formularios personalizados y procesos de aprobación predeterminados para tareas en el nivel de proyecto, consulte la sección &quot;Tareas&quot; en el artículo [Editar proyectos](../../../../manage-work/projects/manage-projects/edit-projects.md).

## Mostrar toda la fila de una tarea principal en negrita en una lista de tareas

En una lista de tareas, la fila que contiene una tarea principal se muestra en negrita. Este cambio es visible cuando la lista se ordena por la estructura de Desglose de trabajo o por el Número de tarea en orden ascendente.

## Invertir cambios en las listas de tareas

Un nuevo botón Guardar automáticamente en la lista de tareas le permite seleccionar si desea que los cambios realizados se guarden automáticamente o si desea ver los efectos que los cambios tienen antes de guardarlos. Esta configuración se aplica tanto a la lista de tareas como al gráfico Gantt.

Antes de esta mejora, todos los cambios se guardaban siempre automáticamente.

Para obtener información acerca de cómo editar tareas en una lista de tareas, consulte [Editar tareas](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Para obtener información acerca de la edición de tareas en el diagrama de Gantt, vea [Actualizar información en la lista de tareas Diagrama de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Valores predeterminados de ancho de columna nuevos en listas nuevas

Ahora, Workfront ajusta automáticamente la anchura de las columnas según la información de formato de valor de cada columna. Por ejemplo, las columnas que muestran un número son más anchas que las que muestran el campo Descripción.

Antes de esta mejora, las anchuras de columna en las vistas de nuevo proyecto y tarea se establecían en 100 píxeles, a menos que se especifique lo contrario.

Para obtener información acerca de los anchos de columna, vea [Modificar el ancho y el orden de las columnas](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Desactivar objetos no utilizados

>[!NOTE]
>
>Esta función se lanzó directamente al entorno de producción durante el periodo de tiempo de la versión de vista previa 2019.2.

Si tiene objetos que ya no se utilizan, ahora puede desactivarlos para ocultarlos de las listas a fin de evitar que los usuarios los asocien a otros objetos.

Ahora, al editar cualquiera de los objetos siguientes, puede indicar si deben estar activos. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.

* Procesos de aprobación
* Compañías
* Formularios personalizados
* Rutas de hitos
* Portafolios
* Programas
* Plantillas

Cualquier cosa que desactive que se utilice actualmente seguirá funcionando como siempre y no se eliminará ni bloqueará.

>[!IMPORTANT]
>
>Al crear estos objetos a través de la API de Workfront, el valor predeterminado del parámetro &quot;isActive&quot; es true. Este es un nuevo campo para todos los objetos y no está disponible para su edición antes de la versión 11 de la API. Este campo ya existía para Portfolio, excepto que el valor predeterminado era false; cambiará a un valor predeterminado de true a partir de la versión 11 de la API.

## Mostrar Costo presupuestado de trabajo programado (CPTP) y realizado (CPTR) en las vistas

Ahora puede mostrar el costo presupuestado del trabajo programado (CPTP) y el costo presupuestado del trabajo realizado (CPTR) en las vistas de proyecto y de tarea.

Aunque estas métricas de rendimiento del proyecto se utilizaban antes en cálculos financieros en Workfront, no eran visibles en el sistema antes de esta mejora.

Para obtener información acerca del cálculo del CPTP, vea [Calcular el costo presupuestado del trabajo programado (CPTP)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Para obtener información acerca del cálculo del CPTR, vea [Calcular el costo presupuestado del trabajo realizado (CPTR)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

