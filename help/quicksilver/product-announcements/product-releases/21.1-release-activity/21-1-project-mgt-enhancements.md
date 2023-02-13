---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: product-releases
title: 21.1 Mejoras en la gestión de proyectos
description: En esta página se describen todas las mejoras de Administración de proyectos realizadas con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 15 de febrero de 2021.
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 1%

---

# 21.1 Mejoras en la gestión de proyectos

En esta página se describen todas las mejoras de Administración de proyectos realizadas con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 15 de febrero de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.1, consulte [Información general sobre la versión 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Exportar ahora disponible en la sección Métricas de un proyecto

Para compartir con mayor facilidad el estado y el progreso de un proyecto, ahora puede exportar todo el panel de la sección Métricas de un proyecto a un archivo .png .

Para obtener más información, consulte [Resumen de las métricas del proyecto](../../../manage-work/projects/manage-projects/project-metrics.md).

Esta función ahora se incluye en la función [Aspectos básicos del planificador para la nueva experiencia de Workfront, parte 3: Administrar un proyecto](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) ruta de aprendizaje en Workfront One.

## Actualización del porcentaje de problema completado cuando el proyecto o la tarea se convierten desde la actualización del problema

Hemos actualizado la forma en que el porcentaje de problemas completos funciona para los problemas que se han convertido en proyectos o tareas. Con la nueva funcionalidad, cuando un problema se convierte en una tarea o un proyecto, el porcentaje completado del problema se actualiza en sincronía con el porcentaje completado de la tarea o proyecto en resolución cuando el estado &quot;Actualizar automáticamente el problema resuelto cuando cambia el estado del objeto en resolución&quot; está habilitado desde la configuración.

Para obtener información sobre la conversión de problemas, consulte [Información general sobre la resolución y resolución de objetos](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Nueva lista de solicitudes enviadas

Para permitirle administrar sus solicitudes enviadas de una manera más fácil y coherente, hemos eliminado las secciones Solicitudes que he enviado y Todas las solicitudes del área Solicitudes y las hemos sustituido por una nueva lista Enviado. La lista tiene un aspecto familiar que coincide con todas las demás listas del sistema, lo que le permite filtrar por diferentes categorías de solicitudes enviadas y buscar rápidamente una solicitud que pueda ser difícil de encontrar.

Para obtener información sobre cómo localizar las solicitudes enviadas, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Esta función ahora se incluye en la función [Aspectos básicos del colaborador para la nueva experiencia de Workfront](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) ruta de aprendizaje en Workfront One.

Esta función ahora se incluye en la función [Solicitudes en la nueva experiencia de Workfront](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) ruta de aprendizaje en Workfront One.

## Campos eliminados de la página Nueva solicitud

>[!NOTE]
>
>Eliminado de la versión.

Como parte del rediseño de la página Nueva solicitud, hemos actualizado los campos de nuevo problema que se configuran en la sección Configuración de cola de un proyecto.

Los siguientes campos de problema nuevo solo se muestran al crear un problema desde la sección Problemas del proyecto. No se muestran al enviar un problema mediante una cola de solicitudes en el área Solicitudes :

* Gravedad
* Horas planificadas
* Fecha planificada de inicio
* Dirección URL
* Asignado a
* Función
* Equipo

Hemos reemplazado los campos Asignado a, Función de trabajo y Equipo con el nuevo campo Asignaciones en la página Nueva solicitud para designar de forma eficaz un usuario, función de trabajo o equipo en un campo común a medida que envía una nueva solicitud.

Para obtener información sobre la definición de nuevos campos de problema para un proyecto, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Nueva experiencia al enviar solicitudes en el área Solicitudes

>[!NOTE]
>
>Eliminado de la versión; permanecerá en Vista previa y se lanzará a Producción con 21.2.

Para mantener la coherencia con la nueva experiencia de Workfront y crear eficacia al enviar solicitudes, hemos rediseñado el cuadro Nueva solicitud del área Solicitudes . Las siguientes son algunas de las mejoras:

* Una interfaz de usuario coherente con el resto de la nueva experiencia de Workfront
* Se ha eliminado el área Nuevas solicitudes para una experiencia más fácil e intuitiva
* Una forma nueva y más eficaz de adjuntar documentos a sus solicitudes

Capacidad para compartir un vínculo a la cola de solicitudes, al grupo de temas o a los temas de la cola cuando se introduce la solicitud.

Para obtener información sobre el envío de solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Compartir un vínculo a una cola de solicitudes al enviar una solicitud

>[!NOTE]
>
>Eliminado de la versión; permanecerá en Vista previa y se lanzará a Producción con 21.2.

Ahora hemos hecho posible compartir un vínculo a una cola de solicitudes, un grupo de temas o un tema de cola. Al crear una solicitud.

Antes de enviar una nueva solicitud, puede copiar un vínculo a la cola de solicitudes, al grupo de temas o al tema de la cola de solicitudes y compartirlo con otros usuarios, o bien incrustarlo en un panel.

Para obtener información sobre cómo compartir un vínculo a una cola de solicitudes al enviar una solicitud, consulte [Compartir un vínculo a una cola de solicitudes](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Busque el grupo que desee asignar a un proyecto y vea sus detalles

Ahora es más fácil asegurarse de identificar el grupo correcto cuando asigna un grupo a un proyecto. Pase el ratón sobre el nombre de un grupo que encuentre en el cuadro Grupo y, a continuación, haga clic en el icono de información que aparece junto al nombre para ver la información de objeto Detalles del grupo .

Esta información sobre herramientas incluye la jerarquía de grupos por encima del grupo, si los hay, y los administradores del grupo.

Según los detalles configurados para el grupo, también puede ver el encabezado comercial y la descripción del grupo.

Con esta información, puede estar seguro de que está seleccionando el grupo adecuado para asignarlo al proyecto.

Para obtener más información, consulte [Administrar información en el área Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Nuevo informe de Delegación de usuarios

Anteriormente, el delegado solo podía ver la información para las delegaciones de aprobación de tareas, problemas y proyectos en su área de inicio. Para permitir que otros usuarios vean esta información, los usuarios del plan ahora pueden crear el informe Delegación de usuarios , que le dice:

* Quién ha delegado estas aprobaciones a otro usuario
* Qué usuario ha delegado estas aprobaciones
* Fecha de inicio y finalización de esas delegaciones

Para obtener más información, consulte [Creación de un informe de delegación de usuarios](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
