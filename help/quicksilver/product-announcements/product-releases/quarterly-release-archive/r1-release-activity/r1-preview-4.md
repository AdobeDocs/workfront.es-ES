---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa de R1 4
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1.4. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 15 de febrero de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Vista previa de R1 4

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1.4. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 15 de febrero de 2017.

Para ver una lista de todos los cambios realizados en R1, consulte [Versión de Workfront R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Aprobaciones de proyectos, tareas y problemas actualizadas

Al crear procesos de aprobación para aprobaciones de proyectos, tareas y problemas, ya están disponibles las siguientes mejoras y cambios: 

* Los &quot;pasos&quot; de aprobación ahora se denominan &quot;etapas&quot; de aprobación.
* Incluya varios tipos de aprobadores por fase.\
  Esto incluye usuarios, equipos y funciones del puesto.\
  Antes de este cambio, solo podía incluir varios aprobadores del mismo tipo. Por ejemplo, puede incluir varios roles, pero no un rol ni un equipo.

* Se han eliminado las siguientes limitaciones preexistentes relacionadas con la modificación de los procesos de aprobación globales existentes:

   * El proceso de aprobación modificado solo se refleja en objetos de todo el sistema en los que el proceso de aprobación aún no se ha iniciado o en los que no se ha modificado. Los objetos en los que el proceso de aprobación ya se ha iniciado o en los que se ha modificado no se actualizan con los cambios.
   * No puede modificar el estado que determina cuándo se inicia la aprobación.

* Aspecto y presentación actualizados.

Para obtener más información sobre la creación de procesos de aprobación, consulte [Crear un proceso de aprobación para elementos de trabajo](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Al asociar un proceso de aprobación con un proyecto, tarea o problema, ya están disponibles las siguientes mejoras y cambios:

* Aspecto y presentación actualizados.
* El diagrama de aprobación se muestra en la pestaña Aprobaciones y una representación visual de los pasos de aprobación anteriores, actuales y futuros.

Para obtener más información sobre cómo asociar aprobaciones a proyectos, tareas y problemas, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Cambiar el estado de un proyecto directamente desde la página del proyecto

Ya no es necesario editar un proyecto para cambiar su estado. Ahora puede cambiar el estado de un proyecto directamente desde la página principal del proyecto.

Para obtener más información, consulte [Cambiar el estado de un proyecto](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Programar usuarios para desactivación

Ahora puede programar la desactivación de usuarios en una fecha futura.

Antes de esta mejora, solo podía desactivar manualmente un usuario inmediatamente.

Programar la desactivación de un usuario puede ser útil en una variedad de escenarios. Por ejemplo, si crea usuarios en Workfront que se contratan de forma temporal, puede configurarlos para que se desactiven cuando finalice el contrato.

Esta función también está disponible cuando se editan usuarios por lotes. 

Para obtener más información sobre cómo programar usuarios para su desactivación, consulte [Desactivar o reactivar un usuario](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) y [Adición de usuarios](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nuevas opciones de resumen de correo electrónico para &quot;Acciones necesarias&quot;

La opción de envío Resumen diario ya está disponible en el área &quot;Acción necesaria&quot; de la configuración de Notificaciones.

Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios.

## Mejora de la papelera de reciclaje: Registrado en el flujo de actualización y recibido notificaciones por correo electrónico

Se agregaron las siguientes mejoras al restaurar los proyectos, tareas y problemas eliminados:

* Ahora recibe una notificación por correo electrónico después de restaurar un objeto.\
  Como administrador de Workfront, ahora recibirá una notificación por correo electrónico después de restaurar un proyecto, tarea o problema que se haya eliminado anteriormente. La notificación por correo electrónico le informa sobre el estado del proceso de restauración.\
  Para obtener más información sobre la restauración de objetos en Workfront, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Cuando se restaura el objeto, la eliminación y restauración del objeto se registra ahora en el flujo de actualización del propio objeto y en el flujo de actualización del objeto principal.\
  Anteriormente, solo la eliminación se registraba en el flujo de actualización del objeto principal.\
  Por ejemplo, cuando se restaura la tarea, se agrega un mensaje a la secuencia de actualización del proyecto y de la propia tarea, que indica que la tarea se restauró. (Las eliminaciones y restauraciones no se registran en las subtareas. La información relativa a las eliminaciones y restauraciones de subtareas sólo está disponible en las tareas principales.)\
  Para obtener más información, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Cuadro de diálogo actualizado para Administrar la pertenencia a grupos

Hay una nueva interfaz para la administración de grupos y subgrupos que ofrece una experiencia más fácil y fácil de usar.

El campo Propietarios del grupo y el campo Miembros del grupo ahora se combinan en un único campo, con una lista de miembros del grupo a continuación. Además, puede filtrar la lista de miembros del grupo y cambiar si son propietarios o miembros. 

Para obtener más información acerca de cómo agregar subgrupos a grupos y designar usuarios como miembros o propietarios de grupos, consulte [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) y [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Copiar texto en la aplicación móvil

Puede copiar texto en los siguientes campos de todos los objetos visibles en la aplicación móvil:

* Nombre
* Descripción
* Número de referencia
* Comentarios

Esta funcionalidad debería publicarse en las tiendas de aplicaciones de iOS y Android la semana del 13 de febrero.
