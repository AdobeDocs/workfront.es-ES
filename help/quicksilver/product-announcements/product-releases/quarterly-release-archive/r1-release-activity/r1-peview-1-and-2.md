---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa 1 y 2 de R1
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con las versiones R1.1 y R1.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 19 de enero de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
TQID: https://experienceleague.adobe.com/SjemPIUQMpaqkse8vDfjJWaVLtNtritW3M1lcIe6OaM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1024
ht-degree: 91%

---

# Vista previa 1 y 2 de R1

Esta página describe todos los cambios disponibles en el entorno de vista previa con las versiones R1.1 y R1.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 19 de enero de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [Información general de la actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Restaurar proyectos, tareas y problemas de la papelera de reciclaje 

Los administradores de Workfront pueden restaurar ahora proyectos, tareas y problemas que se hayan eliminado en los últimos 30 días. Se restaura toda la información asociada con el proyecto, la tarea o el problema, incluidos los documentos y los datos personalizados.

También hay nuevas opciones disponibles para configurar qué sucede con las horas registradas en un proyecto, tarea o problema que se elimina. Para obtener más información, consulte [Configurar el efecto sobre las horas cuando se elimina y restaura un objeto](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Para obtener más información sobre cómo restaurar objetos en Workfront, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obtener información sobre cómo ver proyectos, tareas y problemas que se han restaurado recientemente, consulte [Ver elemento restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## El diagrama de aprobación muestra la representación visual de los pasos de aprobación anteriores, actuales y futuros

Ahora, cuando una aprobación está pendiente en un proyecto, tarea o problema, se muestra un diagrama. El diagrama de aprobación muestra el paso actual del proceso de aprobación (que está pendiente) y también le permite ver rápidamente los pasos de aprobación anteriores y futuros sin ir a la pestaña Aprobaciones.

Antes de este cambio, la información sobre los pasos de aprobación estaba disponible solamente en la pestaña Aprobaciones dentro del proyecto, tarea o problema y se mostraba solamente en una vista de lista en lugar de en una vista de diagrama. (Esta información sigue disponible y sin cambios en la pestaña Aprobaciones).

En los proyectos, la información de aprobación se muestra en el encabezado junto al título del proyecto. En tareas y problemas, la información de aprobación se muestra en el panel derecho.

Para obtener más información, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurar objetos para actualizar que están pendientes de aprobación

Cuando un proyecto, tarea o problema tiene la aprobación pendiente, ahora puede configurar si los usuarios pueden:

* Edite el formulario personalizado de un proyecto, tarea o problema que esté pendiente de aprobación.\
  Para obtener información acerca de cómo configurar proyectos, tareas y problemas que se deben editar cuando están pendientes de aprobación, consulte [Configuración de la aprobación global](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Añada problemas a un proyecto que está pendiente de aprobación.\
  Para obtener información sobre cómo configurar proyectos para permitir que los usuarios añadan problemas cuando el proyecto está pendiente de aprobación, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Edite tareas y problemas dentro de un proyecto que está pendiente de aprobación.\
  Para obtener información acerca de cómo configurar proyectos para permitir que los usuarios editen tareas y problemas cuando el proyecto está pendiente de aprobación, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Antes de este cambio, los proyectos, tareas y problemas cuya aprobación estaba pendiente no se podían editar; asimismo, los problemas no se podían añadir a proyectos cuya aprobación estaba pendiente y las tareas y los problemas no se podían editar dentro de proyectos cuya aprobación estaba pendiente.

## Asignar plantillas de diseño a grupos

Ahora puede asignar plantillas de diseño a grupos.

Antes de este cambio, podía asignar plantillas de diseño a usuarios, equipos y funciones del puesto. Al asignar una plantilla de diseño a grupos, se obtiene la clasificación más baja en la prioridad de asignación de plantillas de diseño. 

Para obtener más información, consulte “Creación y administración de plantillas de diseño”.

## Cambios en las notificaciones de usuario de edición masiva

La funcionalidad ha cambiado la edición por lotes de la configuración de las notificaciones por correo electrónico de los usuarios. Cuando selecciona varios usuarios para editar su configuración de correo electrónico de notificación, solo cambian las notificaciones específicas que está actualizando para todos los usuarios seleccionados. Todos los ajustes de notificación por correo electrónico sin modificar siguen siendo los mismos para todos los usuarios seleccionados, aunque sean diferentes de un usuario a otro. 

Antes de este cambio, se guardaba la configuración de notificaciones por correo electrónico seleccionada y el resto de configuraciones de notificaciones sin modificar se anulaban al guardar los cambios. 

Para obtener más información, consulte “Modificar la configuración de notificaciones de usuario masiva” en [Modificar sus propias notificaciones por correo electrónico](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Apariencia actualizada de varias notificaciones por correo electrónico

La apariencia de las siguientes notificaciones por correo electrónico se ha actualizado con una nueva interfaz de usuario:

* Asignación de un problema
* Cambios en la fecha de confirmación
* Se activa un proyecto en el que participo
* Decisión de aprobación a las partes interesadas
* Finalización de las tareas predecesoras a dependientes de tareas
* Aprobación pendiente (proyecto, tarea, problemas)
* Cambio de estado en proyectos, tareas y problemas

Recuerde actualizar la dirección de correo electrónico asociada a la cuenta para poder probar esta funcionalidad, ya que la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios.    Para obtener más información sobre las notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nuevas opciones de resumen de correo electrónico para varias áreas de notificaciones

Se ha añadido la opción “Resumen diario” a las áreas de notificaciones siguientes:

* Información sobre proyectos en los que participo
* Información sobre proyectos que patrocino
* Información de aprobación
* Información sobre trabajo asignado a mí
* Comunicación

Para obtener más información, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md). Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad, ya que la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios. 

## Hacer público un grupo

Cuando se hace público un grupo, ahora se puede añadir ese grupo a los usuarios sin necesidad de ser su propietario. Deberá tener acceso administrativo de usuario para poder editar usuarios.

Para obtener más información sobre cómo se hace público un grupo, consulte la sección [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Compartir la URL de un objeto en la aplicación móvil 

Ahora puede compartir la URL en los siguientes objetos de la aplicación móvil de Workfront:

* Proyectos
* Tareas
* Problemas
* Hojas de horas
* Documentos

Puede compartir la URL de un objeto en las siguientes aplicaciones:

* Mensajes de texto
* Correo electrónico
* Unidad de almacenamiento (por ejemplo, iCloud Drive)
* Otra aplicación instalada (por ejemplo, Notes, Facebook)
* Puede copiar un vínculo al objeto en el portapapeles y pegarlo más adelante en cualquier otra aplicación. 

## Ayuda contextual en la configuración

Todas las áreas del menú Configuración se han actualizado con un icono Ayuda en la esquina superior derecha del área. Este icono proporciona un vínculo a un artículo del sitio de ayuda sobre esa área. Algunas secciones dentro de las áreas de Configuración también se han actualizado con el icono Ayuda. 

## Añadir tasas de gasto más precisas

Ahora puede añadir tasas de gasto más exactas al crear tipos de gastos. Las tasas de gasto pueden contener hasta 4 caracteres después del decimal (por ejemplo, 1,0375). Esto significa que cualquier campo que utilice esta tasa puede ser más preciso.

Antes de este cambio, las tasas de gasto solo podían contener hasta 2 caracteres después del decimal (por ejemplo, 1,03).

Para obtener más información sobre la creación de tasas de gasto, consulte [Crear tipos de gastos personalizados](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Grabación del seminario web sobre la versión R1 Preview 1 y 2

El equipo de preparación de la versión de Workfront presentó este seminario web el 19 de enero de 2017. Este seminario web se centró en los cambios de la versión de 2017 y abarcó las nuevas funcionalidades disponibles para realizar pruebas en vista previa.
