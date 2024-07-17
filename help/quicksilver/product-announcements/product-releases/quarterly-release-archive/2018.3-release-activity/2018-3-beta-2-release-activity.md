---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2 de Beta 2018.3
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2 de Beta 2018.3. La funcionalidad estará disponible en el entorno de vista previa el 1 de agosto de 2018. Las mejoras de revisión incluidas en Beta 2 estarán disponibles en el entorno de vista previa el miércoles 18 de julio. Estará disponible en el entorno de producción en noviembre de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Actividad de la versión 2 de Beta 2018.3

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2 de Beta 2018.3. La funcionalidad estará disponible en el entorno de vista previa el 1 de agosto de 2018. Las mejoras de revisión incluidas en Beta 2 estarán disponibles en el entorno de vista previa el miércoles 18 de julio. Estará disponible en el entorno de producción en noviembre de 2018.

>[!NOTE]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2018.3, consulte  [resumen de la actividad de la versión 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

La versión 2 de Beta 2018.3 contiene mejoras para administradores de Workfront y otros usuarios:

**Para Administradores**

* [Actualizar la dirección de correo electrónico en el perfil de usuario como administrador de grupo](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Para Todos Los Usuarios**

* [Ver aprobaciones delegadas a mí en el área de inicio](#view-approvals-delegated-to-me-in-the-home-area)
* [Exportar datos de un período determinado en el Planificador de recursos](#export-data-for-a-given-period-in-the-resource-planner)
* [Los totales diarios ahora se muestran en rojo cuando el usuario está sobreasignado](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Las tareas y los problemas están ocultos en la escala de tiempo de programación al minimizarse](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtrar comentarios y respuestas por usuario en el visor de revisión](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Comentario sobre un rango de material de archivo en una prueba de vídeo](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nueva herramienta de polilínea para la marca de comentarios en el visor de revisión](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Eliminación de Flashes para compartir informes, calendarios y documentos](#flash-removal-for-report-calendar-and-document-sharing)

## Actualizar la dirección de correo electrónico en el perfil de usuario como administrador de grupo {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Ahora puede actualizar las direcciones de correo electrónico de los usuarios que pertenecen a un grupo que usted administra. 

Anteriormente, solo los administradores de Workfront podían actualizar las direcciones de correo electrónico de otros usuarios. 

Para obtener más información, consulte [Administradores de grupo](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Ver aprobaciones delegadas en mí en el área de inicio {#view-approvals-delegated-to-me-in-the-home-area}

Ahora puede usar el área de Inicio para ver las aprobaciones de proyectos, tareas y problemas que se le han delegado.

Antes de este cambio, solo podía ver las aprobaciones delegadas en el área Mi trabajo.

Para obtener más información, consulte [Delegar solicitud de aprobación](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exportar datos de un período determinado en el Planificador de recursos {#export-data-for-a-given-period-in-the-resource-planner}

Ahora se muestra una nueva ventana al exportar la información en el Planificador de recursos, que le permite seleccionar un intervalo de tiempo específico para el archivo exportado.

Antes de esta mejora, solo se podía exportar la información mostrada en la pantalla.

Para obtener más información sobre cómo exportar datos desde el Planificador de recursos, consulte [Resumen de navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) en el artículo [Resumen de navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Los totales diarios ahora se muestran en rojo cuando el usuario está sobreasignado {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Cuando un usuario está sobreasignado, los totales diarios de los días en que el usuario está sobreasignado ahora se muestran en rojo. Esta opción solo se muestra cuando la opción Mostrar los totales de horas planificadas diariamente está habilitada en la configuración de la escala de tiempo de la programación. Antes de esta mejora, había un indicador de barra rojo para los días en que el usuario estaba sobreasignado, pero los totales diarios se mostraban sin un resaltado rojo.

Para obtener más información sobre las asignaciones de usuarios, consulte &quot;Administrar asignaciones de usuarios en las áreas de programación&quot;.

## Las tareas y los problemas se ocultan en la cronología de programación cuando se minimizan {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Cuando se minimizan las tareas y los problemas de la escala de tiempo de la programación, ahora se ocultan para los usuarios y las funciones si la opción Mostrar totales de horas planificadas diariamente está activada en la configuración. Las tareas y los problemas del área Sin asignar se muestran en una vista comprimida.

Anteriormente, al minimizar las tareas y los problemas, permanecían en la cronología de programación para los usuarios y las funciones, pero se mostraban en una vista comprimida.

Para obtener más información sobre cómo minimizar las tareas y los problemas en la escala de tiempo de la programación, consulte  &quot;Introducción a la programación de recursos&quot;.

## Filtrar comentarios y respuestas por usuario en el visor de pruebas {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Ahora puede incluir respuestas al filtrar los comentarios realizados por los usuarios especificados. Esto resulta útil cuando desea centrarse en todos los comentarios realizados por un revisor importante, como un cliente o un jefe de proyecto.

Anteriormente, el filtrado por usuario se limitaba únicamente a los comentarios creados (iniciados) por los revisores especificados.

## Comentario sobre un rango de material de archivo en una prueba de vídeo {#comment-on-a-range-of-footage-in-a-video-proof}

Puede crear un comentario para un rango de material de archivo en una prueba de vídeo. Esto resulta útil, por ejemplo, cuando necesita indicar que es necesario volver a grabar o quitar un segmento de material de archivo.

Anteriormente, solo se podía crear un comentario para un único punto de una cronología de vídeo.

## Nueva herramienta Polilínea para marcado de comentarios en el visor de revisiones {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Ahora puede utilizar el marcado de polilíneas para dibujar líneas segmentadas y formas al agregar un comentario a una prueba. Puede crear una línea segmentada abierta o una forma cerrada. Esta herramienta es especialmente útil cuando se trabaja con imágenes complejas, como imágenes técnicas o arquitectónicas.

Anteriormente, al marcar una prueba para agregar un comentario, se podía dibujar un rectángulo, una línea recta, una línea o forma a mano alzada o una flecha.

## Eliminación de Flashes para compartir informes, calendarios y documentos {#flash-removal-for-report-calendar-and-document-sharing}

Se ha eliminado el Flash de los siguientes cuadros de diálogo de uso compartido en Workfront:

* Informes
* Calendarios
* Documentos

Puede compartir estos objetos como lo hizo anteriormente, pero ahora la experiencia ya no depende del Flash.
