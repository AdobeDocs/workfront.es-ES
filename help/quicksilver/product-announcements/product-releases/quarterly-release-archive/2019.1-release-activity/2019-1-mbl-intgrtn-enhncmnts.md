---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Mejoras en la integración de dispositivos móviles y 2019.1
description: Esta página describe todas las mejoras de Administración de recursos incluidas en la versión 2019.1. La funcionalidad ya está disponible en el entorno de producción.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 6b86ba0d-977a-4c89-8832-e81bf28d9dad
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Mejoras en la integración de dispositivos móviles y 2019.1

Esta página describe todas las mejoras de Administración de recursos incluidas en la versión 2019.1. La funcionalidad ya está disponible en el entorno de producción.

Para obtener una lista de todos los cambios realizados en 2019.1, consulte [Resumen de la actividad de la versión 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Se ha actualizado el filtro predeterminado en el Planificador de recursos

El filtro predeterminado en el Planificador de recursos ya no filtra por el grupo del proyecto.

Al ver el Planificador de recursos, ahora solo ve los proyectos que son actuales y que distinguen entre fechas de forma predeterminada. La información de los siguientes proyectos se incluye de forma predeterminada:

* Con una fecha planificada de finalización que es posterior a la primera fecha del mes actual.
* Con una fecha de inicio planificada que sea anterior a la última fecha del cuarto mes a partir de hoy.
* Con un estado de Actual o Planificación.

Anteriormente, el filtro predeterminado recuperaba la información de los siguientes proyectos adicionales:

* Con una fecha planificada de finalización que es posterior a la primera fecha del mes actual.
* Con una fecha de inicio planificada que sea anterior a la última fecha del cuarto mes a partir de hoy.
* Con un estado de Actual o Planificación.
* Con un Grupo que coincida con el Grupo de inicio del usuario que ha iniciado sesión.

Para obtener información sobre cómo aplicar filtros al Planificador de recursos, consulte [Información sobre filtros en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Uso de caracteres comodín para los filtros del Planificador de recursos

Ahora puede utilizar caracteres comodín al crear filtros en el Planificador de recursos. Por ejemplo, puede usar $$USER.ID para filtrar por información sobre el usuario que ha iniciado sesión, o $$USER.companyID para filtrar por información sobre todos los usuarios que pertenecen a la misma empresa que el usuario que ha iniciado sesión. Para obtener una lista completa de las variables basadas en usuarios, consulte la sección [Variables de filtro comodín basadas en usuarios](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) en [Variables de filtro comodín](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Anteriormente, los caracteres comodín no estaban disponibles para los filtros del Planificador de recursos.

Para obtener información acerca del filtrado en el Planificador de recursos, vea [Filtrar información en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)

VÍDEO

## Compatibilidad con variables de filtro comodín basadas en fechas en el Planificador de recursos

Ahora puede usar cualquier versión de la variable de filtro comodín $$TODAY cuando genere un filtro en el Planificador de recursos.

Antes de esta mejora, solo podía utilizar variables de filtro comodín basadas en el usuario.

Para obtener información sobre el filtrado en el Planificador de recursos, consulte [Filtrar información en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Para obtener información acerca de las variables de filtro comodín, vea [Variables de filtro comodín](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

VÍDEO

## Opciones de exportación para la vista de rol en el Planificador de recursos

Ahora puede seleccionar los niveles de información que desea exportar desde el Planificador de recursos en la vista de funciones.

Puede exportar cualquiera de las siguientes opciones:

* Solo roles
* Roles y proyectos
* Roles, proyectos y usuarios

Antes de esta mejora, todos los niveles de información se exportaban en la vista de funciones. Estas opciones se han introducido en las vistas Proyecto y Usuario en una versión anterior.

Para obtener información acerca de cómo exportar información desde el Planificador de recursos, vea [Exportar información desde el Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VÍDEO

## Opciones de formato de datos para exportar el Planificador de recursos

Ahora puede seleccionar cómo desea mostrar la información en el archivo de Excel cuando se exporta desde el Planificador de recursos.

Puede mostrar la disponibilidad y la asignación de la información exportada desde el Planificador de recursos de las siguientes maneras:

* Desagrupado por el nombre de los objetos a los que pertenece. En este caso, los nombres de los objetos a los que pertenece se muestran en cada fila de datos. (esta es la opción predeterminada)
* Agrupado por el nombre de los objetos a los que pertenece. En este caso, la información del archivo exportado aparece tal y como aparece en Workfront.

Antes de esta mejora, la información del archivo exportado aparecía como aparece en Workfront.

Para obtener información acerca de cómo exportar información desde el Planificador de recursos, vea [Exportar información desde el Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VÍDEO

## Cronología de programación persistente

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

La programación de escalas de tiempo ahora mantiene el periodo de tiempo seleccionado al actualizar la escala de tiempo o al salir de la página.

Antes de esta mejora, las escalas de tiempo de programación volvían al periodo de tiempo predeterminado cuando se actualizaba o se navegaba fuera de la página.

Esta mejora está disponible en las siguientes áreas:

* Pestaña Programación del área Personas
* Ficha Equipo trabajando en
* Subpestaña Programación en la pestaña Asignación de personal de un proyecto

Para obtener información sobre cómo trabajar con la escala de tiempo en las áreas de Horario de recursos, consulte &quot;Introducción a Horario de recursos&quot;.

VÍDEO

## Nuevas opciones de exportación en el Planificador de recursos

Ahora puede seleccionar los niveles de información que desea exportar desde el Planificador de recursos.

En la vista Proyecto, puede exportar cualquiera de las siguientes opciones:

* Solo proyectos
* Proyectos y roles
* Proyectos, funciones y usuarios

En la vista de usuario, puede exportar cualquiera de las siguientes opciones:

* Solo usuarios
* Usuarios y proyectos
* Usuarios, proyectos, funciones, tareas y problemas

Antes de esta mejora, todos los niveles de información se exportaban de forma predeterminada en todas las vistas del Planificador de recursos.

Para obtener información acerca de cómo exportar información desde el Planificador de recursos, vea [Exportar información desde el Planificador de recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VÍDEO

## Actualización de la vista de usuario en el Planificador de recursos

Ahora todos los usuarios del sistema aparecen en la Vista de usuario del Planificador de recursos, pero sólo los usuarios asociados con los proyectos filtrados muestran información sobre las horas.

Antes de esta actualización, en la vista de usuario del Planificador de recursos solo se mostraban los usuarios asignados a elementos de trabajo en los proyectos por los que filtraba.

Puede utilizar filtros basados en usuarios para reducir el número de usuarios que se muestran en la vista de usuarios a aquellos que están asignados a los proyectos que desea mostrar.

Para obtener información sobre los filtros del Planificador de recursos, consulte [Información sobre filtros en el Planificador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
