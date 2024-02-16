---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión beta 1 de 2018.1
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión beta 1 de 2018.1. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 1 de diciembre de 2017. Estará disponible en el entorno de producción en marzo de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Actividad de la versión beta 1 de 2018.1

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión beta 1 de 2018.1. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 1 de diciembre de 2017. Estará disponible en el entorno de producción en marzo de 2018.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2018.1, consulte  [información general sobre la actividad de la versión 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versión beta 1 de 2018.1 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores**

* [Plantilla de diseño actualizada para admitir el área de inicio](#updated-layout-template-to-support-the-home-area)
* [Deshabilitar la corrección de notificaciones por correo electrónico enviadas desde Workfront](#disable-proofing-email-notifications-sent-from-workfront)
* [Nuevos recursos añadidos a suscripciones a eventos](#new-resources-added-to-event-subscriptions)

**Para todos los usuarios**

* [Área de inicio (se ha actualizado mi área de trabajo)](#home-area-updated-my-work-area)
* [Mostrar datos del Planificador de recursos bajo el Caso comercial y el Resumen de caso comercial actualizado](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Mostrar el porcentaje de asignación de horas planificada en el planificador de recursos](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [El Déclencheur de actualización &quot;Automático y al cambiar&quot; y &quot;Solo cambiar&quot; actualiza los objetos principales al mismo tiempo que se actualizan las tareas](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Instantánea de cronología disponible en el gráfico Gantt](#timeline-snapshot-available-in-the-gantt-chart)

## Área de inicio (se ha actualizado mi área de trabajo) {#home-area-updated-my-work-area}

El nuevo área de Inicio proporciona una vista alternativa y mejorada de los mismos datos que están disponibles actualmente en el área de Mi trabajo. El área de Inicio proporciona los siguientes beneficios sobre el área de Mi trabajo:

* Una interfaz más ágil e intuitiva
* Rendimiento mejorado
* Actualizar tareas y problemas con formato de texto enriquecido

## Plantilla de diseño actualizada para admitir el área de inicio {#updated-layout-template-to-support-the-home-area}

Como administrador de Workfront, puede determinar si los usuarios de su organización tienen acceso al área de Inicio configurando la plantilla de diseño a la que están asignados. Los usuarios que no tengan asignada una plantilla de diseño siempre pueden acceder al área de Inicio.

Para obtener más información, consulte &quot;Creación y administración de plantillas de diseño&quot;.

## Deshabilitar la corrección de notificaciones por correo electrónico enviadas desde Workfront {#disable-proofing-email-notifications-sent-from-workfront}

Ahora puede configurar si los usuarios de la instancia de Workfront recibirán notificaciones por correo electrónico de Workfront cuando se realice un comentario en una prueba.

Anteriormente, los correos electrónicos de prueba siempre se enviaban desde Workfront cuando se realizaba un comentario sobre una prueba. Si las notificaciones también estaban habilitadas en Workfront Proof, los usuarios recibían notificaciones duplicadas. 

Para los clientes de Workfront existentes, Workfront está configurado de forma predeterminada para enviar correos electrónicos cuando se realiza un comentario sobre una prueba.

Para obtener información sobre cómo deshabilitar las notificaciones por correo electrónico para pruebas en Workfront de modo que los correos electrónicos de prueba se envíen únicamente desde Workfront Proof, consulte  

## Mostrar datos del Planificador de recursos bajo el Caso comercial y el Resumen de caso comercial actualizado {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

El área de Presupuestación de recursos ahora está disponible en el caso comercial de un proyecto. En esta área, puede revisar las horas presupuestadas estimadas de sus recursos en el Planificador de recursos y el costo de mano de obra presupuestado asociado con ellos.

Se ha cambiado el nombre del área Estimaciones de recursos del caso empresarial a Estimaciones de recursos de legado.

Como parte de este cambio, el Resumen de caso comercial ahora incluye información financiera basada en las Estimaciones de recursos y el Presupuesto de recursos.

Antes de este cambio, no podía ver la información del Planificador de recursos en el Caso comercial del proyecto. Solo podía ver la información de Estimaciones de recursos que se especifica en el Planificador de capacidades de los conjuntos de recursos de legado.

Para obtener más información sobre la creación de un caso empresarial, consulte [Crear un caso comercial para un proyecto](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Mostrar el porcentaje de asignación de horas planificada en el planificador de recursos {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

La Vista de usuario del Planificador de recursos ahora incluye una nueva columna que le permite ver la Asignación de horas planificada como un porcentaje del total de horas disponibles para el usuario y el rol.

Antes de este cambio, podía ver el total de horas planificadas y disponibles para los usuarios y los roles de trabajo solo en columnas independientes.

Para obtener más información sobre la columna Porcentaje de asignación de horas planificadas, consulte la sección &quot;Visualización de la diferencia entre las horas disponibles y planificadas o FTE en el Planificador de recursos&quot; en [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## El Déclencheur de actualización &quot;Automático y al cambiar&quot; y &quot;Solo cambiar&quot; actualiza los objetos principales al mismo tiempo que se actualizan las tareas {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Hemos cambiado la forma en que se actualizan las tareas principales y el proyecto cuando se actualiza un objeto de nivel inferior en un proyecto. La hora a la que se actualiza un objeto principal viene determinada por el campo Tipo de actualización de un proyecto. Puede seleccionar entre los siguientes tipos de actualización:

* Automático y al cambiar
* Solo al cambiar
* Solo automático
* Solo manual

Ahora, al seleccionar los tipos de actualización &quot;Automático y al cambiar&quot; o &quot;Solo cambiar&quot;, los cambios que aplique a las tareas individuales también se aplican a la tarea principal y al proyecto inmediatamente.

Antes de este cambio, tenía que actualizar la página para asegurarse de que los objetos principales y la cronología del proyecto también se actualizaran.

Para obtener más información sobre el tipo de actualización de un proyecto, consulte [Seleccione el tipo de actualización del proyecto](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Instantánea de cronología disponible en el gráfico Gantt {#timeline-snapshot-available-in-the-gantt-chart}

Ahora puede desplazarse rápidamente a un determinado punto de la duración de un proyecto utilizando la nueva instantánea de escala de tiempo del gráfico Gantt.

Al seleccionar un lapso de tiempo más granular para el gráfico Gantt mientras ve una tarea o una lista de proyectos, se muestra una barra de desplazamiento horizontal en la parte inferior del gráfico Gantt. Al hacer clic en la barra de desplazamiento, puede ver toda la cronología del proyecto en una instantánea. Puede hacer clic en cualquier lugar dentro de la instantánea del gráfico Gantt para desplazarse a un punto específico de la duración del proyecto.

Antes de este cambio, tenía que desplazarse horizontalmente por todo el diagrama de Gantt para encontrar un determinado punto en el tiempo o tenía que alejarse de la vista granular.

Para obtener más información sobre cómo se muestra la información en el diagrama de Gantt, consulte [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Nuevos recursos añadidos a suscripciones a eventos {#new-resources-added-to-event-subscriptions}

Ahora puede crear suscripciones de eventos para los siguientes recursos:

* **Gasto:** Le avisa cuando se agrega o modifica un gasto.
* **Asignación:** Le avisa cuando se agrega o modifica una asignación en una tarea o problema de un usuario, rol o equipo.
* **Hoja de horas:** Le avisa cuando se envía, rechaza o aprueba una plantilla de horas.

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción de evento](../../../../wf-api/general/event-subs-api.md).
