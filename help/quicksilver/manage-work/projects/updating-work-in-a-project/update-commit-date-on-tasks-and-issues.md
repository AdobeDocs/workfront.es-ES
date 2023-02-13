---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar fechas de confirmación en tareas y problemas
description: Puede actualizar manualmente la fecha de confirmación de una tarea o un problema que haya asignado. Para obtener más información sobre fechas de confirmación en Adobe Workfront, consulte Información general sobre fechas de confirmación.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Actualizar fechas de confirmación en tareas y problemas

Puede actualizar manualmente la fecha de confirmación de una tarea o un problema que haya asignado. Para obtener más información sobre cómo confirmar fechas en Adobe Workfront, consulte [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisitos de acceso

<!--drafted for P&P

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   For the current licenses:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For legacy licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior para tareas</p> 
   <p>Solicitar o superior para problemas</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos sobre la tarea o el problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de comenzar, debe asignarse a la tarea o al problema para el que debe actualizar la Fecha de confirmación.

## Actualizar fechas de confirmación en tareas y problemas

La actualización de la fecha de confirmación es idéntica para las tareas y los problemas.

1. Vaya a una tarea o problema al que esté asignado como **Propietario de la tarea**.

   Para obtener más información sobre quién es el propietario de la tarea para un problema o tarea, consulte la sección [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) en el artículo [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Haga clic en Trabajar en ella en el encabezado de la tarea o del problema

   O

   Haga clic en **Iniciar tarea** o **Iniciar problema** si el botón Trabajar en él se ha personalizado en su entorno para indicar que está trabajando en el elemento de trabajo.

   En este momento, la fecha de confirmación y la fecha de finalización planeada de la tarea o emisión son iguales.

1. (Opcional) Si hizo clic en Iniciar tarea o en Iniciar problema, haga clic en **Deshacer** en la esquina inferior izquierda de la pantalla. Se elimina la fecha de confirmación.

   Para obtener información sobre cómo reemplazar el botón Trabajar en él por un botón Inicio, consulte  [Reemplazar el botón Trabajar en él con un botón Inicio](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

   >[!TIP]
   >
   >La opción para deshacer la selección para iniciar el trabajo no está disponible al hacer clic en **Trabaje en él**.

1. Haga clic en **Actualizaciones** en el panel izquierdo y, a continuación, haga clic en el **Iniciar una nueva actualización** >**Fecha de confirmación**

   O

   Haga clic en **Detalles de la tarea** o **Detalles del problema** en el panel izquierdo y, a continuación, haga doble clic en **Fecha de confirmación** y seleccione una nueva fecha del calendario y, a continuación, haga clic en **Guardar cambios**.
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)

   Las siguientes cosas suceden después de realizar este cambio: 

   * La fecha de confirmación y la fecha de finalización prevista ya no son la misma.

      En su lugar, la fecha de confirmación y la fecha de finalización prevista de la tarea o el problema son iguales.

      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Los cambios se guardan automáticamente cuando selecciona una nueva fecha en el área Actualizaciones .
   * Se notifica al propietario del proyecto que ha sugerido una nueva fecha de confirmación para la tarea o el problema y que, en este momento, puede actualizar la fecha de finalización planeada de la tarea o el problema para que coincida con la fecha de confirmación sugerida.

      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

      Para obtener información sobre las notificaciones y actualizaciones activadas por este cambio, consulte la sección [Notificaciones y actualizaciones activadas al cambiar la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) en el artículo [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
