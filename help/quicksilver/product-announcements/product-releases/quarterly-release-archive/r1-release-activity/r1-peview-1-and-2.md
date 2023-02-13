---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa 1 y 2 de R1
description: Esta página describe todos los cambios disponibles en el entorno de Vista previa con las versiones R1.1 y R1.2. La funcionalidad de esta página estuvo disponible en el entorno de vista previa el 19 de enero de 2017.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# Vista previa 1 y 2 de R1

Esta página describe todos los cambios disponibles en el entorno de Vista previa con las versiones R1.1 y R1.2. La funcionalidad de esta página estuvo disponible en el entorno de vista previa el 19 de enero de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [Información general sobre la actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Restaurar proyectos, tareas y problemas desde la papelera de reciclaje 

Los administradores de Workfront ahora pueden restaurar proyectos, tareas y problemas que se han eliminado en los últimos 30 días. Se restaura toda la información asociada con el proyecto, la tarea o el problema, incluidos los documentos y los datos personalizados.

También hay nuevas opciones disponibles para configurar lo que sucede con las horas que se registran en un proyecto, tarea o problema que se elimina. Para obtener más información, consulte [Configurar el efecto en horas en las que se elimina y se restaura un objeto](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Para obtener más información sobre la restauración de objetos en Workfront, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obtener información sobre cómo ver proyectos, tareas y problemas que se han restaurado recientemente, consulte [Ver elemento restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Diagrama de aprobación muestra la representación visual de los pasos de aprobación anteriores, actuales y futuros

Ahora, cuando una aprobación está pendiente en un proyecto, tarea o problema, se muestra un diagrama. El diagrama de aprobación muestra el paso actual del proceso de aprobación (que está pendiente) y también le permite ver rápidamente los pasos de aprobación anteriores y futuros sin tener que navegar a la pestaña Aprobaciones .

Antes de este cambio, la información sobre los pasos de aprobación solo estaba disponible en la pestaña Approvals del proyecto, la tarea o el problema, y solo se mostraba en una vista de lista en lugar de en una vista de diagrama. (Esta información sigue disponible y no se ha modificado en la pestaña Aprobaciones ).

En los proyectos, la información de aprobación se muestra en el encabezado junto al título del proyecto. En las tareas y los problemas, la información de aprobación se muestra en el panel derecho.

Para obtener más información, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en  [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurar objetos para actualizar que estén pendientes de aprobación

Cuando un proyecto, tarea o problema está pendiente de aprobación, ahora puede configurar si los usuarios pueden:

* Edite la forma personalizada de un proyecto, tarea o problema que esté pendiente de aprobación.\
   Para obtener información sobre cómo configurar proyectos, tareas y problemas que se deben editar cuando están pendientes de aprobación, consulte [Configuración de la aprobación global](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Agregue problemas a un proyecto que esté pendiente de aprobación.\
   Para obtener información sobre cómo configurar proyectos para permitir que los usuarios agreguen problemas cuando el proyecto está pendiente de aprobación, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Edite tareas y problemas dentro de un proyecto que esté pendiente de aprobación.\
   Para obtener información sobre cómo configurar proyectos para permitir que los usuarios editen tareas y problemas cuando el proyecto está pendiente de aprobación, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Antes de este cambio, no se podían editar los proyectos, tareas y problemas que estaban pendientes de aprobación; además, no se podían añadir problemas a proyectos que estaban pendientes de aprobación, y las tareas y los problemas no podían editarse en proyectos que estaban pendientes de aprobación.

## Asignar plantillas de diseño a grupos

Ahora puede asignar plantillas de diseño a grupos.

Antes de este cambio, se podían asignar plantillas de diseño a usuarios, equipos y funciones de trabajo. La asignación de una plantilla de diseño a grupos tiene la clasificación más baja en la prioridad de asignación de plantillas de diseño. 

Para obtener más información, consulte &quot;Creación y administración de plantillas de diseño&quot;.

## Cambios en las notificaciones de usuario de edición masiva

La funcionalidad ha cambiado en torno a la edición masiva de la configuración de notificaciones por correo electrónico del usuario. Cuando selecciona varios usuarios para editar la configuración del correo electrónico de notificación, solo se cambian las notificaciones específicas que está actualizando para todos los usuarios seleccionados. Todos los ajustes de notificación por correo electrónico no modificados son los mismos para todos los usuarios seleccionados, incluso si son diferentes de un usuario a otro. 

Antes de este cambio, la configuración de notificación de correo electrónico que seleccionó se guardaba y el resto de la configuración de notificación sin modificar se anulaba la selección cuando guardó los cambios. 

Para obtener más información, consulte &quot;Modificación de la configuración de notificación de usuario de forma masiva&quot; en [Activar o desactivar sus propias notificaciones de eventos](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Aspecto actualizado de varias notificaciones de correo electrónico

El aspecto de las siguientes notificaciones por correo electrónico se ha actualizado con una nueva interfaz de usuario:

* Asignación de problemas
* Confirmar cambios de fecha
* Se activa un proyecto en el que participo
* Decisión de aprobación a las partes interesadas
* Finalización de una tarea predecesora a dependientes de la tarea
* Pendiente de aprobación (proyecto, tarea, problemas)
* Cambio de estado en proyectos, tareas, problemas

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad, ya que el espacio aislado de vista previa borra las direcciones de correo electrónico de todos los usuarios.    Para obtener más información sobre las notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nuevas opciones de resumen de correo electrónico para varias áreas de notificaciones

Se ha añadido la opción &quot;Resumen diario&quot; a las siguientes áreas de notificaciones:

* Información sobre Proyectos en los que estoy
* Información sobre proyectos que patrocino
* Información de aprobación
* Información sobre trabajo asignado a mí
* Comunicación

Para obtener más información, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad, ya que el espacio aislado de vista previa borra las direcciones de correo electrónico de todos los usuarios. 

## Convertir un grupo en público

Cuando publica un grupo, ahora puede agregarlo a los usuarios sin ser propietario de un grupo. Debe tener acceso de administrador de usuarios para poder editar usuarios.

Para obtener más información sobre cómo hacer público un grupo, consulte la [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Compartir la URL de un objeto en la aplicación móvil 

Ahora puede compartir la URL en los siguientes objetos de la aplicación móvil de Workfront:

* Proyectos
* Tareas
* Problemas
* Plantillas de horas
* Documentos

Puede compartir una URL de un objeto en las siguientes aplicaciones:

* Mensaje de texto
* Correo electrónico
* Unidad de almacenamiento (por ejemplo iCloud Drive)
* Otra aplicación instalada (por ejemplo, Notes, Facebook)
* Puede copiar un vínculo al objeto en el portapapeles y pegarlo más adelante en cualquier otra aplicación. 

## Ayuda contextual en la configuración

Todas las áreas del menú Configuración se han actualizado con un icono Ayuda en la esquina superior derecha del área. Este icono proporciona un vínculo al artículo de un sitio de ayuda sobre esa área. Algunas secciones dentro de las áreas de configuración también se han actualizado con el icono Ayuda. 

## Agregar tasas de gastos más precisas

Ahora puede agregar tasas de gastos más exactas al crear tipos de gastos. Las tasas de gastos pueden contener hasta 4 caracteres después del decimal (por ejemplo, 1.0375). Esto significa que cualquier campo que utilice esta tasa puede ser más preciso.

Antes de este cambio, las tasas de gastos solo podían contener 2 caracteres después del decimal (por ejemplo, 1,03).

Para obtener más información sobre la creación de tasas de gastos, consulte [Crear tipos de gastos personalizados](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Grabación del seminario web sobre la vista previa 1 y la versión 2 de R1

Este seminario web fue presentado por el equipo de preparación para la versión de Workfront el 19 de enero de 2017. Este seminario web se centró en los cambios de la versión de 2017 y abarcó las nuevas funciones que se pueden probar en Vista previa.
