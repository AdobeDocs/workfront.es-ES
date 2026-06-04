---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Mejoras en la administración de recursos
description: En esta página se describen todas las mejoras de Administración de recursos incluidas en la versión 2019.1. Esta funcionalidad ya está disponible en el entorno de producción.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
TQID: https://experienceleague.adobe.com/5P0V7i-nS8PMlAPzS5oLEv3KvDOLGQ4vAGpRaF51ZCc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 959
ht-degree: 100%

---

# 2019.1 Mejoras en la administración de recursos

En esta página se describen todas las mejoras de Administración de recursos incluidas en la versión 2019.1. Esta funcionalidad ya está disponible en el entorno de producción.

Para obtener una lista de todos los cambios realizados en 2019.1, consulte [Información general sobre la actividad de la versión 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Se ha actualizado el filtro predeterminado en el Planificador de recursos

El filtro predeterminado en el Planificador de recursos ya no filtra por grupo de proyecto.

Cuando visualice el Planificador de recursos, ahora solo verá los proyectos que son actuales y que distinguen entre fechas de forma predeterminada. Se ha incluido la información de los siguientes proyectos de forma predeterminada:

* Con una fecha planificada de finalización que es posterior a la primera fecha del mes actual.
* Con una fecha de inicio planificada que es anterior a la última fecha del cuarto mes a partir de hoy.
* Con un estado de Actual o Planificación.

Anteriormente, el filtro predeterminado recuperaba la información de los siguientes proyectos adicionales:

* Con una fecha planificada de finalización que es posterior a la primera fecha del mes actual.
* Con una fecha de inicio planificada que es anterior a la última fecha del cuarto mes a partir de hoy.
* Con un estado de Actual o Planificación.
* Con un Grupo que coincide con el grupo de inicio del usuario que ha iniciado sesión.

Para obtener información sobre la aplicación de filtros al Planificador de recursos, consulte [Información sobre filtros en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Uso de caracteres comodín para los filtros del Planificador de recursos

Ahora puede utilizar caracteres comodín al crear filtros en el Planificador de recursos. Por ejemplo, puede utilizar $$USER.ID para filtrar por la información sobre el usuario que ha iniciado sesión, o $$USER.companyID para filtrar por la información sobre todos los usuarios que pertenecen a la misma compañía que el usuario que ha iniciado sesión. Para obtener una lista completa de las variables basadas en usuarios, consulte [Variables de filtro comodín basadas en usuarios](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) en [Variables de filtro comodín](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Anteriormente, los caracteres comodín no estaban disponibles para los filtros del Planificador de recursos.

Para obtener información sobre el filtrado en el Planificador de recursos, consulte [Filtrar información en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Compatibilidad con variables de filtro de comodín basadas en fechas en el Planificador de recursos

Ahora puede usar cualquier versión de la variable de filtro comodín $$TODAY cuando genere un filtro en el Planificador de recursos.

Antes de esta mejora, solo se podían utilizar variables de filtro comodín basadas en el usuario.

Para obtener información sobre el filtrado en el Planificador de recursos, consulte [Filtrar información en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Para obtener información sobre las variables de filtro comodín, consulte [Variables de filtro comodín](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Opciones de exportación para la vista de función en el Planificador de recursos

Ahora puede seleccionar los niveles de información que desea exportar desde el Planificador de recursos en la vista de funciones. Puede exportar cualquiera de los siguientes niveles:

* Solo funciones
* Roles y proyectos
* Funciones, proyectos y usuarios

Antes de esta mejora, todos los niveles de información se exportaban en la vista de función. Estas opciones se han introducido en las vistas Proyecto y Usuario en una versión anterior.

Para obtener información sobre cómo exportar información desde el Planificador de recursos, consulte [Exportar información del Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Opciones de formato de datos para exportar el Planificador de recursos

Ahora puede seleccionar cómo desea mostrar la información en el archivo de Excel cuando se exporta desde el Planificador de recursos.

Puede mostrar la disponibilidad y la asignación de la información exportada desde el Planificador de recursos de las siguientes maneras:

* Desagrupada por el nombre de los objetos a los que pertenece. En este caso, los nombres de los objetos a los que pertenece se muestran en cada fila de datos. (esta es la opción predeterminada)
* Agrupada por el nombre de los objetos a los que pertenece. En este caso, la información del archivo exportado aparece tal y como aparece en Workfront.

Antes de esta mejora, la información del archivo exportado aparecía tal y como aparece en Workfront.

Para obtener información sobre la exportación de información desde el Planificador de recursos, consulte [Exportar información del Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Cronología de programación persistente

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre el Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

La programación de cronologías ahora conserva el periodo de tiempo que haya seleccionado al actualizar la cronología o al salir de la página.

Antes de esta mejora, las cronologías de programación volvían al periodo de tiempo predeterminado cuando se actualizaba la página o se salía de ella.

Se ha informado de este problema en las siguientes áreas:

* Pestaña Programación del área Personas
* Pestaña Equipo trabajando
* Subpestaña Programación en la pestaña Personal de un proyecto

Para obtener información sobre cómo trabajar con la cronología en las áreas de Horario de recursos, consulte “Introducción al horario de recursos”.

## Nuevas opciones de exportación en el Planificador de recursos

Ahora puede seleccionar los niveles de información que desea exportar desde el Planificador de recursos. En la vista Proyecto, puede exportar cualquiera de los siguientes niveles:

* Solo proyectos
* Proyectos y roles
* Proyectos, funciones y usuarios

En la vista de usuario, puede exportar cualquiera de los siguientes niveles:

* Solo usuarios
* Usuarios y proyectos
* Usuarios, proyectos, funciones, tareas y problemas

Antes de esta mejora, todos los niveles de información se exportaban de forma predeterminada en todas las vistas del Planificador de recursos.

Para obtener información sobre la exportación desde el Planificador de recursos, consulte [Exportar información del Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Actualización de la vista de usuario en el Planificador de recursos

Ahora todos los usuarios del sistema aparecen en la Vista de usuario del Planificador de recursos, pero solo los usuarios asociados con los proyectos filtrados muestran información sobre las horas.

Antes de esta actualización, solo se mostraban en la Vista de usuario del Planificador de recursos los usuarios asignados a elementos de trabajo en los proyectos por los que filtraba.

Puede utilizar filtros basados en usuarios para reducir el número de usuarios que se muestran en la Vista de usuario a aquellos que se han asignado a los proyectos que desea mostrar.

Para obtener información sobre los filtros del Planificador de recursos, consulte [Información sobre filtros en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
