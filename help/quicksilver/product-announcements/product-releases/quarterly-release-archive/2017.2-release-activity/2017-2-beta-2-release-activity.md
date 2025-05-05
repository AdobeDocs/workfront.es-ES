---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2 de Beta 2017.2
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2 de Beta 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Actividad de la versión 2 de Beta 2017.2

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2 de Beta 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para obtener una lista de todos los cambios realizados en 2017.2, consulte [Resumen de la actividad de la versión 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versión 2 de Beta 2017.2 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Mejora de API: Suscripciones de eventos](#api-enhancement-event-subscriptions)

**Para Todos Los Usuarios:**

* [Suscribirse a proyectos](#subscribe-to-projects)
* [Cancelar la suscripción a elementos del correo electrónico](#unsubscribe-from-items-from-email)
* [Configurar cómo se muestran los hitos en el gráfico Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Plantillas de conjuntos de recursos](#resource-pools-templates)
* [Ver versiones de documentos revisados en Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nuevo objeto de solicitante en informe de aprobación de pruebas](#new-requester-object-in-proof-approval-report)

## Mejora de API: Suscripciones de eventos {#api-enhancement-event-subscriptions}

Cuando se produce una acción en un objeto Workfront compatible con las suscripciones de evento, ahora puede configurar Workfront para que envíe una respuesta al extremo deseado. Esto significa que las integraciones pueden interactuar con la API de Workfront en tiempo real.

Para obtener más información, consulte [API de suscripción a evento](../../../../wf-api/general/event-subs-api.md). 

## Suscribirse a proyectos {#subscribe-to-projects}

Ahora puede suscribirse a nuevos comentarios sobre proyectos para los que no forma parte del equipo del proyecto. Antes de esta versión, solo podía suscribirse a comentarios sobre problemas y tareas.

Para obtener más información acerca de la suscripción a elementos, vea [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Cancelar suscripción a elementos del correo electrónico {#unsubscribe-from-items-from-email}

Puede cancelar la suscripción a elementos mediante el vínculo &quot;Cancelar la suscripción&quot; del correo electrónico de suscripción. Anteriormente, solo se podía cancelar la suscripción de un elemento desde la interfaz de Workfront.

Para obtener más información sobre cómo cancelar la suscripción a los correos electrónicos de suscripción, consulte la sección &quot;Exclusión de las notificaciones por correo electrónico&quot; en [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Configurar cómo se muestran los hitos en el gráfico Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORRECCIÓN &#x200B;**: esta característica no se encuentra actualmente en el entorno de vista previa de espacio aislado. Está planificado para su lanzamiento en una fecha posterior, durante el mes de junio de 2017.*

Ahora hay dos opciones para ver la información de los hitos en un gráfico Gantt. Puede configurar uno o ambos de los siguientes indicadores de hito:

* Diamantes de hito (icono)

  Este icono aparece en el diagrama de Gantt después de cualquier tarea asociada a un hito.

* Líneas de hito

  Se muestra una línea después de cualquier tarea asociada con el hito en todas las tareas del gráfico Gantt.

Antes de este cambio, solo había una opción para permitir que los hitos se mostraran en un gráfico Gantt, llamado &quot;hitos&quot;. Esta opción habilitó tanto el icono de diamante de hito como la línea de hito. Estos indicadores no se han podido separar. Las dos opciones ahora están disponibles en todos los gráficos Gantt, incluidas todas las listas de proyectos e informes. 

Para obtener más información acerca de cómo configurar cómo se muestra la información en el gráfico Gantt, vea [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Plantillas de conjuntos de recursos {#resource-pools-templates}

Ahora puede especificar conjuntos de recursos para las plantillas. Antes de esta versión, solo podía asociar conjuntos de recursos a usuarios y proyectos.

Para obtener más información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Ver versiones de documentos revisados en Workfront {#view-versions-of-proofed-documents-within-workfront}

Ahora puede ver las pruebas de todas las versiones de un documento revisado en la interfaz de Workfront. 

Antes de este cambio, solo se podía ver la última versión del documento revisado.

Los usuarios sin licencia de revisión pueden:

* Abrir una revisión en una versión anterior de un documento revisado

Los usuarios con una licencia de revisión pueden realizar cualquiera de las siguientes acciones:

* Abrir una revisión en una versión anterior de un documento revisado
* Ver los detalles de revisión de una versión anterior de un documento revisado

Para obtener más información, consulte [Administrar versiones de documentos](../../../../documents/managing-documents/manage-document-versions.md) en [Administrar versiones de documentos](../../../../documents/managing-documents/manage-document-versions.md).

## Nuevo objeto de solicitante en informe de aprobación de pruebas {#new-requester-object-in-proof-approval-report}

Ahora, al crear un informe de Aprobación de pruebas, hay un nuevo objeto Solicitante. Este objeto le permite informar sobre la información relativa al usuario que solicitó la aprobación de la prueba. 

El nuevo objeto Solicitante del informe de aprobación de pruebas contiene todos los campos disponibles con el objeto Usuario existente en otros tipos de informes de objetos.

>[!NOTE]
>
> Esta información solo está disponible en el informe desde el momento en que se introdujo esta función por primera vez en los entornos de Previsualización o Producción respectivos; la información de los informes relativa al objeto Solicitante antes de que se introdujera esta funcionalidad no está disponible.

Puede acceder al objeto Solicitante al crear un informe de Aprobación de pruebas, tal como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objetos de aprobaciones de pruebas, consulte la sección [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
