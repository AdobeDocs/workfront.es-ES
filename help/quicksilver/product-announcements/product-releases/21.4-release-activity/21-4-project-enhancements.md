---
title: 21.4 Mejoras del proyecto
description: 21.4 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4 Mejoras del proyecto

En esta página se describen todas las mejoras del proyecto realizadas con la versión 21.4 al entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 4 de octubre de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.4, consulte [Resumen de la versión 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Incluir imágenes en actualizaciones

En la ficha Actualizaciones de un objeto, ahora puede añadir imágenes haciendo clic en el icono Imagen de la barra de herramientas. También puede arrastrar y soltar una imagen en el área de actualización. Tenga en cuenta que el administrador de Workfront debe habilitar la adición de imágenes para poder ver el icono Imagen .

Puede agregar imágenes tanto en actualizaciones como en respuestas. Una miniatura de imagen en la actualización indica que los destinatarios pueden obtener una vista previa de la imagen en el explorador o descargarla, y las notificaciones por correo electrónico y en la aplicación muestran que las imágenes están adjuntas a la actualización.

Anteriormente, la única forma de compartir una imagen en Workfront era adjuntarla a un objeto como documento. Las imágenes agregadas en la ficha Actualizaciones solo están disponibles en esa ficha y no en la ficha Documentos.

Para obtener más información, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Para que los usuarios de Workfront puedan incluir imágenes en las actualizaciones, el administrador de Adobe Workfront debe habilitar primero esta función, tal como se describe en [Configuración de preferencias para actualizaciones de usuarios](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algoritmo actualizado para asignaciones inteligentes

Hemos mejorado el algoritmo utilizado al realizar asignaciones inteligentes. Con la nueva mejora, Workfront observa las 30 asignaciones más recientes realizadas por el usuario que ha iniciado sesión para realizar sugerencias cuando asigne tareas y problemas. La lista de sugerencias puede contener hasta 50 usuarios.

Antes de esta mejora, Workfront estaba considerando las asignaciones en las tareas principales y otros atributos de usuario relacionados con esas asignaciones al sugerir usuarios.

Para obtener información sobre las asignaciones inteligentes, consulte [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nueva experiencia al crear un proyecto a partir de una plantilla

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para crear un proyecto a partir de una plantilla. La funcionalidad para crear un proyecto mediante una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen las siguientes:

* Vista previa de la información de la plantilla antes de adjuntarla
* Agregar plantillas a una lista de favoritos durante el proceso de creación del proyecto

Hemos actualizado la interfaz para crear el proyecto tanto al crearlo desde Proyectos como desde el área Plantillas .

Para obtener información, [Creación de un proyecto mediante una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nueva experiencia al adjuntar plantillas a proyectos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para adjuntar una plantilla a un proyecto. La funcionalidad para adjuntar una plantilla no ha cambiado. Sin embargo, hay algunas mejoras en esta interfaz recién rediseñada que incluyen lo siguiente:

* Vista previa de la información de la plantilla antes de adjuntarla
* Agregar plantillas a una lista de favoritos durante el proceso de archivo adjunto
* Ver todas las opciones para administrar la configuración de plantilla y proyecto en una página continua

Para obtener más información, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Valores unitarios de duración y duración unificados para tareas

Para una experiencia de usuario más limpia y optimizada, hemos combinado el valor del campo Duración con la unidad de tiempo de duración. Antes de esta mejora, la unidad de tiempo se mostraba en un campo desplegable independiente después del campo Duration .

Además de los campos Duración de los cuadros Detalles de tarea, Editar tareas y Nueva tarea , también se están actualizando los campos siguientes para que coincidan con esta experiencia:

* Campo de duración al realizar asignaciones avanzadas
* Redistribuir el campo Retardo al crear o editar una tarea
* Campo Frecuencia al crear una tarea recurrente (disponible próximamente)
* Campo de registro al añadir un predecesor (disponible próximamente)

Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Deshabilitar la adición de problemas en línea en los proyectos

Para garantizar que los usuarios proporcionen información precisa al agregar problemas a los proyectos completando un formulario de problemas, hemos introducido una nueva configuración que le permite administrar si pueden agregar problemas a un proyecto o sus tareas en línea. Esta configuración está habilitada de forma predeterminada en el nuevo área Configuración de problemas del cuadro Editar proyecto . Al desactivarlo, se atenúa la opción Agregar más problemas en la sección Problemas de un proyecto para que los usuarios no puedan agregar más problemas en la lista. Los usuarios aún pueden agregar problemas a los proyectos mediante la opción Nuevo problema de la sección Problemas o utilizando una cola de solicitudes si se ha configurado uno para el proyecto.

>[!NOTE]
>
>Esta configuración solo está disponible en la nueva experiencia de Workfront. Los usuarios que trabajen en Workfront Classic podrán añadir problemas en línea a un proyecto o a sus tareas aunque un usuario que trabaje en la nueva experiencia de Workfront haya desactivado esta configuración para el proyecto.

Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Mejora de la visualización de los campos personalizados para casillas de verificación y botones de opción

La visualización y selección de las opciones de casillas de verificación y botones de opción en los formularios personalizados se han vuelto más fáciles: ahora, un campo personalizado con muchas opciones de casillas de verificación o botones de opción se muestra en varias columnas de la página. Anteriormente, se mostraban en una sola columna, lo que requería un desplazamiento adicional para que los usuarios rellenaran el formulario.

Esto depende de cómo se coloquen los campos en el formulario personalizado: si se coloca otro campo en la misma fila con la casilla de verificación o el campo de botón de radio, las opciones solo pueden tener suficiente espacio horizontal para mostrar en una sola columna.

Para obtener información sobre cómo rellenar un formulario personalizado, consulte [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Para obtener información sobre la creación de un campo de casilla de verificación o botón de radio en un formulario personalizado, consulte las secciones [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) y [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) en el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

