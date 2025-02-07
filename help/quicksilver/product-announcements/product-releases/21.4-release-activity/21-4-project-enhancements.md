---
title: 21.4 Mejoras del proyecto
description: 21.4 Mejoras del proyecto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 99%

---

# 21.4 Mejoras del proyecto

En esta página se describen todas las mejoras del proyecto realizadas con la versión 21.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 4 de octubre de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.4, consulte [Descripción general de la versión 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Incluir imágenes en las actualizaciones

En la ficha Actualizaciones de un objeto, ahora puede añadir imágenes haciendo clic en el icono Imagen de la barra de herramientas. También puede arrastrar y soltar una imagen en el área de actualización. Tenga en cuenta que el administrador de Workfront debe habilitar la adición de imágenes para poder ver el icono Imagen.

Puede añadir imágenes tanto en las actualizaciones como en las respuestas. Una miniatura de imagen en la actualización indica que los destinatarios pueden obtener una vista previa de la imagen en el explorador o descargarla, y las notificaciones por correo electrónico y en la aplicación muestran que las imágenes están adjuntas a la actualización.

Anteriormente, la única manera de compartir una imagen en Workfront era adjuntarla a un objeto como documento. Las imágenes añadidas en la ficha Actualizaciones solo están disponibles en esa ficha y no en la ficha Documentos.

Para obtener más información, consulte [Actualizar un trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Para que los usuarios de Workfront puedan incluir imágenes en las actualizaciones, el administrador de Adobe Workfront debe habilitar primero esta característica, tal como se describe en [Configurar preferencias para actualizaciones de usuarios](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algoritmo actualizado para asignaciones inteligentes

Hemos mejorado el algoritmo utilizado al realizar asignaciones inteligentes. Con la nueva mejora, Workfront observa las 30 asignaciones más recientes realizadas por el usuario que ha iniciado sesión para hacer sugerencias al asignar tareas y problemas. La lista de sugerencias puede contener hasta 50 usuarios.

Antes de esta mejora, Workfront tenía en cuenta las asignaciones de las tareas principales y otros atributos de usuario relacionados con dichas asignaciones a la hora de sugerir usuarios.

Para obtener información acerca de las asignaciones inteligentes, consulte [Información general sobre las asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nueva experiencia al crear un proyecto a partir de una plantilla

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para crear un proyecto a partir de una plantilla. La funcionalidad para crear un proyecto con una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen las siguientes:

* Vista previa de la información de plantilla antes de adjuntarla
* Añadir plantillas a una lista de favoritos durante el proceso de creación del proyecto

Hemos actualizado la interfaz para crear el proyecto tanto cuando lo crea desde el área de Proyectos como desde el área de Plantillas.

Para obtener información, consulte [Crear un proyecto a partir de una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nueva experiencia al adjuntar plantillas a proyectos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para adjuntar una plantilla a un proyecto. La funcionalidad para adjuntar una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen lo siguiente:

* Vista previa de la información de plantilla antes de adjuntarla
* Añadir plantillas a una lista de favoritos durante el proceso de datos adjuntos
* Ver todas las opciones para administrar la configuración de plantillas y proyectos en una página continua

Para obtener información, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Valores unificados de duración y unidad de duración para las tareas

Para una experiencia de usuario más limpia y optimizada, hemos combinado el valor del campo Duración con la unidad de tiempo de la duración. Antes de esta mejora, la unidad de tiempo se mostraba en un campo desplegable independiente después del campo Duración.

Además de los campos Duración en los cuadros Detalles de la tarea, Editar tareas y Nueva tarea, también vamos a actualizar los campos siguientes para que coincidan con esta experiencia:

* Campo de duración al realizar asignaciones avanzadas
* Campo Retraso de redistribución al crear o editar una tarea
* Campo Frecuencia al crear una tarea recurrente (disponible próximamente)
* Campo de retardo al añadir una predecesora (disponible próximamente)

Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![Campo de duración](assets/duration-combined-field-350x139.png)

## Deshabilitar la adición de problemas en línea en los proyectos

Para garantizar que los usuarios proporcionen información precisa al añadir problemas a los proyectos completando un formulario de problemas, hemos introducido una nueva configuración que le permite administrar si pueden añadir problemas a un proyecto o sus tareas en línea. Esta opción está habilitada de manera predeterminada en la nueva área de configuración del problema del cuadro Editar proyecto. Si se deshabilita, se atenúa la opción Añadir más problemas en la sección Problemas de un proyecto, de modo que los usuarios no puedan añadir más problemas a la lista. Los usuarios aún pueden añadir problemas a los proyectos mediante la opción Nuevo problema de la sección Problemas o mediante una cola de solicitudes, si hay alguna configurada para el proyecto.

>[!NOTE]
>
>Esta configuración solo está disponible en la nueva experiencia de Workfront. Los usuarios que trabajan en Workfront Classic pueden seguir añadiendo problemas en línea a un proyecto o a sus tareas aunque un usuario que trabaje en la nueva experiencia de Workfront haya deshabilitado esta configuración para el proyecto.

Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Mejora de la visualización de campos personalizados para las casillas de verificación y los botones de opción

Ver y seleccionar las opciones de las casillas de verificación y los botones de opción en los formularios personalizados es ahora más fácil: un campo personalizado con muchas opciones de casillas de verificación o botones de opción se muestra ahora en varias columnas a lo largo de la página. Anteriormente, se mostraban en una sola columna, lo que requería un desplazamiento adicional para los usuarios que cumplimentaban el formulario.

Esto depende de cómo coloque los campos en el formulario personalizado: si coloca otro campo en la misma fila que la casilla de verificación o el botón de opción, es posible que las opciones solo tengan espacio horizontal suficiente para mostrarse en una sola columna.

Para obtener información sobre cómo rellenar un formulario personalizado, consulte [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

