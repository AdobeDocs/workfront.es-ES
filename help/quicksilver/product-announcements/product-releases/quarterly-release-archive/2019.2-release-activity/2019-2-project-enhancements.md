---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2 Mejoras en los proyectos
description: Esta página describe todas las mejoras en los proyectos incluidas en la versión 2019.2. La funcionalidad está planificada para estar disponible en el entorno de producción la semana del 20 de mayo de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
TQID: https://experienceleague.adobe.com/-4bsOXpJd8x1IKN-bqcvRqHDDiD5JawSrXgyRYmVYqA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 741
ht-degree: 100%

---

# 2019.2 Mejoras en los proyectos

Esta página describe todas las mejoras en los proyectos incluidas en la versión 2019.2. La funcionalidad está planificada para estar disponible en el entorno de producción la semana del 20 de mayo de 2019.

Para obtener una lista de todos los cambios realizados en la versión 2019.2, consulte [Información general de la actividad de la versión 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Búsqueda de grupos más rápida al personalizar estados

El menú desplegable de la pestaña Estados del área Configuración es ahora un menú de escritura anticipada. Esto le permite buscar y encontrar rápidamente cualquier grupo en el sistema, lo que facilita la personalización de los estados.

Anteriormente, el menú desplegable mostraba un número limitado de grupos. Si el grupo deseado no se mostraba, tenía que ir a Configuración > Grupos y buscar el grupo específico para personalizar los estados del grupo.

Para obtener más información, consulte [Crear o editar un estado](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Adjuntar procesos personalizados predeterminados y procesos de aprobación a las tareas

Ahora puede configurar formularios personalizados y procesos de aprobación predeterminados para adjuntarlos a las tareas cuando añada tareas a un proyecto. Puede establecer la configuración predeterminada en el nivel de proyecto.

Para obtener información sobre la configuración de formularios personalizados y procesos de aprobación predeterminados para tareas en el nivel de proyecto, consulte la sección “Tareas” en el artículo [Editar proyectos](../../../../manage-work/projects/manage-projects/edit-projects.md).

## Mostrar toda la fila de una tarea principal en negrita en una lista de tareas

En una lista de tareas, la fila que contiene una tarea principal se muestra en negrita. Este cambio es visible cuando la lista se ordena por la Estructura del desglose de trabajo o por el Número de tareas en orden ascendente.

## Invertir los cambios en las listas de tareas

Un nuevo botón Guardar automáticamente en la lista de tareas le permite seleccionar si desea que los cambios realizados se guarden automáticamente o si desea ver los efectos que los cambios tienen antes de guardarlos. Esta configuración se aplica tanto a la lista de tareas como al gráfico Gantt.

Antes de esta mejora, todos los cambios se guardaban siempre automáticamente.

Para obtener información acerca de cómo editar tareas en una lista de tareas, consulte [Editar tareas](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Para obtener información acerca de la edición de tareas en el gráfico Gantt, vea [Actualizar información en la lista de tareas Gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Nuevos valores predeterminados de anchura de columna en listas nuevas

Ahora Workfront ajusta automáticamente la anchura de las columnas según la información de formato de valor de cada columna. Por ejemplo, las columnas que muestran un número son más anchas que las que muestran el campo Descripción.

Antes de esta mejora, las anchuras de columna en las vistas del nuevo proyecto y tarea se establecían en 100 píxeles, a menos que se especifique lo contrario.

Para obtener información acerca de los anchos de columna, vea [Modificar el ancho y el orden de las columnas](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Desactivación de metas no utilizadas

>[!NOTE]
>
>Esta función se lanzó directamente al entorno de producción durante el periodo de tiempo de vista previa de la versión 2019.2.

Si tiene objetos que ya no se utilizan, ahora puede desactivarlos para ocultarlos de las listas para evitar que los usuarios los asocien a otros objetos.

Ahora, al editar cualquiera de las metas siguientes, puede indicar si deben estar activas. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.

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
>Al crear estos objetos a través de la API de Workfront, el valor predeterminado del parámetro “isActive” es true. Este es un nuevo campo para todos los objetos y no está disponible para su edición antes de la versión 11 de la API. Este campo ya existía para Portafolios, excepto que el valor predeterminado era false; cambiará a un valor predeterminado de true a partir de la versión 11 de la API.

## Mostrar coste presupuestado del trabajo programado (CPTP) y realizado (CPTR) en las vistas

Ahora puede mostrar el coste presupuestado del trabajo programado (CPTP) y el coste presupuestado del trabajo realizado (CPTR) en las vistas de proyecto y de tarea.

Aunque estas métricas de rendimiento del proyecto se utilizaban antes en cálculos financieros en Workfront, no eran visibles en el sistema antes de esta mejora.

Para obtener información acerca del cálculo del CPTP, consulte [Calcular el coste presupuestado de trabajo programado (CPTP)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Para obtener información acerca del cálculo del CPTP, consulte [Calcular el coste presupuestado de trabajo realizado (CPTR)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

