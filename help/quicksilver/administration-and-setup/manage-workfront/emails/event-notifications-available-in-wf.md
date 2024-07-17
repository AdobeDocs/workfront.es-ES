---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Tipos de notificación de eventos
description: Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas y problemas. Este artículo enumera y describe los tipos de notificaciones de eventos disponibles.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '5201'
ht-degree: 7%

---

# Tipos de notificación de eventos

<!-- Audited: 1/2024 -->

Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas y problemas, tal como se explica en [Notificaciones de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

Estas notificaciones se pueden configurar en los sistemas y grupos:

* Para obtener información acerca de cómo configurar notificaciones de eventos en el sistema, consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Para obtener información acerca de cómo configurar notificaciones de eventos en el nivel de grupo, vea [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Los usuarios individuales también pueden activar y desactivar sus notificaciones de eventos individuales en su perfil individual. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

En las tablas siguientes se enumeran todas las notificaciones de eventos de Adobe Workfront, una breve descripción del evento y si el evento está activo o inactivo de forma predeterminada.

>[!NOTE]
>
>Las notificaciones con el valor &quot;Active&quot; en la columna Estado predeterminado están activas tanto para las notificaciones inmediatas como para las diarias de forma predeterminada, a menos que se indique lo contrario.

## Se requiere una acción

Ver también [Notificaciones: Acción necesaria](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Solicitud de acceso</p> </td> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Alguien solicita acceso para mí.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Solicitud de documento agregada</p> </td> 
   <td> <p>Usuario al que se solicita ese documento</p> </td> 
   <td> <p>Alguien ha solicitado que cargue documentos.</p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando recibe una solicitud para cargar un documento.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento pendiente de aprobación</p> </td> 
   <td> <p>Aprobadores</p> </td> 
   <td> <p>Necesito aprobar un documento.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Asignación de problema</p> </td> 
   <td> <p>Usuario al que se ha asignado el problema</p> </td> 
   <td> <p>Se me ha asignado un problema.</p> <p>El usuario asignado del problema recibe una notificación por correo electrónico únicamente si el estado del proyecto es Actual y el estado del problema no es Cerrado o si existe algo equivalente a Cerrado.</p> <p>Los usuarios con una licencia básica, de colaborador, de revisión o de solicitud no reciben ninguna notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema con aprobación pendiente</p> </td> 
   <td> <p>Aprobadores</p> </td> 
   <td> <p>Necesito aprobar un problema.</p> <p>Los usuarios que recibirán una notificación por correo electrónico para este evento dependen de si la opción "Aprobador no debe estar en el equipo del proyecto (para procesos de aprobación que incluyen un rol)" está habilitada (tal como se describe en <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurar la aprobación global</a>). </p> <p>Si esta opción está habilitada</strong>, se enviará una notificación por correo electrónico a todos los usuarios del sistema con la función de trabajo de "aprobador".</p> <p>Si esta opción está deshabilitada</strong>, solamente los miembros del equipo del proyecto con el rol de trabajo de "Aprobador" recibirán una notificación por correo electrónico.</p> <p>Se envía una notificación si el proyecto se encuentra en estado Planificación o Actual. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema con aprobación pendiente</p> </td> 
   <td> <p>Aprobador delegado</p> </td> 
   <td> <p>Necesito revisar una aprobación de problema que se me ha delegado.</p> <p>Cuando alguien delega una aprobación de problema a otro usuario, se notifica a ese usuario. </p> <p>Solo se envía una notificación cuando el proyecto se encuentra en el estado Actual.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Proyecto con aprobación pendiente</p> </td> 
   <td> <p>Aprobadores</p> </td> 
   <td> <p>Necesito aprobar un proyecto.</p> <p>Los usuarios que recibirán una notificación por correo electrónico para este evento dependen de si la opción "Aprobador no debe estar en el equipo del proyecto (para procesos de aprobación que incluyen un rol)" está habilitada (tal como se describe en <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurar la aprobación global</a>).</p> <p>Si esta opción está habilitada</strong>, se enviará una notificación por correo electrónico a todos los usuarios del sistema con la función de trabajo de "aprobador".</p> <p>Si esta opción está deshabilitada</strong>, solamente los miembros del equipo del proyecto con el rol de trabajo de "Aprobador" recibirán una notificación por correo electrónico.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Proyecto con aprobación pendiente</td> 
   <td>Aprobador delegado</td> 
   <td> <p>Necesito revisar una aprobación de proyecto que se me ha delegado.</p> </td> 
   <td> Activo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Asignación de tareas</p> </td> 
   <td> <p>Usuario al que se asigna la tarea</p> </td> 
   <td> <p>Se me establece como el principal asignado a una tarea.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico si se convierte en el usuario asignado principal de la tarea, a menos que el usuario asignado sea el usuario que realizó la asignación.</p> <p>Se envía una notificación si el estado del proyecto es Actual y la tarea no está marcada como Completada.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Tarea con aprobación pendiente</p> </td> 
   <td> <p>Aprobadores</p> </td> 
   <td> <p>Necesito aprobar una tarea.</p> <p>Los usuarios que recibirán una notificación por correo electrónico para este evento dependen de si la opción "Aprobador no debe estar en el equipo del proyecto (para procesos de aprobación que incluyen un rol)" está habilitada (tal como se describe en <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurar la aprobación global</a>). </p> <p>Si esta opción está habilitada</strong>, se enviará una notificación por correo electrónico a todos los usuarios del sistema con la función de trabajo de "aprobador".</p> <p>Si esta opción está deshabilitada</strong>, solamente los miembros del equipo del proyecto con el rol de trabajo de "Aprobador" recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento de la solicitud.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Tarea con aprobación pendiente</p> </td> 
   <td> <p>Aprobador delegado</p> </td> 
   <td> <p>Necesito revisar una aprobación de tarea que se me ha delegado.</p> <p>Cuando alguien delega una aprobación de problema a otro usuario, se notifica a ese usuario. </p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento de la solicitud.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Hoja de horas reabierta</p> </td> 
   <td> <p>Usuario al que pertenece la plantilla de horas</p> </td> 
   <td> <p>Se ha reabierto mi hoja de horas.</p> <p>El propietario de la plantilla de horas recibe una notificación por correo electrónico cuando se vuelve a abrir, a menos que el usuario que volvió a abrir la plantilla de horas sea también el propietario de la plantilla.</p> <p>Solo se envía una notificación por correo electrónico si el estado de la plantilla de horas es Abierto.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Hoja de horas rechazada</p> </td> 
   <td> <p>Usuario al que pertenece la plantilla de horas</p> </td> 
   <td> <p>Se rechaza mi hoja de horas.</p> <p>El propietario de la plantilla de horas recibe una notificación por correo electrónico cuando se rechaza, a menos que el usuario que la rechazó también sea el propietario.</p> <p>Solo se envía una notificación por correo electrónico si el estado de la plantilla de horas es Rechazado.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Envío de hoja de horas</p> </td> 
   <td> <p>Aprobador</p> </td> 
   <td> <p>Necesito aprobar una hoja de horas.</p> <p>El aprobador de hojas de horas recibe una notificación por correo electrónico cuando se envía una hoja de horas que debe aprobar, a menos que el usuario que ha enviado la hoja de horas también sea el aprobador de hojas de horas.</p> <p>Solo se envía una notificación si se envía el estado de la plantilla de horas.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Asignación</p> </td> 
   <td> <p>Solicitud de elemento de trabajo</p> </td> 
   <td> <p>Miembros del equipo para el que se solicita el elemento</p> </td> 
   <td> <p>Mi equipo recibe una nueva solicitud de trabajo.</p> <p>Los integrantes del equipo reciben una notificación por correo electrónico cuando el equipo recibe una nueva solicitud de trabajo. (El usuario que envió la solicitud no recibe una notificación si es miembro del equipo).</p> <p>Se enviará una notificación únicamente si el estado del proyecto es Actual en el momento de realizar la Solicitud de Trabajo y el estado de la Solicitud de Trabajo es Nuevo.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Asignación</p> </td> 
   <td> <p>Solicitud de elemento de trabajo</p> </td> 
   <td> <p>Usuario para el que se ha solicitado el elemento de trabajo</p> </td> 
   <td> <p>Recibo una nueva solicitud de trabajo.</p> <p>El usuario asignado del elemento de trabajo recibe una notificación por correo electrónico, a menos que el usuario que realiza la solicitud también sea el usuario asignado. </p> <p>No se envía una notificación si el estado de la tarea es Completa o el estado del problema es Cerrado.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual en el momento de la solicitud.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitudes que he realizado

Ver también [Notificaciones: solicitudes que he hecho](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Cambio de estado de aprobación de documento</p> </td> 
   <td> <p>Solicitante</p> </td> 
   <td> <p>Se completó una solicitud de aprobación de documento.</p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se completa la solicitud de aprobación del documento.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitud de documento completa</p> </td> 
   <td> <p>Solicitante</p> </td> 
   <td> <p>Se completa una solicitud de carga de documento.</p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se completa una solicitud para cargar un documento.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Agrego un problema a un proyecto.</p> <p>El contacto principal de un problema recibe una notificación cuando añade un problema en un proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Asignación de problema</td> 
   <td>Contacto principal del problema</td> 
   <td> <p>Se asigna a alguien a un problema en el cual soy el contacto principal.</p> <p>El contacto principal de un problema recibe una notificación cuando el problema se asigna a un usuario. </p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> Inactivo</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Enviar correo electrónico al creador del problema cuando se resuelva el problema.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio de estado del proyecto</p> </td> 
   <td> <p>Usuario que creó el proyecto (ingresado por)</p> </td> 
   <td> <p>El estado cambia en un proyecto que he creado.</p> <p>El usuario que ha creado el proyecto recibe una notificación por correo electrónico cuando cambia el estado del proyecto.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitud de adición</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Yo envío una solicitud (confirmación).</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando envía un problema.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual y si el proyecto utiliza una Vista "Es servicio de asistencia".</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitar asignación</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Alguien está asignado a mi solicitud.</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se asigna un usuario al problema, a menos que el contacto principal y el usuario asignado sean el mismo usuario.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual y si el proyecto utiliza una Vista "Es servicio de asistencia".</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Solicitud cerrada</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Mi solicitud se ha cerrado (confirmación).</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se cierra la solicitud.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual y si el proyecto utiliza una Vista "Es servicio de asistencia".</p> <p>Si las notificaciones de "finalización de problema" están habilitadas, siempre se almacenarán en déclencheur en lugar de "Solicitud cerrada al autor del problema". Si desea que esta notificación se almacene en déclencheur, debe desactivar las notificaciones de "finalización de problemas".</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitar documento agregado</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Se ha cambiado o subido un documento en un problema en el cual soy el autor.</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se carga o cambia un documento en el problema, a menos que el usuario que cargó o cambió el documento también sea el contacto principal.</p> <p>Se envía una notificación únicamente si el estado del proyecto es Actual y si el proyecto tiene la "Publish como Cola de solicitudes de ayuda" habilitada en la ficha Configuración de cola.</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de estado de solicitud</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>El estado cambia en mi solicitud.</p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando cambia el estado del problema, a menos que el usuario que ha cambiado el estado también sea el contacto principal.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual y si el proyecto utiliza la Vista "Es servicio de asistencia".</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Comunicación

Vea también [Notificaciones: Comunicación](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Comentario sobre el documento</p> </td> 
   <td> <p>Propietario de documento</p> </td> 
   <td> <p>Se agrega un comentario en mi documento.</p> <p>El propietario de un documento en Workfront recibe una notificación por correo electrónico cuando se publica un comentario en el documento, a menos que el usuario que publicó el comentario también sea el propietario del documento.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Comentario sobre &lt;Nombre de solicitud&gt; en &lt;Nombre de proyecto&gt; (ref# &lt;Número de referencia de solicitud&gt;)</em></p> <p> El asunto de la notificación de resumen diario es:<em> Resumen de la comunicación &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Agregar nota de solicitud</p> </td> 
   <td> <p>Contacto principal del problema</p> </td> 
   <td> <p>Cuando se publica un comentario en una solicitud, enviar por correo electrónico al autor del problema.</p> <p>El contacto principal de un problema recibe una notificación por correo electrónico cuando se publica un comentario en una solicitud, a menos que el usuario que publicó el comentario también sea el contacto principal del problema.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td>Actualización dirigida</td> 
   <td>Usuario</td> 
   <td> <p>Alguien me incluye en una actualización dirigida.</p> <p>Una actualización dirigida es cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a>.</p> <p>En este caso, el usuario que se incluye en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico se envía únicamente si el usuario tiene derechos de acceso al objeto y si lo mantiene activado en su perfil.  </p> <p>Esta notificación de eventos está activada de forma predeterminada y no se puede desactivar.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Equipo</p> </td> 
   <td> <p>Actualización dirigida</p> </td> 
   <td> <p>Integrantes del equipo</p> </td> 
   <td> <p>Alguien incluye a mi equipo en una actualización dirigida.</p> <p>Una actualización dirigida es cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a>.</p> <p>En este caso, cualquier miembro del equipo que se incluya en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico se envía únicamente a los usuarios que tienen derechos de acceso al objeto de la actualización.</p> <p>Si el usuario que envía la actualización dirigida es miembro del equipo que se incluye, el usuario que envía la actualización no recibe una notificación por correo electrónico.</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentario del elemento de trabajo</p> </td> 
   <td> <p>Participantes del hilo</p> </td> 
   <td> <p>Alguien agrega un comentario a un hilo en el que participo.</p> <p>Los participantes en el hilo y los usuarios incluidos en un mensaje directo reciben una notificación por correo electrónico cuando un usuario hace un comentario en el hilo.</p> <p>Los usuarios deben tener acceso de visualización para recibir una notificación.</p> <p>Los siguientes usuarios no reciben una notificación:</p> 
    <ul> 
     <li> <p>Equipos incluidos en un mensaje directo</p> </li> 
     <li> <p>El propietario de la nota</p> </li> 
     <li> <p>El contacto principal</p> </li> 
    </ul> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Comentario del elemento de trabajo</p> </td> 
   <td> <p>Usuario asignado de elemento de trabajo</p> </td> 
   <td> <p>Alguien agrega comentarios a uno de mis elementos de trabajo.</p> <p>El usuario asignado del elemento de trabajo recibe una notificación por correo electrónico cada vez que un usuario agrega una actualización a un elemento de trabajo, a menos que el usuario que agrega la actualización también sea el usuario asignado.</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Respuesta de solicitud de trabajo</p> </td> 
   <td> <p> Solicitante de trabajo</p> </td> 
   <td> <p>Alguien responde a mi solicitud.</p> <p>Una vez que un usuario envía una solicitud y otro usuario responde a ella, el usuario que la envió recibe una notificación por correo electrónico.</p> <p>No se envía una notificación por correo electrónico si:</p> 
    <ul> 
     <li> <p>El usuario que responde es el mismo usuario que realizó la solicitud</p> </li> 
     <li> <p>El usuario no tiene acceso para ver la nota</p> </li> 
    </ul> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Información de aprobación

Ver también [Notificaciones: Información de aprobación](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Delegación de aprobación</p> </td> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Se me ha delegado como aprobador.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de estado de aprobación delegada de problema</p> </td> 
   <td> <p>Usuario que delegó la aprobación</p> </td> 
   <td> <p>Se completó una solicitud de aprobación delegada de problema. </p> <p>Cuando delega la aprobación de un problema a otra persona, recibe una notificación por correo electrónico cuando finaliza esa aprobación (independientemente de si aprueba o rechaza la aprobación del problema). </p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio de estado de aprobación delegada de proyecto</p> </td> 
   <td> <p>Usuario que delegó la aprobación</p> </td> 
   <td> <p>Se completó una solicitud de aprobación delegada de proyecto.</p> <p>Cuando delega una aprobación de proyecto a otra persona, recibe una notificación por correo electrónico cuando finaliza esa aprobación (tanto si la aprueba como si rechaza).</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de estado de aprobación delegada de tarea</p> </td> 
   <td> <p>Usuario que delegó la aprobación</p> </td> 
   <td> <p>Se completó un estado de aprobación delegada de tarea.</p> <p>Cuando delega una aprobación de tarea a otra persona, recibe una notificación por correo electrónico cuando finaliza esa aprobación (independientemente de si aprueba o rechaza la aprobación de la tarea).</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aprobación de documento cancelada para aprobador</p> </td> 
   <td> <p>Usuario que delegó la aprobación</p> </td> 
   <td> <p>Se canceló una solicitud de aprobación de documento.</p> <p>El aprobador del documento recibe una notificación por correo electrónico cuando se cancela la solicitud de aprobación del documento.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hoja de horas</p> </td> 
   <td> <p>Aprobación de hoja de horas</p> </td> 
   <td> <p>Usuario al que pertenece la plantilla de horas</p> </td> 
   <td> <p>Se aprueba mi hoja de horas.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información sobre el trabajo asignado a mí

Ver también [Notificaciones: información sobre el trabajo asignado a mí](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tarea</td> 
   <td>Finalización de todas las tareas predecesoras</td> 
   <td>Miembros del equipo asignados a tareas dependientes</td> 
   <td> <p>Se completan todas las tareas predecesoras del equipo.</p> <p>Los usuarios asignados a la tarea (todos los miembros del equipo) reciben una notificación por correo electrónico.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td>Inactivo</td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de todas las tareas predecesoras</p> </td> 
   <td> <p>Usuario asignado a tareas dependientes</p> </td> 
   <td> <p>Se han finalizado todas las tareas predecesoras de mis tareas.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisión de aprobación</p> </td> 
   <td> <p>Usuario al que se ha asignado el problema</p> </td> 
   <td> <p>Se aprueba o rechaza un problema que resuelvo.</p> <p>El usuario asignado de un problema recibe una notificación por correo electrónico cuando se toma una decisión de aprobación (aprobada o rechazada).</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Decisión de aprobación</p> </td> 
   <td> <p>Usuario al que está asignada la tarea</p> </td> 
   <td> <p>Se aprueba o rechaza una tarea que finalizo.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se aprueba o rechaza la tarea.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema</p> </td> 
   <td> <p>Usuario al que se ha asignado el problema</p> </td> 
   <td> <p>Se resuelve un problema al que estoy asignado.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambió la fecha planificada de finalización de problema</p> </td> 
   <td> <p>Usuario al que se ha asignado el problema</p> </td> 
   <td> <p>Cambia la fecha límite de un problema al que estoy asignado.</p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando cambia la fecha planificada de finalización, a menos que el usuario que cambió la fecha planificada de finalización también sea el asignado.</p> <p>Solo se envía una notificación si el estado del proyecto es distinto de Planificación.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de estado de problema</p> </td> 
   <td> <p>Usuario al que se ha asignado el problema</p> </td> 
   <td> <p>El estado cambia en uno de mis elementos de trabajo.</p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando cambia el estado, a menos que el usuario que ha cambiado el estado también sea el asignado.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitar documento agregado</p> </td> 
   <td> <p>Usuario al que se ha asignado el problema</p> </td> 
   <td> <p>Los documentos se cargan o se cambian en las solicitudes a las que estoy asignado.</p> <p>El usuario asignado del problema recibe una notificación por correo electrónico cuando se cargan o modifican documentos sobre un problema que ha añadido.</p> <p>No se envía una notificación por correo electrónico si el usuario que ha introducido el problema es el usuario asignado del problema.</p> <p>Se envía una notificación únicamente si el estado del proyecto es Actual y si el proyecto tiene la "Publish como Cola de solicitudes de ayuda" habilitada en la ficha Configuración de cola.</p> </td> 
   <td> <p>Activo (solo diario)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea</p> </td> 
   <td> <p>Usuario al que está asignada la tarea</p> </td> 
   <td> <p>Se finaliza una tarea a la que estoy asignado.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa la tarea. Las notificaciones no se envían cuando se completa una tarea personal.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia básica, de colaborador, de revisor o de solicitante no reciben ninguna notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea</p> </td> 
   <td> <p>Usuario asignado a tarea dependiente</p> </td> 
   <td> <p>Se ha completado una tarea predecesora de una de mis tareas.</p> <p>El usuario asignado de la tarea recibe una notificación por correo electrónico cuando se completa una de las tareas predecesoras de la tarea.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambió la fecha planificada de finalización de tarea</p> </td> 
   <td> <p>Usuario al que está asignada la tarea</p> </td> 
   <td> <p>Cambia la fecha límite de una tarea a la que estoy asignado.</p> <p>El usuario asignado a la tarea recibe una notificación por correo electrónico cuando cambia la fecha planificada de finalización de la tarea, a menos que el usuario que cambió la fecha planificada de finalización también sea el usuario asignado a la tarea.</p> <p>Solo se envía una notificación si el estado del proyecto es distinto de Planificación.</p> <p>No se envía ninguna notificación con respecto a las tareas personales.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de estado de Tarea</p> </td> 
   <td> <p>Usuario al que está asignada la tarea</p> </td> 
   <td> <p>El estado cambia en una tarea a la que estoy asignado.</p> <p>El Usuario asignado a la tarea recibe una notificación por correo electrónico cuando cambia el estado de la tarea, a menos que el usuario que ha cambiado el estado también sea el asignado.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Información sobre proyectos en los que participo

Ver también [Notificaciones: información sobre proyectos en los que estoy](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Estado actual del proyecto</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se activa un proyecto en el que participo.</p> <p>Los usuarios del proyecto reciben una notificación por correo electrónico cuando el proyecto se activa.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento agregado</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se agrega un documento a un proyecto en el que participo.</p> <p>Los usuarios del equipo del proyecto reciben una notificación por correo electrónico cuando se agrega un documento al proyecto, excepto por el usuario que agregó el documento.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y el documento no es Privado. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se agrega un problema a un proyecto en el que participo.</p> <p>Los usuarios de un proyecto reciben una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se resuelve un problema en un proyecto en el que trabajo.</p> <p>Cualquier usuario del proyecto recibe una notificación.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea de hito</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se completa una tarea de hito en un proyecto en el que participo.</p> <p>Todos los usuarios del equipo del proyecto reciben una notificación cuando se completa una tarea de hito. </p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Finalización del proyecto</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se completa un proyecto en el que participo.</p> <p>Los usuarios de un equipo del proyecto reciben una notificación por correo electrónico cuando se completa el estado del proyecto.</p> <p>Sugerencia: si los proyectos se finalizan con regularidad, activar esta opción puede crear mucho correo electrónico para los usuarios que tienen un número limitado de tareas en muchos proyectos. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio de estado del proyecto</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>El estado cambia en un proyecto en el que participo.</p> <p>Los usuarios del equipo del proyecto reciben una notificación por correo electrónico cuando cambia el estado del proyecto. </p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario de proyecto</p> </td> 
   <td> <p>Adición de usuario de proyecto</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se me agrega a un proyecto.</p> <p>El usuario que se añadió al proyecto recibe una notificación por correo electrónico cuando se agregan, a menos que el usuario se haya agregado automáticamente al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se finaliza una tarea en un proyecto en el que participo.</p> <p>Los miembros del equipo del proyecto reciben una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Se agregó problema sin asignar</p> </td> 
   <td> <p>Miembros del equipo del proyecto</p> </td> 
   <td> <p>Se agrega un problema no asignado a un proyecto en el que participo.</p> <p>Los usuarios de un proyecto reciben una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información sobre proyectos de mi propiedad

Ver también [Notificaciones: información sobre proyectos de mi propiedad](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento agregado</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se agrega un documento a mi proyecto.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el usuario que agregó el documento también sea el propietario del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y el documento no es Privado.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se agrega un problema a un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Cambio de fecha de confirmación de problema</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Cambia la fecha de confirmación de un problema en uno de mis proyectos.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de un problema del proyecto, a menos que el usuario que cambia la fecha de confirmación sea el mismo usuario que el propietario del proyecto.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se resuelve un problema en un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea de hito</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se completa una tarea de hito en un proyecto de mi propiedad.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Asignación de propietario del proyecto</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se me asigna como propietario de un nuevo proyecto.</p> <p>Cuando se asigna a un usuario como propietario de un proyecto, ese usuario recibe una notificación por correo electrónico.</p> <p>Si el propietario del proyecto es el mismo usuario que realizó la asignación, no se envía una notificación por correo electrónico</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio del avance del proyecto</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se retrasa un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando el proyecto está retrasado.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio de fecha de confirmación de tarea</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Cambia la fecha de confirmación de una tarea en uno de mis proyectos.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de una tarea del proyecto, a menos que el usuario que ha cambiado la fecha de confirmación también sea el propietario del proyecto.</p> </td> 
   <td> <p>Activo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se finaliza una tarea en un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación. </p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio del avance de la tarea</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se retrasa una tarea en un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema no asignado</p> </td> 
   <td> <p>Propietario del proyecto</p> </td> 
   <td> <p>Se agrega un problema no asignado a un proyecto de mi propiedad.</p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información sobre proyectos que patrocino

Ver también [Notificaciones: información sobre proyectos que patrocino](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento agregado</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se agrega un documento a un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el patrocinador del proyecto agregue el documento.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual y si el documento no es Privado.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se agrega un problema a un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Resolución del problema</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Enviar mensaje de correo electrónico al patrocinador del proyecto al resolver un problema.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea de hito</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se finaliza una tarea de hito en un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se completa una tarea de hito en un proyecto que patrocina.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Cambio del avance del proyecto</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se retrasa un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa con respecto a la programación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Asignación de patrocinador del proyecto</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se me asigna como patrocinador de un proyecto.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se le establece como patrocinador de un proyecto.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Finalización de tarea</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se finaliza una tarea en un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Cambio del avance de la tarea</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se retrasa una tarea en un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agregar problema no asignado</p> </td> 
   <td> <p>Patrocinador de proyecto</p> </td> 
   <td> <p>Se agrega un problema no asignado a un proyecto que patrocino.</p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información variada

Ver también [Notificaciones: información diversa](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descripción</th> 
   <th> Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Anuncio</td> 
   <td> <p>Se agregó el anuncio</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Se envía un mensaje al Centro de anuncios.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Solicitud de documento cancelada</p> </td> 
   <td> <p>Usuario al que se solicita ese documento</p> </td> 
   <td> <p>Cancelar una solicitud de carga de documento mía.</p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se cancela una solicitud de documento.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notificación de error</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Se ha encontrado un error que precisa su atención.</p> <p>Se genera una notificación por correo electrónico después de que Workfront intente conectarse a una cuenta POP y no pueda hacerlo. Después de 25 intentos, Workfront deshabilita la conexión a la cuenta POP para conservar los recursos y envía una notificación. </p> <p>La notificación por correo electrónico se envía al propietario del proyecto, si el correo electrónico POP está asociado a una cola de solicitudes, o a los administradores de Workfront, si la cuenta POP está asociada a la función "Correo entrante" en la configuración de correo electrónico.
   </p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Asignación de problema</p> </td> 
   <td> <p>Propietario del recurso</p> </td> 
   <td> <p>Un cambio de asignación de problema afecta a alguien de mi grupo.</p> <p>El administrador de usuarios asignados del problema recibe una notificación por correo electrónico cuando un cambio afecta a un usuario que administra.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Nuevo usuario</p> </td> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Cuando se crea un nuevo usuario en Workfront, enviar un correo electrónico al usuario.</p> <p>Una vez creado el nuevo usuario, este recibe una invitación por correo electrónico en la que se le notifica que se ha creado una cuenta de Workfront y se le solicita que defina su contraseña.</p> <p>Al crear un usuario nuevo, los usuarios pueden seleccionar la opción "Enviar un correo electrónico de invitación a esta persona" (como se describe en <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Agregar usuarios</a><span style="font-weight: 400;">). Sin embargo, cuando la opción "Nuevo usuario a usuario" está habilitada globalmente, todos los usuarios nuevos reciben la invitación por correo electrónico independientemente de si la opción "Enviar un correo electrónico de invitación a esta persona" está seleccionada.</span></p> </td> 
   <td> Inactivo </td> 
  </tr> 
  <tr> 
   <td> <p>Equipo</p> </td> 
   <td> <p>Objeto compartido</p> </td> 
   <td> <p>Miembros del equipo con los que se compartió el objeto</p> </td> 
   <td> <p>Alguien comparte un objeto con mi equipo.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario</p> </td> 
   <td> <p>Objeto compartido</p> </td> 
   <td> <p>Usuario con el que se compartió el objeto</p> </td> 
   <td> <p>Alguien comparte un objeto conmigo.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario de proyecto</p> </td> 
   <td> <p>Adición de usuario de proyecto</p> </td> 
   <td> <p>Propietario del recurso</p> </td> 
   <td> <p>Se agrega a una persona de mi equipo a un proyecto.</p> <p>Un administrador recibe una notificación por correo electrónico cuando se agrega uno de sus informes directos a un proyecto.</p> <p>Los usuarios con una licencia Ligera o Revisar no reciben una notificación.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>Se agrega un proyecto a un portafolio o programa</p> </td> 
   <td> <p>Portfolio o propietario del programa</p> </td> 
   <td> <p>Alguien agrega un proyecto a un portafolio o programa de mi propiedad.</p> </td> 
   <td> <p>Activo (solo instantáneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea</p> </td> 
   <td> <p>Asignación de tareas</p> </td> 
   <td> <p>Propietario del recurso</p> </td> 
   <td> <p>Un cambio de asignación de tarea afecta a alguien de mi grupo.</p> <p>El administrador de la persona asignada a la tarea recibe una notificación por correo electrónico.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> </td> 
   <td> <p>Inactivo</p> </td> 
  </tr> 
  <tr> 
   <td> Problema <br>de tarea <br> del proyecto</td> 
   <td>Nueva actualización</td> 
   <td>Suscriptor </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Se envía un mensaje de correo electrónico cuando se actualiza una tarea, un problema o un proyecto al que estoy suscrito.</span> </p> </td> 
   <td>Activo (solo instantáneo)</td> 
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

Vea también [Notificaciones: Delegación](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Tipo de objeto | Evento | Destinatario | Descripción | Estado predeterminado |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Tareas y problemas | Delegación de tarea y problema | Asignado | Yo delego mis tareas y problemas (confirmación) | Activo (solo instantáneo) |
| Tareas y problemas | Detener la delegación de tareas y problemas | Asignado | Yo detengo la delegación de mis tareas y problemas (confirmación) | Activo (solo instantáneo) |
| Tareas y problemas | Delegación de tarea y problema | Delegar | Alguien me delega sus tareas y problemas | Activo (solo instantáneo) |
| Tareas y problemas | Detener tareas y delegación de problemas | Delegar | Alguien detiene la delegación de sus tareas y problemas en mí | Activo (solo instantáneo) |
