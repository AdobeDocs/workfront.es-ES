---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2018.3 de Beta 2
description: En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.3 de Beta 2. La funcionalidad estará disponible en el entorno de vista previa el 1 de agosto de 2018. Las mejoras de revisión incluidas en Beta 2 estarán disponibles en el entorno de vista previa el miércoles 18 de julio. Está disponible en el entorno de producción desde noviembre de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
TQID: https://experienceleague.adobe.com/2VzVuejEi80fNoxQ2KRGdLbDbiIX-7z4b5P33o-3N8s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 913
ht-degree: 100%

---

# Actividad de la versión 2018.3 de Beta 2

En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.3 de Beta 2. La funcionalidad estará disponible en el entorno de vista previa el 1 de agosto de 2018. Las mejoras de revisión incluidas en Beta 2 estarán disponibles en el entorno de vista previa el miércoles 18 de julio. Está disponible en el entorno de producción desde noviembre de 2018.

>[!NOTE]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en 2018.3, consulte  [Información general de la actividad de la versión 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

La versión 2018.3 de Beta 2 contiene mejoras para administradores de Workfront y otros usuarios:

**Para los administradores**

* [Actualizar la dirección de correo electrónico en el perfil de usuario como administrador de grupos](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Para todos los usuarios**

* [Ver las aprobaciones que me han delegado en el área de inicio](#view-approvals-delegated-to-me-in-the-home-area)
* [Exportar datos de un periodo determinado en el Planificador de recursos](#export-data-for-a-given-period-in-the-resource-planner)
* [Los totales diarios ahora se muestran en rojo cuando el usuario tiene asignaciones excesivas](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Las tareas y los problemas quedan ocultos en la cronología de programación cuando se han minimizado](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtrar comentarios y respuestas por usuario en el visualizador de revisión](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Comentario sobre un rango de material de archivo en una prueba de vídeo](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nueva herramienta de polilínea para el marcado de comentarios en el visualizador de revisión](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Eliminación de Flash para compartir informes, calendarios y documentos](#flash-removal-for-report-calendar-and-document-sharing)

## Actualizar la dirección de correo electrónico en el perfil de usuario como administrador de grupos {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Ahora puede actualizar las direcciones de correo electrónico de los usuarios que pertenecen a un grupo que usted administra. 

Anteriormente, solo los administradores de Workfront podían actualizar las direcciones de correo electrónico de otros usuarios. 

Para obtener más información, consulte [Administradores de grupos](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Ver las aprobaciones que me han delegado en el área de inicio {#view-approvals-delegated-to-me-in-the-home-area}

Ahora puede usar el área de Inicio para ver las aprobaciones de proyectos, tareas y problemas que han delegado en usted.

Antes de este cambio, solo podía ver las aprobaciones delegadas en el área Mi trabajo.

Para obtener más información, consulte [Delegar solicitud de aprobación](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exportar datos de un periodo determinado en el Planificador de recursos {#export-data-for-a-given-period-in-the-resource-planner}

Ahora se muestra una nueva ventana al exportar la información en el Planificador de recursos, lo que le permite seleccionar un periodo de tiempo específico para el archivo exportado.

Antes de esta mejora, solo se podía exportar la información mostrada en la pantalla.

Para obtener más información sobre cómo exportar datos desde el Planificador de recursos, consulte [Información general de navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) en el artículo [Información general de navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Los totales diarios ahora se muestran en rojo cuando el usuario tiene asignaciones excesivas {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el equilibrador de carga de trabajo, consulte [Información general del equilibrador de carga de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Cuando un usuario tiene asignaciones excesivas, los totales diarios de los días en que el usuario tiene demasiadas asignaciones ahora se muestran en rojo. Esta opción solo se muestra cuando la opción Mostrar los totales de horas planificadas diariamente está habilitada en la configuración de la cronología de programación. Antes de esta mejora, había un indicador de barra rojo para los días en que el usuario tenía demasiadas asignaciones, pero los totales diarios se mostraban sin el resaltado en rojo.

Para obtener más información sobre las asignaciones de un usuario, consulte “Administrar asignaciones de usuarios en las áreas de programación”.

## Las tareas y los problemas quedan ocultos en la cronología de programación cuando se han minimizado {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Cuando se minimizan las tareas y los problemas en la cronología de programación, ahora quedan ocultos para los usuarios y las funciones si la opción Mostrar totales de horas planificadas diariamente está habilitada en la configuración. Las tareas y los problemas del área Sin asignar se muestran en una vista comprimida.

Anteriormente, al minimizar las tareas y los problemas, ambos permanecían en la cronología de programación para los usuarios y las funciones, pero se mostraban en una vista comprimida.

Para obtener más información sobre cómo minimizar las tareas y los problemas en la cronología de programación, consulte “Introducción a la programación de recursos”.

## Filtrar comentarios y respuestas por usuario en el visor de corrección {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Ahora puede incluir respuestas al filtrar los comentarios realizados por los usuarios especificados. Esto resulta útil cuando desea centrarse en todos los comentarios realizados por un revisor importante, como un cliente o un administrador de proyectos.

Anteriormente, el filtrado por usuario se limitaba únicamente a los comentarios creados (iniciados) por los revisores especificados.

## Comentario sobre un rango de material de archivo en una prueba de vídeo {#comment-on-a-range-of-footage-in-a-video-proof}

Puede crear un comentario para un intervalo de material de archivo en una prueba de vídeo. Esto resulta útil, por ejemplo, cuando necesita indicar que es necesario volver a grabar o eliminar un segmento de material de archivo.

Anteriormente, solo se podía crear un comentario para un único punto de una cronología de vídeo.

## Nueva herramienta Polilínea para marcado de comentarios en el visor de corrección {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Ahora puede utilizar el marcado de polilíneas para dibujar líneas segmentadas y formas al añadir un comentario a una prueba. Puede crear una línea segmentada abierta o una forma cerrada. Esta herramienta es especialmente útil cuando se trabaja con imágenes complejas, como imágenes técnicas o arquitectónicas.

Anteriormente, al marcar una revisión para añadir un comentario, se podía dibujar un rectángulo, una línea recta, una línea o forma a mano alzada o una flecha.

## Eliminación de Flash para compartir informes, calendarios y documentos {#flash-removal-for-report-calendar-and-document-sharing}

Se ha eliminado Flash de los siguientes cuadros de diálogo de uso compartido en Workfront:

* Informes
* Calendarios
* Documentos

Puede compartir estos objetos como lo hizo anteriormente, pero ahora la experiencia ya no depende de Flash.
