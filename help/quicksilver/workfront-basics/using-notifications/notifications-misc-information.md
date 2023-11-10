---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información diversa"
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 8%

---

# Notificaciones: Información variada

Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.

Para obtener información sobre cómo configurar qué notificaciones recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>No puede habilitar ni deshabilitar las notificaciones diarias y no recibe correos electrónicos de resumen diario para los eventos de esta categoría. Puede habilitar o deshabilitar notificaciones instantáneas individuales para [!UICONTROL Varios] categoría.

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
   <td> <p><strong>Se envía un mensaje al Centro de anuncios de [!UICONTROL]</strong> </p> <p>Recibirá una notificación por correo electrónico cuando se envíe un nuevo mensaje al Centro de anuncios de [!UICONTROL]. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL [!DNL Adobe Workfront] Anuncio]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Asunto del anuncio<br>Texto del mensaje incluido en el anuncio<br>Documento(s) adjunto(s)<br>Nombre del usuario que envió el anuncio<br>Fecha y hora en que se envió el anuncio </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando un cambio de asignación de tarea afecte a alguien de mi grupo</strong> </p> <p>Cuando se asigna a una nueva tarea uno de los informes directos de un usuario designado como administrador, el administrador recibe un correo electrónico sobre la asignación. </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Asignación de recursos de tareas]: &lt;task name=""&gt;</em></p> </td> 
   <td>Nombre de proyecto<br>Nombre de tarea<br>Fecha y hora en que se creó la tarea<br>Nombre del usuario que creó la tarea<br>Nombres de asignación<br>Fecha de vencimiento (fecha planificada de finalización)<br>Estado de tarea<br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Después de recibir una solicitud de carga de documento, se cancela la solicitud</strong> </p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se cancela una solicitud de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; canceló la solicitud de documento. </em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL ya no necesita que suba nada con respecto a la solicitud que recibió anteriormente. Solo queríamos hacértelo saber.]</em> </p> </td> 
   <td>Nombre del usuario que canceló la solicitud<br>Texto de la solicitud original de carga de documento<br>Un titular "[!UICONTROL CANCELADO]" sobre la solicitud de documento original<br>Fecha y hora de la solicitud de documento original<br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha encontrado un error que precisa mi atención</strong> </p> <p>El usuario que responde a un comentario por correo electrónico recibe una notificación por correo electrónico cuando no se puede enviar la respuesta.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL No se pudo procesar en] &lt;subject of="" original="" message=""&gt;</em></p> <p>Para obtener información sobre cómo utilizar el correo electrónico para responder a los comentarios, consulte <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Responder a notificaciones por correo electrónico</a>.</p> </td>
   <td> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando un cambio de asignación de problema afecte a alguien de mi grupo</strong> </p> <p>El administrador de un usuario asignado a un problema recibe una notificación por correo electrónico cuando ese usuario se elimina de un problema o se asigna a un problema. </p> <p>Se envía una notificación solo si el estado del proyecto es Actual o Planificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Asignación de problema: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que realizó la asignación<br>Tipo de problema<br>Nombre del usuario asignado al problema<br>Fecha de emisión ingresada<br>Prioridad de problema<br>Contacto principal<br>Problema [!UICONTROL Fecha planificada de finalización]<br>Estado del problema<br><strong>[!UICONTROL Ver más detalles]</strong> botón</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega a una persona de mi equipo a un proyecto</strong> </p> <p>Un administrador recibe una notificación por correo electrónico cuando se agrega uno de sus usuarios a un proyecto. Esta notificación se envía independientemente del estado del proyecto. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico es: <em>Asignación de proyecto: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó a la persona al proyecto<br>Nombre del usuario que se añadió al proyecto<br>Proyecto [!UICONTROL Fecha planificada de inicio]<br>Proyecto [!UICONTROL Fecha planificada de finalización]<br>Porcentaje completado del proyecto<br>Nombres de otras personas en el proyecto<br>Estado del proyecto<br>Propietario de proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br><br><br></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien agrega un proyecto a un portafolio o programa de mi propiedad</strong> </p> <p>El portafolio y/o el propietario del programa reciben una notificación cuando se agrega un nuevo proyecto a un portafolio o programa.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se ha agregado un proyecto [!UICONTROL a] &lt;portfolio name=""&gt;[GUID de proyecto]</em></p> </td> 
   <td> Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó el proyecto al portafolio/programa<br><br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien comparte un objeto conmigo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando alguien lo agregue a la lista de permisos de [!UICONTROL Sharing] sobre un objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Acceso concedido]: &lt;object name=""&gt;</em></p> <p>Se envía una notificación sólo si el proyecto se encuentra en estado [!UICONTROL Actual].</p> </td> 
   <td> Nombre de objeto<br>Nombre del objeto principal<br>Número de referencia de objeto<br>Acceso original al objeto<br>Nuevo acceso concedido al objeto<br>Fecha y hora en que se concedió el acceso <br>Nombre del usuario que concedió el acceso </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien comparte un objeto con mi equipo</strong> </p> <p>Recibirá una notificación por correo electrónico cuando alguien agregue su equipo a la lista de permisos de uso compartido de un objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Acceso concedido]: &lt;object name=""&gt; [GUID de regla de acceso]</em></p> </td> 
   <td> Nombre de objeto<br>Nombre del objeto principal<br>Número de referencia de objeto<br>Acceso antiguo<br>Nuevo acceso<br>Fecha y hora en que se concedió el acceso<br>Nombre de su equipo<br>Nombre del usuario que concedió el acceso </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se hace una actualización a una tarea, un problema o un proyecto al cual me he suscrito</strong> </p> <p>Recibes una notificación por correo electrónico cuando alguien comenta un artículo al que estás suscrito.</p> <p>El asunto del correo electrónico de suscripción es: <em>[!UICONTROL Se ha realizado una actualización en] &lt;object type=""&gt; se ha suscrito a: &lt;object name=""&gt;</em></p> </td> 
   <td> Nombre de objeto<br> Número de referencia de objeto<br> Nombre del usuario que hizo un comentario sobre el elemento suscrito<br> Fecha en la que se realizó el comentario<br> Comentario añadido al elemento suscrito  </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
