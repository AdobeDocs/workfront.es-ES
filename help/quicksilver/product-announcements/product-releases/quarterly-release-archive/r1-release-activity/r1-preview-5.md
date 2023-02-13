---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa R1 5
description: Esta página describe todos los cambios disponibles en el entorno de Vista previa con la versión R1 Preview 5. La funcionalidad de esta página estuvo disponible en el entorno de vista previa el 16 de marzo de 2017.
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 13%

---

# Vista previa R1 5

Esta página describe todos los cambios disponibles en el entorno de Vista previa con la versión R1 Preview 5. La funcionalidad de esta página estuvo disponible en el entorno de vista previa el 16 de marzo de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [Información general sobre la actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Seguimiento del progreso del proyecto con un informe de uso

Ahora un usuario con acceso de administración a un proyecto puede realizar un seguimiento del progreso del proyecto mediante un informe de utilización.

El informe de utilización le permite mantener el proyecto dentro del presupuesto, ya que le permite ver rápidamente cómo se rastrean las horas reales en comparación con las horas presupuestadas o las horas planificadas para una semana o mes determinados, o para el proyecto general. Además, puede ver información detallada sobre la cantidad de horas en cada categoría (presupuestada, planificada y real), clasificada por función de trabajo o usuario individual.

Para obtener más información sobre el seguimiento de la utilización en un proyecto, consulte [Resumen del informe de Utilización de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

Como administrador del sistema, puede configurar si la pestaña Utilización está disponible para los usuarios. De forma predeterminada, la ficha Utilización se encuentra en el menú desplegable Más de un proyecto. Puede mover la ficha Utilización a otra ubicación o puede ocultarla por completo. Si ha definido plantillas de diseño personalizadas para los usuarios de su organización, debe agregar manualmente la pestaña Utilización a las plantillas de diseño personalizadas.

Para obtener más información sobre la configuración de la ubicación de la ficha Utilización, consulte &quot;Personalizar fichas&quot; en &quot;Creación y administración de plantillas de diseño&quot;.

## Modificación de un Proceso de Aprobación Global Existente para un Objeto Individual

Ahora puede modificar un proceso de aprobación global existente al asociar ese proceso de aprobación global con un objeto. Las modificaciones que realice se aplicarán únicamente al proceso de aprobación del objeto al que lo asocie.

Para obtener más información, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) en [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Configuración de informes para mostrar el nuevo diagrama de Gantt de forma predeterminada

Puede configurar los informes de proyecto y tarea que cree para mostrar el nuevo diagrama de Gantt de forma predeterminada con la nueva opción &quot;Mostrar este informe en una vista de Gantt de forma predeterminada&quot;.

Para obtener más información sobre la configuración de informes para mostrar el nuevo diagrama de Gantt, consulte [Editar la configuración del informe](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

Para obtener más información sobre la visualización del diagrama de Gantt en los informes de proyectos y de tareas, consulte [Ver información en el diagrama de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; [Ver información en el diagrama de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Mejora de la Papelera de reciclaje: Las tareas y subtareas se restauran a su orden anterior

Ahora, cuando restaura una tarea o subtarea después de eliminarla, la tarea o subtarea se restaura a su ubicación anterior (ya sea en la lista de tareas o debajo de la tarea principal), en el mismo orden en que aparecía antes de eliminarse.

Antes de este cambio, las tareas y subtareas restauradas siempre se restauraban como la última tarea (ya fuera en la lista de tareas o debajo de la tarea principal), independientemente del orden en que aparecían antes de eliminarse.

Para obtener más información sobre la restauración de objetos en Workfront, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Mejoras en la vista Milestone

Ahora están disponibles las siguientes mejoras al ver una lista de proyectos o un informe de proyectos en la vista Milestone:

* **Configure si el estado de progreso y el porcentaje completado se muestran en la vista:** Hay una nueva opción que le permite configurar si los iconos Estado de progreso se muestran en la vista Milestone. Además, también puede configurar si la información de porcentaje completado se muestra relacionada con proyectos y tareas.\
   Para obtener más información, consulte [Uso de la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) en [Uso de la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Edite el porcentaje completado directamente desde la vista Milestone:** Ahora puede editar el porcentaje de finalización de proyectos y tareas directamente desde la vista Milestone.\
   Para obtener más información, consulte [Uso de la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) en [Uso de la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## Aspecto actualizado de varias páginas de configuración del sistema

Se ha actualizado el aspecto de las siguientes páginas del menú Sistema del área Configuración (la funcionalidad sigue siendo la misma):

* Diagnósticos
* Inicio de sesión único (SSO) que incluye:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Actualizar usuarios para SSO

## Se han actualizado las agrupaciones de notificaciones de eventos en el área de configuración de correo electrónico

Los encabezados organizativos de las Notificaciones de eventos en el área Configuración de correo electrónico ahora coinciden con los encabezados de sección que se usan en el área de configuración del perfil del usuario.

Para obtener más información sobre las notificaciones de eventos, consulte  [Configurar notificaciones de eventos para todos los miembros del sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Excluir notificaciones instantáneas: Configuración de compendio en contexto

Las siguientes opciones ya están disponibles en las notificaciones de correo electrónico instantáneo. Estas opciones solo están disponibles para notificaciones instantáneas que también tienen una contrapartida de compendio diaria:

* “Agregar esto a un resumen diario”
* &quot;Detener correos electrónicos de este tipo&quot;

Ahora, cuando reciba una notificación por correo electrónico instantánea, puede agregar esa notificación a una notificación diaria de compendio o cancelar la suscripción por completo a esa notificación.

Estas opciones están disponibles en la notificación por correo electrónico. Para obtener más información sobre la recepción de notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Se han movido varias notificaciones por correo electrónico de la sección &quot;Acción necesaria&quot; a otras secciones relacionadas con el proyecto

Se han movido varias notificaciones de la sección &quot;Acción necesaria&quot; de la página de perfil del usuario a otras secciones, de la siguiente manera:

Para obtener más información sobre la configuración de las notificaciones por correo electrónico, consulte [Activar o desactivar sus propias notificaciones de eventos](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Notificación</strong> </th> 
   <th><strong>Sección antigua</strong> </th> 
   <th><strong>Nueva sección</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Se agrega un problema a un proyecto de mi propiedad</td> 
   <td> <p> Se requiere una acción </p> </td> 
   <td>   <p>Información sobre proyectos de mi propiedad</p></td> 
  </tr> 
  <tr> 
   <td>Se agrega un problema a un proyecto en el que participo</td> 
   <td>   <p>Se requiere una acción</p><p> </p></td> 
   <td> <p> Información sobre proyectos de mi propiedad </p>   </td> 
  </tr> 
  <tr> 
   <td>Se agrega un problema no asignado a un proyecto de mi propiedad</td> 
   <td>   <p>Se requiere una acción</p></td> 
   <td>   <p>Información sobre proyectos de mi propiedad</p></td> 
  </tr> 
  <tr> 
   <td> <p> Se agrega un problema no asignado a un proyecto en el que participo </p> </td> 
   <td> <p> Se requiere una acción </p>   </td> 
   <td> <p> Información sobre proyectos de mi propiedad </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> Cambia la fecha de confirmación de una tarea en uno de mis proyectos </p> </td> 
   <td>   <p>Se requiere una acción</p></td> 
   <td>   <p>Información sobre proyectos de mi propiedad</p></td> 
  </tr> 
  <tr> 
   <td> <p> Si cambia la fecha de confirmación de un problema en uno de mis proyectos </p>   </td> 
   <td>   <p>Se requiere una acción</p></td> 
   <td> <p> Información sobre proyectos de mi propiedad </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> Cambio de fecha límite de una tarea a la que estoy asignado </p> </td> 
   <td>   <p>Se requiere una acción</p></td> 
   <td>   <p>Información sobre trabajo asignado a mí</p></td> 
  </tr> 
  <tr> 
   <td> <p> Si cambia la fecha planificada de finalización de un problema, notificar al usuario asignado </p> </td> 
   <td> <p> Se requiere una acción </p>   </td> 
   <td>   <p>Información sobre trabajo asignado a mí</p></td> 
  </tr> 
  <tr> 
   <td> <p> El estado cambia en una tarea a la que he sido asignado </p>   </td> 
   <td> <p> Se requiere una acción </p>   </td> 
   <td> <p> Información sobre trabajo asignado a mí </p>   </td> 
  </tr> 
 </tbody> 
</table>

## Nueva funcionalidad de planificación de recursos (no disponible en producción en R1)

>[!NOTE]
>
>Esta funcionalidad está disponible actualmente en el entorno de Vista previa. Se eliminará del entorno de Vista previa aproximadamente un mes antes de la versión R1 de Producción. A continuación, se volverá a introducir en el entorno de vista previa en la vista previa 1 de R2.

 

Se agregaron los siguientes cambios para admitir la futura funcionalidad de planificación de recursos:

* Se ha cambiado el nombre de la ficha &quot;Planificación de recursos&quot; actual a &quot;Planificación de recursos heredada&quot; en el área Personas. 
* Se ha introducido una nueva pestaña &quot;Planificación de recursos&quot; en el área Personas donde se desarrollará la nueva funcionalidad.\
   Para obtener más información sobre la nueva ficha Planificación de recursos, consulte [Introducción a la planificación de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* Se ha cambiado el nombre del objeto &quot;Grupo de recursos&quot; actual a &quot;Grupo de recursos heredado&quot;.\
   Para obtener más información sobre la creación de los nuevos grupos de recursos basados en el usuario, consulte [Resumen de los grupos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* Se ha creado un nuevo objeto &quot;Grupo de recursos&quot; para admitir los nuevos grupos de recursos (basados en el usuario).

   >[!NOTE]
   * Si actualmente está ejecutando informes en los grupos de recursos heredados existentes, los informes existentes no cambiarán.
   * Si desea crear un nuevo informe para los grupos de recursos heredados existentes (basados en funciones), deberá seleccionar &quot;Grupos de recursos heredados&quot; como objeto del informe.
   * Si desea crear un nuevo informe para los nuevos grupos de recursos (basados en el usuario), deberá seleccionar &quot;Grupos de recursos&quot; como objeto del informe.

  >   
