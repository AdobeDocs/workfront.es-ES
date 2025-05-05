---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: product-releases
title: 21.1 Mejoras en la administración de proyectos
description: En esta página se describen todas las mejoras realizadas en la Administración de proyectos con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción la semana del 15 de febrero de 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 99%

---

# 21.1 Mejoras en la administración de proyectos

En esta página se describen todas las mejoras realizadas en la Administración de proyectos con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción la semana del 15 de febrero de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.1, consulte [Información general sobre la versión 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## La exportación ya está disponible en la sección de Métricas de un proyecto

Para compartir más fácilmente el estado y el progreso de un proyecto, ahora puede exportar todo el tablero de la sección Métricas de un proyecto a un archivo .png.

Para obtener más información, consulte [Información general de las métricas del proyecto](../../../manage-work/projects/manage-projects/project-metrics.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del planificador para la nueva experiencia de Workfront, Parte 3: Administrar un proyecto](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/home) en Workfront One.

## Actualizar el porcentaje completado del problema cuando el proyecto o la tarea se convirtieron a partir de la actualización del problema

Hemos actualizado el modo en que funciona el porcentaje completado de los problemas para los problemas que se han convertido en proyectos o tareas. Con la nueva funcionalidad, cuando un problema se convierte en una tarea o un proyecto, el porcentaje completado del problema se actualiza de forma sincronizada con el porcentaje completado de la tarea o el proyecto de resolución cuando la configuración “Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución” está habilitada desde la configuración.

Para obtener información acerca de la conversión de problemas, consulte [Información general sobre los objetos de resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md). 

## Nueva lista de solicitudes enviadas

Para permitirle administrar sus Solicitudes enviadas de una manera más fácil y coherente, hemos eliminado las secciones Solicitudes que he enviado y Todas las solicitudes en el área Solicitudes y las hemos sustituido por una nueva lista de enviadas. La lista tiene una apariencia familiar que coincide con todas las demás listas del sistema, lo que le permite filtrar por diferentes categorías de solicitudes enviadas y buscar rápidamente una solicitud que pueda ser difícil de encontrar.

Para obtener información sobre cómo localizar las solicitudes enviadas, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Esta característica ahora se incluye en [Aspectos básicos de colaborador para la nueva ruta de aprendizaje de Workfront Experience](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request) en Workfront One.

Esta característica ahora se incluye en [Solicitudes en la nueva ruta de aprendizaje de la experiencia Workfront](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/understand-request-queues) en Workfront One.

## Campos eliminados de la página Nueva solicitud

>[!NOTE]
>
>Se ha eliminado de la versión.

Como parte del rediseño de la página Nueva solicitud, se han actualizado los campos Nuevo problema que se configuran en la sección Configuración de cola de un proyecto.

Los siguientes Campos de nuevos problemas solo se muestran al crear un problema desde la sección Problemas del proyecto. No se muestran al enviar un problema mediante una cola de solicitudes en el área Solicitudes:

* Gravedad
* Horas planificadas
* Fecha planificada de inicio
* URL
* Asignado a
* Función
* Equipo

Hemos reemplazado los campos Asignado a, Función y Equipo por el nuevo campo Asignaciones en la página Nueva solicitud para designar de forma eficaz un usuario, función o equipo en un campo común al enviar una nueva solicitud.

Para obtener información acerca de cómo definir nuevos campos de problema para un proyecto, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Nueva experiencia al enviar solicitudes en el área de solicitudes

>[!NOTE]
>
>Se ha eliminado de la versión; permanecerá en la versión preliminar y se lanzará al entorno de producción con 21.2.

Para mantener la coherencia con la nueva experiencia de Workfront y aumentar la eficacia al enviar solicitudes, hemos rediseñado el cuadro Nueva solicitud en el área Solicitudes. A continuación se indican algunas de las mejoras:

* Una interfaz de usuario coherente con el resto de la nueva experiencia de Workfront
* Se ha eliminado el área Nuevas solicitudes para ofrecer una experiencia más fácil e intuitiva
* Una forma nueva y más eficaz de adjuntar documentos a sus solicitudes

Posibilidad de compartir un vínculo a la cola de solicitudes, al grupo de temas o al tema de la cola al introducir la solicitud.

Para obtener información sobre cómo enviar solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Compartir un vínculo a una cola de solicitudes al enviar una solicitud

>[!NOTE]
>
>Se ha eliminado de la versión; permanecerá en la versión preliminar y se lanzará al entorno de producción con 21.2.

Ahora, es posible compartir un vínculo a una cola de solicitudes, a un grupo de temas o a un tema de la cola cuando se crea una solicitud.

Antes de enviar una nueva solicitud, puede copiar un vínculo a la cola de solicitudes, al grupo de temas o al tema de la cola de la solicitud y compartirlo con otros usuarios, o incrustarlo en un panel.

Para obtener información sobre cómo compartir un vínculo a una cola de solicitudes al enviar una solicitud, consulte [Compartir un vínculo a una cola de solicitudes](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Busque un grupo que desee asignar a un proyecto y vea sus detalles

Ahora es más fácil asegurarse de identificar el grupo correcto al asignar un grupo a un proyecto. Pase el ratón sobre el nombre de un grupo que encuentre en el cuadro Grupo y, a continuación, haga clic en el icono de información que aparece junto al nombre para ver la información sobre el grupo.

Esta información sobre herramientas incluye la jerarquía de grupos por encima del grupo, si los hay, y los administradores del grupo.

Según los detalles configurados para el grupo, también puede ver el coordinador empresarial y la descripción del grupo.

Con esta información, puede estar seguro de que está seleccionando el grupo correcto para asignarlo al proyecto.

Para obtener más información, consulte [Administrar información en el área Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Nuevo informe de delegación de usuario

Con anterioridad, la información sobre las delegaciones de tareas, problemas y aprobaciones de proyectos solo la podían ver el delegado en el área de Inicio. Para permitir que otros usuarios vean esta información, los usuarios de Plan ahora pueden crear el informe de delegación de usuarios, que le informa de lo siguiente:

* Quién ha delegado estas aprobaciones a otro usuario
* Qué usuario ha delegado estas aprobaciones
* La fecha de inicio y finalización de estas delegaciones

Para obtener más información, consulte [Crear un informe de delegación de usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
