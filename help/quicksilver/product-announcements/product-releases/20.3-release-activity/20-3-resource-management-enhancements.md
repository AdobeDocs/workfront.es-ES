---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Mejoras en la gestión de recursos
description: En esta página se describen todas las mejoras realizadas en la administración de recursos con la versión 20.3 para el entorno de producción. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 10 de agosto de 2020.
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3 Mejoras en la gestión de recursos

En esta página se describen todas las mejoras realizadas en la administración de recursos con la versión 20.3 para el entorno de producción. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 10 de agosto de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.3, consulte [Información general sobre la versión 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Incluir horas de problemas en el área Trabajo asignado del equilibrador de carga de trabajo

Para permitirle ver una imagen completa de todas las cargas de trabajo de sus personas, hemos introducido un ajuste que le permite incluir horas de problemas en el área Trabajo asignado del equilibrador de carga de trabajo.

Para obtener información sobre cómo trabajar en el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar asignaciones para días no laborables en el equilibrador de carga de trabajo

Puede ajustar las asignaciones de sus recursos para los días no laborables mediante el equilibrador de carga de trabajo.

Para obtener información sobre la administración de asignaciones en el equilibrador de carga de trabajo, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtros de variable disponibles en el equilibrador de carga de trabajo

Para mejorar su experiencia y darle más flexibilidad cuando comparte información, hemos implementado filtros de variable para el equilibrador de carga de trabajo. Se han agregado los siguientes filtros al equilibrador de carga de trabajo:

* &quot;Me&quot; (al filtrar por usuarios)
* &quot;Mi función principal&quot; (al filtrar por funciones)
* &quot;My Home Team&quot; o &quot;All My Teams&quot; (cuando se filtra por equipos).

Estos filtros reemplazan a las variables de filtro comodín de $$USER.ID, $$USER.roleID, $$USER.homeTeamID y $$USER.teamIDs

Cuando aplique uno de estos filtros y luego comparta el equilibrador de carga de trabajo o lo coloque en un tablero, todos los demás usuarios verán su propia información.

Para obtener información sobre la aplicación de filtros al equilibrador de carga de trabajo, consulte [Filtrar información en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nueva clasificación para proyectos en el equilibrador de carga de trabajo

El equilibrador de carga de trabajo ahora ordena los proyectos en función primero de la fecha de inicio prevista más temprana y, en segundo lugar, de la fecha de finalización planeada más reciente de las tareas del proyecto que se producen durante el periodo de tiempo que el usuario muestra en la pantalla. Esto le permite organizar el trabajo en una jerarquía similar a un árbol, lo que le ayuda a identificar el trabajo con mayor facilidad durante un día.

Para obtener información sobre la visualización de proyectos y elementos de trabajo en el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Mostrar el progreso real del trabajo en el equilibrador de carga de trabajo

Para ofrecerle una perspectiva precisa del progreso de su carga de trabajo, hemos introducido una nueva configuración en el equilibrador de carga de trabajo que muestra la cronología de tareas y problemas según sus fechas proyectadas. Puede activar la opción Mostrar fechas proyectadas para ver la cronología proyectada del elemento de trabajo además de la cronología planificada.

Además, con esta mejora, si una tarea o un problema se completa antes de la fecha de finalización prevista, se pulsan las horas asignadas de los días restantes para indicar que no se cuentan en la asignación general del usuario.

Para obtener información sobre cómo navegar por el equilibrador de carga de trabajo y habilitar la configuración, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Funciones del equilibrador de carga de trabajo comunicadas anteriormente como lanzadas con la versión 20.2

* [Ajustar la asignación diaria y semanal en el equilibrador de carga de trabajo](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Actualizar las horas planificadas de la tarea en el equilibrador de carga de trabajo](#update-task-planned-hours-in-the-workload-balancer)
* [Una forma más conveniente de actualizar las asignaciones en el equilibrador de carga de trabajo](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Ajustar la asignación diaria y semanal en el equilibrador de carga de trabajo {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Para evitar que se agoten los recursos, ahora puede ajustar la asignación diaria y semanal de los usuarios para que funcione con el equilibrador de carga de trabajo.

Antes de esta mejora, esto solo era posible mediante las herramientas de programación de recursos.

Para obtener información sobre la administración de asignaciones en el equilibrador de carga de trabajo, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

### Actualizar las horas planificadas de la tarea en el equilibrador de carga de trabajo {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Esta mejora estará disponible en Producción poco después de la versión 2020.2.

Una nueva opción en el área de Gestión de Recursos del nivel de acceso ahora permite a los usuarios con este acceso editar las horas planificadas desde el equilibrador de carga de trabajo. Al ajustar las asignaciones en el equilibrador de carga de trabajo, el total de asignaciones diarias no necesita coincidir con el número de horas planificadas de las tareas. Una vez guardadas las asignaciones, el total de horas de asignación se convertirá en las horas planificadas de la tarea. Esto solo es posible para tareas que tienen un tipo de duración simple.

Para obtener información sobre la administración de asignaciones en el equilibrador de carga de trabajo, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obtener información sobre la concesión de acceso a la Administración de recursos, consulte [Conceder acceso a la Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Una forma más conveniente de actualizar las asignaciones en el equilibrador de carga de trabajo {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Para que resulte más conveniente administrar las asignaciones de un usuario a un elemento de trabajo en el equilibrador de carga de trabajo, ahora puede hacer doble clic en el elemento de trabajo. También puede seguir utilizando la opción de menú Editar asignaciones existente. Además, ya no es necesario habilitar la visualización de asignaciones para poder actualizarlas.

Para obtener información sobre la administración de asignaciones en el equilibrador de carga de trabajo, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
