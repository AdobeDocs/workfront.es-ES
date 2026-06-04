---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Mejoras de los proyectos en 2020.1
description: Esta página describe todas las mejoras realizadas en los proyectos con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y están disponibles en el entorno de producción desde finales de marzo o principios de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
TQID: https://experienceleague.adobe.com/uaajPvdZOKhI6HDmwIRnvevVny9weroPYO4nxy5DwZ0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 543
ht-degree: 100%

---

# Mejoras de los proyectos en 2020.1

Esta página describe todas las mejoras realizadas en los proyectos con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y están disponibles en el entorno de producción desde finales de marzo o principios de abril de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.1, consulte [Información general de la versión 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Es más fácil ver quién está etiquetado en una actualización

Ahora es más fácil ver qué usuarios están etiquetados en una actualización. El nombre de los usuarios etiquetados se muestra en azul y se vincula al perfil del usuario.

Los usuarios etiquetados también se enumeran en el cuadro de comentarios.

Antes de esta mejora, los usuarios etiquetados anteriormente no aparecían en el cuadro Notificar.

Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Incluir e identificar texto citado en un comentario o respuesta de actualización

A medida que escribe un comentario, puede marcar parte del comentario como texto citado para distinguirlo de su propio comentario. Utilice el botón Cita en bloque del editor de HTML.

Para obtener más información, consulte [Trabajo de actualización](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Citar un comentario anterior en un comentario o respuesta de actualización

Cuando comenta en un hilo de actualización, puede incluir rápidamente texto de un comentario anterior en el hilo. Busque la opción Citar respuesta en el menú Más junto al comentario que desea citar.

Para obtener más información, consulte [Trabajo de actualización](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Información adicional sobre riesgos

Para ayudarle a comprender mejor los riesgos de sus proyectos, ahora puede ver quién y cuándo se introdujo un riesgo y cuándo se actualizó en un proyecto. Puede acceder a esta información en una vista de riesgos y a través de la API pública de Workfront. Estos campos estarán disponibles con la versión 11 de la API, que se lanza con la versión de producción 2020.1.

Para obtener información sobre los riesgos en Workfront, consulte [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Campos adicionales añadidos a líneas de base y tareas de la línea de base

Para ayudarle a comprender mejor el progreso financiero de sus proyectos, ahora puede incluir información adicional de costes e ingresos en un informe de línea de base o de tarea prevista. La información financiera adicional no se añade a las líneas de base que tenga guardadas actualmente, pero sí a las nuevas líneas de base.

Para obtener información sobre los campos financieros de proyectos y tareas a los que se puede acceder desde los objetos de línea de base y tarea de línea de base, consulte [Finanzas del proyecto incluidas en las líneas de base del proyecto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Los problemas en estado &quot;Cerrado: aprobación pendiente&quot; se consideran incompletos

Se ha cambiado la forma en que Workfront gestiona los problemas en un estado de “Aprobación completa-pendiente”. Ahora, estos problemas se perciben como Abiertos y el proyecto no puede marcarse como Completo hasta que se resuelva la aprobación.

Antes de este cambio, los problemas con el estado &quot;Cerrado: aprobación pendiente&quot; se consideraban Cerrados.

Todos los problemas que se hayan clasificado como Cerrados: pendientes de aprobación antes de este cambio se comportarán del mismo modo que antes, se considerarán completados y también permitirán que se complete el proyecto. Todos los problemas que estén en este estado después de realizar este cambio se considerarán incompletos.

Para obtener información sobre los estados de los proyectos, consulte [Acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

