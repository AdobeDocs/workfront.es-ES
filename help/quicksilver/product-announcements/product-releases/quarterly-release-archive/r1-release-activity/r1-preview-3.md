---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa R1 3
description: Esta página describe todos los cambios disponibles en el entorno de Vista previa con la versión R1.3. La funcionalidad de esta página estuvo disponible en el entorno de vista previa el 1 de febrero de 2017.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# Vista previa R1 3

Esta página describe todos los cambios disponibles en el entorno de Vista previa con la versión R1.3. La funcionalidad de esta página estuvo disponible en el entorno de vista previa el 1 de febrero de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [Información general sobre la actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Método mejorado para vincular archivos externos

La opción para vincular documentos de un origen externo (como Google Drive, Box, Dropbox, etc.) se encuentra ahora en una ubicación más prominente del área Documentos. 

Además, la acción de autorizar un proveedor de documentos antes de vincular archivos de ese proveedor por primera vez es ahora más intuitiva (simplemente es un paso adicional al vincular archivos de un proveedor externo).

Antes de estos cambios, la opción de vincular archivos de un origen externo se encontraba dentro del cuadro de diálogo Agregar documentos dentro del área Documentos. Antes de vincular un documento desde un origen externo por primera vez, el usuario que vinculaba el documento tenía que autorizar a ese proveedor de documentos en el área Configuración.

Para obtener más información, consulte  [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Equipo Actualizado Que Trabaja En El Calendario

El calendario de trabajo disponible para los equipos ahora contiene funciones adicionales y una apariencia actualizada. El equipo Trabajo en el calendario ahora funciona de forma similar a la herramienta de programación de recursos para los proyectos.

El equipo actualizado Working On calendar incluye las siguientes mejoras:

* Ver usuarios alfabéticamente o agrupados por rol.
* Filtre la cronología de la programación por prioridades de proyecto, estado y proyectos individuales. También puede filtrar la cronología de programación por funciones y usuarios. (El área Filtro incluye menos opciones que al programar recursos para proyectos).
* Incluya problemas en la cronología de la programación.
* Muestre las asignaciones de usuario y modifique la cantidad de horas que los usuarios asignan a determinadas tareas y problemas para cada día.
* Vea indicadores que muestran cuándo se sobreasigna a los usuarios en un día determinado.
* Configure si el trabajo completado se muestra en la cronología de programación.

Diferencias con respecto a la herramienta de programación de recursos al programar recursos para proyectos:

* Todos los integrantes del equipo se muestran en el calendario Trabajando en .\
   Al programar recursos para proyectos, solo se muestran los usuarios que tienen una función asociada a ellos que coincida con la función de una o más tareas del área No asignada.
* La herramienta Intercambiar no está disponible no se incluye en el calendario Trabajo en equipo.
* Cualquier miembro del equipo puede realizar cambios en el calendario de Trabajo en el equipo.\
   Al programar recursos para proyectos, solo los gestores de recursos pueden tomar decisiones de recursos para el proyecto.
* Los problemas se muestran de forma predeterminada en el equipo que trabaja en el calendario.\
   Al programar recursos para proyectos, los problemas no se muestran de forma predeterminada.

Para obtener más información sobre el uso del calendario actualizado de Trabajo en equipo, consulte [Programación de recursos](../../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

## Mejoras en la programación de recursos

La cronología de programación incluye las siguientes mejoras:

* [Utilice el filtro para controlar qué usuarios se muestran en la línea de tiempo de programación](#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline)
* [Los usuarios permanecen en la línea de tiempo después de recibir una tarea](#users-remain-on-the-timeline-after-being-assigned-a-task)

### Utilice el filtro para controlar qué usuarios se muestran en la línea de tiempo de programación {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

El filtro ahora se puede utilizar para controlar qué usuarios se muestran en la cronología de la programación, además de qué tareas y problemas se muestran en el área No asignado. Cuando los usuarios están seleccionados en el filtro, solo se muestran los usuarios seleccionados, independientemente de si tienen una asignación de funciones que coincida con la asignación de funciones de tareas en el área No asignado. También se muestran todas las tareas asignadas actualmente a ese usuario.

Antes de este cambio, el filtro controlaba solo qué tareas y problemas se mostraban en el área Sin asignar. Los usuarios se mostraban en la cronología de la programación solo si el usuario coincidía con la asignación de funciones de una tarea en el área No asignada.

Para obtener más información sobre el uso del filtro para controlar lo que se muestra en la cronología de programación, consulte  [Filtrado de información en el área Programación](../../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)y  [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) en [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Los usuarios permanecen en la línea de tiempo después de recibir una tarea {#users-remain-on-the-timeline-after-being-assigned-a-task}

Los usuarios permanecen en la cronología de programación después de que se les asigne una tarea o un problema, incluso si no quedan tareas o problemas que tengan una asignación de función coincidente. Esto le permite realizar los cambios necesarios una vez asignados los usuarios.

Antes de este cambio, los usuarios desaparecían de la cronología de programación inmediatamente después de que se les asignara una tarea o problema si no quedaban tareas o problemas en el área No asignado con una asignación de función coincidente.

Para obtener más información, consulte  [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) en [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Personalización de la terminología de Workfront mediante el cambio de los nombres de objeto

Ahora puede personalizar la terminología de Workfront cambiando los nombres de ciertos objetos.\
Con una plantilla de diseño, ahora puede cambiar los nombres de los siguientes objetos de trabajo para adaptarlos a las necesidades de su organización:

* Portafolio
* Programar
* Proyecto
* Tarea
* Problema

Por ejemplo, si en su organización trabaja con campañas en lugar de con proyectos, puede reemplazar el nombre del objeto &quot;Proyecto&quot; por &quot;Campaña&quot;.

Al realizar este reemplazo, las siguientes áreas de la aplicación muestran el nombre actualizado de los objetos:

* Barra de navegación global
* Todas las pestañas
* Todos los menús 
* Creador de informes y elementos de informes (vistas, filtros y agrupaciones)
* Botones Guardar
* Archivos exportados
* Correos electrónicos

Las siguientes áreas no muestran el nombre actualizado de los objetos:

* Estimaciones de recursos
* Administrador de presupuesto de recursos
* Planificador de capacidades
* Cuadrícula de recursos
* Generador de equipos
* Optimizador de Portfolio 
* Aplicaciones móviles
* Complemento de Outlook

Para obtener más información sobre cómo personalizar la terminología de Workfront mediante una plantilla de diseño, consulte la sección &quot;Personalización de terminología&quot; en &quot;Creación y administración de plantillas de diseño&quot; y la sección &quot;Explicación de las implicaciones de la personalización de nombres de objeto&quot; en [Explicación de los objetos en Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Incluir las fechas de inicio y finalización de la aprobación en los informes

Ahora puede incluir los campos siguientes al crear o modificar informes:

* Fecha de inicio de ruta de aprobación
* Fecha de finalización de la ruta de aprobación

Estos campos le permiten conocer cuándo se inició la ruta de aprobación actual o la más reciente y cuándo se marcó como Completa.

Para obtener más información sobre estos campos, consulte [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obtener más información sobre las rutas de aprobación, cómo se crean y activan, y la función que sirven en los procesos de aprobación, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Los campos siguientes se eliminaron de Workfront y ya no se pueden incluir en los informes (estos campos proporcionan información sobre el proyecto en lugar de información sobre las aprobaciones mismas, y a menudo se utilizan incorrectamente):

* Aprobaciones Fecha de inicio planificada
* Fecha proyectada de inicio de aprobación
* Fecha estimada de inicio de aprobación

## Nuevas opciones de resumen de correo electrónico para &quot;Solicitudes que he realizado&quot;

La opción de entrega Resumen diario se ha agregado al área &quot;Solicitudes que he realizado&quot; de la configuración de Notificaciones.

Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque el espacio aislado de vista previa borra las direcciones de correo electrónico de todos los usuarios.

## Aspecto actualizado de las notificaciones por correo electrónico de aprobación de documentos

El aspecto de la notificación de &quot;Aprobación de documentos&quot; se ha actualizado con una nueva interfaz de usuario:

Para obtener más información sobre las notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque el espacio aislado de vista previa borra las direcciones de correo electrónico de todos los usuarios.

## Mejoras en la vista Milestone

La vista Milestone que está disponible al visualizar una lista de proyectos o un informe de proyecto ahora contiene las siguientes mejoras:

* Las fechas planeadas son editables
* Se muestra el porcentaje completado para proyectos y tareas

Antes de este cambio, para editar las fechas o ver el porcentaje completado, tenía que ir a la tarea individual.

Para obtener más información, consulte [Uso de la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
