---
title: 21.3 Mejoras del proyecto
description: 21.3 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
TQID: https://experienceleague.adobe.com/K1JbwFaLdvR5-W16bISI7wadbVnld2Kmtt-6gkZg9N0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1146
ht-degree: 100%

---

# 21.3 Mejoras del proyecto

Esta página describe todas las mejoras del proyecto realizadas con la versión 21.3 en el entorno de previsualización. Estas mejoras estaban disponibles en el entorno de producción en la semana del 21 de julio de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.3, consulte [Información general sobre la versión 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Asociación de una plantilla a un grupo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para ayudarle a optimizar el proceso de creación de proyectos, así como a identificar e informar con mayor facilidad de qué grupos poseen qué plantillas de proyecto, hemos añadido la capacidad de asignar un grupo a una plantilla de proyecto.

Al asignar un grupo a una plantilla de proyecto, todos los proyectos creados a partir de la plantilla se asocian de forma automática al grupo de la plantilla. Para obtener más información, consulte [Edición de plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Además, puede adjuntar un proceso de aprobación de grupo a una plantilla y a sus tareas de plantilla si la plantilla está asociada a su grupo. Para obtener más información, vea [Asociación de un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Edición más sencilla de campos en la sección Detalles

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Las siguientes mejoras le permiten editar con mayor facilidad la información en la sección Detalles de cualquier objeto:

* Un contorno gris alrededor de un campo al pasar el puntero por encima indica que es editable.
* Puede editar los campos haciendo clic en ellos una vez.

Antes de esta mejora no estaba claro qué campos eran editables y tenía que hacer doble clic para editarlos.

## Consideración de los predecesores al calcular las fechas de transferencia

Gracias a una nueva mejora en la forma en que Adobe Workfront calcula las fechas de transferencia de las tareas, ahora se tienen en cuenta las dependencias entre proyectos.

Antes, las fechas de transferencia se calculaban solo en función de los predecesores de la tarea desde el mismo proyecto.

Ahora, para asegurarse de que siempre tiene una fecha de transferencia precisa para una tarea con un predecesor entre proyectos, debe volver a calcular la cronología del proyecto de la tarea sucesora. Después de recalcular la cronología, las fechas de transferencia de la tarea tienen en cuenta las dependencias entre proyectos de las tareas.

Para obtener más información sobre las fechas de entrega, consulte [Información general sobre la fecha de transferencia de la tarea](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Adición de historias y problemas existentes del tablero de Scrum

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede añadir una historia o un problema existente de forma directa desde el tablero de Scrum. Esto facilita la adición de historias existentes a la iteración actual sin tener que ir a la página de registro de asuntos pendientes.

Para obtener más información, consulte [Adición de historias y problemas del tablero de Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Adición de nuevas historias y problemas del tablero de Scrum

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede crear una nueva historia o problema de forma directa desde el tablero de Scrum. Esto facilita la adición rápida de una nueva historia a la iteración actual.

Para obtener más información, consulte [Adición de historias y problemas del tablero de Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Eliminación de historias o problemas del tablero Kanban

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora puede eliminar una historia o un problema de forma directa del tablero Kanban haciendo clic en el icono Más en una tarjeta de historia o problema y seleccionando Eliminar. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.

Para obtener más información, consulte [Eliminación de historias o problemas del tablero Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Actualización del encabezado de las tarjetas de Agile y del tablero de historias

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

En los tableros de Scrum y Kanban, ya están disponibles las siguientes mejoras:

* Las tarjetas de historia y las columnas del tablero tienen una anchura fija, de modo que los tamaños de las tarjetas no cambiarán si ajusta el tamaño de la ventana del explorador.
* Se ha cambiado el nombre de la columna Historias a Historia principal.
* Cada tarjeta tiene una etiqueta en la parte superior para identificarla como historia principal, subtarea (asociada a una historia principal), historia (no asociada a una principal) o problema.
* El sombreado de fondo separa de forma visual las columnas.

Para obtener más información, consulte [Información general de las iteraciones](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Preferencias de proyectos de grupo, tareas y problemas

Como comunicamos antes, implementamos personalizaciones de nivel de grupo para las preferencias de proyecto, tarea y problema en fases anteriores al 24 de junio de 2021. Ahora se ha completado el despliegue y están disponibles en el entorno de producción para todos los clientes.

Para obtener más información, consulte los siguientes artículos:

* [Configurar preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
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

Ahora puede exportar a un archivo de información .pdf desde la sección Detalles de portafolios y programas. Antes de esta mejora, podía exportar información desde la sección Detalles solo desde proyectos, tareas y problemas.

Para obtener información sobre cómo exportar formularios personalizados desde un objeto, consulte [Exportar formularios personalizados y detalles del objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Se ha agregado la marca de fecha planificada de finalización en el encabezado del objeto

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para facilitar el acceso, la comodidad y la precisión, se ha añadido la opción de seleccionar una marca de tiempo en la fecha planificada de finalización del encabezado de proyectos, tareas o problemas.

Antes de esta mejora, cuando se actualizaba la fecha planificada de finalización de un objeto, Workfront seleccionaba medianoche como hora predeterminada. Ahora, puede personalizar la hora y la fecha de finalización.

Para obtener información sobre los encabezados de objeto en la nueva experiencia de Workfront, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Añadir un formulario personalizado a un objeto sin editarlo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Hemos facilitado la adición de un formulario personalizado que otra persona rellenará (o que usted rellenará más adelante) a un objeto. El formulario ya no entrará en modo de edición automáticamente cuando lo añada. Simplemente puede guardar el formulario vacío en el objeto.

Anteriormente, cuando se agregaba un formulario personalizado a un objeto, la página entraba en modo de edición y era necesario completar los campos obligatorios en el formulario para poder guardarlo en el objeto. Esto resultaba incómodo cuando el formulario estaba pensado para que lo rellenara otro usuario o cuando aún no sabía qué poner en un campo obligatorio del formulario.

Para obtener información acerca de cómo añadir un formulario personalizado a un objeto, consulte [Añadir un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

