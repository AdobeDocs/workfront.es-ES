---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa de R1 3
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 1 de febrero de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 2%

---

# Vista previa de R1 3

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 1 de febrero de 2017.

Para ver una lista de todos los cambios realizados en R1, consulte [Resumen de actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Método mejorado para vincular archivos externos

La opción para vincular documentos desde una fuente externa (como Google Drive, Box, Dropbox, etc.) ahora se encuentra en una ubicación más destacada del área Documentos. 

Además, la acción de autorizar a un proveedor de documentos antes de vincular archivos de ese proveedor por primera vez es ahora más intuitiva (es simplemente un paso adicional al vincular archivos de un proveedor externo).

Antes de realizar estos cambios, la opción para vincular archivos de un origen externo se encontraba en el cuadro de diálogo Agregar documentos dentro del área Documentos. Antes de vincular un documento desde una fuente externa por primera vez, el usuario que lo vinculaba tenía que autorizar al proveedor de documentos en el área de Configuración.

Para obtener más información, consulte  [Vinculación de documentos desde aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Calendario actualizado de Equipo trabajando en

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

El calendario de Trabajando en disponible para los equipos ahora contiene funcionalidades adicionales y una apariencia actualizada. El calendario Equipo que trabaja en funciona ahora de forma similar a la herramienta de programación de recursos de los proyectos.

El calendario actualizado de Trabajando en equipo incluye las siguientes mejoras:

* Ver los usuarios alfabéticamente o agrupados por función.
* Filtre la cronología de programación por prioridades de proyecto, estado y proyectos individuales. También puede filtrar la cronología de programación por funciones y usuarios. (El área Filtro incluye menos opciones que al programar recursos para proyectos).
* Incluya problemas en la cronología de programación.
* Muestre las asignaciones de usuarios y modifique el número de horas que se asignan a los usuarios a determinadas tareas y problemas cada día.
* Vea los indicadores que muestran cuándo se asignan excesivamente los usuarios en un día determinado.
* Configure si el trabajo completado se muestra en la escala de tiempo de la programación.

Diferencias con respecto a la herramienta de programación de recursos al programar recursos para proyectos:

* Todos los miembros del equipo se muestran en el calendario del equipo Trabajando en.\
  Al programar recursos para proyectos, sólo se muestran los usuarios que tienen un rol asociado que coincide con un rol de una o varias tareas del área No asignada.
* La herramienta de intercambio no está disponible y no se incluye en el calendario del equipo en el que se trabaja.
* Cualquier miembro del equipo puede realizar cambios en el calendario del equipo Trabajando en.\
  Al programar recursos para proyectos, solamente los administradores de recursos pueden tomar decisiones de asignación de recursos para el proyecto.
* Los problemas se muestran de forma predeterminada en el calendario del equipo que trabaja en.\
  Al programar recursos para proyectos, los problemas no se muestran de forma predeterminada.

Para obtener más información sobre el uso del calendario actualizado de Trabajando en equipo, consulte &quot;Horario de recursos&quot;.

## Mejoras en Resource Scheduling

El calendario de programación incluye las siguientes mejoras:

* &quot;Utilizar el filtro para controlar qué usuarios se muestran en la cronología de programación&quot;
* &quot;Los usuarios permanecen en la cronología después de que se les asigne una tarea&quot;

### Utilice el filtro para controlar qué usuarios se muestran en la cronología de programación {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

El filtro ahora se puede utilizar para controlar qué usuarios se muestran en la escala de tiempo de la programación, además de qué tareas y problemas se muestran en el área sin asignar. Cuando se seleccionan usuarios en el filtro, sólo se muestran los usuarios seleccionados, independientemente de si tienen una asignación de función que coincida con la asignación de función de las tareas del área No asignada. También se muestran todas las tareas asignadas actualmente a ese usuario.

Antes de este cambio, el filtro controlaba solamente qué tareas y problemas se mostraban en el área Sin asignar. Los usuarios se mostraban en la escala de tiempo de la programación sólo si el usuario coincidía con la asignación de funciones de una tarea en el área sin asignar.

Para obtener más información sobre el uso del filtro para controlar lo que se muestra en la cronología de programación, consulte &quot;Filtrar información en el área de programación&quot; y &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

### Los usuarios permanecen en la cronología después de que se les asigne una tarea {#users-remain-on-the-timeline-after-being-assigned-a-task}

Los usuarios permanecen en la escala de tiempo de la programación una vez que se les asigna una tarea o un problema, aunque no queden tareas o problemas con una asignación de función coincidente. Esto le permite realizar los cambios necesarios después de asignar los usuarios.

Antes de este cambio, los usuarios desaparecían de la escala de tiempo de la programación inmediatamente después de que se les asignara una tarea o un problema si no quedaban tareas o problemas en el área Sin asignar con una asignación de función coincidente.

Para obtener más información, consulte &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

## Personalización de la terminología de Workfront mediante el cambio de nombres de objetos

Ahora puede personalizar la terminología de Workfront cambiando los nombres de ciertos objetos.\
Con una plantilla de diseño, ahora puede cambiar los nombres de los siguientes objetos de trabajo para que coincidan con las necesidades de su organización:

* Portafolio
* Programar
* Proyecto
* Tarea
* Problema

Por ejemplo, si en su organización trabaja con campañas en lugar de con proyectos, puede reemplazar el nombre del objeto &quot;Proyecto&quot; por &quot;Campaña&quot;.

Cuando se realiza este reemplazo, las siguientes áreas de la aplicación muestran el nombre actualizado de los objetos:

* Barra de navegación global
* Todas las pestañas
* Todos los menús 
* Report Builder y los elementos de informes (vistas, filtros y agrupaciones)
* Botones Guardar
* Archivos exportados
* Correos electrónicos

Las áreas siguientes no muestran el nombre actualizado de los objetos:

* Estimaciones de recursos
* Administrador de presupuesto de recursos
* Planificador de capacidades
* Cuadrícula de recursos
* Generador de equipos
* Portfolio Optimizer 
* Aplicaciones móviles
* Complemento de Outlook

Para obtener más información sobre cómo personalizar la terminología de Workfront mediante una plantilla de diseño, consulte la sección &quot;Personalización de la terminología&quot; en &quot;Creación y administración de plantillas de diseño&quot; y la sección &quot;Explicación de las implicaciones de la personalización de nombres de objetos&quot; en [Explicación de los objetos en Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Incluir las fechas de inicio y finalización de la aprobación en los informes

Ahora puede incluir los campos siguientes al crear o modificar informes:

* Fecha de inicio de ruta de aprobación
* Fecha de finalización de ruta de aprobación

Estos campos le permiten obtener información sobre cuándo se inició la ruta de aprobación actual o la más reciente y cuándo se marcó como Completa.

Para obtener más información sobre estos campos, consulte [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obtener más información sobre las rutas de aprobación, cómo se crean y activan y la función que cumplen en los procesos de aprobación, consulte [Crear un proceso de aprobación para elementos de trabajo](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Los campos siguientes se han eliminado de Workfront y ya no pueden incluirse en los informes (estos campos proporcionaban información sobre el proyecto en lugar de información sobre las aprobaciones en sí, y a menudo se utilizaban indebidamente):

* Fecha planificada de inicio de aprobaciones
* Fecha proyectada de inicio de aprobación
* Fecha estimada de inicio de aprobación

## Nuevas opciones de resumen de correo electrónico para &quot;Solicitudes que he realizado&quot;

La opción de entrega de resumen diario se ha agregado al área &quot;Solicitudes que he realizado&quot; de la configuración de Notificaciones.

Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios.

## Apariencia actualizada de las notificaciones por correo electrónico de aprobación de documentos

El aspecto de la notificación de &quot;Aprobación del documento&quot; se ha actualizado con una nueva interfaz de usuario:

Para obtener más información sobre las notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque la Vista previa de espacio aislado borra las direcciones de correo electrónico de todos los usuarios.

## Mejoras en la vista de Milestone

La vista de Hito que está disponible al ver una lista de proyectos o un informe de proyectos ahora contiene las siguientes mejoras:

* Las fechas planificadas son editables
* Se muestra el porcentaje completado de proyectos y tareas

Antes de este cambio, para editar las fechas o ver el porcentaje completado, tenía que ir a la tarea individual.

Para obtener más información, consulte [Uso de la vista de Hito](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
