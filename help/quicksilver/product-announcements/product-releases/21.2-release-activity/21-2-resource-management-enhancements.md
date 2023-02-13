---
content-type: release-notes
keywords: notas,trimestral,actualizar,versión
navigation-topic: 2021-2-release-activity
title: 21.2 Mejoras en la gestión de recursos
description: En esta página se describen todas las mejoras realizadas en la administración de recursos con la versión 21.2 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general sobre la versión 21.2.
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2 Mejoras en la gestión de recursos

En esta página se describen todas las mejoras realizadas en la administración de recursos con la versión 21.2 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Resumen de la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vista de nivel de mes en el equilibrador de carga de trabajo

Para ayudarle a administrar la asignación de recursos para períodos de tiempo más largos, hemos implementado una vista de nivel de mes para el equilibrador de carga de trabajo. Puede ver hasta tres meses a la vez y actualizar las asignaciones mensuales de recursos. Antes de este cambio, solo podía ver el equilibrador de carga de trabajo por día o semana.

Para obtener más información, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Conexión entre el planificador de escenarios, el equilibrador de carga de trabajo y la lista de tareas

>[!NOTE]
>
>Disponible solo en la nueva experiencia de Adobe Workfront.

Para ayudarle con la planificación estratégica de sus proyectos y asegurarse de que se ajustan a las iniciativas más amplias del Planificador de escenario, hemos creado un nuevo área en el proyecto que muestra los requisitos de funciones de trabajo de las iniciativas, así como las horas programadas estimadas en los elementos de trabajo del proyecto. Esta área está disponible para el equilibrador de carga de trabajo de nivel de proyecto, así como para la lista de tareas de la nueva experiencia de Workfront. En la experiencia clásica, esto solo está disponible para el equilibrador de carga de trabajo del proyecto.

Para obtener más información, consulte los siguientes artículos:

* [Visión general de la conciliación de las asignaciones de recursos entre proyectos e iniciativas](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Esta nueva funcionalidad es visible para todos los usuarios, tanto en la experiencia nueva como en la clásica de Workfront. Esto también es visible para los clientes que no han adquirido una licencia de Workfront Scenario Planner.

## Utilizar las horas planificadas al calcular los valores netos en el planificador de recursos

Una nueva configuración en el planificador de recursos le permite usar Horario planificado al calcular valores de Neto.

Antes de esta mejora, Workfront calculaba los valores de red solo usando horas presupuestadas. Los valores netos muestran la diferencia entre las horas disponibles y presupuestadas o planeadas, FTE o coste. Horas presupuestadas sigue siendo la configuración predeterminada al calcular valores de red.

Para obtener más información, consulte [Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Vista de 12 semanas en el equilibrador de carga de trabajo

Ahora puede ver hasta 12 semanas de información en el equilibrador de carga de trabajo. Antes de esta mejora, podría ver información de 2, 4 y 6 semanas.

Para obtener información sobre la visualización del equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Vaya al equilibrador de carga de trabajo.

## Cambio en la forma en que funciona el filtro Función de trabajo en el área No asignado del equilibrador de carga de trabajo

Para mejorar la forma en que funciona el filtro Función de trabajo en el equilibrador de carga de trabajo y para que coincida con las expectativas de los usuarios, hemos modificado la funcionalidad del filtro en el área No asignado. Ahora solo puede ver las horas asignadas a las funciones de trabajo que especifique en el filtro.

Antes de esta mejora, al aplicar el filtro Función de trabajo al área No asignada, el equilibrador de carga de trabajo mostraba todas las horas asociadas con los elementos de trabajo asignados a las funciones de trabajo .

Para obtener información sobre el filtrado de información en el equilibrador de carga de trabajo, consulte [Administrar filtros en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
