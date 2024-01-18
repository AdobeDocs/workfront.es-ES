---
title: 21.3 Mejoras del proyecto
description: 21.3 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3 Mejoras del proyecto

Esta página describe todas las mejoras de Project realizadas con la versión 21.3 en el entorno de vista previa. Estas mejoras estaban disponibles en el entorno de producción en la semana del 21 de julio de 2021.

Para ver una lista de todos los cambios disponibles con la versión 21.3, consulte [Resumen de la versión 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Asociar una plantilla a un grupo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para ayudarle a optimizar el proceso de creación de proyectos y para ayudarle a identificar y crear informes más fácilmente sobre los grupos que poseen las plantillas de proyecto, hemos añadido la capacidad de asignar un grupo a una plantilla de proyecto.

Al asignar un grupo a una plantilla de proyecto, todos los proyectos creados a partir de la plantilla se asocian automáticamente al grupo de la plantilla. Para obtener más información, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Además, puede adjuntar un proceso de aprobación de grupo a una plantilla y a sus tareas de plantilla si la plantilla está asociada a su grupo. Para obtener más información, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Edición más sencilla de campos en la sección Detalles

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Las siguientes mejoras le permiten editar con mayor facilidad la información en la sección Detalles de cualquier objeto:

* Un contorno gris alrededor de un campo al pasar el ratón por encima indica que es editable.
* Puede editar los campos haciendo clic en ellos una vez.

Antes de esta mejora no estaba claro qué campos eran editables y tenía que hacer doble clic para editar un campo.

## Tener en cuenta las predecesoras entre proyectos al calcular las fechas de entrega

Con una nueva mejora en la forma en que Adobe Workfront calcula las fechas de entrega de las tareas, ahora se tienen en cuenta las dependencias entre proyectos.

Anteriormente, las fechas de entrega se calculaban únicamente en función de las predecesoras de la tarea desde el mismo proyecto.

Ahora, para asegurarse de que siempre tiene una fecha de transferencia precisa para una tarea con una predecesora entre proyectos, debe volver a calcular la escala de tiempo del proyecto de la tarea sucesora. Después de volver a calcular la escala de tiempo, las fechas de transferencia de la tarea se calculan teniendo en cuenta las dependencias entre proyectos de las tareas.

Para obtener más información sobre las fechas de entrega, consulte [Resumen de fecha de transferencia de tareas](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Agregar historias y problemas existentes del panel de exploración

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede agregar una historia o un problema existente directamente desde el panel de Scrum. Esto facilita la adición de historias existentes a la iteración actual sin tener que ir a la página de registro de pendientes.

Para obtener más información, consulte [Agregar historias y problemas del panel de exploración](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Agregar nuevas historias y problemas del panel de exploración

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede crear una nueva historia o problema directamente desde el panel de Scrum. Esto facilita la adición rápida de una nueva historia a la iteración actual.

Para obtener más información, consulte [Agregar historias y problemas del panel de exploración](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Eliminar historia o problema del Panel Kanban

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede eliminar una historia o un problema directamente del panel Kanban haciendo clic en el icono Más en una historia o tarjeta de emisión y seleccionando Eliminar. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.

Para obtener más información, consulte [Eliminar historias o problemas del Panel Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Actualizaciones del encabezado y del guion gráfico de la tarjeta Agile

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

En los paneles Kanban y Scrum, ya están disponibles las siguientes mejoras:

* Las tarjetas de historia y las columnas del tablero tienen un ancho fijo, de modo que los tamaños de las tarjetas no cambiarán si ajusta el tamaño de la ventana del explorador.
* Se ha cambiado el nombre de la columna Historias a Historia principal.
* Cada tarjeta tiene una etiqueta en la parte superior para identificarla como artículo principal, subtarea (asociada a un artículo principal), artículo (no asociado a un artículo principal) o problema.
* El sombreado de fondo separa visualmente las columnas.

Para obtener más información, consulte [Resumen de iteraciones](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Agrupar preferencias de proyectos, tareas y problemas

Como comunicamos anteriormente, implementamos personalizaciones de nivel de grupo para las preferencias de proyecto, tarea y problema en fases anteriores al 24 de junio de 2021. Ahora se ha completado el despliegue, que está disponible en el entorno de producción para todos los clientes.

Para obtener más información, consulte los siguientes artículos:

* [Configurar las preferencias de proyecto de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Permitir que los usuarios externos aprueben un documento

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede utilizar direcciones de correo electrónico externas para asignar aprobadores a un documento en la nueva experiencia de Workfront.

Anteriormente, solo se podían agregar usuarios externos por dirección de correo electrónico en Workfront Classic.

Para obtener más información, consulte [Solicitar aprobaciones de documentos](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportar información de la sección Detalles de un portafolio o programa

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 20 de mayo de 2021. Se lanzará al entorno de producción el 3 de junio de 2021.

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede exportar a un archivo .pdf información desde la sección Detalles de portafolios y programas. Antes de esta mejora, podía exportar información desde la sección Detalles solo desde proyectos, tareas y problemas.

Para obtener información sobre la exportación de formularios personalizados desde un objeto, consulte [Exportar formularios personalizados y detalles del objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Se ha agregado la marca de fecha planificada de finalización en la cabecera del objeto

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para facilitar el acceso, la comodidad y la precisión, se ha añadido la opción de seleccionar una marca de tiempo en la Fecha planificada de finalización del encabezado de proyectos, tareas o problemas.

Antes de esta mejora, cuando se actualizaba la Fecha planificada de finalización de un objeto, Workfront seleccionaba medianoche como hora predeterminada. Ahora, puede personalizar la hora y la fecha de finalización.

Para obtener información sobre los encabezados de objeto en la nueva experiencia de Workfront, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Agregar un formulario personalizado a un objeto sin editarlo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Hemos facilitado la adición de un formulario personalizado que otra persona rellenará (o que usted rellenará más adelante) a un objeto. El formulario ya no entrará en modo de edición automáticamente cuando lo agregue. Simplemente puede guardar el formulario vacío en el objeto.

Anteriormente, cuando se agregaba un formulario personalizado a un objeto, la página entraba en modo de edición y era necesario completar los campos obligatorios en el formulario para poder guardarlo en el objeto. Esto resultaba incómodo cuando el formulario estaba pensado para que lo rellenara otro usuario o cuando aún no sabía qué colocar en un campo obligatorio del formulario.

Para obtener información sobre cómo agregar un formulario personalizado a un objeto, consulte [Agregar un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

