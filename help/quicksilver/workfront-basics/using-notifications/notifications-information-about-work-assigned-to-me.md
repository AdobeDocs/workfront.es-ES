---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Información sobre el trabajo asignado a mí'
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en un elemento de trabajo asignado a usted.
author: Courtney
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 16%

---

# Notificaciones: Información sobre el trabajo asignado a mí

Las siguientes notificaciones le avisan sobre las actividades que se producen en un elemento de trabajo asignado a usted.

Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se ha completado una tarea predecesora de una tarea asignada a mi equipo</strong> </p> <p>El equipo asignado recibe una notificación por correo electrónico cuando se completa una tarea predecesora de una de sus tareas. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Completado: &lt;Nombre de tarea&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre de tarea predecesora<br>Proyecto de tarea predecesora<br>Número de referencia de la tarea predecesora<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de predecesoras completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </p> </td> 
   <td><strong>Diariamente</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Se completa una de mis tareas predecesoras</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa una tarea predecesora de una de sus tareas. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre de tarea predecesora<br>Proyecto de tarea predecesora<br>Número de referencia de la tarea predecesora<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de predecesoras completadas<br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br> de resumen diario </p> </td> 
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
   <td> <p><strong>Se aprueba o rechaza una tarea que finalizo</strong> </p> <p>El usuario a quien le han asignado la tarea recibe una notificación por correo electrónico cuando se aprueba o rechaza la tarea.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que concedió la aprobación<br>Nuevo estado de la tarea<br>Fecha y hora en que se aprobó o rechazó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> button<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas aprobadas o rechazadas<br>*Nombre de tarea<br>*Nombre del usuario que aprobó o rechazó la tarea<br>*Decisión de aprobación ([!UICONTROL aprobada]/[Rechazado])<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Se completó una tarea a la que estoy asignado</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa la tarea.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a [!UICONTROL Complete], el asunto del correo electrónico seguirá indicando "Complete".</p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Se han finalizado todas las tareas predecesoras de una tarea asignada a mi equipo</strong> </p> <p>El equipo asignado recibe una notificación por correo electrónico cuando una tarea predecesora de una de sus tareas se marca como completada.</p> <p>Los usuarios con una licencia de revisión o solicitante no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Tarea completada: &lt;Nombre&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen del trabajo asignado a usted &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Proyecto de tarea<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó el predecesor<br>Estado anterior de la tarea predecesora<br><strong>Ver más detalles</strong> button<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td>
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
   <td> <p><strong>Se han completado todas las tareas predecesoras de mis tareas</strong> </p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico de cada predecesora que se complete.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt;</em><br></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Proyecto de tarea<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea predecesora<br>Estado de la tarea predecesora<br>Fecha y hora en que se completó la predecesora<br>Estado anterior de la tarea predecesora<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
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
   <td> <p><strong>Se aprueba o rechaza un problema que resuelvo</strong> </p> <p>El usuario a quien le han asignado un problema recibe una notificación por correo electrónico cuando se toma una decisión de aprobación (aprobada o rechazada).</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Problema con aprobación pendiente: &lt;Fecha planificada de inicio&gt; &lt;Número de referencia del problema&gt; - &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen del trabajo asignado a usted &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que aprobó o rechazó el problema<br>Decisión de aprobación (aprobada o rechazada)<br>Estado del problema<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver más detalles]</strong> button<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas aprobados o rechazados<br>*Nombre del problema<br>*Nombre del usuario que aprobó o rechazó el problema<br>*Decisión de aprobación (aprobada o rechazada Rechazado)<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Se ha completado un problema al que estoy asignado</strong> </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Completado: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p><em> El asunto de la notificación de resumen diario es: Resumen del trabajo asignado a usted &lt;Fecha del resumen diario&gt; </em> </p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que completó el problema<br>Nuevo estado del problema<br>Fecha y hora en que se completó el problema<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario que completó el problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Los documentos se han cargado o cambiado en las solicitudes a las que estoy asignado</strong> </p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando se cargan documentos o se cambian los detalles del documento sobre un problema que ha añadido.</p> <p>No se envía una notificación por correo electrónico si el usuario que activó el problema es el usuario asignado del mismo.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y si el proyecto está configurado como una cola de solicitudes de ayuda (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Documento agregado a] &lt;Nombre de solicitud&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre de solicitud<br>Nombre del proyecto (Nombre de la cola de solicitud)<br>Número de referencia del documento <br>Nombre del usuario que cargó el documento<br>Nombre del documento <br>Añadido en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Vista previa]</strong> y <strong>[!UICONTROL Descarga]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos cargados o cambiados<br>*Nombre del documento<br>*Objeto Nombre<br>*Nombre del usuario que cargó el documento<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambio de fecha límite de una tarea que tengo asignada</strong> </p> <p>El usuario asignado a la tarea recibe una notificación por correo electrónico cuando cambia la [!UICONTROL Fecha planificada de finalización] de la tarea, a menos que el usuario que cambió la fecha planificada de finalización también sea el usuario asignado a la tarea.</p> <p>Solo se envía una notificación si el estado del proyecto no es [!UICONTROL Planning].</p> <p>No se envía ninguna notificación con respecto a las tareas personales.</p> <p> Los usuarios con una licencia de revisión o solicitante no reciben ninguna notificación. </p> <p> El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL La fecha de vencimiento se ha cambiado.]</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nueva fecha de vencimiento ([!UICONTROL Fecha planificada de finalización])<br>Fecha y hora en que se cambió la fecha de vencimiento<br>Nombre del usuario que cambió la fecha de vencimiento<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas en las que cambió la fecha de vencimiento (fecha planificada de finalización)<br>*Nombre de tarea<br>*Nueva fecha planificada de finalización<br>*Nombre del usuario que cambió la fecha de vencimiento<br>*Fecha de resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia la fecha límite de un problema al que estoy asignado</strong> </p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando cambia la fecha planificada de finalización de , a menos que el usuario que cambió la fecha planificada de finalización de  también sea el usuario asignado.</p> <p>Solo se envía una notificación si el estado del proyecto no es [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL La fecha de vencimiento se ha cambiado]</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nueva fecha de vencimiento ([!UICONTROL Fecha planificada de finalización])<br>Fecha y hora en que se cambió la fecha de vencimiento<br>Nombre del usuario que cambió la fecha de vencimiento<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas en los que cambió la fecha de vencimiento ([!UICONTROL Fecha planificada de finalización])<br>*Nombre del problema<br>*Nueva fecha planificada de <br>*Nombre del usuario que cambió la fecha de vencimiento<br> el resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>El estado cambia en una tarea a la que estoy asignado</strong> <p>El usuario asignado a la tarea recibe una notificación por correo electrónico al cambiar el estado de la tarea, a menos que el usuario que cambie el estado sea el asignado.</p> <p>Nota: Esta notificación no se envía cuando el estado de la tarea cambia a completo. Se utiliza una notificación independiente para las tareas completadas. Ver <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Se completó una tarea a la que estoy asignado</a>, más arriba.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;Nombre de tarea&gt; de &lt;Nombre de proyecto&gt; es &lt;Nuevo estado&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado<br>Estado de vista previa<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas en las que cambió el estado<br>*Nombre de tarea<br>*Estado de tarea anterior<br>*Nuevo estado de tarea<br>*Nombre del usuario que cambió el estado<br>*Fecha del resumen diario<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en uno de mis elementos de trabajo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando cambie el estado de un problema al que esté asignado, a menos que cambie el estado usted mismo. </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] o [!UICONTROL Requestor] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;Nombre del problema&gt; de &lt;Nombre del proyecto&gt; es &lt;Nuevo estado&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen del trabajo asignado a usted] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado<br>Estado del problema anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas en los que cambió el estado<br>*Nombre de la tarea<br>*Estado del problema anterior<br>*Estado del problema nuevo<br>*Nombre del usuario que cambió el estado<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
