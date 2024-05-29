---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar fechas de confirmación en tareas y problemas
description: Puede actualizar manualmente la fecha de confirmación de una tarea o un problema al que esté asignado. Para obtener más información sobre las fechas de compromiso en Adobe Workfront, consulte Información general sobre las fechas de compromiso.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 44073ea242803e28ca00c82811ae2865747d11c3
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---


# Actualizar fechas de confirmación en tareas y problemas

{{highlighted-preview}}

Puede actualizar manualmente la fecha de confirmación de una tarea o un problema al que esté asignado. Para obtener más información sobre las fechas de compromiso en Adobe Workfront, consulte [Resumen de fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisitos de acceso

<!--Audited: 01/2024-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
   Para las nuevas licencias:
   <ul>
   <li><p>Estándar para tareas</p> </li>
   <li><p>Colaborador o superior para problemas</p></li>
   </ul>
   Para licencias actuales:
<ul>
   <li><p>Trabajo o superior para tareas</p></li> 
   <li><p>Solicitud de problemas o superior</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas y Problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos sobre la tarea o el problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Antes de poder editar la fecha de confirmación de una tarea o problema, se le debe asignar la tarea o problema cuya fecha de confirmación necesite actualizar.

## Actualizar fechas de confirmación en tareas y problemas


Puede actualizar la fecha de confirmación de una tarea o problema en las siguientes áreas de Workfront:

* La sección Detalles de una tarea o problema
<!--
* <span class="preview">The task or issue header
   Your Workfront or group administrator must add the Commit Date to the task or issue header of your layout template to view it from the task or issue page. </span>
   For information, see [Customize object headers using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). -->

La actualización de la fecha de confirmación es idéntica para las tareas y los problemas.

>[!NOTE]
>
>Puede pedir al administrador del sistema o del grupo que añada el campo Fecha de confirmación al panel de resumen para que sea más fácil actualizarlo en varias áreas de Workfront.
>
>Para obtener más información, consulte los siguientes artículos:
>
>* [Resumen, descripción general](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizar Inicio y resumen mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Vaya a una tarea o un problema que esté asignado como **Propietario**.

   Para obtener más información sobre cómo averiguar quién es el propietario de la tarea de un problema o tarea, consulte la sección [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) en el artículo [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--1. <span class="preview">(Conditional and optional) If your Workfront or group administrator added the Commit Date to your task or issue header, click the **Commit Date** field in the header, then select a date from the calendar. If the Commit Date is not in the header, proceed with the following steps. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>-->

1. Clic **Detalles de tarea** o **Detalles del problema** en el panel izquierdo.
1. Clic **Información general** para expandirlo.
1. Actualice el **Fecha de confirmación** field.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Haga clic en **Guardar cambios**.

   Lo siguiente ocurre después de realizar este cambio: 

   * La fecha de compromiso y la fecha planificada de finalización de la tarea o problema ya no son la misma.

     En su lugar, la fecha de compromiso y la fecha de finalización prevista de la tarea o problema serán las mismas.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Se notifica al propietario del proyecto en una notificación en la aplicación de Workfront de que ha sugerido una nueva fecha de confirmación para la tarea o el problema.
   <!--* The Project Owner is notified in the Updates section that you have suggested a new Commit Date and they can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. This functionality is not supported in the new commenting experience. For information, see [The new commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). -->

   <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

   Para obtener información sobre las notificaciones y actualizaciones activadas por este cambio, consulte la sección &quot;Notificaciones y actualizaciones activadas al cambiar la fecha de confirmación&quot; en el artículo [Resumen de fecha de confirmación](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->