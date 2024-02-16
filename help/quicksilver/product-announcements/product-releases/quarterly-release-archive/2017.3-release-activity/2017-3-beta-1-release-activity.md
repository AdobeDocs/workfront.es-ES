---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión beta 1 de 2017.3
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2017.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 9 de agosto de 2017. Estará disponible en el entorno de producción a principios de noviembre de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# Actividad de la versión beta 1 de 2017.3

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2017.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 9 de agosto de 2017. Estará disponible en el entorno de producción a principios de noviembre de 2017.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2017.3, consulte  [información general sobre la actividad de la versión 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versión beta 1 de 2017.3 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Evitar que se eliminen tareas y problemas al registrar las horas](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Eliminación de la configuración &quot;Acceso anticipado&quot; del área de instalación](#removal-of-the-early-access-setting-from-the-setup-area)
* [Cambio de dirección de correo electrónico predeterminada de Workfront](#workfront-default-email-address-change)

**Para todos los usuarios:**

* [Mejoras en Resource Scheduling](#resource-scheduling-improvements)
* [Pantalla panorámica](#widescreen-display)
* [Cambiar el tamaño y reordenar columnas en informes y listas](#resize-and-reorder-columns-in-reports-and-lists)
* [Opción Borrar datos personalizados al copiar tareas y problemas](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Crear un proyecto directamente a partir de una plantilla](#create-a-project-directly-from-a-template)
* [Notificación en la aplicación para objetos suscritos](#in-app-notification-for-subscribed-objects)
* [@Tagging actualmente no disponible en el entorno de vista previa](#tagging-currently-not-available-in-the-preview-environment)
* [Incluir información de asignación de usuarios en el informe de utilización de un proyecto](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Mejoras en Resource Scheduling {#resource-scheduling-improvements}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Las siguientes mejoras en la programación de recursos están disponibles cuando se programan recursos para un equipo, para un proyecto o para varios proyectos como jefe de recursos:

* [Ver área de programación en modo de pantalla completa](#view-scheduling-area-in-full-screen-mode)
* [Más Opciones de Intervalo de Fechas para Ver el Área de Programación de Recursos](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Ver fechas proyectadas en la línea de tiempo de programación](#view-projected-dates-on-the-scheduling-timeline)

### Ver área de programación en modo de pantalla completa {#view-scheduling-area-in-full-screen-mode}

Puede ver la cronología de la programación en modo de pantalla completa, lo que le permite ver más información en una sola vista. 

Para obtener más información, consulte Introducción a la programación de recursos.

### Más Opciones de Intervalo de Fechas para Ver el Área de Programación de Recursos {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Puede ver las siguientes opciones de intervalo de fechas adicionales al ver la cronología de la programación:

* Vista de un solo día
* Vista de 4 semanas
* Vista de 6 semanas

Antes de este cambio, la cronología de la programación solo se podía ver en una vista de 1, 2 o 3 semanas. Estos intervalos de fechas siguen estando disponibles además de los nuevos intervalos de fechas.

Cuando ve la cronología de la programación en una vista de un solo día, no se pueden mostrar las asignaciones de usuarios (incluidas las horas totales diarias).

Para obtener más información, consulte Introducción a la programación de recursos.

### Ver fechas proyectadas en la línea de tiempo de programación {#view-projected-dates-on-the-scheduling-timeline}

Ahora puede configurar la cronología de la programación para mostrar las fechas proyectadas en lugar de las fechas planificadas para las tareas y los problemas. 

Antes de este cambio, las tareas y los problemas de la cronología de programación solo mostraban las fechas planificadas.

Cuando vea Fechas proyectadas en la escala de tiempo de la programación, no se podrán mostrar las asignaciones de usuarios (incluyendo las horas totales diarias).

Para obtener más información, consulte Introducción a la programación de recursos.

## Pantalla panorámica {#widescreen-display}

Cuando se muestra cualquiera de los siguientes objetos en Workfront, toda la ventana del explorador se rellena automáticamente:

* Proyectos
* Tareas
* Problemas
* Informes
* Paneles
* Calendarios

Antes de este cambio, había dos barras laterales blancas a cada lado del área mostrada. Ahora, la vista panorámica se ajusta dinámicamente a la anchura de la pantalla y de la ventana del explorador.

## Cambiar el tamaño y reordenar columnas en informes y listas {#resize-and-reorder-columns-in-reports-and-lists}

Ahora puede reordenar y cambiar el tamaño de las columnas de un informe o una lista, sin tener que editar el informe. (Esta funcionalidad se eliminó con la desaprobación del entorno de acceso anticipado a principios de este año. Ahora se está reintroduciendo).

Esta funcionalidad no está disponible para listas de tableros o informes, ya que esas listas se han rediseñado en una nueva estructura de cuadrícula de datos. Todas las demás listas tendrán esta funcionalidad habilitada con esta versión.

Para obtener más información sobre cómo cambiar el tamaño y reordenar las columnas, consulte [Modificar el ancho y el orden de las columnas](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Opción Borrar datos personalizados al copiar tareas y problemas {#clear-custom-data-option-when-copying-tasks-and-issues}

Al copiar una tarea o un problema, ahora puede seleccionar una opción para borrar cualquier dato personalizado. Cuando borra los datos personalizados de una tarea o problema, el formulario se copia en el nuevo elemento, pero los datos personalizados del formulario no. Borrar datos personalizados también afecta a los formularios personalizados adjuntos a los documentos adjuntos a los elementos o a los formularios personalizados adjuntos a los gastos de la tarea.

Antes de este cambio, los datos personalizados incluidos en un formulario personalizado también se copiaban al nuevo elemento cuando se copiaba la tarea o el problema. 

Para obtener más información sobre cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener más información sobre cómo copiar problemas, consulte [Copiar problemas](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Crear un proyecto directamente a partir de una plantilla {#create-a-project-directly-from-a-template}

Ahora puede crear un proyecto a partir de una plantilla, en el nivel de plantilla.

Antes de este cambio, solo podía crear un proyecto a partir de una plantilla en la pestaña Proyectos del área de Workfront, utilizando **Nuevo proyecto a partir de plantilla** opción.

Para obtener más información sobre la creación de un proyecto a partir de una plantilla, consulte [Creación de un proyecto con una plantilla](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Evitar que se eliminen tareas y problemas al registrar las horas {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Ahora puede configurar Workfront para permitir o evitar la eliminación de tareas y problemas que tienen horas registradas.

Antes de este cambio, cuando eliminaba una tarea o un problema en el que se registraban horas, las horas se eliminaban con la tarea o el problema o se movían al proyecto, según la plantilla de horas y las preferencias de horas.

Para obtener más información sobre la eliminación de tareas, consulte [Eliminar tareas](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Para obtener más información sobre la eliminación de problemas, consulte [Eliminar problemas](../../../../manage-work/issues/manage-issues/delete-issues.md).

Para obtener más información sobre cómo habilitar la configuración del sistema para la eliminación de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Eliminación de la configuración &quot;Acceso anticipado&quot; del área de instalación {#removal-of-the-early-access-setting-from-the-setup-area}

Se está eliminando la configuración que permitía a los administradores de Workfront inscribir a usuarios para participar en el entorno de acceso anticipado. Esta funcionalidad ha quedado obsoleta desde finales de 2016. No hemos lanzado ninguna funcionalidad nueva para Acceso anticipado en 2017 y todas las funciones que permanecían en ese entorno se han trasladado a Producción.

Antes de este cambio, los administradores de Workfront aún podían agregar usuarios al entorno de acceso anticipado, aunque no había nuevas funciones a las que acceder.

## Cambio de dirección de correo electrónico predeterminada de Workfront {#workfront-default-email-address-change}

La dirección de correo electrónico predeterminada para el correo saliente de Workfront ha cambiado de [noreply@attask.com](mailto:noreply@attask.com) hasta [noreply@my.workfront.com](mailto:noreply@workfront.com).

Si actualmente filtra los correos electrónicos enviados desde Workfront, debe cambiar el filtro para reflejar la nueva dirección predeterminada. 

El cambio en la dirección predeterminada no afecta a las direcciones de correo electrónico configuradas de Workfront. 

Para obtener más información, consulte .

## Notificación en la aplicación para objetos suscritos {#in-app-notification-for-subscribed-objects}

Cuando un usuario realiza un comentario sobre proyectos, tareas y problemas a los que está suscrito, ahora recibe una notificación en la aplicación. Para obtener más información sobre las notificaciones en la aplicación de suscripción, consulte [Visualización y administración de notificaciones en la aplicación](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Según las funciones que haya habilitado el administrador de Workfront, también puede recibir notificaciones por correo electrónico de los elementos suscritos. Puede cancelar fácilmente la suscripción de un artículo mediante un vínculo en un correo electrónico de suscripción, tal como se describe en [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Antes de este cambio, siempre recibía una notificación por correo electrónico de los elementos suscritos y no había ninguna opción de recibir una notificación en la aplicación.

Aunque puede desactivar el correo electrónico de suscripción, no puede desactivar las notificaciones en la aplicación para los elementos suscritos. Para obtener más información, consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Para obtener más información sobre la suscripción a elementos, consulte [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Tagging actualmente no disponible en el entorno de vista previa {#tagging-currently-not-available-in-the-preview-environment}

Mientras trabajamos para incorporar la funcionalidad de formato de texto enriquecido al flujo de actualización, temporalmente no podrá utilizar el símbolo @ para etiquetar a otros usuarios en el flujo de actualización para los siguientes objetos en el entorno de vista previa:

* Proyecto
* Tarea
* Problema
* Hoja de horas

Puede seguir etiquetando a otros haciendo clic en el **Incluir a otros en esta actualización** icono.

Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Incluir información de asignación de usuarios en el informe de utilización de un proyecto {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

El informe de utilización de un proyecto ahora tiene en cuenta si las horas planificadas se han reasignado a lo largo de la duración de una tarea. Cuando se modifica la asignación de usuarios para las horas (como se describe en &quot;Administrar asignaciones de usuarios en las áreas de programación&quot;), los datos del informe de utilización pueden verse afectados si las fechas seleccionadas en el informe de utilización contienen solo una parte de una tarea.

Para obtener más información, consulte [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
