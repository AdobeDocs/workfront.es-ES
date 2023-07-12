---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información sobre el trabajo asignado a mí"
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en un elemento de trabajo asignado a usted.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 901605917347297a1ee077f00905b03427582650
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 6%

---

# Notificaciones: Información sobre el trabajo asignado a mí

Las siguientes notificaciones le avisan sobre las actividades que se producen en un elemento de trabajo asignado a usted.

Para obtener información sobre cómo configurar qué notificaciones recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th> <p>Campos incluidos </p> <p> *Solo campos de resumen diario</p> </th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Se ha finalizado una tarea predecesora de una tarea asignada a mi equipo</strong> </p> <p>El equipo asignado recibe una notificación por correo electrónico cuando se completa una tarea predecesora de una de sus tareas. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Completado: &lt;task name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de tarea predecesora<br>Proyecto de tarea predecesora<br>Número de referencia de tarea predecesora<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó la tarea predecesora<br>Estado anterior de la tarea predecesora<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de predecesoras completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </p> </td> 
   <td><strong>Diariamente</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Se completa una de mis tareas predecesoras</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa una tarea predecesora de una de sus tareas. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de tarea predecesora<br>Proyecto de tarea predecesora<br>Número de referencia de tarea predecesora<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó la tarea predecesora<br>Estado anterior de la tarea predecesora<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de predecesoras completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </p> </td> 
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
   <td> <p><strong>Se aprueba o rechaza una tarea que finalizo</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se aprueba o rechaza la tarea.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt; el &lt;project name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que concedió la aprobación<br>Estado de nueva tarea<br>Fecha y hora en que se aprobó o rechazó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas aprobadas o rechazadas<br>*Nombre de tarea<br>* Nombre del usuario que aprobó o rechazó la tarea<br>*Decisión de aprobación ([!UICONTROL Aprobado]/ [!UICONTROL Rechazado])<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Se finaliza una tarea a la cual estoy asignado</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa la tarea.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt; el &lt;project name=""&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a [!UICONTROL Complete], el asunto del correo electrónico seguirá indicando "Complete".</p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Se han finalizado todas las tareas predecesoras de una tarea asignada a mi equipo</strong> </p> <p>El equipo asignado recibe una notificación por correo electrónico cuando una tarea predecesora de una de sus tareas se marca como completada.</p> <p>Los usuarios con una licencia de revisión o solicitante no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Tarea completada: &lt;name&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen del trabajo asignado a usted &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Proyecto de tarea<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó la tarea predecesora<br>Estado anterior de la tarea predecesora<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td>
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
   <td> <p><strong>Al finalizar todas mis tareas predecesoras</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico de cada predecesora que se complete.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt;</em><br></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Proyecto de tarea<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó la tarea predecesora<br>Estado anterior de la tarea predecesora<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
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
   <td> <p><strong>Cuando se apruebe o rechace un problema, enviar mensaje al usuario asignado</strong> </p> <p>El usuario asignado de un problema recibe una notificación por correo electrónico cuando se toma una decisión de aprobación (aprobada o rechazada).</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Problema con aprobación pendiente: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen del trabajo asignado a usted &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que aprobó o rechazó el problema<br>Decisión de aprobación (aprobada o rechazada)<br>Estado del problema<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas aprobados o rechazados<br>*Nombre del problema<br>* Nombre del usuario que aprobó o rechazó el problema<br>*Decisión de aprobación (aprobada o rechazada)<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Enviar correo electrónico al usuario asignado cuando se resuelva el problema</strong> </p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Completado: &lt;issue name=""&gt; el &lt;project name=""&gt;</em></p> <p><em> El asunto de la notificación de resumen diario es: Resumen del trabajo asignado a usted &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que ha completado el problema<br>Nuevo estado del problema<br>Fecha y hora en que se completó el problema<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas resueltos<br>*Nombre del problema<br>*Nombre del usuario que ha completado el problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando se suba o actualice un documento en una solicitud que se me haya asignado</strong> </p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando se cargan documentos o se cambian los detalles del documento sobre un problema que ha añadido.</p> <p>No se envía una notificación por correo electrónico si el usuario que activó el problema es el usuario asignado del mismo.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] y si el proyecto está configurado como Cola de solicitudes de ayuda (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se agregó un documento [!UICONTROL a] &lt;request name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de solicitud<br>Nombre de proyecto (nombre de cola de solicitudes)<br>Número de referencia del documento <br>Nombre del usuario que cargó el documento<br>Nombre de documento <br>Añadido el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de documentos cargados o cambiados<br>*Nombre del documento<br>*Nombre del objeto<br>*Nombre del usuario que ha cargado el documento<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambio de fecha límite de una tarea que tengo asignada</strong> </p> <p>El usuario asignado a la tarea recibe una notificación por correo electrónico cuando cambia la [!UICONTROL Fecha planificada de finalización] de la tarea, a menos que el usuario que cambió la fecha planificada de finalización también sea el usuario asignado a la tarea.</p> <p>Solo se envía una notificación si el estado del proyecto no es [!UICONTROL Planning].</p> <p>No se envía ninguna notificación con respecto a las tareas personales.</p> <p> Los usuarios con una licencia de revisión o solicitante no reciben ninguna notificación. </p> <p> El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL La fecha de vencimiento ha cambiado.]</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nueva fecha de vencimiento ([!UICONTROL Fecha planificada de finalización])<br>Fecha y hora en que se cambió la fecha de vencimiento<br>El nombre del usuario que cambió la fecha de vencimiento<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas donde cambió la fecha de vencimiento (fecha planificada de finalización)<br>*Nombre de tarea<br>*Nueva fecha planificada de finalización<br>*Nombre del usuario que ha cambiado la fecha de vencimiento<br>*Fecha del resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y a diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Si cambia la fecha planificada de finalización de un problema, notificar al usuario asignado</strong> </p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando cambia la fecha planificada de finalización de [!UICONTROL], a menos que el usuario que cambió la fecha planificada de finalización de [!UICONTROL] también sea el usuario asignado.</p> <p>Solo se envía una notificación si el estado del proyecto no es [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL La fecha de vencimiento se ha cambiado]</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nueva fecha de vencimiento ([!UICONTROL Fecha planificada de finalización])<br>Fecha y hora en que se cambió la fecha límite<br>Nombre del usuario que cambió la fecha límite<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas donde cambió la fecha de vencimiento ([!UICONTROL Fecha planificada de finalización])<br>*Nombre del problema<br>*Nueva fecha planificada de finalización de [!UICONTROL]<br>*Nombre del usuario que ha cambiado la fecha de vencimiento<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y a diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>El estado cambia en una tarea a la que he sido asignado</strong> <p>El Usuario asignado a la tarea recibe una notificación por correo electrónico cuando cambia el estado de la tarea, a menos que el usuario que ha cambiado el estado también sea el asignado.</p> <p>Nota: Esta notificación no se envía cuando el estado de la tarea cambia a completo. Se utiliza una notificación independiente para las tareas completadas. Consulte <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Se finaliza una tarea a la que estoy asignado</a>, arriba.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;task name=""&gt; de &lt;project name=""&gt; es &lt;new status=""&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado<br>Previsualizar estado<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas en las que se cambió el estado<br>*Nombre de tarea<br>*Estado de la tarea anterior<br>*Estado de la nueva tarea<br>*Nombre del usuario que ha cambiado el estado<br>*Fecha del resumen diario<br></td> 
   <td><strong>[!UICONTROL diario]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en uno de mis elementos de trabajo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando cambie el estado de un problema al que esté asignado, a menos que cambie el estado usted mismo. </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;issue name=""&gt; de &lt;project name=""&gt; es &lt;new status=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado<br>Estado del problema anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas en los que ha cambiado el estado<br>*Nombre de tarea<br>*Estado de problema anterior<br>*Nuevo estado del problema<br>*Nombre del usuario que ha cambiado el estado<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
