---
title: 21.3 Mejoras del proyecto
description: 21.3 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3 Mejoras del proyecto

En esta página se describen todas las mejoras del proyecto realizadas con la versión 21.3 al entorno de vista previa. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 21 de julio de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.3, consulte [Resumen de la versión 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Asociación de una plantilla a un grupo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para ayudarle a optimizar el proceso de creación de proyectos (y para ayudarle a identificar y a informar con mayor facilidad sobre los grupos que poseen qué plantillas de proyecto), hemos añadido la capacidad de asignar un grupo a una plantilla de proyecto.

Al asignar un grupo a una plantilla de proyecto, todos los proyectos creados a partir de la plantilla se asocian automáticamente al grupo de la plantilla. Para obtener más información, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Además, puede adjuntar un proceso de aprobación de grupo a una plantilla y sus tareas de plantilla si la plantilla está asociada a su grupo. Para obtener más información, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Edición de campos más sencilla en la sección Detalles

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Las siguientes mejoras le permiten editar con mayor facilidad la información en la sección Detalles de cualquier objeto:

* Un contorno gris alrededor de un campo al pasar el ratón por encima indica que es editable.
* Puede editar los campos haciendo clic en ellos una vez.

Antes de esta mejora, no estaba claro qué campos se podían editar y tenía que hacer doble clic para editar un campo.

## Tenga en cuenta los predecesores entre proyectos al calcular fechas de entrega

Con una nueva mejora en la forma en que Adobe Workfront calcula las fechas de entrega de las tareas, ahora se tienen en cuenta las dependencias entre proyectos.

Anteriormente, las fechas de entrega se calculaban solo en función de los predecesores de la tarea del mismo proyecto.

Ahora, para asegurarse de que siempre tiene una fecha de entrega precisa para una tarea con un predecesor entre proyectos, debe volver a calcular la cronología del proyecto de la tarea sucesora. Después de volver a calcular la cronología, las fechas de entrega de la tarea calculan teniendo en cuenta las dependencias entre proyectos de las tareas.

Para obtener más información sobre las fechas de entrega, consulte [Información general sobre la fecha de entrega de tareas](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Agregar artículos y problemas existentes desde el panel Anular

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede agregar un artículo o problema existente directamente desde el panel Anular. Esto facilita la adición de artículos existentes a la iteración actual sin tener que ir a la página de atrasos.

Para obtener más información, consulte [Agregar artículos y problemas desde el panel Anular](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Agregar nuevos artículos y problemas desde el panel Anular

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede crear un nuevo artículo o número directamente desde el panel Anulación. Esto facilita añadir rápidamente un nuevo artículo a la iteración actual.

Para obtener más información, consulte [Agregar artículos y problemas desde el panel Anular](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Eliminar artículo o problema del panel Kanban

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede eliminar un artículo o problema directamente desde el panel de Kanban haciendo clic en el icono Más de un artículo o tarjeta de publicación y seleccionando Eliminar. Cuando elimina un artículo o problema, este se mueve a la Papelera de reciclaje durante 30 días y solo puede recuperarlo el administrador del sistema.

Para obtener más información, consulte [Eliminar artículos o problemas del panel Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Actualizaciones en el encabezado y el tablero de historia de la tarjeta Agile

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ya están disponibles las siguientes mejoras en las placas Kanban y Scrum:

* Las tarjetas de artículo y las columnas de tablero tienen una anchura fija, por lo que los tamaños de tarjeta no cambiarán si ajusta el tamaño de la ventana del navegador.
* Se ha cambiado el nombre de la columna Artículos a Artículo principal.
* Cada tarjeta tiene una etiqueta en la parte superior para identificarla como un artículo principal, una subtarea (asociada con un artículo principal), un artículo (no asociado con un artículo principal) o un problema.
* El sombreado de fondo separa visualmente las columnas.

Para obtener más información, consulte [Información general sobre iteraciones](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Agrupar las preferencias de proyecto, tarea y problema

Como nos comunicamos anteriormente, hemos implementado personalizaciones a nivel de grupo para preferencias de proyectos, tareas y problemas en fases anteriores al 24 de junio de 2021. Ahora el despliegue se ha completado y están disponibles en Producción para todos los clientes.

Para obtener más información, consulte los siguientes artículos:

* [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Permitir que los usuarios externos aprueben un documento

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede utilizar direcciones de correo electrónico externas para asignar aprobadores a un documento en la nueva experiencia de Workfront.

Anteriormente, solo se podían añadir usuarios externos por dirección de correo electrónico en Workfront Classic.

Para obtener más información, consulte [Solicitar aprobaciones de documentos](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportar información de la sección Detalles de un portafolio o programa

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 20 de mayo de 2021. Se lanzará al entorno Producción el 3 de junio de 2021.

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede exportar a un archivo .pdf información de la sección Detalles de portafolios y programas. Antes de esta mejora, podía exportar información de la sección Detalles únicamente desde proyectos, tareas y problemas.

Para obtener información sobre la exportación de formularios personalizados desde un objeto, consulte [Exportar formularios personalizados y detalles de objetos](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Se ha añadido la marca de fecha y hora de finalización planeada en el encabezado del objeto

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para facilitar el acceso, la comodidad y la precisión, hemos añadido la opción de seleccionar una marca de tiempo en la Fecha de Finalización Planificada del encabezado de proyectos, tareas o problemas.

Antes de esta mejora, al actualizar la fecha de finalización prevista de un objeto, Workfront seleccionaba la medianoche como hora predeterminada. Ahora, puede personalizar la hora y la fecha de finalización.

Para obtener información sobre los encabezados de objeto en la nueva experiencia de Workfront, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Agregar un formulario personalizado a un objeto sin editarlo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Hemos facilitado la adición de un formulario personalizado que alguien rellenará (o que rellenará más tarde) a un objeto. El formulario ya no entra en modo de edición automáticamente al agregarlo. Puede guardar el formulario vacío en el objeto.

Anteriormente, cuando se agregaba un formulario personalizado a un objeto, la página se ponía en modo de edición y era necesario rellenar los campos obligatorios del formulario antes de guardarlo en el objeto. Esto resultaba incómodo cuando el formulario estaba pensado para que otro usuario lo rellenara o cuando todavía no sabía qué poner en un campo requerido del formulario.

Para obtener información sobre cómo agregar un formulario personalizado a un objeto, consulte [Adición de un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

