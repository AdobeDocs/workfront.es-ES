---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa R1 4
description: Esta página describe todos los cambios disponibles en el entorno de Vista previa con la versión R1.4. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 15 de febrero de 2017.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Vista previa R1 4

Esta página describe todos los cambios disponibles en el entorno de Vista previa con la versión R1.4. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 15 de febrero de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [La versión Workfront R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Aprobaciones actualizadas de proyectos, tareas y problemas

Al crear procesos de aprobación para aprobaciones de proyectos, tareas y problemas, ya están disponibles las siguientes mejoras y cambios: 

* Los &quot;Pasos&quot; de aprobación ahora se llaman &quot;Pasos&quot; de aprobación.
* Incluya varios tipos de aprobadores por etapa.\
   Esto incluye usuarios, equipos y funciones de trabajo.\
   Antes de este cambio, podría incluir varios aprobadores del mismo tipo únicamente. Por ejemplo, puede incluir varias funciones de trabajo, pero no una función de trabajo y un equipo.

* Se han eliminado las siguientes limitaciones preexistentes relacionadas con la modificación de los procesos de aprobación global existentes:

   * El proceso de aprobación modificado se refleja únicamente en los objetos de todo el sistema en los que el proceso de aprobación aún no se ha iniciado o en los que no se ha modificado el proceso de aprobación. Los objetos en los que el proceso de aprobación ya se ha iniciado o en los que se ha modificado el proceso de aprobación no se actualizan con los cambios.
   * No se puede modificar el estado que determina cuándo se inicia la aprobación.

* Aspecto actualizado.

Para obtener más información sobre la creación de procesos de aprobación, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Al asociar un proceso de aprobación con un proyecto, tarea o problema, ya están disponibles las siguientes mejoras y cambios:

* Aspecto actualizado.
* El diagrama de aprobación se muestra en la pestaña Approvals , que muestra una representación visual de los pasos de aprobación anteriores, actuales y futuros.

Para obtener más información sobre cómo asociar aprobaciones con proyectos, tareas y problemas, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Cambiar el estado de un proyecto directamente desde la página Proyecto

Ya no es necesario editar un proyecto para cambiar su estado. Ahora puede cambiar el estado de un proyecto directamente desde la página principal del proyecto.

Para obtener más información, consulte [Cambiar el estado de un proyecto](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Programar usuarios para su desactivación

Ahora puede programar que los usuarios se desactiven en una fecha futura.

Antes de esta mejora, solo podía desactivar manualmente a un usuario inmediatamente.

Programar a un usuario para desactivarlo puede resultar útil en diversos escenarios. Por ejemplo, si crea usuarios en Workfront que se contratan de forma temporal, puede configurarlos para que se desactiven cuando termine el contrato.

Esta función también está disponible cuando se editan usuarios de forma masiva. 

Para obtener más información sobre la programación de usuarios para la desactivación, consulte [Desactivar o reactivar un usuario](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) y [Agregar usuarios](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nuevas opciones de resumen de correo electrónico para las &quot;acciones necesarias&quot;

La opción de entrega Resumen diario ya está disponible en el área &quot;Acción necesaria&quot; de la configuración de Notificaciones.

Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque el espacio aislado de vista previa borra las direcciones de correo electrónico de todos los usuarios.

## Mejora de la Papelera de reciclaje: Grabado en el flujo de actualización y recibir notificación por correo electrónico

Se agregaron las siguientes mejoras al restaurar proyectos, tareas y problemas eliminados:

* Ahora recibe una notificación por correo electrónico después de restaurar un objeto.\
   Como administrador de Workfront, ahora recibirá una notificación por correo electrónico después de restaurar un proyecto, tarea o problema que se haya eliminado anteriormente. La notificación por correo electrónico le informa sobre el estado del proceso de restauración.\
   Para obtener más información sobre la restauración de objetos en Workfront, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Cuando se restaura el objeto, la eliminación y restauración del objeto se registran ahora en el flujo de actualización del propio objeto y en el flujo de actualización del objeto principal.\
   Anteriormente, solo la eliminación se registraba en el flujo de actualización del objeto principal.\
   Por ejemplo, cuando se restaura la tarea, se añade un mensaje al flujo de actualización del proyecto y de la propia tarea, indicando que esta se ha restaurado. (Las eliminaciones y restores no se registran en las subtareas. La información sobre las eliminaciones y restores de subtareas solo está disponible en las tareas principales).\
   Para obtener más información, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Cuadro de diálogo actualizado para administrar la pertenencia a un grupo

Hay una nueva interfaz para la administración de Grupos y Subgrupos que ofrece una experiencia más fácil y fácil de usar.

El campo Propietarios del grupo y el campo Miembros del grupo ahora se combinan en un solo campo, con una lista de miembros del grupo a continuación. Además, puede filtrar la lista de miembros del grupo y cambiar si son propietarios o miembros. 

Para obtener más información sobre cómo agregar subgrupos a grupos, así como designar usuarios como miembros o propietarios de grupos, consulte [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) y [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Copiar texto en la aplicación móvil

Puede copiar texto en los campos siguientes de todos los objetos visibles en la aplicación móvil:

* Nombre
* Descripción
* Número de referencia
* Comentarios

Esta funcionalidad debe lanzarse a las tiendas de aplicaciones de iOS y Android durante la semana del 13 de febrero.
