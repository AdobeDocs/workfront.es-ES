---
title: 22.2&nbsp;Mejoras del proyecto
description: 22.2&nbsp;Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# 22.2 Mejoras del proyecto

Esta página describe todas las mejoras de Project realizadas con la versión 22.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción de

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.2, consulte [Información general de la versión 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Los tableros de Adobe Workfront ya están disponibles.

Los tableros son herramientas flexibles que permiten la colaboración entre equipos al proporcionar acceso a un tablero compartido que contiene columnas y tarjetas.

Con los tableros, puede:

* Configurar rápidamente un panel de tareas con varias columnas
* Configurar columnas para mostrar un estado o una categoría
* Agregar otros usuarios al tablero y asignarlos a tarjetas
* Agregue rápidamente tarjetas abiertas y listas de comprobación

Tenga en cuenta que las tarjetas de un tablero no están conectadas a objetos y elementos de trabajo en Adobe Workfront.

Un administrador del sistema debe habilitar Tableros en plantillas de diseño para que la opción esté disponible para todos los usuarios en el menú principal.

Para obtener más información, consulte [Información general de tableros](../../../agile/boards-overview.md).

## Mejoras adicionales en los tableros de Workfront

Las siguientes mejoras adicionales ya están disponibles para los tableros de Workfront:

* Etiquetar tarjetas en tableros

  Ahora puede categorizar las tarjetas en el tablero con etiquetas con códigos de color. Las etiquetas permiten identificar tarjetas rápidamente. Incluso puede ordenar el tablero según las etiquetas aplicadas.

* Administrar tarjetas en los tableros

  Hemos agregado las siguientes funciones para ayudarle a administrar tarjetas en el tablero:

   * Copiar una tarjeta: cree una copia de una tarjeta existente en el tablero.
   * Mover una tarjeta: mueva rápidamente las tarjetas a la parte superior o inferior de un tablero con las nuevas opciones de menú Parte superior de la columna y Parte inferior de la columna.

* Buscar en tableros

  Hemos agregado una barra de búsqueda para ayudarte a buscar en todas las tarjetas del tablero.

* Establecer una fecha límite para una tarjeta en los paneles

  Ahora puede establecer una fecha límite para las tarjetas individuales en el tablero.

Para obtener más información, consulte [Introducción a los tableros en Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Opción Deshacer para Actualizar publicaciones

Ahora es más fácil detectar errores al publicar una actualización. Al finalizar un comentario en la pestaña Actualizar de un objeto, ahora se crea una ventana emergente durante 7 segundos que le permite cancelar la publicación y volver a la edición, antes de que el sistema lo marque con la hora o envíe correos electrónicos y notificaciones en la aplicación. Si cierra la ventana emergente, abandona la página o espera 7 segundos a que se agote el tiempo de espera de la ventana, la publicación se realizará de forma normal.

Para obtener más información, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Experiencia actualizada al copiar y mover problemas

Para que su uso de Workfront sea coherente con la nueva experiencia de Adobe Workfront, hemos rediseñado la interfaz para copiar y mover problemas. Actualmente, esto está disponible al copiar o mover un solo problema o al copiar o mover problemas de forma masiva desde una lista o un informe.

Algunas de las mejoras de esta interfaz recién rediseñada incluyen:

* Toda la información que debe actualizarse antes de realizar el movimiento se muestra en una página continua.
* Workfront comprueba si tiene acceso al proyecto de destino inmediatamente después de elegir el proyecto. Antes de esta mejora, Workfront le advertía de que no tenía el acceso correcto después de confirmar el movimiento, lo que provocaba pasos adicionales y que no se permitía el movimiento.
* Capacidad para solicitar acceso a un proyecto al que desee mover los problemas sin salir del cuadro Mover tarea.
* Posibilidad de eliminar elementos (asignaciones, progreso, documentos, permisos, actualizaciones) de un problema al moverlo a otra ubicación. Anteriormente, esta funcionalidad solo estaba disponible para copiar problemas.
* Posibilidad de seleccionar una tarea de destino además de seleccionar un proyecto de destino al copiar un problema.

Para obtener más información sobre cómo mover o copiar problemas, consulte los siguientes artículos:

* [Copiar problemas](../../../manage-work/issues/manage-issues/copy-issues.md)
* [Mover problemas](../../../manage-work/issues/manage-issues/move-issues.md)

## Nueva experiencia al copiar un proyecto

Para que el uso de Workfront sea coherente con la nueva experiencia de Adobe Workfront, hemos rediseñado la interfaz para copiar proyectos. Actualmente, esto está disponible al copiar un proyecto desde la página del proyecto o al copiar un proyecto desde una lista o informe. Antes de esta actualización, solo se podía copiar un proyecto desde la página del proyecto.

Para obtener más información, consulte [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

## Capacidad para administrar proyectos desde listas e informes desde un nuevo menú Más

Se ha agregado un nuevo menú Más en las listas de proyectos y los informes para permitirle realizar las siguientes acciones desde estas áreas:

* Para varios proyectos a la vez:
* Recalcular escala de tiempo
* Recalcular finanzas
* Volver a calcular las expresiones personalizadas
* Para un solo proyecto:
* Adjuntar plantilla
* Exportar a MS Project
* Suscribirse

Para obtener más información, consulte los siguientes artículos:

* [Recalcular escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [Recalcular finanzas del proyecto](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Exportar un proyecto a un proyecto de Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Suscribirse a elementos en Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Mantener a los usuarios en el tablero, la lista o el informe después de convertir el problema en un proyecto

Para aumentar la eficacia y eliminar el número de clics, hemos publicado una mejora al convertir problemas a proyectos desde una lista, un informe o un panel.

Los usuarios permanecen en la lista, el informe o un panel después de convertir un problema en un proyecto en lugar de ser redirigidos a la página del proyecto. Una vez completada la conversión, se muestra una notificación de éxito con el vínculo al proyecto para permitirle navegar fácilmente al proyecto, si es necesario.

Para obtener más información, consulte [Conversión de un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Las horas de asignación ya no se eliminarán al realizar cambios en las asignaciones

>[!NOTE]
>
>Originalmente, esta función se había planificado para su lanzamiento con la versión 22.2. Se publicará en Production el 21 de abril de 2022.

Para garantizar la precisión de sus datos, hemos realizado un cambio para conservar las horas de asignación y mantener las Horas planificadas de la tarea sin cambios al realizar cambios en las asignaciones de la tarea.

Se han realizado los siguientes cambios en las tareas con un tipo de duración simple:

* Las horas planificadas se conservan al eliminar a todas las personas asignadas.
* Las asignaciones de asignación individuales se conservan al reemplazar usuarios y roles.
* Las asignaciones de asignación individuales se conservan en el rol al eliminar el usuario. (Se ha eliminado de la versión. Ahora, las horas planificadas se establecerán en 0 después de eliminar a todas las personas asignadas).

Para obtener más información sobre las horas planificadas, consulte [Resumen de horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

## Compartir carpetas solo en los cinco niveles principales de una jerarquía de carpetas

>[!NOTE]
>
>Esta función no está disponible temporalmente. Actualizaremos esta nota de la versión cuando la función esté disponible en Producción.

Para garantizar el mejor rendimiento a los usuarios que comparten carpetas, actualmente limitamos el uso compartido a los cinco niveles principales de una jerarquía de carpetas en un objeto.

Cada carpeta del sexto nivel o inferior hereda sus configuraciones de uso compartido de la carpeta directamente superior a ella.

Para obtener más información sobre cómo compartir carpetas, consulte [Compartir una carpeta de documentos](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

