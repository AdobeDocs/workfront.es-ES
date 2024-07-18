---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Mejoras de proyectos en 2019.3
description: Esta página describe todos los cambios realizados en las mejoras de Project con la versión 2019.3. Se publicó en el entorno de producción la semana del 19 de agosto de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Mejoras de proyectos en 2019.3

Esta página describe todos los cambios realizados en las mejoras de Project con la versión 2019.3. Se publicó en el entorno de producción la semana del 19 de agosto de 2019.

Para obtener una lista de todos los cambios realizados en 2019.3, consulte [Resumen de la actividad de la versión 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Cambiar el tipo de visualización de un campo en un formulario personalizado

Ahora puede cambiar el tipo de visualización de un campo en un formulario personalizado.

Por ejemplo, si ha creado un campo Casillas de verificación, puede cambiarlo a un campo Desplegable o a un campo Botones de opción. Estos tres tipos de visualización de campo son intercambiables.

O bien, si ha creado un campo de texto de una sola línea, puede cambiarlo a un campo de texto de párrafo. Estos dos tipos de visualización de campo son intercambiables.

Anteriormente, para cambiar el tipo de visualización de un campo personalizado, se tenía que crear un nuevo campo y eliminar el antiguo. Esto requería la transferencia de datos, lo que a menudo llevaba mucho tiempo.

>[!NOTE]
>
>Disponibilidad de vista previa: 9 de agosto de 2019
>
>Disponibilidad de producción: 30 de agosto de 2019

## Creación de calendarios e informes de días libres

Ahora puede ver el tiempo libre del usuario para una mejor planificación y ejecución. También puede agregar nuevos informes y calendarios de días libres a sus paneles para obtener una vista en tiempo real de la disponibilidad del usuario.

>[!NOTE]
>
>Disponibilidad de vista previa: 9 de agosto de 2019
>
>Disponibilidad de producción: 30 de agosto de 2019

## El filtro Abrir ahora muestra más resultados en una lista de Problemas

Al aplicar el filtro Abrir a una lista de problemas, la lista incluye problemas que:

* Está en estado Cerrado - Pendiente de aprobación
* Están asociados a un objeto de resolución

Antes de este cambio, estos problemas no se incluían en la lista al aplicar el filtro Abrir.

## Nueva experiencia al editar en línea información en listas

Cuando edita en línea información en las nuevas listas, las filas que se han editado se atenúan, pero la información permanece visible. Antes de este cambio, las filas editadas estaban atenuadas y la información no era visible.

Puede encontrar las nuevas listas en las siguientes áreas de Workfront:

* Listas de proyectos y tareas
* Pestaña Horas para proyectos, tareas y problemas

## Listas actualizadas para las fichas de horas de proyecto, tarea y problemas

Las vistas de lista mejoradas ahora están disponibles en las pestañas Horas de los proyectos, tareas y problemas.

Antes de esta mejora, las nuevas listas se aplicaban únicamente a lo siguiente:

* Una lista de tareas
* Una lista de proyectos

Para obtener información sobre cómo ver elementos en una lista, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Editar Gantt sin activar un modo especial de edición

Ahora puede editar el gráfico Gantt de lista de tareas cuando el guardado automático esté habilitado o no. No se pueden deshacer los cambios cuando la opción está activada. En este caso, los cambios realizados en el proyecto se guardan automáticamente.

Para obtener información acerca de cómo editar el gráfico Gantt de lista de tareas, vea [Actualizar información en el gráfico Gantt de lista de tareas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Eliminación de la pestaña Problemas del Panel Kanban

Se está eliminando la pestaña Problemas del panel Kanban de la versión de producción 19.3. Puede seguir accediendo a la subpestaña Problemas desde el Registro de asuntos pendientes del panel Kanban.

## Eliminación de las pestañas Documentos y Problemas de la página de detalles de iteración

>[!NOTE]
>
>Este cambio se producirá en Producción con la versión 2019.3. No se realizará en el entorno de vista previa antes del lanzamiento de producción.

Se están eliminando las fichas Documentos y Problemas de la página de detalles de iteración Agile:

* **Documentos:** Todos los documentos almacenados en la ficha Documentos deben moverse antes de la versión de producción. Si no mueve sus documentos, ya no tendrá acceso a ellos.
* **Problemas:** Esta ficha se encuentra generalmente en el menú desplegable Más. Puede seguir accediendo a la subpestaña Problemas desde la pestaña Elementos de trabajo en la iteración.

## Tener en cuenta o ignorar los días libres del usuario en las fechas de tareas

Ahora puede decidir si desea permitir el tiempo libre programado de la Persona principal asignada de una tarea para ajustar las fechas planificadas.

Puede tomar esta decisión en el nivel del sistema, como administrador de Workfront o en el nivel de proyecto, como administrador de proyectos.

Antes de este cambio, el tiempo libre de la persona asignada principal siempre ajustaba las fechas planificadas de la tarea, si la restricción de tarea permite modificar las fechas.

Para obtener información sobre la configuración de tiempo libre del usuario en el nivel de sistema, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obtener información sobre la configuración de tiempo libre del usuario en el nivel de proyecto, consulte [Editar proyectos](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Disponibilidad de vista previa: 22 de julio de 2019
>
>Disponibilidad de producción: 9 de agosto de 2019

## Condiciones personalizadas

Ahora puede hacer lo siguiente para personalizar las condiciones que utiliza para proyectos, tareas y problemas y satisfacer mejor las necesidades de su organización:

* Cree condiciones personalizadas con sus propias etiquetas y colores.
* Cambie el orden de las condiciones en las listas desplegables donde los usuarios las seleccionan.
* Utilice las condiciones personalizadas que cree en lugar de las condiciones predeterminadas integradas que Workfront asigna automáticamente a los elementos de trabajo.
* Cambie los nombres y colores de las Condiciones predeterminadas integradas para proyectos, tareas y problemas.

Además, si tiene derechos para editar una tarea o un problema pero no se le ha asignado (tal vez porque la está supervisando), ahora puede cambiar su Condición mediante la columna Condiciones en una vista de lista.

Anteriormente, las condiciones no se podían personalizar ni cambiar, y solo los usuarios podían cambiar la condición de una tarea o problema si se les asignaba.

Para obtener más información, consulte [Condiciones personalizadas](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Disponibilidad de vista previa: 4 de julio de 2019
>
>Disponibilidad de producción: finales de septiembre o principios de octubre

## Nueva notificación por correo electrónico para equipos

Hay una nueva notificación de eventos de correo electrónico para los equipos. Los integrantes del equipo reciben una notificación por correo electrónico cuando se activa un proyecto con tareas asignadas a su equipo. Esta configuración está desactivada de forma predeterminada.

Anteriormente, los integrantes del equipo no podían recibir notificaciones cuando se activaban proyectos en los que estaban.

Para obtener más información, consulte Notificaciones: Información sobre proyectos en los que participo.

>[!NOTE]
>
>Disponibilidad de vista previa: 4 de julio de 2019
>
>Disponibilidad de producción: 18 de julio de 2019

## Las actualizaciones de documentos ahora aparecen en el objeto y proyecto asociados

Al realizar comentarios en un documento, la actualización aparece ahora en la ficha Actualizaciones tanto para el documento como para el objeto donde está adjunto.

Si el objeto forma parte de un proyecto, el comentario del documento también aparecerá en la ficha Actualizaciones del proyecto.

Anteriormente, los comentarios de actualización solo aparecían en la pestaña Actualizaciones del documento.

Para obtener más información, consulte la sección [Actualización del trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) en el artículo [Actualización del trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Disponibilidad previa: 6 de junio de 2019
>
>Disponibilidad de producción: 20 de junio de 2019

## Visibilidad del horario de descanso de un usuario al asignarlo a tareas y problemas

Al asignar un usuario a una tarea o un problema, ahora puede ver una advertencia en línea si el usuario seleccionado tiene tiempo libre programado en cualquier momento entre las fechas planificadas de la tarea o el problema.

Para obtener información sobre cómo asignar tareas, vea [Asignar tareas](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Para obtener información sobre los días libres, consulte [Configurar los días libres personales](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Disponibilidad previa: 30 de mayo de 2019
>
>Disponibilidad de producción: 13 de junio de 2019

## Agregar campos que representen objetos en Forms personalizado

Hemos creado un nuevo tipo de campo en el generador de formularios personalizado llamado Escritura anticipada. Este campo permite agregar campos que representan objetos a los formularios personalizados. Actualmente, el objeto Usuario está habilitado con Escritura anticipada y otros objetos aparecerán más adelante.

Anteriormente, los administradores tenían que mantener manualmente a los usuarios como opciones individuales en los menús desplegables de formularios personalizados.

>[!NOTE]
>
>Disponibilidad previa: 30 de mayo de 2019
>
>Disponibilidad de producción: 13 de junio de 2019
>
>Antes de la fecha de lanzamiento de Producción, los nuevos campos personalizados no eran compatibles con Mobile, Outlook, MS Teams ni con la integración nativa de Salesforce.
>
>En Producción, ahora se admiten Outlook y MS Teams. Mobile ha recibido asistencia desde finales de junio o principios de julio; las integraciones de Salesforce lo han hecho desde junio.

## Se cambió el nombre del nuevo campo de solicitud &quot;Asunto&quot; a &quot;Nombre&quot;

>[!NOTE]
>
>Esta función se ha eliminado y no se incluirá en la versión 2019.3.

Ahora, cuando envíe una nueva solicitud a una Cola de solicitudes, introduzca el nombre de la solicitud en el campo &quot;Nombre&quot; del nuevo formulario de solicitud.

Antes de este cambio, debe introducir el nombre de la solicitud en el campo &quot;Asunto&quot;.

Para obtener información sobre cómo crear solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

