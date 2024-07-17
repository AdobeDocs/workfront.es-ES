---
title: 21.4 Mejoras del proyecto
description: 21.4 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# 21.4 Mejoras del proyecto

Esta página describe todas las mejoras de Project realizadas con la versión 21.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 4 de octubre de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.4, consulte [Descripción general de la versión 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Incluir imágenes en las actualizaciones

En la pestaña Actualizaciones de un objeto, ahora puede añadir imágenes haciendo clic en el icono Imagen de la barra de herramientas. También puede arrastrar y soltar una imagen en el área de actualización. Tenga en cuenta que el administrador de Workfront debe habilitar la adición de imágenes para poder ver el icono Imagen.

Puede agregar imágenes tanto en las actualizaciones como en las respuestas. Una miniatura de imagen en la actualización indica que los destinatarios pueden obtener una vista previa de la imagen en el explorador o descargarla, y las notificaciones por correo electrónico y en la aplicación muestran que las imágenes están adjuntas a la actualización.

Anteriormente, la única manera de compartir una imagen en Workfront era adjuntarla a un objeto como documento. Las imágenes agregadas en la ficha Actualizaciones sólo están disponibles en esa ficha y no en la ficha Documentos.

Para obtener más información, consulte [Trabajo de actualización](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Para que los usuarios de Workfront puedan incluir imágenes en las actualizaciones, el administrador de Adobe Workfront debe habilitar primero esta característica, tal como se describe en [Configurar las preferencias para las actualizaciones de usuarios](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algoritmo actualizado para asignaciones inteligentes

Hemos mejorado el algoritmo utilizado al realizar asignaciones inteligentes. Con la nueva mejora, Workfront observa las 30 asignaciones más recientes realizadas por el usuario que ha iniciado sesión para hacer sugerencias al asignar tareas y problemas. La lista de sugerencias puede contener hasta 50 usuarios.

Antes de esta mejora, Workfront tenía en cuenta las asignaciones de las tareas principales y otros atributos de usuario relacionados con esas asignaciones al sugerir usuarios.

Para obtener información acerca de las asignaciones inteligentes, vea [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nueva experiencia al crear un proyecto a partir de una plantilla

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para crear un proyecto a partir de una plantilla. La funcionalidad para crear un proyecto con una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen las siguientes:

* Vista previa de la información de plantilla antes de adjuntarla
* Agregar plantillas a una lista de favoritos durante el proceso de creación del proyecto

Hemos actualizado la interfaz para crear el proyecto tanto al crearlo desde el área Proyectos como desde el área Plantillas.

Para obtener información, [Cree un proyecto con una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nueva experiencia al adjuntar plantillas a proyectos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para adjuntar una plantilla a un proyecto. La funcionalidad para adjuntar una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen lo siguiente:

* Vista previa de la información de plantilla antes de adjuntarla
* Agregar plantillas a una lista de favoritos durante el proceso de datos adjuntos
* Ver todas las opciones para administrar la configuración de plantillas y proyectos en una página continua

Para obtener información, vea [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Valores unificados de duración y unidad de duración para tareas

Para una experiencia de usuario más limpia y optimizada, hemos combinado el valor del campo Duración con la unidad de tiempo de la duración. Antes de esta mejora, la unidad de tiempo se mostraba en un campo desplegable independiente después del campo Duración.

Además de los campos Duración en los cuadros Detalles de la tarea, Editar tareas y Nueva tarea, también vamos a actualizar los campos siguientes para que coincidan con esta experiencia:

* Campo de duración al realizar asignaciones avanzadas
* Retraso por nivelación del campo al crear o editar una tarea
* Campo Frecuencia al crear una tarea recurrente (disponible próximamente)
* Campo de retardo al añadir un predecesor (disponible próximamente)

Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Deshabilitar la adición de problemas en línea en proyectos

Para garantizar que los usuarios proporcionen información precisa al agregar problemas a los proyectos completando un formulario de problemas, hemos introducido una nueva configuración que le permite administrar si pueden agregar problemas a un proyecto o sus tareas en línea. Esta opción está habilitada de manera predeterminada en el área Nueva configuración de problema del cuadro Editar proyecto. Si se deshabilita, se atenúa la opción Agregar más problemas en la sección Problemas de un proyecto, de modo que los usuarios no puedan agregar más problemas en la lista. Los usuarios aún pueden agregar problemas a los proyectos mediante la opción Nuevo problema de la sección Problemas o mediante una cola de solicitudes, si hay alguna configurada para el proyecto.

>[!NOTE]
>
>Esta configuración solo está disponible en la nueva experiencia de Workfront. Los usuarios que trabajan en Workfront Classic pueden seguir agregando problemas en línea a un proyecto o a sus tareas aunque un usuario que trabaje en la nueva experiencia de Workfront haya deshabilitado esta configuración para el proyecto.

Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Mejora de la visualización de campos personalizados para casillas de verificación y botones de opción

Ver y seleccionar las opciones de casilla de verificación y botón de radio en los formularios personalizados se ha vuelto más fácil: ahora se muestra un campo personalizado con muchas opciones de casilla de verificación o botón de radio en varias columnas de la página. Anteriormente, se mostraban en una sola columna, lo que requería un desplazamiento adicional para los usuarios que rellenaban el formulario.

Esto depende de cómo coloque los campos en el formulario personalizado: si coloca otro campo en la misma fila con el campo de casilla de verificación o del botón de radio, es posible que las opciones solo tengan espacio horizontal suficiente para mostrar en una sola columna.

Para obtener información sobre cómo rellenar un formulario personalizado, consulte [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Para obtener información sobre cómo crear un campo de casilla de verificación o de botón de opción en un formulario personalizado, consulte las secciones [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) y [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) en el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

