---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.3 Beta 4
description: Esta página describe todos los cambios más recientes disponibles en el entorno de vista previa con la versión 2017.3 Beta 4. La funcionalidad de esta página se lanzó en el entorno de vista previa la semana del 25 de septiembre de 2017. Estuvo disponible en el entorno de producción a principios de noviembre de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
TQID: https://experienceleague.adobe.com/JB7Mhf1RUya-cG9B1OJ-xuAW-y9aq-V2Jxa3Xpf7VFI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1625
ht-degree: 96%

---

# Actividad de la versión 2017.3 Beta 4

Esta página describe todos los cambios más recientes disponibles en el entorno de vista previa con la versión 2017.3 Beta 4. La funcionalidad de esta página se lanzó en el entorno de vista previa la semana del 25 de septiembre de 2017. Estuvo disponible en el entorno de producción a principios de noviembre de 2017.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en 2017.3, consulte [Información general de la actividad de la versión 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versión 2017.3 Beta 4 contiene mejoras para administradores de Workfront y otros usuarios:

**Para los administradores**

* [Nueva área de preferencias de administración de recursos en el área de configuración](#new-resource-management-preferences-area-in-the-setup-area)

**Para todos los usuarios**

* [Duplicar tareas](#duplicate-tasks)
* [Automatizar asignaciones al programar recursos](#automate-assignments-when-scheduling-resources)
* [Modificar asignaciones para varias tareas al programar recursos](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [Aplicar distribución de FTE al planificador de recursos](#apply-fte-distribution-to-the-resource-planner)
* [La sección de función para la configuración de usuario incluye el porcentaje de disponibilidad de FTE](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Guardar y administrar filtros en el informe de utilización de un proyecto](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Opciones de filtrado adicionales en el informe de utilización](#additional-filtering-options-in-the-utilization-report)
* [Ver el informe de utilización por programa o portafolio](#view-the-utilization-report-by-program-or-portfolio)
* [Mostrar información original del problema en los informes de proyectos y tareas](#show-original-issue-information-in-project-and-task-reports)
* [El sistema de filtrado de actualizaciones en el flujo de actualizaciones es ahora persistente entre objetos](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Informe sobre etapas de pruebas activas en Workfront](#report-on-active-proof-stages-within-workfront)
* [Asignar perfiles de permisos de Workfront Proof personalizados a usuarios de Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Recurso de hora añadido a suscripciones de evento](#hour-resource-added-to-event-subscriptions)

## Duplicar tareas {#duplicate-tasks}

Ahora puede duplicar rápidamente una tarea o un conjunto de tareas dentro de un proyecto. Esta acción crea una tarea idéntica a la original. No existen opciones adicionales durante el proceso de duplicación que le permitan realizar cambios en la tarea recién creada.  

Antes de este cambio, podía copiar una tarea en un proyecto nuevo o en el proyecto existente y modificar parte de la información a medida que la copiaba.

Para obtener más información sobre la duplicación de tareas, consulte [Copiar y duplicar tareas](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatizar asignaciones al programar recursos {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el distribuidor de cargas de trabajo, consulte [Información general del distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Ahora puede permitir que Workfront proponga automáticamente asignaciones para tareas y problemas sin asignar al programar recursos para varios proyectos (desde la pestaña Programación) o al programar recursos para un único proyecto (desde la pestaña Personal).

Workfront analiza las asignaciones de trabajo actuales de los usuarios disponibles y propone asignaciones lógicas e inteligentes para cualquier tarea o problema que aún no se haya asignado. Puede modificar las asignaciones propuestas o existentes antes de finalizar las asignaciones.

Para obtener más información, consulte “Asignar manualmente tareas y problemas no asignados en las áreas de programación”.

## Modificar asignaciones para varias tareas al programar recursos {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Al asignar, intercambiar o cancelar la asignación de usuarios por lotes al programar recursos (desde la pestaña Programación o la pestaña Personal), ahora puede modificar las asignaciones de tareas específicas que designe (incluidas todas las subtareas y problemas asociados) dentro de uno o más proyectos.

Antes de este cambio, solo podía modificar las asignaciones a tareas y problemas de proyectos completos (no podía designar tareas específicas dentro de un proyecto).

Para obtener más información, consulte “Asignar manualmente tareas y problemas no asignados en las áreas de programación”.

## Aplicar distribución de FTE al planificador de recursos {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Actualmente, esta funcionalidad no está disponible en la vista previa en todos los clústeres.

Ahora puede mostrar la cantidad correcta de horas disponibles para cada función del usuario en función del porcentaje de disponibilidad de FTE para cada función, cuando los usuarios tienen más de una función.

Por ejemplo, si la programación de un usuario indica que está disponible para trabajar 100 horas en un mes, y su porcentaje de disponibilidad de FTE para el rol principal es del 75 % y el porcentaje de disponibilidad de FTE de su otro rol es del 25 %, el planificador de recursos listará al usuario con 75 horas disponibles en la función principal y con 25 horas disponibles en su otra función.

Antes de este cambio, el nombre del usuario aparecía en el planificador de recursos solo para la función principal y la disponibilidad completa del usuario según su programación (100 horas) se asociaba únicamente a la función principal. La otra función del usuario solo se mostraba en el planificador de recursos si se había asignado a un usuario una tarea de esa función y las horas disponibles para el usuario de la otra función eran cero.

Para obtener más información acerca de cómo se calculan las horas disponibles y el FTE disponibles para los usuarios y las funciones en el planificador de recursos, consulte [Información general sobre el cálculo de horas y el FTE para los usuarios y las funciones en el planificador de recursos](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## La sección Función para la configuración de usuario incluye el porcentaje de disponibilidad de FTE {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Actualmente, esta funcionalidad no está disponible en la vista previa en todos los clústeres.

Ahora, al actualizar un perfil de usuario, puede añadir funciones de trabajo adicionales a un usuario y definir el porcentaje de FTE asignado a cada función.

Antes de este cambio, no se podía asignar una cantidad específica de FTE a ninguna de las funciones con las que estaba asociado el usuario.

Para obtener más información sobre cómo actualizar el porcentaje de disponibilidad de FTE para las funciones del usuario, consulte [Editar el perfil de un usuario](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) o [Establecer mi configuración](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Nueva área de preferencias de administración de recursos en el área de configuración {#new-resource-management-preferences-area-in-the-setup-area}

Ahora puede encontrar una nueva área en Configuración llamada Administración de recursos. En esta área, hemos introducido una configuración que le permite especificar cómo calcular la disponibilidad del usuario en el planificador de recursos. Se puede calcular mediante los métodos siguientes:

* De forma manual: se utiliza el horario predeterminado del sistema, además del valor de FTE individual del usuario, para determinar la disponibilidad horaria del usuario en el planificador de recursos. Se ignora la programación del usuario.
* Automáticamente: el Horario del usuario se utiliza para determinar la disponibilidad horaria del usuario en el Planificador de recursos. La disponibilidad de FTE se calcula según el Horario del usuario y el Horario predeterminado. Se ignora el valor de FTE del usuario. 

Para obtener más información acerca de cómo configurar las preferencias de Administración de recursos para su sistema, consulte [Configurar las preferencias de Administración de recursos](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Guardar y administrar filtros en el informe de utilización de un proyecto {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Ahora puede guardar los filtros que cree en el informe de utilización. Además, puede cambiar el nombre de un filtro guardado, duplicarlo, eliminarlo o modificarlo.

Anteriormente, había que especificar opciones de filtro individuales cada vez que se filtraba el informe de utilización.

Para obtener más información sobre cómo guardar y administrar filtros en el informe de utilización, consulte [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Opciones de filtrado adicionales en el informe de utilización {#additional-filtering-options-in-the-utilization-report}

Ahora, al ejecutar el informe Utilización, hay disponibles nuevos campos de filtrado para portafolios, programas y proyectos al crear el filtro, además de los campos Tareas, Problemas y Funciones disponibles previamente.

Antes de este cambio, solo podía filtrar por portafolio, programa y proyecto, añadiendo una nueva regla de filtro.

Para obtener más información, consulte [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Ver el informe de utilización por programa o portafolio {#view-the-utilization-report-by-program-or-portfolio}

Ahora puede visualizar un informe de utilización por programa o portafolio. Esto permite ver información de varios proyectos dentro de un solo informe de utilización.

Para facilitar este cambio, la pestaña Utilización está ahora disponible tanto en el área Informes dentro de Workfront, como dentro de un proyecto individual.

Antes de este cambio, solo se podía acceder a los informes de utilización dentro de un proyecto.

Para obtener más información, consulte [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Mostrar información del problema original en Informes de proyectos y tareas {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Actualmente, esta funcionalidad no está disponible en la vista previa en todos los clústeres.

Ahora puede encontrar la siguiente información sobre el problema original en un informe de proyecto o tarea para los proyectos y tareas que se crearon al convertir un problema:

* Fecha de entrada del problema original
* Nombre del problema original
* ID de generador de problema original

Esta información se puede mostrar en un informe o lista de tareas o proyectos creando una vista personalizada en modo de texto.

Antes de este cambio, no se podía informar sobre estos datos.

Para obtener más información acerca de cómo crear la vista de modo de texto personalizado que captura la información del problema original, vea [Ver: mostrar la información del problema original en las listas de tareas o proyectos](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Las actualizaciones del sistema de filtros en el flujo de actualizaciones ahora son persistentes entre objetos {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Esta funcionalidad no se lanzó en el entorno de vista previa con Beta 4. Estará disponible en Vista previa la primera quincena de octubre.

La opción Filtrar actualizaciones del sistema ahora es persistente entre objetos del sitio de Workfront. Esto le permite ocultar las actualizaciones del sistema y ver solamente los comentarios del usuario en el flujo de actualización de un objeto, así como mantener esa configuración mientras navega a otros objetos.

Antes de este cambio, tenía que filtrar las actualizaciones del sistema para cada objeto a medida que navegaba por el sitio de Workfront.

Para obtener más información, consulte [Actualizar trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Informe sobre etapas de prueba activas en Workfront {#report-on-active-proof-stages-within-workfront}

Al crear un informe de versión de documento en Workfront, ahora hay una columna llamada “Fases de revisión activas”. Esta columna le permite ver la fase de revisión que está activa actualmente en cada versión del documento del informe. El nombre de la fase se muestra en la columna “Fases de prueba activas”. Si actualmente no hay ninguna fase activa en el documento, la columna está en blanco.

Para obtener más información sobre los campos disponibles en vistas e informes, consulte [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Asignar perfiles de permisos de Workfront Proof personalizados a usuarios dentro de Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Ahora, al habilitar las capacidades de revisión para un usuario en Workfront, puede asignar un perfil de permiso de Workfront Proof personalizado. 

Antes de este cambio, solo estaban disponibles los siguientes perfiles de permiso: Supervisor, Responsable, Administrador.

## Recurso de hora añadido a suscripciones de evento {#hour-resource-added-to-event-subscriptions}

Con el nuevo recurso de hora, ahora puede crear una suscripción a evento para mantener la aplicación de facturación sincronizada con Workfront.

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción a eventos](../../../../wf-api/general/event-subs-api.md).
