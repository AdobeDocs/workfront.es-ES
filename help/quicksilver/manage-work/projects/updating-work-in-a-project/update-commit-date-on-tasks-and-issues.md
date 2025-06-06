---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar fechas de confirmación en tareas y problemas
description: Puede actualizar manualmente la fecha de confirmación de una tarea o un problema al que esté asignado. Para obtener más información sobre las fechas de confirmación en Adobe Workfront, consulte Información general sobre las fechas de confirmación.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 94%

---


# Actualización de fechas de confirmación de tareas y problemas

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Puede actualizar manualmente la fecha de confirmación de una tarea o un problema al que esté asignado. Para obtener más información sobre las fechas de confirmación en Adobe Workfront, consulte [Información general sobre la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisitos de acceso

<!--Audited: 01/2024-->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
   Nuevo:
   <ul>
   <li><p>Estándar para tareas</p> </li>
   <li><p>Colaborador o superior para problemas</p></li>
   </ul>
   Actual:
<ul>
   <li><p>Trabajo o superior para tareas</p></li> 
   <li><p>Permiso de solicitud o superior para los problemas</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea o problema</p>
   <p> Debe estar asignado a la tarea o al problema para actualizar la fecha de confirmación </p>
    </td> 
  </tr> 
 </tbody> 
</table>

* Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de poder editar la fecha de confirmación de una tarea o problema, se le debe asignar la tarea o problema cuya fecha de confirmación necesite actualizar.

## Actualización de fechas de confirmación de tareas y problemas


Puede actualizar la fecha de confirmación de una tarea o problema en las siguientes áreas de Workfront:

* La sección Detalles de una tarea o problema
* El encabezado de la tarea o del problema

  El administrador de Workfront o de grupos debe añadir la fecha de confirmación al encabezado de la tarea o problema de la plantilla de diseño para verla desde la página de tarea o problema.
Para obtener más información, consulte [Personalización de los encabezados de los objetos mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

La actualización de la fecha de confirmación es idéntica para las tareas y los problemas.

>[!NOTE]
>
>Puede pedir al administrador del sistema o del grupo que añada el campo Fecha de confirmación al panel de resumen para que sea más fácil actualizarlo en varias áreas de Workfront.
>
>Para obtener más información, consulte los siguientes artículos:
>
>* [Resumen general](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizar el panel de resumen mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Vaya a una tarea o problema al que esté asignado como **Propietario**.

   Para obtener más información sobre cómo averiguar quién es el propietario de la tarea para un problema o tarea, consulte la sección [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) en el artículo [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Condicional y opcional) Si el administrador del grupo o de Workfront ha añadido la fecha de confirmación al encabezado de la tarea o del problema, haga clic en el campo **Fecha de confirmación** del encabezado y, a continuación, seleccione una fecha del calendario. Si la fecha de confirmación no está en el encabezado, siga estos pasos.

   ![](assets/commit-date-task-header.png)

1. Haga clic en **Detalles de la tarea** o en **Detalles del problema** en el panel izquierdo.
1. Haga clic en **Información general** para expandirla.
1. Actualice el campo **Fecha de confirmación**.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Haga clic en **Guardar cambios**.

   Después de realizar este cambio, se produce lo siguiente:

   * La fecha de confirmación y la fecha planificada de finalización de la tarea o problema ya no son las mismas.

     En cambio, la fecha de confirmación y la fecha proyectada de finalización de la tarea o problema serán las mismas.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Se notifica al propietario del proyecto en una notificación en la aplicación de Workfront de que ha sugerido una nueva fecha de confirmación para la tarea o el problema.
   * El propietario del proyecto recibe una notificación en la sección Actualizaciones de que ha sugerido una nueva fecha de confirmación y pueden, en este momento, actualizar la fecha planificada de finalización de la tarea o problema para que coincida con la fecha de confirmación sugerida.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Para obtener información acerca de las notificaciones y actualizaciones activadas por este cambio, consulte la sección “Notificaciones y actualizaciones activadas al cambiar la fecha de confirmación” en el artículo [Información general sobre la fecha de confirmación](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
