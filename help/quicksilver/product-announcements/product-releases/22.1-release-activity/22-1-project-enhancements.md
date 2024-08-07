---
title: 22.1 Mejoras del proyecto
description: 22.1 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# 22.1 Mejoras del proyecto

Esta página describe todas las mejoras de Project realizadas con la versión 22.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción de

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.1, consulte [Información general sobre la versión 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Cambiar la opción predeterminada para las tareas predecesoras al copiar o mover tareas

Para minimizar el número de pasos manuales al copiar o mover tareas, hemos actualizado la información que se copia o mueve con la tarea de forma predeterminada. Ahora, todas las predecesoras se copian o mueven con la tarea de forma predeterminada, ya que la opción All Predecessors está seleccionada de forma predeterminada.

Antes de esta mejora, la opción Todas las predecesoras no estaba seleccionada de forma predeterminada al copiar o mover una tarea.

Para obtener más información, consulte los artículos:

* [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Barra de herramientas actualizada en la lista de paneles e informes en los paneles

La barra de herramientas de las cuatro páginas del panel ahora tiene una apariencia moderna que coincide con otras listas de Workfront, como proyectos, tareas y problemas. Esta intuitiva barra de herramientas ahora facilita la adición, edición, uso compartido, copia y eliminación de paneles.

Las páginas con la barra de herramientas actualizada son:

* Informes de tareas (mostrados en los paneles)
* Lista Todos los paneles
* Lista Mis paneles
* Lista de paneles compartidos

Para obtener más información, consulte [Crear y administrar paneles](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Agregar y editar formularios personalizados Panel de resumen para documentos

Ahora puede agregar y editar formularios personalizados directamente en el panel Resumen del documento.

Con este cambio, también verá una nueva apariencia en el documento Resumen. Hay una nueva sección Información general, que contiene la miniatura de la imagen así como los detalles del documento. También puede proteger y desproteger documentos en la sección de detalles del documento.

Anteriormente, había que ir a la pestaña de formularios personalizados en Detalles del documento para realizar ediciones o agregar formularios personalizados.

Para obtener más información, consulte [Resumen de documentos](../../../documents/managing-documents/summary-for-documents.md).

## Nueva experiencia al copiar una o varias tareas

Para que el uso de Workfront sea coherente con la nueva experiencia de Adobe Workfront, hemos rediseñado la interfaz al copiar una tarea. Actualmente, esto está disponible al copiar una tarea en el nivel de tarea o al copiar una tarea o varias tareas en una lista.

Algunas de las mejoras incluyen:

* Toda la información que debe actualizar antes de copiar la tarea se muestra en una página continua.
* Workfront comprueba si tiene acceso al proyecto de destino inmediatamente después de elegir el proyecto. Antes de esta mejora, se mostraba un mensaje de advertencia que indicaba que no tenía el acceso correcto después de confirmar la copia, lo que provocaba pasos adicionales y que no se permitía la copia.
* Capacidad para solicitar acceso a un proyecto en el que desea copiar la tarea sin salir del cuadro Copiar tarea.

Para obtener más información, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Nueva experiencia al mover una o varias tareas de una lista

Para ofrecer una experiencia coherente al realizar la misma tarea, ahora hemos actualizado la interfaz para mover una o varias tareas de una lista para que coincidan con la experiencia al mover la tarea en el nivel de tarea. (En una versión de vista previa anterior, habíamos actualizado la experiencia para mover una tarea a nivel de tarea).

Para obtener más información, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nueva experiencia al mover una tarea a nivel de tarea

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para mover una tarea. Actualmente, esto está disponible al mover una tarea en el nivel de tarea. En una versión posterior, ampliaremos este rediseño para mover una tarea de una lista.

Algunas de las mejoras de esta interfaz recién rediseñada incluyen:

* Toda la información que debe actualizarse antes de realizar el movimiento se muestra en una página continua.
* Workfront comprobará si tiene acceso al proyecto de destino inmediatamente después de elegir el proyecto. Antes de esta mejora, Workfront le advertía de que no tenía el acceso correcto después de confirmar el movimiento, lo que provocaba pasos adicionales y que no se permitía el movimiento.
* Capacidad para solicitar acceso a un proyecto al que desee mover la tarea sin salir del cuadro Mover tarea.

Para obtener más información, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nueva experiencia al convertir un problema en un proyecto mediante una plantilla en el nivel de problema

>[!NOTE]
>
>Esta función se eliminó temporalmente del entorno de producción el 4 de marzo de 2022. Más tarde se publicó en una implementación por fases a partir del 28 de abril de 2022. El despliegue se completó el 5 de mayo de 2022. Ahora está disponible en Previsualización y Producción para todos los clientes. (Para obtener las últimas actualizaciones sobre el estado de esta característica que se lanza a producción, consulte [Descripción general de la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)).

Para que su uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en un proyecto al utilizarlo cuando lo convierte desde la página de problemas.

Ahora puede acceder más fácilmente a su lista de favoritos inmediatamente después de seleccionar para convertir el problema.

La interfaz rediseñada coincide con la experiencia al crear un proyecto a partir de una plantilla que también hemos actualizado recientemente.

Para obtener más información, consulte [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Convertir problemas en proyectos mediante una plantilla de listas, informes y paneles

>[!NOTE]
>
>Esta función se eliminó temporalmente del entorno de producción el 4 de marzo de 2022. Más tarde se publicó en una implementación por fases a partir del 28 de abril de 2022. El despliegue se completó el 5 de mayo de 2022. Ahora está disponible en Previsualización y Producción para todos los clientes. (Para obtener las últimas actualizaciones sobre el estado de esta característica que se lanza a producción, consulte [Descripción general de la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)).

Para aumentar la eficacia de su trabajo y facilitar la conversión de problemas en un entorno acelerado, hemos añadido la capacidad de convertir un problema en un proyecto mediante una plantilla de una lista, un informe o un panel.

Antes de esta mejora, esta funcionalidad solo existía cuando convertía el problema desde la página de problemas.

Para obtener más información, consulte [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## La lista Filtrar por usuario en los paneles Agile muestra primero los usuarios con la mayoría de las asignaciones

>[!NOTE]
>
>Esta función no se incluirá en la versión 22.1. Se eliminó del entorno de vista previa.

Ahora el filtro muestra los usuarios con la mayor cantidad de asignaciones primero, de modo que sea más fácil localizarlos sin necesidad de desplazarse por la lista.

Anteriormente, el filtro por lista de usuarios en los paneles Kanban y Scrum se mostraba alfabéticamente.

Para obtener más información, consulte la siguiente información

* [Filtrar por usuario en el panel de exploración](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtrar por usuario en el panel Kanban](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limitar la capacidad de agregar documentos a una plantilla que esté compartiendo

A veces, las personas agregan documentos a una plantilla de proyecto pensando que los están agregando a un proyecto. Ahora puede ayudar a evitarlo: cuando comparte una plantilla con acceso de visualización, puede deshabilitar la nueva configuración avanzada Agregar documentos. Esto deshabilita la capacidad de los destinatarios para agregar documentos a la plantilla.

Para obtener instrucciones sobre cómo compartir una plantilla, consulte [Compartir plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Para obtener información acerca de la nueva configuración avanzada Agregar documentos, vea la sección en el artículo [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Compartir una carpeta de documentos

Ahora puede compartir una carpeta de documentos y su contenido desde el área Documentos. Anteriormente, esto no era posible; tenía que compartir cada documento en una carpeta por separado.

Para obtener más información, vea [Compartir una carpeta de documentos](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

