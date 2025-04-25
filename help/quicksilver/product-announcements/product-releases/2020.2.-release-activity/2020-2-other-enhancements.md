---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Otras mejoras de 2020.2
description: En esta página se describen todas las demás mejoras realizadas en la versión 2020.2 del entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 99%

---

# Otras mejoras de 2020.2

En esta página se describen todas las demás mejoras realizadas en la versión 2020.2 del entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.2, consulte [Información general sobre la versión 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Para los administradores de Workfront: las plantillas de diseño más recientes creadas en Workfront Classic ahora están disponibles en la nueva experiencia de Workfront

Las plantillas de diseño creadas en Workfront Classic después del otoño de 2019 ya están disponibles en la nueva experiencia de Workfront. Es aconsejable actualizar estas plantillas de diseño en la nueva experiencia de Workfront para aprovechar la nueva funcionalidad y hacerlas lo más útiles posible para los usuarios de ese entorno.

Para obtener más información, consulte [Plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

## Los procesos de aprobación específicos del grupo están disponibles para todos los objetos

Para utilizar completamente los procesos de aprobación específicos del grupo, ahora puede añadirlos a tareas, problemas y proyectos cuando edite estos objetos.

También puede adjuntar automáticamente un proceso de aprobación específico del grupo a una tarea en el área de tareas del cuadro Editar proyecto, así como a problemas, al configurar colas de solicitudes o temas de la cola en un proyecto.

Para obtener información sobre cómo añadir procesos de aprobación a proyectos, tareas y problemas, consulte los siguientes artículos:

* [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Crear temas de la cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Creación de procesos de aprobación para grupos mediante estados personalizados

Para que los grupos la administración puedan administrar más fácilmente sus propios flujos de trabajo únicos, ahora puede utilizar estados personalizados específicos del grupo en los procesos de aprobación.

Anteriormente, un grupo no podía utilizar sus propios estados personalizados con sus procesos de aprobación específicos del grupo. Solo estaban disponibles los estados de todo el sistema, que no siempre se ajustaban a los procesos de aprobación de grupos.

Los estados personalizados ahora se pueden utilizar en procesos de aprobación de un solo uso y en todo el sistema:

* Cree un proceso de aprobación de un solo uso para un objeto (proyecto, tarea o problema) y báselo en los estados asociados al grupo que trabaja en ese objeto. Esto incluye cualquier estado personalizado asociado al grupo.
* Cree un proceso de aprobación global y póngalo a disposición solo del grupo o de todas las personas del sistema

En el caso de los usuarios con acceso administrativo a los procesos de aprobación, la información sobre la configuración de los procesos de aprobación está disponible en [Crear un proceso de aprobación para los elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (o si utiliza Adobe Workfront Classic, consulte [Creación de procesos de aprobación](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

En el caso de los usuarios, la información sobre cómo asociar procesos de aprobación a elementos de trabajo está disponible en [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (o si está usando Adobe Workfront Classic, consulte [Asociación de un proceso de aprobación nuevo o existente con el trabajo](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Nuevas páginas de superposición para la búsqueda

Para que los usuarios puedan navegar más fácilmente por las páginas de búsqueda y las páginas anteriores en la nueva experiencia de Workfront, hemos añadido una página de superposición de búsqueda que cubre parcialmente la pantalla.

Ahora, al hacer clic en Búsqueda avanzada en el menú de búsqueda o realizar una búsqueda básica, se abre una página en la parte derecha de la pantalla.

Para obtener más información, consulte [Búsqueda en Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

## Actualizaciones de suscripciones a eventos

Para que los usuarios puedan clasificar, solucionar y resolver mejor los problemas, hemos modificado el comportamiento y hemos añadido más datos a la API de suscripciones a eventos. También hemos realizado los siguientes cambios:

* Tecnologías de mensajería subyacentes migradas
* Se ha vuelto a compilar el servicio para que tenga dependencias menos complejas y, por lo tanto, se escale más eficientemente
* Se han realizado mejoras en la monitorización y las alertas

Para obtener más información, consulte [Preguntas frecuentes: suscripciones a eventos](../../../wf-api/general/event-subs-faq.md) y [Prácticas recomendadas de suscripción a eventos](../../../wf-api/general/event-sub-best-practice.md).
