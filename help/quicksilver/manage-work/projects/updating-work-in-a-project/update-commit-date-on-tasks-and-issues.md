---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar fechas de confirmación en tareas y problemas
description: Puede actualizar manualmente la fecha de confirmación de una tarea o un problema al que esté asignado. Para obtener más información sobre las fechas de compromiso en Adobe Workfront, consulte Información general sobre las fechas de compromiso.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# Actualizar fechas de confirmación en tareas y problemas

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en el entorno de producción para los clientes que habilitaron versiones rápidas de.</span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la versión actual, consulte [Información general sobre la versión del tercer trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

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
* <span class="preview">El encabezado de la tarea o del problema</span>

  <span class="preview">El administrador de Workfront o del grupo debe agregar la fecha de confirmación al encabezado de tarea o problema de la plantilla de diseño para verla desde la página de tareas o problemas.
Para obtener más información, consulte [Personalización de encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

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

1. <span class="preview">(Condicional y opcional) Si el administrador del grupo o de Workfront ha agregado la fecha de confirmación al encabezado de la tarea o del problema, haga clic en **Fecha de confirmación** en el encabezado y, a continuación, seleccione una fecha del calendario. Si la fecha de confirmación no está en el encabezado, siga estos pasos. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

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
   * El propietario del proyecto recibe una notificación en la sección Actualizaciones de que ha sugerido una nueva fecha de compromiso y puede, en este momento, actualizar la fecha planificada de finalización de la tarea o problema para que coincida con la fecha de compromiso sugerida.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Para obtener información sobre las notificaciones y actualizaciones activadas por este cambio, consulte la sección &quot;Notificaciones y actualizaciones activadas al cambiar la fecha de confirmación&quot; en el artículo [Resumen de fecha de confirmación](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->