---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa de R1 5
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1 Preview 5. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 16 de marzo de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 13%

---

# Vista previa de R1 5

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1 Preview 5. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 16 de marzo de 2017.

Para ver una lista de todos los cambios realizados en R1, consulte [Resumen de actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Seguimiento del progreso del proyecto con un informe de utilización

Ahora un usuario con acceso de Administrar a un proyecto puede realizar un seguimiento del progreso del proyecto con un informe de utilización.

El informe de utilización permite mantener el proyecto dentro del presupuesto, ya que permite ver rápidamente cómo se cotejan las horas reales con las horas presupuestadas o planificadas para una semana o mes determinados, o para el proyecto general. Además, puede ver información detallada sobre el número de horas de cada categoría (presupuestadas, planificadas y reales), clasificadas por rol o usuario individual.

Para obtener más información sobre el seguimiento de la utilización en un proyecto, consulte [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

Como administrador del sistema, puede configurar si la pestaña Utilización está disponible para los usuarios. De forma predeterminada, la pestaña Utilización se encuentra en el menú desplegable Más dentro de un proyecto. Puede mover la ficha Utilización a otra ubicación u ocultarla por completo. Si ha definido plantillas de diseño personalizadas para los usuarios de su organización, debe añadir manualmente la pestaña Utilización a las plantillas de diseño personalizadas.

Para obtener más información sobre la configuración de la ubicación de la pestaña Utilización, consulte &quot;Personalizar pestañas&quot; en &quot;Creación y administración de plantillas de diseño&quot;.

## Modificar un proceso de aprobación global existente para un objeto individual

Ahora puede modificar un proceso de aprobación global existente al asociar ese proceso de aprobación global con un objeto. Las modificaciones realizadas se aplican únicamente al proceso de aprobación del objeto donde se asocian.

Para obtener más información, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Configurar informes para mostrar el nuevo gráfico Gantt de forma predeterminada

Puede configurar los informes de proyectos y tareas que cree para mostrar el nuevo gráfico Gantt de forma predeterminada con la nueva opción, &quot;Mostrar este informe en una vista Gantt de forma predeterminada&quot;.

Para obtener más información sobre la configuración de informes para mostrar el nuevo gráfico Gantt, consulte [Editar configuración del informe](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

Para obtener más información sobre la visualización del diagrama de Gantt en los informes de proyecto y de tarea, consulte [Ver información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; en [Ver información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Mejora de la papelera de reciclaje: las tareas y subtareas se restauran a su orden anterior

Ahora, cuando restaura una tarea o subtarea después de eliminarla, la tarea o subtarea se restaura a su ubicación anterior (ya sea en la lista de tareas o debajo de la tarea principal), en el mismo orden en que aparecía antes de eliminarse.

Antes de este cambio, las tareas y subtareas restauradas siempre se restauraban como la última tarea (en la lista de tareas o debajo de la tarea principal), independientemente del orden en que aparecieran antes de eliminarse.

Para obtener más información sobre la restauración de objetos en Workfront, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Mejoras en la vista de Milestone

Las siguientes mejoras están ahora disponibles cuando se visualiza una lista de proyectos o un informe de proyectos en la vista de Hito:

* **Configure si Estado de progreso y Porcentaje completado se muestran en la vista:** Hay una nueva opción que le permite configurar si los iconos de estado de progreso se muestran en la vista de Hito. Además, también puede configurar si la información de Porcentaje completado se muestra relacionada con los proyectos y las tareas.\
  Para obtener más información, consulte [Uso de la vista de Hito](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Uso de la vista de Hito](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Edite el porcentaje completado directamente desde la vista de Hito:** Ahora puede editar el Porcentaje completado de proyectos y tareas directamente desde la vista de Hito.\
  Para obtener más información, consulte [Uso de la vista de Hito](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Uso de la vista de Hito](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## Aspecto actualizado de varias páginas de configuración del sistema

Se ha actualizado el aspecto de las siguientes páginas del menú Sistema del área Configuración (la funcionalidad sigue siendo la misma):

* Diagnósticos
* Inicio de sesión único (SSO) que incluye:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Actualizar usuarios para SSO

## Se han actualizado las agrupaciones de notificación de eventos en el área de configuración de correo electrónico

Los encabezados organizativos de las notificaciones de eventos en el área de configuración de correo electrónico ahora coinciden con los encabezados de sección que se utilizan en el área de configuración de perfil de usuario.

Para obtener más información sobre las notificaciones de eventos, consulte  [Configurar notificaciones de eventos para todos los usuarios del sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Desactivar notificaciones instantáneas: configuración de resumen en contexto

Las siguientes opciones ya están disponibles en las notificaciones instantáneas por correo electrónico. Estas opciones solo están disponibles para notificaciones instantáneas que también tienen un homólogo de resumen diario:

* &quot;Agregar esto a un resumen diario&quot;
* &quot;Detener correos electrónicos de este tipo&quot;

Ahora, cuando reciba una notificación instantánea por correo electrónico, puede agregar esa notificación a una notificación de resumen diario o puede cancelar completamente la suscripción a esa notificación.

Estas opciones están disponibles en la notificación por correo electrónico. Para obtener más información sobre la recepción de notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Varias notificaciones por correo electrónico se movieron de la sección &quot;Acción necesaria&quot; a otras secciones relacionadas con el proyecto

Se han movido varias notificaciones de la sección &quot;Acción necesaria&quot; de la página de perfil del usuario a otras secciones, como se indica a continuación:

Para obtener más información sobre la configuración de notificaciones por correo electrónico, consulte [Modificar sus propias notificaciones por correo electrónico](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

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
>Actualmente, esta funcionalidad está disponible en el entorno de vista previa. Se eliminará del entorno de vista previa aproximadamente un mes antes del lanzamiento de R1 en Producción. A continuación, se volverá a introducir al entorno de vista previa en R2 Preview 1.

 

Se agregaron los cambios siguientes para admitir la futura funcionalidad de planificación de recursos:

* Se ha cambiado el nombre de la pestaña actual &quot;Planificación de recursos&quot; a &quot;Planificación de recursos de legado&quot; en el área Personas. 
* Se ha introducido una nueva pestaña &quot;Planificación de recursos&quot; en el área Personas, donde se desarrollará la nueva funcionalidad.\
  Para obtener más información sobre la nueva ficha Planificación de recursos, consulte [Introducción a la planificación de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* Se ha cambiado el nombre del objeto actual &quot;Conjunto de recursos&quot; a &quot;Conjunto de recursos heredado&quot;.\
  Para obtener más información sobre la creación de los nuevos conjuntos de recursos basados en usuarios, consulte [Resumen de conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* Se ha creado un nuevo objeto &quot;Conjunto de recursos&quot; para admitir los nuevos conjuntos de recursos (basados en el usuario).

  >[!NOTE]
  >
  >
  >   
  >   
  * Si está ejecutando informes sobre los conjuntos de recursos heredados existentes, los informes existentes no cambiarán.
  * Si desea crear un nuevo informe para los conjuntos de recursos heredados existentes (basados en funciones del puesto), deberá seleccionar &quot;Conjuntos de recursos heredados&quot; como objeto para el informe.
  * Si desea crear un nuevo informe para los nuevos conjuntos de recursos (basados en el usuario), deberá seleccionar &quot;Conjuntos de recursos&quot; como objeto para el informe.
  >   
  >
