---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Mejoras en la gestión de recursos
description: Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 20.3 en el entorno de producción. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 10 de agosto de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Mejoras en la gestión de recursos

Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 20.3 en el entorno de producción. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 10 de agosto de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.3, consulte [Descripción general de la versión 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Incluir horas de problemas en el área de Trabajo asignado del Distribuidor de cargas de trabajo

Para permitirle ver una imagen completa de todas las cargas de trabajo de sus recursos, hemos introducido una configuración que le permite incluir horas de problemas en el área de Trabajo asignado del Distribuidor de cargas de trabajo.

Para obtener información acerca de cómo trabajar en el Distribuidor de cargas de trabajo, vea [Desplazarse por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar asignaciones para días no laborables en el Distribuidor de cargas de trabajo

Puede ajustar las asignaciones de los recursos para los días no laborables mediante el Distribuidor de cargas de trabajo.

Para obtener información sobre cómo administrar asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtros variables disponibles en el Distribuidor de cargas de trabajo

Para mejorar su experiencia y ofrecerle una mayor flexibilidad a la hora de compartir información, hemos implementado filtros de variables para el Distribuidor de cargas de trabajo. Se han añadido los siguientes filtros al Distribuidor de cargas de trabajo:

* &quot;Yo&quot; (al filtrar por usuarios)
* &quot;Mi función principal&quot; (al filtrar por funciones)
* &quot;Mi equipo de inicio&quot; o &quot;Todos mis equipos&quot; (al filtrar por equipos).

Estos filtros reemplazan las variables de filtro comodín de $$USER.ID, $$USER.roleID, $$USER.homeTeamID y $$USER.teamIDs

Al aplicar uno de estos filtros y, a continuación, compartir el Distribuidor de cargas de trabajo o colocarlo en un panel, los demás usuarios verán su propia información.

Para obtener información sobre cómo aplicar filtros al Distribuidor de cargas de trabajo, consulte [Información sobre filtros en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nueva ordenación de proyectos en el Distribuidor de cargas de trabajo

El Distribuidor de cargas de trabajo ahora ordena los proyectos en función de la primera fecha planificada de inicio y, en segundo lugar, la última fecha planificada de finalización de las tareas del proyecto que se producen durante el periodo de tiempo que el usuario muestra en la pantalla. Esto le permite organizar el trabajo en una jerarquía en forma de árbol, lo que le ayuda a identificar más fácilmente el trabajo de un día.

Para obtener información acerca de cómo ver proyectos y elementos de trabajo en el Distribuidor de cargas de trabajo, vea [Desplazarse por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Mostrar el progreso de trabajo real en el Distribuidor de cargas de trabajo

Para ofrecerle una perspectiva precisa del progreso de su carga de trabajo, hemos introducido una nueva configuración en el Distribuidor de cargas de trabajo que muestra la cronología de las tareas y los problemas según sus fechas proyectadas. Puede activar la configuración Mostrar fechas proyectadas para ver la escala de tiempo proyectada del elemento de trabajo además de la escala de tiempo planificada.

Además, con esta mejora, si una tarea o un problema se finalizan antes de la fecha planificada de finalización, las horas asignadas de los días restantes se tachan para indicar que no se contabilizan en la asignación general del usuario.

Para obtener información sobre cómo navegar por el Distribuidor de cargas de trabajo y habilitar la configuración, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Las funciones del Distribuidor de cargas de trabajo comunicadas anteriormente como la versión 20.2

* [Ajustar la asignación diaria y semanal en el Distribuidor de cargas de trabajo](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Actualizar horas planificadas para la tarea en el Distribuidor de cargas de trabajo](#update-task-planned-hours-in-the-workload-balancer)
* [Una forma más cómoda de actualizar las asignaciones en el Distribuidor de cargas de trabajo](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Ajustar la asignación diaria y semanal en el Distribuidor de cargas de trabajo {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Para evitar el agotamiento de los recursos, ahora puede ajustar la asignación diaria y semanal de los usuarios al trabajo mediante el Distribuidor de cargas de trabajo.

Antes de esta mejora, esto solo era posible mediante las herramientas de Horario de recursos.

Para obtener información sobre cómo administrar asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

### Actualizar horas planificadas de la tarea en el Distribuidor de cargas de trabajo {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Esta mejora estará disponible en producción poco después de la versión 2020.2.

Una nueva opción en el área de Administración de recursos del nivel de acceso ahora permite a los usuarios con este acceso editar las horas planificadas desde el Distribuidor de cargas de trabajo. Al ajustar las asignaciones en el Distribuidor de cargas de trabajo, el total de asignaciones diarias no necesita coincidir con el número de horas planificadas de las tareas. Una vez guardadas las asignaciones, el total de las horas de asignación pasará a ser las horas planificadas de la tarea. Esto solo es posible para tareas que tengan un tipo de duración simple.

Para obtener información sobre cómo administrar asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obtener información acerca de cómo conceder acceso a Administración de recursos, vea [Conceder acceso a Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Una forma más cómoda de actualizar las asignaciones en el Distribuidor de cargas de trabajo {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Para facilitar la administración de las asignaciones de un usuario a un elemento de trabajo en el Distribuidor de cargas de trabajo, ahora puede hacer doble clic en el elemento de trabajo. También puede seguir utilizando la opción de menú Editar asignaciones existente. Además, ya no es necesario habilitar la visualización de asignaciones para poder actualizarlas.

Para obtener información sobre cómo administrar asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
