---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Mejoras de proyecto en 2020.1
description: Esta página describe todas las mejoras realizadas en Proyectos con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y estarán disponibles en el entorno de producción a finales de marzo o principios de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Mejoras de proyecto en 2020.1

Esta página describe todas las mejoras realizadas en Proyectos con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y estarán disponibles en el entorno de producción a finales de marzo o principios de abril de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.1, consulte [Información general de la versión 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Ver más fácilmente quién está etiquetado en una actualización

Ahora es más fácil ver qué usuarios están etiquetados en una actualización. El nombre de los usuarios etiquetados se muestra en azul y se vincula al perfil del usuario.

Los usuarios etiquetados también se enumeran en el cuadro de comentarios.

Antes de esta mejora, los usuarios etiquetados anteriormente no aparecían en el cuadro Notificar.

Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Incluir e identificar el texto citado en un comentario o una respuesta de actualización

A medida que escribe un comentario, puede marcar parte del comentario como texto citado para distinguirlo de su propio comentario. Utilice el botón Cita en bloque del editor de HTML.

Para obtener más información, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Citar un comentario anterior en un comentario o una respuesta de actualización

Cuando comenta en un hilo de actualización, puede incluir rápidamente texto de un comentario anterior en el hilo. Busque la opción Citar respuesta en el menú Más junto al comentario que desea citar.

Para obtener más información, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Información adicional sobre riesgos

Para ayudarle a comprender mejor los riesgos de sus proyectos, ahora puede ver quién y cuándo se introdujo un riesgo y cuándo se actualizó en un proyecto. Puede acceder a esta información en una vista de riesgos y a través de la API pública de Workfront. Estos campos estarán disponibles con la versión 11 de la API, que se lanza con la versión de producción 2020.1.

Para obtener información sobre los riesgos en Workfront, consulte [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Campos adicionales agregados a Líneas bases y Tareas de línea base

Para ayudarle a comprender mejor el progreso financiero de sus proyectos, ahora puede incluir información adicional de costos e ingresos en un informe de Línea Base o de Tarea Prevista. La información financiera adicional no se añade a las líneas base que ha guardado actualmente, sino que se añade para nuevas líneas base.

Para obtener información acerca de los campos financieros de proyecto y tarea a los que se puede tener acceso desde los objetos Línea base y Tarea prevista, vea [Finanzas del proyecto incluidas en las bases de referencia del proyecto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Los problemas en estado &quot;Cerrado - Pendiente de aprobación&quot; se consideran incompletos

Se ha cambiado la forma en que Workfront gestiona los problemas en un estado de &quot;Aprobación completa-pendiente&quot;. Ahora, estos problemas se perciben como Abiertos y el proyecto no puede marcarse como Completo hasta que se resuelva la aprobación.

Antes de este cambio, los problemas con el estado &quot;Cerrado-Pendiente de aprobación&quot; se consideraban Cerrados.

Todos los problemas que se hayan clasificado como Cerrados - Pendientes de aprobación antes de este cambio se comportarán del mismo modo que antes, ya que se considerarán finalizados y también permitirá que se complete el proyecto. Todos los problemas que se coloquen en este estado después de realizar este cambio se considerarán incompletos.

Para obtener información sobre los estados de los proyectos, consulte [Acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

