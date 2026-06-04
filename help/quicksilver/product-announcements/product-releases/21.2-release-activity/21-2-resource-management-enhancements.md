---
content-type: release-notes
keywords: notas,trimestral,actualizar,versión
navigation-topic: 2021-2-release-activity
title: Mejoras en la administración de recursos de la versión 21.2
description: En esta página se describen todas las mejoras concernientes a la Administración de recursos realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general sobre la versión 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
TQID: https://experienceleague.adobe.com/cAM0R2azvfhRW25brnRKCUXZ5f2ZLGeBVd19okbdBpU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 575
ht-degree: 100%

---

# Mejoras en la administración de recursos de la versión 21.2

En esta página se describen todas las mejoras concernientes a la Administración de recursos realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Información general sobre la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vista a nivel mensual en el Distribuidor de cargas de trabajo

Para ayudarle a administrar la asignación de recursos durante períodos de tiempo más largos, ahora hemos implementado una vista a nivel mensual para el Distribuidor de cargas de trabajo. Puede ver hasta tres meses a la vez y actualizar las asignaciones de recursos mensuales. Antes de este cambio, solo era posible ver el Distribuidor de cargas de trabajo por día o semana.

Para obtener más información, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Conexión entre el planificador de escenarios, el distribuidor de cargas de trabajo y la lista de tareas

>[!NOTE]
>
>Disponible solo en la nueva experiencia de Adobe Workfront.

Para ayudarle en la planificación estratégica de sus proyectos y garantizar que estén en consonancia con las iniciativas de mayor alcance del Planificador de escenarios, hemos creado una nueva área en el proyecto que muestra los requisitos de las funciones de las iniciativas, así como las horas planificadas estimadas en los elementos de trabajo del proyecto. Esta área está disponible para el distribuidor de cargas de trabajo de nivel de proyecto, así como para la lista de tareas de la nueva experiencia de Workfront. En la experiencia clásica, esto solo está disponible para el proyecto Distribuidor de cargas de trabajo.

Para obtener más información, consulte los siguientes artículos:

* [Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Esta nueva funcionalidad es visible para todos los usuarios, tanto en la experiencia de Workfront nueva como en la clásica. También pueden verlo los clientes que no hayan adquirido una licencia del Planificador de escenarios de Workfront.

## Utilizar horas planificadas al calcular valores netos en el Planificador de recursos

Una nueva configuración en el Planificador de recursos le permite utilizar las horas planificadas para calcular los valores netos.

Antes de esta mejora, Workfront calculaba los valores netos solo mediante las horas presupuestadas. Los valores netos muestran la diferencia entre las horas disponibles y las presupuestadas o planificadas, las horas completas o el coste. Horas presupuestadas sigue siendo la configuración predeterminada al calcular valores netos.

Para obtener más información, vea [Información general sobre horas, FTE y costes en las vistas Proyecto y Función del Planificador de recursos](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Vista de 12 semanas en el Distribuidor de cargas de trabajo

Ahora puede ver hasta 12 semanas de información en el Distribuidor de cargas de trabajo. Antes de esta mejora, se podían ver 2, 4 y 6 semanas de información.

Para obtener información sobre cómo ver el Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navegar por el Distribuidor de cargas de trabajo.

## Cambio en la forma en que funciona el filtro Función en el área Sin asignar del Distribuidor de cargas de trabajo

Para mejorar el modo en que funciona el filtro de Función en el Distribuidor de cargas de trabajo y cumplir las expectativas de los usuarios, hemos modificado la funcionalidad del filtro en el área sin asignar. Ahora solo puede ver las horas asignadas a las funciones que especifique en el filtro.

Antes de esta mejora, al aplicar el filtro de Función al área sin asignar, el Distribuidor de cargas de trabajo mostraba todas las horas asociadas con los elementos de trabajo asignados a las funciones.

Para obtener información sobre el filtrado en el Distribuidor de cargas de trabajo, consulte [Administrar filtros en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
