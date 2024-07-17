---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa 1 y 2 de R1
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con las versiones R1.1 y R1.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 19 de enero de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%

---

# Vista previa 1 y 2 de R1

Esta página describe todos los cambios disponibles en el entorno de vista previa con las versiones R1.1 y R1.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 19 de enero de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [Descripción general de la actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Restaurar proyectos, tareas y problemas desde la papelera de reciclaje 

Los administradores de Workfront ahora pueden restaurar proyectos, tareas y problemas que se hayan eliminado en los últimos 30 días. Se restaura toda la información asociada con el proyecto, la tarea o el problema, incluidos los documentos y los datos personalizados.

También hay nuevas opciones disponibles para configurar qué sucede con las horas registradas en un proyecto, tarea o problema que se elimina. Para obtener más información, vea [Configurar el efecto en horas cuando se elimina y restaura un objeto](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Para obtener más información acerca de cómo restaurar objetos en Workfront, vea [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obtener información sobre cómo ver proyectos, tareas y problemas que se han restaurado recientemente, vea [Ver elemento restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## El diagrama de aprobación muestra la representación visual de los pasos de aprobación anteriores, actuales y futuros

Ahora, cuando una aprobación está pendiente en un proyecto, tarea o problema, se muestra un diagrama. El diagrama de aprobación muestra el paso actual del proceso de aprobación (que está pendiente) y también le permite ver rápidamente los pasos de aprobación anteriores y futuros sin ir a la pestaña Approvals.

Antes de este cambio, la información sobre los pasos de aprobación estaba disponible solamente en la pestaña Aprobaciones dentro del proyecto, tarea o problema y se mostraba solamente en una vista de lista en lugar de en una vista de diagrama. (Esta información sigue disponible y sin cambiar en la pestaña Approvals ).

En los proyectos, la información de aprobación se muestra en el encabezado junto al título del proyecto. En las tareas y los problemas, la información de aprobación se muestra en el panel derecho.

Para obtener más información, consulte [Aprobación de trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en  [Aprobando trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurar objetos que se van a actualizar y que tengan aprobación pendiente

Cuando un proyecto, tarea o problema tiene la aprobación pendiente, ahora puede configurar si los usuarios pueden:

* Editar el formulario personalizado de un proyecto, tarea o problema que esté pendiente de aprobación.\
  Para obtener información acerca de cómo configurar proyectos, tareas y problemas que se deben editar cuando están pendientes de aprobación, vea [Configurar la aprobación global](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Agregar problemas a un proyecto que está pendiente de aprobación.\
  Para obtener información sobre cómo configurar proyectos para permitir que los usuarios agreguen problemas cuando el proyecto está pendiente de aprobación, consulte [Configurar preferencias de proyectos en todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Editar tareas y problemas dentro de un proyecto que está pendiente de aprobación.\
  Para obtener información acerca de cómo configurar proyectos para permitir que los usuarios editen tareas y problemas cuando el proyecto está pendiente de aprobación, vea [Configurar las preferencias de proyectos en todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Antes de este cambio, los proyectos, las tareas y los problemas cuya aprobación estaba pendiente no se podían editar; asimismo, los problemas no se podían añadir a proyectos cuya aprobación estaba pendiente y las tareas y los problemas no se podían editar dentro de proyectos cuya aprobación estaba pendiente.

## Asignar plantillas de diseño a grupos

Ahora puede asignar plantillas de diseño a grupos.

Antes de este cambio, podía asignar plantillas de diseño a usuarios, equipos y funciones del puesto. Al asignar una plantilla de diseño a grupos, se obtiene la clasificación más baja en la prioridad de asignación de plantillas de diseño. 

Para obtener más información, consulte &quot;Creación y administración de plantillas de diseño&quot;.

## Cambios en las notificaciones de usuario de edición masiva

La funcionalidad ha cambiado la edición por lotes de la configuración de las notificaciones por correo electrónico de los usuarios. Cuando selecciona varios usuarios para editar su configuración de correo electrónico de notificación, solo cambian las notificaciones específicas que está actualizando para todos los usuarios seleccionados. Todos los ajustes de notificación por correo electrónico sin modificar siguen siendo los mismos para todos los usuarios seleccionados, aunque sean diferentes de un usuario a otro. 

Antes de este cambio, se guardaba la configuración de notificaciones por correo electrónico que seleccionó y el resto de configuraciones de notificaciones sin modificar se anulaban al guardar los cambios. 

Para obtener más información, consulte &quot;Modificar la configuración de notificaciones de usuario en lotes&quot; en [Modificar tus propias notificaciones por correo electrónico](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Aspecto actualizado de varias notificaciones por correo electrónico

El aspecto de las siguientes notificaciones por correo electrónico se ha actualizado con una nueva interfaz de usuario:

* Asignación de problema
* Confirmar cambios de fecha
* Se activa un proyecto en el que participo
* Decisión de aprobación a las partes interesadas
* Finalización de una tarea predecesora a dependientes de tareas
* Aprobación pendiente (proyecto, tarea, problemas)
* Cambio de estado en proyectos, tareas y problemas

Recuerde actualizar la dirección de correo electrónico asociada a la cuenta para poder probar esta funcionalidad, ya que la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios.    Para obtener más información sobre las notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nuevas opciones de resumen de correo electrónico para varias áreas de notificaciones

Se ha agregado la opción &quot;Resumen diario&quot; a las áreas de notificaciones siguientes:

* Información sobre proyectos en los que participo
* Información sobre proyectos que patrocino
* Información de aprobación
* Información sobre trabajo asignado a mí
* Comunicación

Para obtener más información, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  Recuerde actualizar la dirección de correo electrónico asociada a la cuenta para poder probar esta funcionalidad, ya que la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios. 

## Convertir un grupo en público

Cuando hace público un grupo, ahora puede agregar ese grupo a los usuarios sin ser el propietario de un grupo. Deberá tener acceso administrativo de usuario para poder editar usuarios.

Para obtener más información sobre cómo convertir un grupo en público, consulte la sección [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Compartir la URL de un objeto en la aplicación móvil 

Ahora puede compartir la URL en los siguientes objetos de la aplicación móvil de Workfront:

* Proyectos
* Tareas
* Problemas
* Hojas de horas
* Documentos

Puede compartir la URL de un objeto en las siguientes aplicaciones:

* Mensaje de texto
* Correo electrónico
* Unidad de almacenamiento (por ejemplo, iCloud Drive)
* Otra aplicación instalada (por ejemplo, Notes, Facebook)
* Puede copiar un vínculo al objeto en el portapapeles y pegarlo más adelante en cualquier otra aplicación. 

## Ayuda contextual en la configuración

Todas las áreas del menú Configuración se han actualizado con un icono Ayuda en la esquina superior derecha del área. Este icono proporciona un vínculo a un artículo del sitio de ayuda sobre esa área. Algunas secciones dentro de las áreas de Configuración también se han actualizado con el icono Ayuda. 

## Agregar tasas de gastos más precisas

Ahora puede agregar tasas de gastos más exactas al crear tipos de gastos. Las tasas de gasto pueden contener hasta 4 caracteres después del decimal (por ejemplo, 1,0375). Esto significa que cualquier campo que utilice esta tasa puede ser más preciso.

Antes de este cambio, las tasas de gasto solo podían contener hasta 2 caracteres después del decimal (por ejemplo, 1,03).

Para obtener más información sobre cómo crear tasas de gastos, vea [Crear tipos de gastos personalizados](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Seminario web de grabación de la versión R1 Preview 1 y 2

Este seminario web fue presentado por el equipo de preparación para la versión de Workfront el 19 de enero de 2017. Este seminario web se centró en los cambios de la versión en 2017 y abarcó las nuevas funcionalidades disponibles para probar en Vista previa.
