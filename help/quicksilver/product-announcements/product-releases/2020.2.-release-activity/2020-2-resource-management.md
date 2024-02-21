---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: "Mejoras en la administración de recursos de 2020.2: Distribuidor de cargas de trabajo"
description: Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# Mejoras en la administración de recursos de 2020.2: Distribuidor de cargas de trabajo

Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.2, consulte [información general sobre la versión 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

Las personas son un activo de nivel 1. Con el Distribuidor de cargas de trabajo, puede protegerlos del agotamiento y empoderarlos para que hagan su mejor trabajo, al tiempo que los alinea con las estrategias clave de la compañía. Presentamos una experiencia de programación reinventada que le permite visualizar y administrar las cargas de trabajo y la demanda de las personas en la misma vista. La interfaz de usuario proporciona una asignación visual clara del exceso y la infrautilización, y es transparente para todas las partes interesadas. Los gestores de personas pueden utilizar esa información como entrada y, desde la misma pantalla, reequilibrar el esfuerzo a través de la cronología, que luego se refleja en el resto de la plataforma de Workfront.

>[!NOTE]
>
>El Distribuidor de cargas de trabajo comenzó a lanzarse como una versión beta con la versión 2019.4. Todas las mejoras del Distribuidor de cargas de trabajo suelen estar disponibles con la versión 2020.2. Las mejoras descritas en esta página se agregaron con la versión 2020.2. Para obtener una descripción general del Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Ajustar la asignación diaria y semanal en el Distribuidor de cargas de trabajo

Para evitar el agotamiento de los recursos, ahora puede ajustar la asignación diaria y semanal de los usuarios al trabajo mediante el Distribuidor de cargas de trabajo.

Antes de esta mejora, esto solo era posible mediante las herramientas de Horario de recursos.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Filtros del Distribuidor de cargas

Para que la información del Distribuidor de cargas de trabajo sea relevante para usted, ahora puede crear filtros para las áreas de Trabajo no asignado y Trabajo asignado del Distribuidor de cargas de trabajo y guardarlos para usarlos en el futuro. A continuación, puede editar la versión guardada para realizar pequeños cambios en ella en lugar de empezar desde cero con un nuevo filtro.

Para obtener información sobre el filtrado en el Distribuidor de cargas de trabajo, consulte [Administrar filtros en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Mostrar las horas restantes en el Distribuidor de cargas de trabajo

Para ayudarle a tomar las decisiones de asignación correctas, una nueva configuración ahora le permite ver la diferencia de horas entre las horas que un usuario está disponible para trabajar según su horario y las horas que ya se les ha asignado para trabajar (las horas restantes). La nueva configuración ya está disponible en el Distribuidor de cargas de trabajo.

Para obtener información sobre la visualización de información en el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o si utiliza Adobe Workfront Classic, consulte [Navegación por el Distribuidor de cargas de trabajo](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).)

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

## Mostrar horas planificadas diariamente para tareas y proyectos en el área de Trabajo no asignado del Distribuidor de cargas de trabajo

Para ayudarle a comprender cómo afectarán las tareas a la carga de trabajo de los usuarios antes de asignarles, la configuración &quot;Mostrar asignaciones&quot; administra ahora la información que se muestra en el área Trabajo no asignado del Distribuidor de cargas de trabajo. Cuando esta configuración está habilitada, las horas planificadas tanto para tareas como para proyectos se muestran en el área de trabajo no asignado del Distribuidor de cargas de trabajo.

Antes de este cambio, esta configuración solo actualizaba información en el área de Trabajo asignado del Distribuidor.

Para obtener información sobre cómo navegar por el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o si utiliza Adobe Workfront Classic, consulte [Navegación por el Distribuidor de cargas de trabajo](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront (anteriormente disponible solo para tareas)

## Nueva casilla de configuración para el Distribuidor de cargas de trabajo

Para optimizar su experiencia, ahora hay disponible un cuadro Configuración que muestra herramientas adicionales para actualizar la vista en el Distribuidor de cargas de trabajo. Este cuadro incluye la siguiente configuración:

* Agrupar por proyecto
* Muestra las horas asignadas o las horas restantes de las tareas y proyectos.

Para obtener información sobre la visualización de información en el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o si utiliza Adobe Workfront Classic, consulte [Navegación por el Distribuidor de cargas de trabajo](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Uso compartido del Distribuidor de cargas de trabajo con un vínculo

Ahora puede compartir la carga de trabajo de sus empleados con los ejecutivos para que puedan tener contexto sobre sus necesidades de personal. Para ello, ahora puede compartir el Distribuidor de cargas de trabajo compartiendo una URL única del Distribuidor de cargas de trabajo con cualquier otra persona.

Para obtener información sobre cómo navegar por el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o si utiliza Adobe Workfront Classic, consulte [Navegación por el Distribuidor de cargas de trabajo](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Modificar el intervalo de fechas en el Distribuidor de cargas de trabajo

Para personalizar aún más la duración de la cronología del Distribuidor de cargas de trabajo para que coincida con sus necesidades, ahora puede seleccionar un período personalizado de 2, 4 o 6 semanas para mostrarlo a la vez.

Antes de esta mejora, el Distribuidor de cargas de trabajo siempre mostraba información a partir de la semana actual.

Para obtener información sobre cómo navegar por el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o si utiliza Adobe Workfront Classic, consulte [Navegación por el Distribuidor de cargas de trabajo](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront (disponible anteriormente)

## Mover y copiar tareas a otro proyecto mantiene la restricción de tareas cuando estas pueden ajustarse a la escala de tiempo del proyecto

Hemos mejorado la forma en que Workfront gestiona la restricción de tarea específica de una tarea al copiar la tarea o moverla a otro proyecto. Algunos ejemplos de restricciones de tareas específicas de fecha son Debe comenzar el, Debe finalizar el, Fechas fijas, No comenzar después del, etc.

Por ejemplo, cuando mueve o copia una tarea con una delimitación Debe comenzar el a otro proyecto cuya fecha planificada de inicio es anterior a la fecha de inicio de la tarea, la tarea mantiene la delimitación después de copiarla o moverla. Cuando se mueve o copia una tarea con una delimitación Debe comenzar el a un proyecto cuya fecha planificada de inicio es posterior a la fecha de inicio de la tarea, la delimitación de la tarea cambia a Lo antes posible.

Antes de este cambio, la restricción de tarea siempre cambia a Lo antes posible.

Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md) (o si utiliza Adobe Workfront Classic, consulte [Mover tareas](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Para obtener información sobre cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (o si utiliza Adobe Workfront Classic, consulte [Copiar y duplicar tareas](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Para obtener una descripción general de todas las restricciones de tarea, consulte [Información general sobre restricciones de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (o si utiliza Adobe Workfront Classic, consulte [Información general sobre restricciones de tarea](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Prevención de la pérdida de datos al realizar cambios en la pestaña Detalles o en una lista de tareas

Para evitar la pérdida de datos al actualizar información en la página Detalles de un objeto o tareas de una lista de tareas en el nivel de proyecto al guardar los cambios manualmente, ahora se muestra un mensaje de advertencia para notificarle que tiene cambios sin guardar antes de intentar editar la información en el encabezado. Las únicas acciones permitidas antes de guardar los cambios son suscribirse o agregar el objeto a los favoritos.

Para obtener información sobre la edición de tareas en una lista, consulte [Edición de tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

## Creación de procesos de aprobación para grupos mediante estados personalizados

Para facilitar a los grupos la administración de sus propios flujos de trabajo únicos, ahora puede utilizar estados personalizados específicos de grupo en los procesos de aprobación.

Anteriormente, un grupo no podía utilizar sus propios estados personalizados con sus procesos de aprobación específicos del grupo. Solo estaban disponibles los estados de todo el sistema, que no siempre se ajustaban a los procesos de aprobación de grupos.

Los estados personalizados ahora se pueden utilizar en procesos de aprobación de un solo uso y en todo el sistema:

* Cree un proceso de aprobación de un solo uso para un objeto (proyecto, tarea o problema) y baselo en los estados asociados con el grupo que trabaja en ese objeto. Esto incluye cualquier estado personalizado asociado con el grupo.
* Cree un proceso de aprobación global y haga que esté disponible solo para el grupo o para todos los miembros del sistema.

Para los usuarios con acceso administrativo a los procesos de aprobación, la información sobre la configuración de los procesos de aprobación está disponible en [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (o si utiliza Adobe Workfront Classic, consulte [Creación de procesos de aprobación](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Para los usuarios de, la información sobre la asociación de procesos de aprobación con elementos de trabajo está disponible en [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (o si utiliza Adobe Workfront Classic, consulte [Asociar un proceso de aprobación nuevo o existente con trabajo](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Una forma más cómoda de actualizar las asignaciones en el Distribuidor de cargas de trabajo

Para facilitar la administración de las asignaciones de un usuario a un elemento de trabajo en el Distribuidor de cargas de trabajo, ahora puede hacer doble clic en el elemento de trabajo. También puede seguir utilizando la opción de menú Editar asignaciones existente. Además, ya no es necesario habilitar la visualización de asignaciones para poder actualizarlas.

Para obtener información sobre la administración de asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Actualizar horas planificadas de la tarea en el Distribuidor de cargas de trabajo

>[!NOTE]
>
>Esta mejora estará disponible en producción poco después de la versión 2020.2.

Una nueva opción en el área de Administración de recursos del nivel de acceso ahora permite a los usuarios con este acceso editar las horas planificadas desde el Distribuidor de cargas de trabajo. Al ajustar las asignaciones en el Distribuidor de cargas de trabajo, el total de asignaciones diarias no necesita coincidir con el número de horas planificadas de las tareas. Una vez guardadas las asignaciones, el total de las horas de asignación pasará a ser las horas planificadas de la tarea. Esto solo es posible para tareas que tengan un tipo de duración simple.

Para obtener información sobre la administración de asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obtener información sobre la concesión de acceso a Administración de recursos, consulte [Conceder acceso a Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Eliminación de la etiqueta &quot;beta&quot; del Distribuidor de cargas de trabajo

Con la versión 2020.2, el Distribuidor de cargas de trabajo ya no estará en estado beta y podrá utilizar el Distribuidor de recursos para revisar y administrar las asignaciones y asignaciones de recursos. La etiqueta &quot;beta&quot; se ha eliminado en el entorno de vista previa. Este mismo cambio se realizará con la versión de producción 20.2. Para obtener información sobre el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
