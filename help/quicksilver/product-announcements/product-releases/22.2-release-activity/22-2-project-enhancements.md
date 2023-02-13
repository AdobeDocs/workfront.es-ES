---
title: 22.2&nbsp;Mejoras del proyecto
description: 22.2&nbsp;Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 1%

---

# 22.2 Mejoras del proyecto

En esta página se describen todas las mejoras realizadas en el proyecto con la versión 2.2 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022. Para obtener una lista de todos los cambios disponibles con la versión 2.2, consulte [Resumen de la versión 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Los tableros de Adobe Workfront ya están disponibles.

Los tableros son herramientas flexibles que permiten la colaboración entre equipos al proporcionar acceso a un tablero compartido que contiene columnas y tarjetas.

Con los tableros, puede:

* Configuración rápida de un panel de tareas con varias columnas
* Configuración de columnas para mostrar un estado o una categoría
* Agregar otros usuarios al tablero y asignarlos a tarjetas
* Agregar rápidamente tarjetas y listas de comprobación abiertas

Tenga en cuenta que las tarjetas de un tablero no están conectadas a objetos ni a elementos de trabajo en Adobe Workfront.

Un administrador del sistema debe habilitar Tableros en plantillas de diseño para que la opción esté disponible para todos los usuarios en el menú principal.

Para obtener más información, consulte [Información general sobre los tableros](../../../agile/boards-overview.md).

## Mejoras adicionales en los tableros de Workfront

Ya están disponibles las siguientes mejoras adicionales para los Workfront Boards:

* Etiquetar tarjetas en tableros

   Ahora puede categorizar las tarjetas en el tablero con etiquetas con códigos de color. Las etiquetas permiten identificar rápidamente las tarjetas. Incluso puede ordenar el tablero en función de las etiquetas aplicadas.

* Administrar tarjetas en tableros

   Hemos añadido las siguientes funciones para ayudarle a administrar tarjetas en su tablero:

   * Copiar una tarjeta: Cree una copia de una tarjeta existente en el tablero.
   * Mover una tarjeta: Mueva rápidamente las tarjetas a la parte superior o inferior de un tablero con las nuevas opciones de menú Superior de columna e Inferior de columna .

* Buscar en tableros

   Hemos agregado una barra de búsqueda para ayudarle a buscar todas las tarjetas en su tablero.

* Establecer una fecha de vencimiento para una tarjeta en los tableros

   Ahora puede establecer una fecha de vencimiento para tarjetas individuales en el tablero.

Para obtener más información, consulte [Introducción a los tableros en Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Opción Deshacer para Actualizar anuncios

Ahora es más fácil capturar errores al publicar una actualización. Al finalizar un comentario en la ficha Actualizar de un objeto, ahora se crea una ventana emergente durante 7 segundos que permite cancelar el anuncio y volver a la edición, antes de que el sistema lo marque o envíe correos electrónicos y notificaciones en la aplicación. Si descarta la ventana emergente, abandona la página o espera 7 segundos para que se agote el tiempo de espera de la ventana, la publicación se realizará de forma normal.

Para obtener más información, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Experiencia actualizada al copiar y mover problemas

Para que el uso de Workfront sea coherente con la nueva experiencia de Adobe Workfront, hemos rediseñado la interfaz para copiar y mover problemas. Actualmente está disponible al copiar o mover un solo problema o al copiar o mover problemas de forma masiva desde una lista o informe.

Algunas de las mejoras de esta interfaz recién rediseñada incluyen:

* Toda la información que debe actualizar antes del movimiento se muestra en una página continua.
* Workfront comprueba si tiene acceso al proyecto de destino inmediatamente después de elegir el proyecto. Antes de esta mejora, Workfront le advirtió de que no tiene el acceso correcto después de confirmar el movimiento, lo que provocaba que se realizaran pasos adicionales y que el movimiento no estuviera permitido.
* Capacidad para solicitar acceso a un proyecto en el que desee mover los problemas sin salir del cuadro Mover tarea .
* Posibilidad de eliminar elementos (asignaciones, progreso, documentos, permisos, actualizaciones) de un problema cuando se mueve a otra ubicación. Anteriormente, esta funcionalidad solo estaba disponible para copiar problemas.
* Posibilidad de seleccionar una tarea de destino además de seleccionar un proyecto de destino al copiar un problema.

Para obtener más información sobre cómo mover o copiar problemas, consulte los siguientes artículos:

* [Copiar problemas](../../../manage-work/issues/manage-issues/copy-issues.md)
* [Mover problemas](../../../manage-work/issues/manage-issues/move-issues.md)

## Nueva experiencia al copiar un proyecto

Para que el uso de Workfront sea coherente con la nueva experiencia de Adobe Workfront, hemos rediseñado la interfaz para copiar proyectos. Actualmente está disponible al copiar un proyecto de la página del proyecto o al copiar un proyecto de una lista o informe. Antes de esta actualización, solo podía copiar un proyecto de la página del proyecto.

Para obtener más información, consulte [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

## Capacidad para administrar proyectos desde listas e informes desde un nuevo menú Más

Se ha agregado un nuevo menú Más en listas de proyectos e informes para que pueda realizar las siguientes acciones desde estas áreas:

* Para varios proyectos a la vez:
* Recalcular escala de tiempo
* Recalcular finanzas
* Volver a calcular las expresiones personalizadas
* Para un solo proyecto:
* Adjuntar plantilla
* Exportar a MS Project
* Suscribirse

Para obtener más información, consulte los siguientes artículos:

* [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [Volver a calcular las finanzas del proyecto](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Exportar un proyecto a un proyecto de Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Suscripción a elementos en Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Mantener a los usuarios en el tablero, la lista o el informe después de convertir el problema en proyecto

Para aumentar la eficacia y eliminar el número de clics, hemos publicado una mejora al convertir problemas a proyectos desde una lista, un informe o un panel.

Los usuarios permanecen en la lista, el informe o un panel después de convertir un problema en un proyecto en lugar de redirigirse a la página del proyecto. Se muestra una notificación de éxito con el vínculo al proyecto una vez finalizada la conversión para que pueda navegar fácilmente al proyecto si es necesario.

Para obtener más información, consulte [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Ya no se quitarán las horas de asignación al realizar cambios en las asignaciones

>[!NOTE]
>
>Esta función estaba originalmente planificada para su lanzamiento con la versión 2.2. Se lanzará a Producción el 21 de abril de 2022.

Para garantizar la precisión de sus datos, se ha realizado un cambio para conservar las horas de asignación y mantener las horas planificadas de la tarea sin cambios al realizar cambios en las asignaciones de la tarea.

Se han realizado los siguientes cambios en las tareas con un tipo de duración simple:

* Las horas planificadas se conservan cuando se eliminan todos los asignadores.
* Las asignaciones de asignaciones individuales se conservan al reemplazar usuarios y funciones.
* Las asignaciones de asignaciones individuales se conservan en la función al eliminar el usuario. (Eliminado de la versión. Ahora, el valor de Horario planeado se establecerá en 0 después de eliminar todos los usuarios asignados).

Para obtener más información sobre las horas planificadas, consulte [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

## Compartir carpetas solo en los cinco niveles superiores de una jerarquía de carpetas

>[!NOTE]
>
>Esta función no está disponible temporalmente. Actualizaremos esta nota de la versión cuando la función esté disponible en Producción.

Para garantizar el mejor rendimiento para los usuarios que comparten carpetas, actualmente limitamos el uso compartido a los cinco niveles superiores de una jerarquía de carpetas en un objeto.

Cada carpeta del sexto nivel o inferior hereda sus configuraciones de uso compartido de la carpeta directamente superior.

Para obtener más información sobre cómo compartir carpetas, consulte [Compartir una carpeta de documento](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

