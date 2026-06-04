---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: '2019.3: Mejoras en los proyectos'
description: Esta página describe todos los cambios realizados en las mejoras de proyectos con la versión 2019.3. Se publicó en el entorno de producción la semana del 19 de agosto de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
TQID: https://experienceleague.adobe.com/f-IlcpRr2VY8bfdWtfKWs5snkxwPocgPgKgeEi5Nvms
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1385
ht-degree: 100%

---

# 2019.3: Mejoras en los proyectos

Esta página describe todos los cambios realizados en las mejoras de proyectos con la versión 2019.3. Se publicó en el entorno de producción la semana del 19 de agosto de 2019.

Para obtener una lista de todos los cambios realizados en 2019.3, consulte [Información general de la actividad de la versión 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Cambiar el tipo de visualización de un campo en un formulario personalizado

Ahora puede cambiar el tipo de visualización de un campo en un formulario personalizado.

Por ejemplo, si ha creado un campo Casillas de verificación, puede cambiarlo por un campo Desplegable o por un campo Botones de opción. Estos tres tipos de visualización de campo son intercambiables.

O bien, si ha creado un campo de texto de una única línea, puede cambiarlo por un campo de texto de párrafo. Estos dos tipos de visualización de campo son intercambiables.

Anteriormente, para cambiar el tipo de visualización de un campo personalizado, se tenía que crear un nuevo campo y eliminar el antiguo. Esto requería transferir datos, lo que a menudo llevaba mucho tiempo.

>[!NOTE]
>
>Disponibilidad de vista previa: 9 de agosto de 2019
>
>Disponibilidad de producción: 30 de agosto de 2019

## Creación de calendarios e informes de días libres

Ahora puede ver el tiempo libre del usuario para una mejor planificación y ejecución. También puede añadir nuevos informes y calendarios de días libres a sus paneles de control para obtener una vista en tiempo real de la disponibilidad del usuario.

>[!NOTE]
>
>Disponibilidad de vista previa: 9 de agosto de 2019
>
>Disponibilidad de producción: 30 de agosto de 2019

## El filtro Abrir ahora muestra más resultados en una lista de problemas

Al aplicar el filtro Abrir a una lista de problemas, la lista incluye los siguientes problemas:

* Están en un estado Cerrado: pendiente de aprobación
* Están asociados a un objeto de resolución

Antes de este cambio, estos problemas no se incluían en la lista al aplicar el filtro Abrir.

## Nueva experiencia al editar en línea información en listas

Cuando edita en línea información en las nuevas listas, las filas que se han editado se atenúan, pero la información permanece visible. Antes de este cambio, las filas editadas aparecían en gris y la información no era visible.

Puede encontrar las nuevas listas en las siguientes áreas de Workfront:

* Listas de proyectos y tareas
* Pestaña Horas para proyectos, tareas y problemas

## Listas actualizadas de las pestañas Horas para proyectos, tareas y problemas

Las vistas de lista mejoradas ahora están disponibles en las pestañas Horas para proyectos, tareas y problemas.

Antes de esta mejora, las nuevas listas se aplicaban únicamente a lo siguiente:

* Una lista de tareas
* Una lista de proyectos

Para obtener información sobre la visualización de elementos en una lista, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Editar Gantt sin habilitar un modo de edición especial

Ahora puede editar el gráfico Gantt de lista de tareas cuando el guardado automático está habilitado o no. No puede deshacer los cambios cuando la opción está activada. En este caso, los cambios realizados en el proyecto se guardan automáticamente.

Para obtener información sobre la edición del gráfico Gantt de lista de tareas, consulte [Actualizar información en el gráfico Gantt de la lista de tareas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Eliminación de la pestaña Problemas del tablero Kanban

Estamos eliminando la pestaña Problemas del tablero Kanban de la versión de producción 19.3. Puede seguir accediendo a la subpestaña Problemas desde el Registro de asuntos pendientes del tablero Kanban.

## Eliminación de las pestañas Documentos y Problemas de la página de detalles de iteración

>[!NOTE]
>
>Este cambio se producirá en Producción con la versión 2019.3. No se realizará en el entorno de vista previa antes de la versión de producción.

Se están eliminando las pestañas Documentos y Problemas de la página de detalles de iteración Agile:

* **Documentos:** todos los documentos almacenados en la pestaña Documentos deben moverse antes de la versión de producción. Si no mueve sus documentos, ya no tendrá acceso a ellos.
* **Problemas:** esta pestaña se encuentra generalmente en el menú desplegable Más. Puede seguir accediendo a la subpestaña Problemas desde la pestaña Elementos de trabajo en la iteración.

## Tener en cuenta o ignorar los días libres del usuario en las fechas de tareas

Ahora puede decidir si desea permitir la programación de días libres del usuario asignado principal de una tarea para ajustar las fechas planificadas.

Puede tomar esta decisión en el nivel del sistema, como administrador de Workfront, o en el nivel de proyecto, como administrador de proyectos.

Antes de este cambio, los días libres del usuario asignado principal siempre ajustaban las fechas planificadas de la tarea, si la función de Restricción de tarea permite la modificación de las fechas.

Para obtener información sobre la configuración de días libres del usuario en el nivel de sistema, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obtener información sobre la configuración de días libres del usuario en el nivel de proyecto, consulte [Editar proyectos](../../../../manage-work/projects/manage-projects/edit-projects.md).

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
* Cambie los nombres y colores de las condiciones predeterminadas integradas para proyectos, tareas y problemas.

Además, si tiene derechos para editar una tarea o un problema, pero no se le ha asignado (tal vez porque la está supervisando), ahora puede cambiar su condición mediante la columna Condiciones en una vista de lista.

Anteriormente, las condiciones no se podían personalizar ni cambiar, y solo los usuarios podían cambiar la condición de una tarea o problema si se les había asignado.

Para obtener más información, consulte [Condiciones personalizadas](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Disponibilidad de vista previa: 4 de julio de 2019
>
>Disponibilidad de producción: finales de septiembre o principios de octubre

## Nueva notificación por correo electrónico para equipos

Hay una nueva notificación de eventos por correo electrónico para los equipos. Los integrantes del equipo reciben una notificación por correo electrónico cuando se activa un proyecto con tareas asignadas a su equipo. Esta configuración está desactivada de forma predeterminada.

Anteriormente, los integrantes del equipo no podían recibir notificaciones cuando se activaban los proyectos en los que estaban.

Para obtener más información, consulte Notificaciones: Información sobre proyectos en los que participo.

>[!NOTE]
>
>Disponibilidad de vista previa: 4 de julio de 2019
>
>Disponibilidad de producción: 18 de julio de 2019

## Las actualizaciones de documentos ahora aparecen en el objeto y proyecto asociados

Al realizar comentarios en un documento, la actualización aparece ahora en la pestaña Actualizaciones tanto para el documento como para el objeto donde está adjunto.

Si el objeto forma parte de un proyecto, el comentario del documento también aparecerá en la pestaña Actualizaciones del proyecto.

Anteriormente, los comentarios de actualización solo aparecían en la pestaña Actualizaciones del documento.

Para obtener más información, consulte la sección [Actualizar trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) en el artículo [Actualizar trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Disponibilidad de vista previa: 6 de junio de 2019
>
>Disponibilidad de producción: 20 de junio de 2019

## Visibilidad de la programación de días libres de un usuario al asignarlo a tareas y problemas

Al asignar un usuario a una tarea o un problema, ahora puede ver una advertencia en línea si el usuario seleccionado tiene días libres programados en algún momento entre las fechas planificadas de la tarea o el problema.

Para obtener información sobre la asignación de tareas, consulte [Asignar tareas](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md).

Para obtener información sobre los días libres, consulte [Configurar días libres personales](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Disponibilidad de vista previa: 30 de mayo de 2019
>
>Disponibilidad de producción: 13 de junio de 2019

## Añadir campos que representen objetos en formularios personalizados

Hemos creado un nuevo tipo de campo en el generador de formularios personalizado llamado Typeahead. Este campo permite añadir campos que representan objetos a los formularios personalizados. Actualmente, el objeto User está habilitado con Typeahead y habrá otros objetos disponibles más adelante.

Anteriormente, los administradores tenían que mantener manualmente a los usuarios como opciones individuales en los menús desplegables de formularios personalizados.

>[!NOTE]
>
>Disponibilidad de vista previa: 30 de mayo de 2019
>
>Disponibilidad de producción: 13 de junio de 2019
>
>Antes de la fecha de lanzamiento de Producción, los nuevos campos personalizados no eran compatibles con Mobile, Outlook, MS Teams ni con la integración nativa de Salesforce.
>
>En Producción, ahora se admiten Outlook y MS Teams. Mobile se admite desde finales de junio o principios de julio; las integraciones de Salesforce se admiten desde junio.

## Al campo “Asunto” de Nueva solicitud se le cambiado el nombre a “Nombre”

>[!NOTE]
>
>Esta función se ha eliminado y no se incluirá en la versión 2019.3.

Ahora, cuando envíe una nueva solicitud a una Cola de solicitudes, introduzca el nombre de la solicitud en el campo “Nombre” del formulario de nueva solicitud.

Antes de este cambio, se introducía el nombre de la solicitud en el campo “Asunto”.

Para obtener información sobre cómo crear solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

