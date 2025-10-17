---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Información diversa'
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.
author: Courtney
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 100%

---

# Notificaciones: Información diversa

Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.

Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>No puede habilitar o deshabilitar las notificaciones diarias y no recibe correos electrónicos de resumen diario para los eventos de esta categoría. Puede habilitar o deshabilitar notificaciones instantáneas individuales para la categoría [!UICONTROL Varios].

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
   <td> <p><strong>Se envía un mensaje al [!UICONTROL Announcement Center]</strong> </p> <p>Recibirá una notificación por correo electrónico cuando se envíe un nuevo mensaje al [!UICONTROL Announcement Center]. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL [!DNL Adobe Workfront] Announcement]: &lt;Asunto del anuncio&gt;</em></p> </td> 
   <td> Asunto del anuncio<br>Texto del mensaje incluido en el anuncio<br>Documento(s) adjunto(s)<br>Nombre del usuario que envió el anuncio<br>Fecha y hora en que se envió el anuncio </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando un cambio de asignación de tarea afecte a alguien de mi grupo</strong> </p> <p>Cuando se asigna a una nueva tarea uno de los informes directos de un usuario designado como administrador, el administrador recibe un correo electrónico sobre la asignación. </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Task Resource Assignment]: &lt;Nombre de la tarea&gt;</em></p> </td> 
   <td>Nombre de proyecto<br>Nombre de tarea<br>Fecha y hora en que se creó la tarea<br>Nombre del usuario que creó la tarea<br>Nombres de asignación<br>Fecha de vencimiento (fecha planificada de finalización)<br>Estado de la tarea<br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Después de recibir una solicitud de carga de documento, se cancela la solicitud</strong> </p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se cancela una solicitud de documento.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>&lt;Nombre del usuario que canceló la solicitud&gt; canceló la solicitud de documento. </em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hi] &lt;Su nombre&gt;, <br><br>&lt;Nombre del usuario que canceló la solicitud&gt;[!UICONTROL no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.]</em> </p> </td> 
   <td>Nombre del usuario que canceló la solicitud<br>El texto de la solicitud de carga del documento original<br>Un titular "[!UICONTROL CANCELED]" sobre la solicitud del documento original<br>Fecha y hora de la solicitud del documento original<br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se encuentra un error que precisa mi atención</strong> </p> <p>El usuario que responde a un comentario por correo electrónico recibe una notificación por correo electrónico cuando no se puede enviar la respuesta.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Failed to Process on] &lt;asunto del mensaje original&gt;</em></p> <p>Para obtener información sobre cómo usar el correo electrónico para responder a los comentarios, consulte <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Responder a las notificaciones por correo electrónico</a>.</p> </td>
   <td> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando un cambio de asignación de problema afecte a alguien de mi grupo</strong> </p> <p>El administrador de un usuario asignado a un problema recibe una notificación por correo electrónico cuando ese usuario se elimina de un problema o se asigna a un problema. </p> <p>Se envía una notificación solo si el estado del proyecto es Actual o en Planificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Asignación de problema: &lt;Nombre del problema&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que realizó la asignación<br>Tipo de problema<br>Nombre del usuario asignado al problema<br>Fecha del problema que se introdujo<br>Prioridad del problema<br>Contacto principal<br>[!UICONTROL Planned Completion Date] del problema<br>Estado del problema<br><strong>Botón [!UICONTROL See More Details]</strong></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se añade a una persona de mi equipo a un proyecto</strong> </p> <p>Un administrador recibe una notificación por correo electrónico cuando se añade uno de sus usuarios a un proyecto. Esta notificación se envía independientemente del estado del proyecto. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico es: <em>Asignación de proyecto: &lt;Nombre de usuario&gt;[&lt;Project GUID&gt;_ &lt;User GUID&gt;]</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Nombre del usuario que añadió a la persona al proyecto<br>Nombre del usuario que se añadió al proyecto<br>[!UICONTROL Planned Start Date] del proyecto<br>[!UICONTROL Planned Completion Date] del proyecto<br>Porcentaje completado del proyecto<br>Nombres de otros en el proyecto<br>Estado del proyecto<br>Propietario del proyecto<br><strong>Botón [!UICONTROL See More Details]</strong><br><br><br></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien añade un proyecto a un portafolio o programa de mi propiedad</strong> </p> <p>El portafolio y/o el propietario del programa reciben una notificación cuando se añade un nuevo proyecto a un portafolio o programa.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Project added to] &lt;Portfolio Name&gt;[Project GUID]</em></p> </td> 
   <td> Nombre del portafolio<br>Número de referencia del proyecto<br>Nombre del usuario que ha añadido el proyecto al portafolio/ programa<br><br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien comparte un objeto conmigo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando alguien lo añada a la lista de permisos de [!UICONTROL Sharing] sobre un objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Access Granted]: &lt;Object Name&gt;</em></p> <p>Se envía una notificación solo si el proyecto se encuentra en estado [!UICONTROL Current].</p> </td> 
   <td> Nombre de objeto<br>Nombre de objeto principal<br>Número de referencia del objeto<br>Acceso original al objeto<br>Nuevo acceso concedido al objeto<br>Fecha y hora en que se concedió el acceso <br>Nombre del usuario que concedió el acceso </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien comparte un objeto con mi equipo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando alguien añada su equipo a la lista de permisos de uso compartido sobre un objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Access Granted]: &lt;Object Name&gt; [GUID de regla de acceso]</em></p> </td> 
   <td> Nombre de objeto<br>Nombre de objeto principal<br>Número de referencia del objeto<br>Acceso anterior<br>Nuevo acceso<br>Fecha y hora en que se concedió el acceso<br>Nombre del equipo<br>Nombre del usuario que concedió el acceso </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se actualiza una tarea, un problema o un proyecto al que me he suscrito</strong> </p> <p>Recibe una notificación por correo electrónico cuando alguien comenta un artículo al que está suscrito.</p> <p>El asunto del correo electrónico de suscripción es: <em>[!UICONTROL An update was made to the] &lt;Object Type&gt; al que está suscrito: &lt;Object Name&gt;</em></p> </td> 
   <td> Nombre de objeto<br> Número de referencia de objeto<br> Nombre del usuario que hizo un comentario en el elemento suscrito<br> Fecha en la que se hizo el comentario<br> Comentario añadido al elemento suscrito  </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
