---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.2 beta 2
description: En esta página se describen todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
TQID: https://experienceleague.adobe.com/DMqQO0ANmU91bTeg5IYpb0XnfhmcpaqSWFc9b3jcdpM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 95%

---

# Actividad de la versión 2017.2 beta 2

En esta página se describen todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para obtener una lista de todos los cambios realizados en la versión 2017.2, consulte [Información general sobre la actividad de la versión 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versión 2017.2 Beta 2 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Mejora de la API: suscripciones a eventos](#api-enhancement-event-subscriptions)

**Para todos los usuarios:**

* [Suscribirse a proyectos](#subscribe-to-projects)
* [Cancelar la suscripción a elementos desde el correo electrónico](#unsubscribe-from-items-from-email)
* [Configurar cómo se muestran los hitos en el gráfico Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Plantillas de conjuntos de recursos](#resource-pools-templates)
* [Ver versiones de documentos revisados en Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nuevo objeto de solicitante en informe de aprobación de revisión](#new-requester-object-in-proof-approval-report)

## Mejora de la API: suscripciones a eventos {#api-enhancement-event-subscriptions}

Cuando se produce una acción en un objeto Workfront compatible con las suscripciones a eventos, ahora puede configurar Workfront para que envíe una respuesta al punto final deseado. Esto significa que las integraciones pueden interactuar con la API de Workfront en tiempo real.

Para obtener más información, consulte [API de suscripción a eventos](../../../../wf-api/general/event-subs-api.md). 

## Suscribirse a proyectos {#subscribe-to-projects}

Ahora puede suscribirse a nuevos comentarios sobre proyectos de los que no forme parte del equipo. Antes de esta versión, solo podía suscribirse a comentarios sobre problemas y tareas.

Para obtener más información acerca de la suscripción a elementos, consulte [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Cancelar suscripción a elementos desde el correo electrónico {#unsubscribe-from-items-from-email}

Puede cancelar la suscripción a elementos mediante el vínculo “Cancelar la suscripción” del correo electrónico de suscripción. Anteriormente, solo se podía cancelar la suscripción de un elemento desde la interfaz de Workfront.

Para obtener más información sobre cómo darse de baja de los correos electrónicos de suscripción, consulte la sección &quot;Cómo darse de baja de las notificaciones por correo electrónico&quot; en [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Configuración de la vista de los hitos en el gráfico Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORRECCIÓN &#x200B;**: esta característica no se encuentra actualmente en el entorno de vista previa de zona protegida. Su lanzamiento está previsto para una fecha posterior, durante el mes de junio de 2017.*

Ahora dispone de dos opciones para ver la información de los hitos en un gráfico Gantt. Puede configurar uno de los siguientes indicadores de hito o ambos:

* Diamantes de hito (icono)

  Este icono aparece en el gráfico Gantt después de cualquier tarea asociada a un hito.

* Líneas de hito

  Se muestra una línea después de cualquier tarea asociada con el hito en todas las tareas del gráfico Gantt.

Antes de este cambio, solo había una opción para permitir que los hitos se mostraran en un gráfico Gantt, llamado &quot;hitos&quot;. Esta opción habilitó tanto el icono de diamante de hito como la línea de hito. Estos indicadores no se han podido separar. Las dos opciones ahora están disponibles en todos los gráficos Gantt, incluidas todas las listas de proyectos e informes. 

Para obtener más información sobre la configuración de cómo se muestra la información en el gráfico Gantt, consulte [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Plantillas de conjuntos de recursos {#resource-pools-templates}

Ahora puede especificar conjuntos de recursos para las plantillas. Antes de esta versión, solo podía asociar conjuntos de recursos a usuarios y proyectos.

Para obtener más información acerca de los conjuntos de recursos, consulte [Información general sobre los conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Ver versiones de documentos revisados en Workfront {#view-versions-of-proofed-documents-within-workfront}

Ahora puede ver las pruebas de todas las versiones de un documento revisado en la interfaz de Workfront. 

Antes de este cambio, solo se podía ver la última versión del documento revisado.

Los usuarios sin licencia de revisión pueden:

* Abrir una prueba de una versión anterior de un documento revisado

Los usuarios con licencia de revisión pueden realizar cualquiera de las siguientes acciones:

* Abrir una prueba de una versión anterior de un documento revisado
* Ver los detalles de la prueba de una versión anterior de un documento revisado

Para obtener más información, consulte [Administrar versiones de documentos](../../../../documents/managing-documents/manage-document-versions.md) en [Administrar versiones de documentos](../../../../documents/managing-documents/manage-document-versions.md).

## Nuevo objeto de solicitante en informe de aprobación de revisión {#new-requester-object-in-proof-approval-report}

Ahora, al crear un informe de Aprobación de pruebas, hay un nuevo objeto Solicitante. Este objeto le permite informar sobre la información relativa al usuario que solicitó la aprobación de la prueba. 

El nuevo objeto Solicitante del informe de aprobación de revisión contiene todos los campos disponibles con el objeto Usuario existente en otros tipos de informes de objetos.

>[!NOTE]
>
> Esta información solo está disponible en el informe desde el momento en que se introdujo esta función por primera vez en los entornos de vista previa o producción correspondientes; la información de los informes relativa al objeto Solicitante antes de que se introdujera esta funcionalidad no está disponible.

Puede acceder al objeto Solicitante cuando crea un informe de aprobación de revisión, tal como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objetos de aprobaciones de revisión, consulte la sección [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
