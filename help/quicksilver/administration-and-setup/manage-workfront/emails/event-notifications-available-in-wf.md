---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Notificaciones de eventos disponibles en Adobe Workfront
description: Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos tales como proyectos, tareas y problemas, como se explica en Notificaciones de eventos .
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 25625291f691f7858634d9961fccb4465008dc3c
workflow-type: tm+mt
source-wordcount: '5008'
ht-degree: 28%

---

# Notificaciones de eventos disponibles en Adobe Workfront

Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas y problemas, tal como se explica en [Notificaciones de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

Estas notificaciones se pueden configurar a nivel de sistema y de grupo:

* Para obtener información sobre la configuración de notificaciones de eventos en el sistema, consulte [Configurar notificaciones de eventos para todos los miembros del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Para obtener información sobre la configuración de notificaciones de eventos en el nivel de grupo, consulte [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Los usuarios individuales también pueden activar y desactivar sus notificaciones de eventos individuales en su perfil individual. Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

En las tablas siguientes se enumeran todas las notificaciones de eventos de Adobe Workfront, una breve descripción del evento y si el evento está activo o inactivo de forma predeterminada.

## Se requiere una acción

Consulte también [Notificaciones: Acción necesaria](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Solicitud de acceso al usuario</p> </td> 
   <td> <p>Alguien solicita acceso para mí.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Solicitud de documento agregada a solicitante</p> </td> 
   <td> <p>Solicitar cargar documentos.</p> <p>La solicitud de documento recibe una notificación por correo electrónico cuando recibe una solicitud para cargar un documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento pendiente de aprobación a los aprobadores</p> </td> 
   <td> <p>Necesito aprobar un documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Asignación de problema a Problema asignado a</p> </td> 
   <td> <p>Cuando cambie la asignación de un problema, enviar correo electrónico al usuario recientemente asignado.</p> <p>El destinatario del problema recibe una notificación por correo electrónico solo si el estado del proyecto es Actual y el estado del problema no es Cerrado o si algo coincide con Cerrado.</p> <p>Los usuarios con una licencia de revisión o solicitud no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema con aprobación pendiente para aprobadores</p> </td> 
   <td> <p>Necesito aprobar un problema.</p> <p>Los usuarios que reciben una notificación por correo electrónico para este evento dependen de si el ajuste "Aprobador no requerido para pertenecer al equipo del proyecto (para procesos de aprobación que incluyen una función)" está habilitado (tal y como se describe en <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuración de la aprobación global</a>). </p> <p>Si esta opción está habilitada</strong>, se envía una notificación por correo electrónico a todos los usuarios del sistema con la función de trabajo "Aprobador".</p> <p>Si esta opción está desactivada</strong>, solo los miembros del equipo del proyecto con la función de trabajo "Aprobador" reciben una notificación por correo electrónico.</p> <p>Se envía una notificación si el proyecto está en estado Planning o Current . </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema con aprobación pendiente para aprobador delegado</p> </td> 
   <td> <p>Necesito revisar una aprobación de problema que se ha delegado.</p> <p>Cuando alguien delega la aprobación de un problema a otro usuario, se notifica al usuario. </p> <p>Solo se envía una notificación cuando el proyecto está en estado Actual.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Proyecto con aprobación pendiente para aprobadores</p> </td> 
   <td> <p>Cuando un proyecto tiene su aprobación pendiente, envíe un mensaje al aprobador.</p> <p>Los usuarios que reciben una notificación por correo electrónico para este evento dependen de si el ajuste "Aprobador no requerido para pertenecer al equipo del proyecto (para procesos de aprobación que incluyen una función de trabajo)" está habilitado (tal como se describe en <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuración de la aprobación global</a>).</p> <p>Si esta opción está habilitada</strong>, se envía una notificación por correo electrónico a todos los usuarios del sistema con la función de trabajo "Aprobador".</p> <p>Si esta opción está desactivada</strong>, solo los miembros del equipo del proyecto con la función de trabajo "Aprobador" reciben una notificación por correo electrónico.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Proyecto con aprobación pendiente para aprobador delegado</td> 
   <td> <p>Necesito revisar una aprobación de proyecto que se me ha delegado.</p> </td> 
   <td> Activo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Asignación de tareas a Tarea asignada a</p> </td> 
   <td> <p>Se me establece como el principal asignado a una tarea.</p> <p>El asignador de tareas recibe una notificación por correo electrónico si se convierte en el asignador principal de la tarea, a menos que el usuario asignado sea el usuario que realizó la asignación.</p> <p>Se envía una notificación si el estado del proyecto es Current y la tarea no está marcada como Complete.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Tarea con aprobación pendiente para aprobadores</p> </td> 
   <td> <p>Necesito aprobar una tarea.</p> <p>Los usuarios que reciben una notificación por correo electrónico para este evento dependen de si el ajuste "Aprobador no requerido para pertenecer al equipo del proyecto (para procesos de aprobación que incluyen una función)" está habilitado (tal y como se describe en <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuración de la aprobación global</a>). </p> <p>Si esta opción está habilitada</strong>, se envía una notificación por correo electrónico a todos los usuarios del sistema con la función de trabajo "Aprobador".</p> <p>Si esta opción está desactivada</strong>, solo los miembros del equipo del proyecto con la función de trabajo "Aprobador" reciben una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento de la solicitud.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Tarea con aprobación pendiente para aprobador delegado</p> </td> 
   <td> <p>Necesito revisar una aprobación de tarea que se me ha delegado.</p> <p>Cuando alguien delega la aprobación de un problema a otro usuario, se notifica al usuario. </p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento de la solicitud.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Reapertura de una hoja de horas a Usuario</p> </td> 
   <td> <p>Se ha reabierto mi hoja de horas.</p> <p>El propietario del parte de horas recibe una notificación por correo electrónico cuando se vuelve a abrir el parte de horas, a menos que el usuario que volvió a abrir el parte de horas también sea el propietario del parte de horas.</p> <p>Solo se envía una notificación por correo electrónico si el estado del parte de horas es Abrir.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Hoja de horas rechazada a usuario</p> </td> 
   <td> <p>Cuando se rechaza una hoja de horas, enviar correo electrónico al usuario.</p> <p>El propietario del parte de horas recibe una notificación por correo electrónico cuando se rechaza el parte de horas, a menos que el usuario que rechazó el parte de horas también sea el propietario.</p> <p>Solo se envía una notificación por correo electrónico si el estado del parte de horas es Rechazado.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Envío de hoja de horas a Aprobador</p> </td> 
   <td> <p>Necesito aprobar una hoja de horas.</p> <p>El aprobador de parte de horas recibe una notificación por correo electrónico cuando se envía un parte de horas que necesitan aprobar, a menos que el usuario que ha enviado el parte de horas también sea el aprobador de parte de horas.</p> <p>Solo se envía una notificación si se envía el estado del parte de horas.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Asignación</p> </td> 
   <td> <p>Solicitud de elemento de trabajo al equipo</p> </td> 
   <td> <p>Mi equipo recibe una nueva solicitud de trabajo.</p> <p>Los integrantes del equipo reciben una notificación por correo electrónico cuando el equipo recibe una nueva solicitud de trabajo. (El usuario que ha enviado la solicitud no recibe ninguna notificación si es miembro del equipo).</p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento en que se realiza la solicitud de trabajo y el estado de la solicitud de trabajo es Nuevo.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Asignación</p> </td> 
   <td> <p>Solicitud de elemento de trabajo a la persona asignada al elemento</p> </td> 
   <td> <p>Recibo una nueva solicitud de trabajo.</p> <p>El usuario asignado del elemento de trabajo recibe una notificación por correo electrónico, a menos que el usuario que realiza la solicitud también sea el usuario asignado. </p> <p>No se envía una notificación si el estado de la tarea es Complete o si el estado del problema es Closed.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento de la solicitud.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitudes que he formulado

Consulte también [Notificaciones: Solicitudes que he formulado](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Se cambió el estado de aprobación de documento a solicitante</p> </td> 
   <td> <p>Se completó una solicitud de aprobación de documento.</p> <p>El Solicitante del documento recibe una notificación por correo electrónico cuando se completa la solicitud de aprobación del documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitud de documento completada para solicitante</p> </td> 
   <td> <p>Se completa una solicitud de subir documento.</p> <p>El Solicitante del documento recibe una notificación por correo electrónico cuando se completa una solicitud para cargar un documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema al autor del mismo</p> </td> 
   <td> <p>Agrego un problema a un proyecto.</p> <p>El contacto principal de un problema recibe una notificación cuando añade un problema a un proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Asignación de problema a Creador del problema</td> 
   <td> <p>Se asigna a alguien a un problema en el cual soy el contacto principal.</p> <p>El contacto principal de un problema recibe una notificación cuando el problema se asigna a un usuario. </p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> Inactivo</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema al creador del problema</p> </td> 
   <td> <p>Enviar correo electrónico al creador del problema cuando se resuelva el problema.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Se cambió el estado del proyecto a Ingresado por</p> </td> 
   <td> <p>Cambia el estado de un proyecto que he creado.</p> <p>El usuario que ha creado el proyecto recibe una notificación por correo electrónico cuando cambia el estado del proyecto.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar solicitud al autor del problema</p> </td> 
   <td> <p>Yo envío una solicitud (confirmación).</p> <p>El contacto principal sobre el problema recibe una notificación por correo electrónico cuando envía un problema.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto está utilizando la vista "Es un servicio de asistencia al cliente".</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Asignar solicitud al autor del problema</p> </td> 
   <td> <p>Alguien está asignado a mi solicitud.</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se asigna un usuario al problema, a menos que el contacto principal y el usuario asignado sean el mismo usuario.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto está utilizando la vista "Es un servicio de asistencia al cliente".</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cerrar solicitud al autor del problema</p> </td> 
   <td> <p>Mi solicitud se ha cerrado (confirmación).</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se cierra la solicitud.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto está utilizando la vista "Es un servicio de asistencia al cliente".</p> <p>Si las notificaciones para la "finalización del problema" están habilitadas, siempre se almacenarán en déclencheur en lugar de "Solicitud cerrada para emitir contacto principal". Si desea que esta notificación se déclencheur, debe desactivar las notificaciones de "finalización del problema".</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Agregar documento de solicitud al autor del problema</p> </td> 
   <td> <p>Se ha cambiado o subido un documento en un problema en el cual soy el autor.</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se carga o cambia un documento del problema, a menos que el usuario que cargó o cambió el documento también sea el contacto principal.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto tiene habilitado "Publicar como cola de solicitud de ayuda" en la ficha Configuración de cola.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de estado de solicitud al autor del problema</p> </td> 
   <td> <p>El estado cambia en mi solicitud.</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando cambia el estado del problema, a menos que el usuario que cambió el estado también sea el contacto principal.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y el proyecto está utilizando la vista "Es asistencia técnica".</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Comunicación

Consulte también [Notificaciones: Comunicación](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Comentar en el documento con el propietario del documento</p> </td> 
   <td> <p>Se agrega un comentario en mi documento.</p> <p>El propietario de un documento en Workfront recibe una notificación por correo electrónico cuando se publica un comentario en el documento, a menos que el usuario que publicó el comentario también sea el propietario del documento.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Comentar en &lt;request name=""&gt; en &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> El tema de la notificación diaria de compendio es:<em> Resumen de comunicación &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Activo </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Agregar nota de solicitud al autor del problema</p> </td> 
   <td> <p>Cuando se publique un comentario en una solicitud, envíe un correo electrónico al contacto principal del problema.</p> <p>El contacto principal de un problema recibe una notificación por correo electrónico cuando se publica un comentario en una solicitud, a menos que el usuario que publicó el comentario también sea el contacto principal del problema.</p> <p>Los usuarios que estén incluidos directamente en el comentario también recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td>Actualización dirigida al usuario</td> 
   <td> <p>Alguien me incluye en una actualización dirigida.</p> <p>Una actualización dirigida se produce cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar otros en actualizaciones</a>.</p> <p>En este caso, el usuario incluido en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico se envía únicamente si el usuario tiene derechos de acceso al objeto y si lo mantiene habilitado en su perfil.  </p> <p>Esta notificación de evento está activada de forma predeterminada y no se puede desactivar.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Equipo</p> </td> 
   <td> <p>Actualización dirigida al equipo</p> </td> 
   <td> <p>Alguien incluye a mi equipo en una actualización dirigida.</p> <p>Una actualización dirigida se produce cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar otros en actualizaciones</a>.</p> <p>En este caso, cualquier miembro del equipo incluido en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico solo se envía a los usuarios que tienen derechos de acceso al objeto de la actualización.</p> <p>Si el usuario que envía la actualización dirigida es miembro del equipo que se incluye, el usuario que envía la actualización no recibe una notificación por correo electrónico.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentario en elemento de trabajo a participantes del hilo</p> </td> 
   <td> <p>Alguien agrega un comentario a un hilo en el cual participo.</p> <p>Los participantes en el subproceso y los usuarios incluidos en un mensaje directo reciben una notificación por correo electrónico cuando un usuario hace un comentario en el subproceso.</p> <p>Los usuarios deben tener acceso a Ver para recibir una notificación.</p> <p>Los siguientes usuarios no reciben una notificación:</p> 
    <ul> 
     <li> <p>Equipos que se incluyen en un mensaje directo</p> </li> 
     <li> <p>El propietario de la Nota</p> </li> 
     <li> <p>El contacto principal</p> </li> 
    </ul> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentario de elemento de trabajo a la persona asignada al elemento</p> </td> 
   <td> <p>Alguien agrega comentarios a uno de mis elementos de trabajo.</p> <p>El usuario asignado del elemento de trabajo recibe una notificación por correo electrónico cada vez que un usuario agrega una actualización a un elemento de trabajo, a menos que el usuario que agrega la actualización también sea el usuario asignado.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Respuesta de solicitud de trabajo al solicitante</p> </td> 
   <td> <p>Alguien responde a mi solicitud.</p> <p>Una vez que un usuario envía una solicitud y otro responde a ella, el usuario que la ha enviado recibe una notificación por correo electrónico.</p> <p>No se envía una notificación por correo electrónico si:</p> 
    <ul> 
     <li> <p>El usuario que responde es el mismo usuario que realizó la solicitud</p> </li> 
     <li> <p>El usuario no tiene acceso para ver la nota</p> </li> 
    </ul> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Información de aprobación

Consulte también [Notificaciones: Información de aprobación](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Delegación de aprobación para otro usuario</p> </td> 
   <td> <p>Se me ha delegado como aprobador.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de estado de aprobación delegada de problema</p> </td> 
   <td> <p>Se completó una solicitud de aprobación delegada de problema. </p> <p>Cuando delega una aprobación de problema a otra persona, recibe una notificación por correo electrónico cuando termina esa aprobación (tanto si aprueba como si rechaza la aprobación del problema). </p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio de estado de aprobación delegada de proyecto</p> </td> 
   <td> <p>Se completó una solicitud de aprobación delegada de proyecto.</p> <p>Cuando delega la aprobación de un proyecto a otra persona, recibe una notificación por correo electrónico cuando termina la aprobación (tanto si aprueba como si rechaza la aprobación del proyecto).</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de estado de aprobación delegada de tarea</p> </td> 
   <td> <p>Se completó un estado de aprobación de tarea delegada.</p> <p>Cuando delega una aprobación de tarea a otra persona, recibe una notificación por correo electrónico cuando termina esa aprobación (tanto si aprueba como si rechaza la aprobación de la tarea).</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aprobación de documento cancelada para aprobador</p> </td> 
   <td> <p>Se canceló una solicitud de aprobación de documento.</p> <p>El Aprobador de documento recibe una notificación por correo electrónico cuando se cancela la solicitud de aprobación del documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Aprobación de una hoja de horas a usuario</p> </td> 
   <td> <p>Se aprueba mi hoja de horas.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información sobre el trabajo asignado a mí

Consulte también [Notificaciones: Información sobre el trabajo asignado a mí](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tarea</td> 
   <td>Finalización de todas las tareas predecesoras a dependientes de tareas en el equipo asignado</td> 
   <td> <p>Se completan todos los predecesores de las tareas del equipo.</p> <p>Los asignadores de tareas (todos los miembros del equipo) reciben una notificación por correo electrónico.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td>Inactivo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de todas las tareas predecesoras a dependientes de tareas</p> </td> 
   <td> <p>Al finalizar todas mis tareas predecesoras.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisión de aprobación para emitir asignada a</p> </td> 
   <td> <p>Cuando se apruebe o rechace un problema, enviar mensaje al usuario asignado.</p> <p>El usuario asignado de un problema recibe una notificación por correo electrónico cuando se toma una decisión de aprobación (aprobada o rechazada).</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Decisión de aprobación a la tarea asignada a</p> </td> 
   <td> <p>Se aprueba o rechaza una tarea que finalizo.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando la tarea se aprueba o rechaza.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema a Problema asignado a</p> </td> 
   <td> <p>Enviar correo electrónico al usuario asignado cuando se resuelva el problema.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambió la fecha planificada de finalización de problema</p> </td> 
   <td> <p>Si cambia la fecha planificada de finalización de un problema, notificar al usuario asignado.</p> <p>El destinatario del problema recibe una notificación por correo electrónico cuando cambia la fecha de finalización planeada, a menos que el usuario que cambió la fecha de finalización planeada también sea el usuario asignado.</p> <p>Solo se envía una notificación si el estado del proyecto es cualquier cosa que no sea Planning.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de estado de problema a problema asignado a</p> </td> 
   <td> <p>El estado cambia en uno de mis elementos de trabajo.</p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando cambia el estado, a menos que el usuario que cambió el estado también sea el usuario asignado.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Agregar documento de solicitud a persona a la que se asignó el problema</p> </td> 
   <td> <p>Cuando se suba o actualice un documento en una solicitud que se me haya asignado.</p> <p>El destinatario del problema recibe una notificación por correo electrónico cuando se cargan o cambian documentos en un problema que han añadido.</p> <p>No se envía una notificación por correo electrónico si el usuario que ha introducido el problema es el destinatario del mismo.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto tiene habilitado "Publicar como cola de solicitud de ayuda" en la ficha Configuración de cola.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tareas a Tarea asignada a</p> </td> 
   <td> <p>Se finaliza una tarea a la cual estoy asignado.</p> <p>El asignador de tareas recibe una notificación por correo electrónico cuando se completa la tarea. Las notificaciones no se envían cuando se completa una tarea personal.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de revisión o solicitante no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea a Dependientes de tareas</p> </td> 
   <td> <p>Se ha completado un predecesor de una de mis tareas.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa una de las predecesoras de la tarea.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de fecha planificada de finalización de tarea</p> </td> 
   <td> <p>Cambio de fecha límite de una tarea a la que estoy asignado.</p> <p>El asignador de tareas recibe una notificación por correo electrónico cuando cambia la fecha de finalización planeada de la tarea, a menos que el usuario que cambió la fecha de finalización planeada también sea el asignador de tareas.</p> <p>Solo se envía una notificación si el estado del proyecto es cualquier cosa que no sea Planning.</p> <p>No se envía ninguna notificación con respecto a las tareas personales.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de estado de tarea a Tarea asignada a</p> </td> 
   <td> <p>El estado cambia en una tarea a la que he sido asignado.</p> <p>El asignador de tareas recibe una notificación por correo electrónico cuando cambia el estado de la tarea, a menos que el usuario que ha cambiado el estado también sea el asignado.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Información sobre proyectos en los que estoy

Consulte también [Notificaciones: Información sobre proyectos en los que estoy](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Se cambió el estado del proyecto actual a Equipo del proyecto</p> </td> 
   <td> <p>Se activa un proyecto en el que participo.</p> <p>Los usuarios del proyecto reciben una notificación por correo electrónico cuando el proyecto se activa.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento agregado al equipo del proyecto</p> </td> 
   <td> <p>Se agrega un documento a proyecto en el que participo.</p> <p>Los usuarios del equipo del proyecto reciben una notificación por correo electrónico cuando se agrega un documento al proyecto, excepto para el usuario que lo agregó.</p> <p>Solo se envía una notificación si el estado del proyecto es Current y el documento no es Private. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema agregado al equipo del proyecto</p> </td> 
   <td> <p>Se agrega un problema a un proyecto en el que participo.</p> <p>Los usuarios de un proyecto reciben una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema al equipo del proyecto</p> </td> 
   <td> <p>Se resuelve un problema en un proyecto en el que participo.</p> <p>Cualquier usuario del proyecto recibe una notificación.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea de hito a Equipo del proyecto</p> </td> 
   <td> <p>Se completa una tarea de hito en un proyecto en el que participo.</p> <p>Todos los usuarios del equipo de proyecto reciben una notificación cuando se completa una tarea de hitos. </p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Finalización de proyecto a Equipo del proyecto</p> </td> 
   <td> <p>Se completa un proyecto en el que participo.</p> <p>Los usuarios de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto es Completado.</p> <p>Sugerencia: Si los proyectos se completan con regularidad, la activación de esta opción puede crear un montón de correos electrónicos para los usuarios que tienen un número limitado de tareas en muchos proyectos. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Se cambió el estado del proyecto a Equipo del proyecto</p> </td> 
   <td> <p>Cambia el estado de un proyecto en el que participo.</p> <p>Los usuarios del equipo del proyecto reciben una notificación por correo electrónico cuando cambia el estado del proyecto. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario de proyecto</p> </td> 
   <td> <p>Adición del usuario de proyecto al Usuario de proyecto</p> </td> 
   <td> <p>Se me agrega a un proyecto.</p> <p>El usuario que se añadió al proyecto recibe una notificación por correo electrónico cuando se añade, a menos que se haya autoañadido al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea a Equipo del proyecto</p> </td> 
   <td> <p>Se finaliza una tarea en un proyecto en el que participo.</p> <p>Los miembros del equipo del proyecto reciben una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema no asignado al equipo del proyecto</p> </td> 
   <td> <p>Se agrega un problema no asignado a un proyecto en el que participo.</p> <p>Los usuarios de un proyecto reciben una notificación por correo electrónico cuando se agrega un problema sin asignar al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información sobre proyectos que tengo

Consulte también [Notificaciones: Información sobre proyectos que tengo](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento agregado al propietario del proyecto</p> </td> 
   <td> <p>Se agrega un documento a un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el usuario que agregó el documento también sea el propietario del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Current y el documento no es Private.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema al propietario del proyecto</p> </td> 
   <td> <p>Se agrega un problema a un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Notificar cambio de fecha de confirmación de problema al propietario del proyecto</p> </td> 
   <td> <p>Si cambia la fecha de confirmación de un problema en uno de mis proyectos.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de un problema del proyecto, a menos que el usuario que cambie la fecha de confirmación sea el mismo usuario que el propietario del proyecto.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema al propietario del proyecto</p> </td> 
   <td> <p>Se resuelve un problema en un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea de hito al propietario del proyecto</p> </td> 
   <td> <p>Se completa una tarea de hijo en un proyecto de mi propiedad.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Asignación de propietario del proyecto al propietario del proyecto</p> </td> 
   <td> <p>Se me asigna como propietario de un nuevo proyecto.</p> <p>Cuando se asigna a un usuario como propietario de un proyecto, este recibe una notificación por correo electrónico.</p> <p>Si el propietario del proyecto es el mismo usuario que realizó la asignación, no se envía una notificación por correo electrónico</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio del avance del proyecto a propietario del mismo</p> </td> 
   <td> <p>Se retrasa un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando el proyecto está atrasado.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de fecha de confirmación de tarea al propietario del proyecto</p> </td> 
   <td> <p>Cambia la fecha de confirmación de una tarea en uno de mis proyectos.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de una tarea del proyecto, a menos que el usuario que cambió la fecha de confirmación también sea el propietario del proyecto.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea al propietario del proyecto</p> </td> 
   <td> <p>Finalización de una tarea de un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación. </p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de avance de tarea a propietario del proyecto</p> </td> 
   <td> <p>Se retrasa una tarea en un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa en la programación.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema no asignado al propietario del proyecto</p> </td> 
   <td> <p>Se agrega un problema no asignado a un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema sin asignar al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información sobre los proyectos que patrocino

Consulte también [Notificaciones: Información sobre los proyectos que patrocino](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Adición de documento al patrocinador del proyecto</p> </td> 
   <td> <p>Se añade un documento a un proyecto que patrocina.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el patrocinador del proyecto agregue el documento.</p> <p>Solo se envía una notificación si el estado del proyecto es Current y si el documento no es Private.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema al patrocinador del proyecto</p> </td> 
   <td> <p>Se agrega un problema a un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema al patrocinador del proyecto</p> </td> 
   <td> <p>Enviar mensaje de correo electrónico al patrocinador del proyecto al resolver un problema.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea de hito al patrocinador del proyecto</p> </td> 
   <td> <p>Se finaliza una tarea de hito en un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se completa una tarea de hitos en un proyecto que patrocina.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio del avance del proyecto al patrocinador del mismo</p> </td> 
   <td> <p>Se retrasa un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Asignación del patrocinador del proyecto al patrocinador del proyecto</p> </td> 
   <td> <p>Se me asigna como patrocinador de un proyecto.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se establece como patrocinador de un proyecto.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea al patrocinador del proyecto</p> </td> 
   <td> <p>Se finaliza una tarea en un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio del avance de la tarea al patrocinador del proyecto</p> </td> 
   <td> <p>Se retrasa una tarea en un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa en la programación.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema no asignado al patrocinador del proyecto</p> </td> 
   <td> <p>Se agrega un problema sin asignar a un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema sin asignar al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información diversa

Consulte también [Notificaciones: Información diversa](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Anuncio</td> 
   <td> <p>Se agregó el anuncio</p> </td> 
   <td> <p>Se envía un mensaje al Centro de anuncios.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitud de documento cancelada para solicitante</p> </td> 
   <td> <p>Cancelar una solicitud de carga de documento.</p> <p>La solicitud de documento recibe una notificación por correo electrónico cuando se cancela una solicitud de documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notificación de error</p> </td> 
   <td> <p>Se ha encontrado un error que necesita su atención.</p> <p>Se genera una notificación por correo electrónico después de que Workfront lo intente y no se conecte a una cuenta POP. Después de 25 intentos, Workfront deshabilita la conexión con la cuenta POP para conservar los recursos y envía una notificación. </p> <p>La notificación por correo electrónico se envía al propietario del proyecto, si el correo electrónico POP está asociado a una cola de solicitudes, o a los administradores de Workfront, si la cuenta POP está asociada a la función "Correo entrante" en Configuración de correo electrónico.
   </p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Asignación del problema al propietario del recurso</p> </td> 
   <td> <p>Cuando un cambio de asignación de problema afecte a alguien de mi grupo.</p> <p>El Administrador de asignaciones de problemas recibe una notificación por correo electrónico cuando un cambio afecta a un usuario que administra.</p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Nuevo usuario a usuario</p> </td> 
   <td> <p>Cuando se crea un usuario nuevo en Workfront, enviar correo electrónico al usuario.</p> <p>Una vez creado el nuevo usuario, este recibe una invitación por correo electrónico en la que se le notifica que se ha creado una cuenta de Workfront y se le pide que establezca su contraseña.</p> <p>Al crear un nuevo usuario, los usuarios pueden seleccionar la opción "Enviar un correo electrónico de invitación a esta persona" (tal como se describe en <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Agregar usuarios</a><span style="font-weight: 400;">). Sin embargo, cuando la opción "Nuevo usuario a usuario" está activada globalmente, todos los usuarios nuevos reciben la invitación por correo electrónico independientemente de si la opción "Enviar un correo electrónico de invitación a esta persona" está seleccionada.</span></p> </td> 
   <td> Inactivo </td> 
  </tr> 
  <tr> 
   <td> <p>Equipo</p> </td> 
   <td> <p>Objeto compartido con equipo</p> </td> 
   <td> <p>Alguien comparte un objeto con mi equipo.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Objeto compartido con usuario</p> </td> 
   <td> <p>Alguien comparte un objeto conmigo.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario de proyecto</p> </td> 
   <td> <p>Adición de usuario de proyecto al Propietario del recurso</p> </td> 
   <td> <p>Se agrega a una persona de mi equipo a un proyecto.</p> <p>Un administrador recibe una notificación por correo electrónico cuando se agrega uno de sus informes directos a un proyecto.</p> <p>Los usuarios con una licencia de revisión no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Se agrega un proyecto a un portafolio o programa</p> </td> 
   <td> <p>Alguien agrega un proyecto a un portafolio o programa de mi propiedad.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Asignación de la tarea al propietario del recurso</p> </td> 
   <td> <p>Cuando un cambio de asignación de tarea afecte a alguien de mi grupo.</p> <p>El Administrador del asignado de tareas recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> Proyecto <br>Tarea <br>Problema</td> 
   <td>Nueva actualización para el suscriptor </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Se envía un correo electrónico cuando se actualiza una tarea, un problema o un proyecto al que estoy suscrito.</span> </p> </td> 
   <td>Activo</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Delegación

Consulte también [Notificaciones: Delegación](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Tipo de objeto | Evento | Descripción | Estado predeterminado |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Tareas y problemas | Delegación de tarea y problema a asignado | Yo delego mis tareas y problemas (confirmación) | Activo |
| Tareas y problemas | Detener la delegación de tareas y problemas al asignado | Yo detengo la delegación de mis tareas y problemas (confirmación) | Activo |
| Tareas y problemas | Delegación de tarea y problema a delegado | Alguien delega sus tareas y problemas a mí | Activo |
| Tareas y problemas | Detener tareas y delegación de problemas para delegar | Alguien detiene la delegación de sus tareas y problemas a mí | Activo |
