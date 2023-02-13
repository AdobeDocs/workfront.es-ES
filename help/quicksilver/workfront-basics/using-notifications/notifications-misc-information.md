---
content-type: reference
navigation-topic: notifications
title: '''Notificaciones: Información diversa"'
description: Las siguientes notificaciones le avisan de las actividades que se producen en un proyecto que patrocina.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# Notificaciones: Información diversa

Las siguientes notificaciones le avisan de las actividades que se producen en un proyecto que patrocina.

Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>No puede activar ni desactivar las notificaciones diarias y no recibe correos electrónicos resumidos diarios para los eventos de esta categoría. Puede activar o desactivar notificaciones instantáneas individuales para la variable [!UICONTROL Varios] categoría.

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
   <td> <p><strong>Se envía un mensaje al [!UICONTROL Centro de anuncios]</strong> </p> <p>Recibirá una notificación por correo electrónico cuando se haya enviado un nuevo mensaje al [!UICONTROL Centro de anuncios]. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL [!DNL Adobe Workfront] Anuncio]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Asunto del anuncio<br>Texto del mensaje incluido en el anuncio<br>Documentos adjuntos<br>Nombre del usuario que envió el anuncio<br>Fecha y hora de envío del anuncio </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando un cambio de asignación de tarea afecte a alguien de mi grupo</strong> </p> <p>Cuando se asigna a una nueva tarea uno de los informes directos de un usuario designado como administrador, el administrador recibe un correo electrónico sobre la asignación. </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Task Resource Assignment]: &lt;task name=""&gt;</em></p> </td> 
   <td>Nombre del proyecto<br>Nombre de la tarea<br>Fecha y hora en que se creó la tarea<br>Nombre del usuario que creó la tarea<br>Nombres de asignación<br>Fecha de Vencimiento (Fecha de Finalización Planificada)<br>Estado de la tarea<br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Después de recibir una solicitud de carga de documento, se cancela la solicitud</strong> </p> <p>La solicitud de documento recibe una notificación por correo electrónico cuando se cancela una solicitud de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; se ha cancelado la solicitud de documento. </em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL ya no necesita que cargue nada con respecto a la solicitud que obtuvo anteriormente. Solo queríamos que lo supieras.]</em> </p> </td> 
   <td>Nombre del usuario que ha cancelado la solicitud<br>Texto de la solicitud de carga del documento original<br>Un titular "[!UICONTROL CANCELADO]" sobre la solicitud de documento original<br>Fecha y hora de la solicitud original del documento<br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se encuentra un error que precisa mi atención</strong> </p> <p>El usuario que responda a un comentario por correo electrónico recibe una notificación por correo electrónico cuando no se puede enviar la respuesta.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL No se pudo procesar] &lt;subject of="" original="" message=""&gt;</em></p> <p>Para obtener información sobre el uso del correo electrónico para responder a los comentarios, consulte .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando un cambio de asignación de problema afecte a alguien de mi grupo</strong> </p> <p>El administrador de un usuario asignado a un problema recibe una notificación por correo electrónico cuando se elimina o se asigna al usuario a un problema. </p> <p>Solo se envía una notificación si el estado del proyecto es Current o Planning.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Asignación de problemas: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que realizó la asignación<br>Tipo de problema<br>Nombre del usuario asignado al problema<br>Fecha de emisión introducida<br>Prioridad del problema<br>Contacto principal<br>Problema [!UICONTROL Fecha de finalización planeada]<br>Estado del problema<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega a una persona de mi equipo a un proyecto</strong> </p> <p>Un administrador recibe una notificación por correo electrónico cuando uno de sus usuarios se agrega a un proyecto. Esta notificación se envía independientemente del estado del proyecto. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben una notificación.</p> <p>El asunto del correo electrónico es: <em>Asignación de proyectos: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó la persona al proyecto<br>Nombre del usuario que se agregó al proyecto<br>Proyecto [!UICONTROL Fecha de inicio planeada]<br>Proyecto [!UICONTROL Fecha de finalización planeada]<br>Porcentaje completado del proyecto<br>Nombres de otros en el proyecto<br>Estado del proyecto<br>Propietario del proyecto<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br><br><br></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien agrega un proyecto a un portafolio o programa de mi propiedad</strong> </p> <p>El portafolio o el propietario del programa reciben una notificación cuando se agrega un nuevo proyecto a un portafolio o a un programa.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Proyecto agregado a] &lt;portfolio name=""&gt;[GUID del proyecto]</em></p> </td> 
   <td> Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó el proyecto al portafolio o programa<br><br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien comparte un objeto conmigo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando alguien le añada a la lista de permisos de [!UICONTROL Sharing] en un objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Acceso concedido]: &lt;object name=""&gt;</em></p> <p>Solo se envía una notificación si el proyecto está en estado [!UICONTROL Actual].</p> </td> 
   <td> Nombre del objeto<br>Nombre del objeto principal<br>Número de referencia del objeto<br>Acceso original al objeto<br>Nuevo acceso concedido al objeto<br>Fecha y hora en que se concedió el acceso <br>Nombre del usuario que concedió el acceso </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien comparte un objeto con mi equipo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando alguien agregue su equipo a la lista de permisos de uso compartido de un objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Acceso concedido]: &lt;object name=""&gt; [GUID de regla de acceso]</em></p> </td> 
   <td> Nombre del objeto<br>Nombre del objeto principal<br>Número de referencia del objeto<br>Acceso antiguo<br>Nuevo acceso<br>Fecha y hora en que se concedió el acceso<br>Nombre de su equipo<br>Nombre del usuario que concedió el acceso </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se realiza una actualización de una tarea, un problema o un proyecto al que estoy suscrito</strong> </p> <p>Recibe una notificación por correo electrónico cuando alguien comenta sobre un artículo al que está suscrito.</p> <p>El asunto del correo electrónico de suscripción es: <em>[!UICONTROL Se ha realizado una actualización en el] &lt;object type=""&gt; está suscrito a: &lt;object name=""&gt;</em></p> </td> 
   <td> Nombre del objeto<br> Número de referencia del objeto<br> Nombre del usuario que ha hecho un comentario sobre el elemento suscrito<br> Fecha en que se hizo el comentario<br> Comentario añadido al elemento suscrito  </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
