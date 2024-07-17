---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: otras mejoras de 2020.2
description: Esta página describe todas las demás mejoras realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# otras mejoras de 2020.2

Esta página describe todas las demás mejoras realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.2, consulte [Información general sobre la versión 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Para administradores de Workfront: las plantillas de diseño más recientes creadas en Workfront Classic ahora están disponibles en la nueva experiencia de Workfront

Las plantillas de diseño creadas en Workfront Classic después del otoño de 2019 ya están disponibles en la nueva experiencia de Workfront. Es aconsejable actualizar estas plantillas de diseño en la nueva experiencia de Workfront para aprovechar la nueva funcionalidad y hacerlas lo más útiles posible para los usuarios de ese entorno.

Para obtener más información, consulte [Plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

## Los procesos de aprobación específicos del grupo están disponibles para todos los objetos

Para utilizar completamente los procesos de aprobación específicos del grupo, ahora puede agregarlos a tareas, problemas y proyectos cuando edite estos objetos.

También puede adjuntar automáticamente un proceso de aprobación específico del grupo a una tarea del área Tareas del cuadro Editar proyecto, así como a problemas, al configurar colas de solicitudes o temas de la cola en un proyecto.

Para obtener información sobre cómo agregar procesos de aprobación a proyectos, tareas y problemas, consulte los siguientes artículos:

* [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Creación de procesos de aprobación para grupos mediante estados personalizados

Para facilitar a los grupos la administración de sus propios flujos de trabajo únicos, ahora puede utilizar estados personalizados específicos de grupo en los procesos de aprobación.

Anteriormente, un grupo no podía utilizar sus propios estados personalizados con sus procesos de aprobación específicos del grupo. Solo estaban disponibles los estados de todo el sistema, que no siempre se ajustaban a los procesos de aprobación de grupos.

Los estados personalizados ahora se pueden utilizar en procesos de aprobación de un solo uso y en todo el sistema:

* Cree un proceso de aprobación de un solo uso para un objeto (proyecto, tarea o problema) y baselo en los estados asociados con el grupo que trabaja en ese objeto. Esto incluye cualquier estado personalizado asociado con el grupo.
* Cree un proceso de aprobación global y haga que esté disponible solo para el grupo o para todos los miembros del sistema.

Para los usuarios con acceso administrativo a los procesos de aprobación, la información sobre la configuración de los procesos de aprobación está disponible en [Crear un proceso de aprobación para los elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (o si utiliza Adobe Workfront Classic, consulte [Creación de procesos de aprobación](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Para los usuarios, la información sobre cómo asociar procesos de aprobación con elementos de trabajo está disponible en [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (o si está usando Adobe Workfront Classic, vea [Asociar un proceso de aprobación nuevo o existente con el trabajo](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Nuevas páginas de superposición para la búsqueda

Para permitir que los usuarios naveguen más fácilmente entre las páginas de búsqueda y las páginas anteriores en la nueva experiencia de Workfront, hemos agregado una página de superposición de búsqueda que cubre parcialmente la pantalla.

Ahora, al hacer clic en Búsqueda avanzada en el menú Buscar o realizar una búsqueda básica, se abre una página desde la parte derecha de la pantalla.

Para obtener más información, consulte [Buscar en Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

## Actualizaciones en Suscripciones de eventos

Para permitir que los usuarios clasifiquen, resuelvan problemas y resuelvan problemas mejor, hemos modificado el comportamiento y añadido más datos a la API de suscripciones a eventos. También hemos realizado los siguientes cambios:

* Tecnologías de mensajería subyacentes migradas
* Se ha vuelto a compilar el servicio para que tenga dependencias menos complejas y, por lo tanto, se escale más eficientemente
* Se han realizado mejoras en la monitorización y las alertas

Para obtener más información, consulte [Preguntas más frecuentes - Suscripciones de eventos](../../../wf-api/general/event-subs-faq.md) y [Prácticas recomendadas de suscripción de eventos](../../../wf-api/general/event-sub-best-practice.md).
