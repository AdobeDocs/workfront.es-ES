---
content-type: reference
navigation-topic: notifications
title: '''Notificaciones: Información sobre el trabajo asignado a mí"'
description: Las siguientes notificaciones le avisan de las actividades que se producen en un elemento de trabajo asignado a usted.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 39ba9e93a8597d4354472a19b1ac1c5f530f4398
workflow-type: tm+mt
source-wordcount: '2092'
ht-degree: 6%

---

# Notificaciones: Información sobre el trabajo asignado a mí

Las siguientes notificaciones le avisan de las actividades que se producen en un elemento de trabajo asignado a usted.

Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th> <p>Campos incluidos </p> <p> *Solo campos de resumen diarios</p> </th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Se ha finalizado una tarea predecesora de una tarea asignada a mi equipo</strong> </p> <p>El equipo asignado recibe una notificación por correo electrónico cuando se completa un predecesor de una de sus tareas. </p> <p>Los usuarios con una licencia [!UICONTROL Review] o Re[!UICONTROL Requestor]questor no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Completar: &lt;task name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de tarea de predecesor<br>Proyecto de tarea de predecesor<br>Número de referencia de tarea de predecesor<br>Nombre del usuario que ha completado la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de predecesores completados<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario </p> </td> 
   <td><strong>Diariamente</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Al finalizar una tarea predecesora de una de mis tareas.</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa un predecesor de una de sus tareas. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de tarea de predecesor<br>Proyecto de tarea de predecesor<br>Número de referencia de tarea de predecesor<br>Nombre del usuario que ha completado la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de predecesores completados<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario </p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Se aprueba o rechaza una tarea que finalizo</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando la tarea se aprueba o rechaza.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que concedió la aprobación<br>Nuevo estado de tarea<br>Fecha y hora en que se aprobó o rechazó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas aprobadas o rechazadas<br>*Nombre de tarea<br>*Nombre del usuario que aprobó o rechazó la tarea<br>*Decisión de aprobación ([!UICONTROL Aprobado]/ [!UICONTROL Rechazado])<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Se finaliza una tarea a la cual estoy asignado</strong> </p> <p>El asignador de tareas recibe una notificación por correo electrónico cuando se completa la tarea.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p> <p>Nota: Si la tarea se cambia a un estado igual a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando "Completado".</p> </p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Se han finalizado todas las tareas predecesoras de una tarea asignada a mi equipo</strong> </p> <p>El equipo asignado recibe una notificación por correo electrónico cuando se marca como completado un predecesor de una de sus tareas.</p> <p>Los usuarios con una licencia de revisión o solicitante no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Tarea finalizada: &lt;name&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> Resumen de trabajo asignado a usted &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Proyecto de tarea<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario </td>
   <td><strong>Instantáneo</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Al finalizar todas mis tareas predecesoras</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico para cada predecesor que se haya completado.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em><br></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Proyecto de tarea<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Cuando se apruebe o rechace un problema, enviar mensaje al usuario asignado</strong> </p> <p>El usuario asignado de un problema recibe una notificación por correo electrónico cuando se toma una decisión de aprobación (aprobada o rechazada).</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Problema pendiente de aprobación: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; en &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> Resumen de trabajo asignado a usted &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que aprobó o rechazó el problema<br>Decisión de aprobación (aprobada o rechazada)<br>Estado del problema<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas aprobados o rechazados<br>*Nombre del problema<br>*Nombre del usuario que aprobó o rechazó el problema<br>*Decisión de aprobación (aprobada o rechazada)<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Enviar correo electrónico al usuario asignado cuando se resuelva el problema</strong> </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Completar: &lt;issue name=""&gt; en &lt;project name=""&gt;</em></p> <p><em> El tema de la notificación diaria de compendio es: Resumen de trabajo asignado a usted &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que ha completado el problema<br>Nuevo estado del problema<br>Fecha y hora en que se completó el problema<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario que ha completado el problema<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando se suba o actualice un documento en una solicitud que se me haya asignado</strong> </p> <p>El destinatario del problema recibe una notificación por correo electrónico cuando se cargan documentos o se cambian los detalles del documento en un problema que ha añadido.</p> <p>No se envía una notificación por correo electrónico si el usuario que activó el problema es el usuario asignado.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y si el proyecto está configurado como cola de solicitud de ayuda (tal y como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Documento agregado a] &lt;request name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de la solicitud<br>Nombre del proyecto (nombre de la cola de solicitud)<br>Número de referencia del documento <br>Nombre del usuario que cargó el documento<br>Nombre del documento <br>Se agregó en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos cargados o modificados<br>*Nombre del documento<br>*Nombre del objeto<br>*Nombre del usuario que cargó el documento<br>*Fecha del compendio diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambio de fecha límite de una tarea a la que estoy asignado</strong> </p> <p>El asignador de tareas recibe una notificación por correo electrónico cuando cambia el [!UICONTROL Fecha de finalización planeada] de la tarea, a menos que el usuario que cambió la fecha de finalización planeada también sea el asignador de tareas.</p> <p>Solo se envía una notificación si el estado del proyecto es cualquier cosa que no sea [!UICONTROL Planning].</p> <p>No se envía ninguna notificación con respecto a las tareas personales.</p> <p> Los usuarios con una licencia de revisión o solicitante no reciben una notificación. </p> <p> El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Se ha cambiado la fecha de vencimiento.]</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nueva fecha de vencimiento ([!UICONTROL Fecha de finalización planeada])<br>Fecha y hora en que se cambió la fecha de vencimiento<br>Nombre del usuario que ha cambiado la fecha de vencimiento<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas en las que ha cambiado la Fecha de vencimiento (Fecha de finalización planeada)<br>*Nombre de tarea<br>*Nueva fecha de finalización planificada<br>*Nombre del usuario que ha cambiado la Fecha de vencimiento<br>*Fecha del compendio diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Si cambia la fecha planificada de finalización de un problema, notificar al usuario asignado</strong> </p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando cambia la [!UICONTROL Fecha de finalización planeada], a menos que el usuario que cambió [!UICONTROL Fecha de finalización planeada] también sea el usuario asignado.</p> <p>Solo se envía una notificación si el estado del proyecto es cualquier cosa que no sea [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de vencimiento ha cambiado]</em></p> <p> </p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nueva fecha de vencimiento ([!UICONTROL Fecha de finalización planeada])<br>Fecha y hora en que se cambió la fecha de vencimiento<br>Nombre del usuario que ha cambiado la fecha de vencimiento<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas en los que ha cambiado la Fecha de vencimiento ([!UICONTROL Fecha de finalización planeada])<br>*Nombre del problema<br>*Nuevo [!UICONTROL Fecha de finalización planeada]<br>*Nombre del usuario que ha cambiado la Fecha de vencimiento<br>*Fecha del compendio diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>El estado cambia en una tarea a la que he sido asignado</strong> <p>El asignador de tareas recibe una notificación por correo electrónico cuando cambia el estado de la tarea, a menos que el usuario que ha cambiado el estado también sea el asignado.</p> <p>Nota: Esta notificación no se envía cuando el estado de la tarea cambia a complete . Se utiliza una notificación independiente para las tareas completadas. Consulte <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Se completó una tarea a la que estoy asignado</a>, más arriba.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;task name=""&gt; from &lt;project name=""&gt; es &lt;new status=""&gt;</em></p> <p> </p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado<br>Estado de vista previa<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas en las que ha cambiado el estado<br>*Nombre de tarea<br>*Estado de la tarea anterior<br>*Nuevo estado de tarea<br>*Nombre del usuario que ha cambiado el estado<br>*Fecha del compendio diario<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en uno de mis elementos de trabajo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando el estado cambie en un problema al que esté asignado, a menos que usted mismo cambie el estado. </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;issue name=""&gt; from &lt;project name=""&gt; es &lt;new status=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado<br>Estado del problema anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas en los que ha cambiado el estado<br>*Nombre de tarea<br>*Estado del problema anterior<br>*Nuevo estado del problema<br>*Nombre del usuario que ha cambiado el estado<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
