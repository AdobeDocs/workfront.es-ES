---
content-type: release-notes
keywords: notas, trimestral, actualizar, versión
navigation-topic: 2021-2-release-activity
title: 21.2 Mejoras en la gestión de recursos
description: Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general de la versión 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2 Mejoras en la gestión de recursos

Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Información general sobre la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vista de nivel de mes en el Distribuidor de cargas de trabajo

Para ayudarle a administrar la asignación de recursos durante períodos de tiempo más largos, ahora hemos implementado una vista de nivel mensual para el Distribuidor de cargas de trabajo. Puede ver hasta tres meses a la vez y actualizar las asignaciones de recursos mensuales. Antes de este cambio, solo podía ver el Distribuidor de cargas de trabajo por día o semana.

Para obtener más información, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Conexión entre el Planificador de escenarios, el Distribuidor de cargas de trabajo y la lista de tareas

>[!NOTE]
>
>Disponible solo en la nueva experiencia de Adobe Workfront.

Para ayudarle con la planificación estratégica de sus proyectos y garantizar que se alinean con las iniciativas de mayor alcance del Scenario Planner, hemos creado una nueva área en el proyecto que muestra los requisitos de rol de las iniciativas, así como las horas planificadas estimadas en los elementos de trabajo del proyecto. Esta área está disponible para el Distribuidor de cargas de trabajo de nivel de proyecto, así como para la lista de tareas de la nueva experiencia de Workfront. En la experiencia clásica, esto solo está disponible para el proyecto Distribuidor de cargas de trabajo.

Para obtener más información, consulte los siguientes artículos:

* [Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Esta nueva funcionalidad es visible para todos los usuarios, tanto en la experiencia de Workfront nueva como en la clásica. También pueden verlo los clientes que no hayan adquirido una licencia de Workfront Scenario Planner.

## Utilizar horas planificadas al calcular valores netos en el planificador de recursos

Una nueva configuración en el Planificador de recursos le permite utilizar las horas planificadas para calcular los valores netos.

Antes de esta mejora, Workfront calculaba los valores netos solo mediante las horas presupuestadas. Los valores netos muestran la diferencia entre las horas disponibles y las presupuestadas o planificadas, las horas completas o el coste. Horas presupuestadas sigue siendo la configuración predeterminada al calcular valores netos.

Para obtener más información, vea [Información general sobre horas, ETC e información de costos en las vistas Proyecto y Rol del Planificador de recursos](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Vista de 12 semanas en el Distribuidor de cargas de trabajo

Ahora puede ver hasta 12 semanas de información en el Distribuidor de cargas de trabajo. Antes de esta mejora, se podían ver 2, 4 y 6 semanas de información.

Para obtener información sobre cómo ver el Distribuidor de cargas de trabajo, consulte [Desplazarse por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Desplazarse por el Distribuidor de cargas de trabajo.

## Cambio en la forma en que funciona el filtro Rol en el área sin asignar del Distribuidor de cargas de trabajo

Para mejorar el modo en que funciona el filtro de Función en la Distribuidor de cargas de trabajo y cumplir las expectativas de los usuarios, hemos modificado la funcionalidad del filtro en el área No asignada. Ahora solo puede ver las horas asignadas a los roles que especifique en el filtro.

Antes de esta mejora, al aplicar el filtro de rol al área sin asignar, el Distribuidor de cargas de trabajo mostraba todas las horas asociadas con los elementos de trabajo asignados a los roles

Para obtener información sobre el filtrado en el Distribuidor de cargas de trabajo, consulte [Administrar filtros en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
