---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Comunicación'
description: Las siguientes notificaciones le avisan sobre la comunicación, como un comentario de actualización, que se produce en un elemento de trabajo con el que está involucrado. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte Modificación de sus propias notificaciones por correo electrónico.
author: Courtney
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 100%

---

# Notificaciones: Comunicación

Las siguientes notificaciones le avisan sobre la comunicación, como un comentario de actualización, que se produce en un elemento de trabajo con el que está involucrado. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Estas notificaciones le avisan sobre todos los comentarios que se han publicado sobre un elemento específico. Por este motivo, debe seleccionar o deseleccionar todas las notificaciones al mismo tiempo para que se envíen en un correo electrónico de resumen diario. Si desea que se le notifique sobre ciertos comentarios únicamente a medida que se producen, puede especificar las notificaciones individuales que se deben enviar instantáneamente.

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
   <td> <p><strong>Alguien me incluye en una actualización dirigida</strong> </p> <p>Una actualización dirigida es cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] actualizaciones</a>.</p> <p>En este caso, el usuario que se incluye en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico solo se envía si el usuario tiene derechos de acceso al objeto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;Nombre del usuario que le incluyó en la actualización&gt; [!UICONTROL wanted you to know]</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Digest of Communication] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del objeto donde se realizó la actualización<br>Nombre del objeto principal<br>Número de referencia del objeto<br>Nombres de todos los usuarios y equipos incluidos en la actualización dirigida<br>Fecha y hora en que se realizó la actualización<br>Texto de la actualización dirigida<br><strong>[!UICONTROL Comment]</strong> botón<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*<strong>[!UICONTROL See All Notifications]</strong> botón<br>*Fecha del resumen diario<br></td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien responde a mi solicitud</strong> </p> <p>Una vez que un usuario envía una solicitud de trabajo y otro usuario responde a esa solicitud de trabajo, el usuario que la envió recibe una notificación por correo electrónico.</p> <p>No se envía una notificación por correo electrónico si:</p> 
    <ul> 
     <li> <p>El usuario que responde es el mismo usuario que realizó la solicitud</p> </li> 
     <li> <p>El usuario no tiene acceso para ver la nota</p> </li> 
    </ul><strong>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comment on] &lt;Nombre de solicitud&gt; el &lt;Nombre de proyecto&gt; (ref# &lt;Número de referencia de solicitud&gt;)</em></strong> El asunto de la notificación de resumen diaria es:<em> [!UICONTROL Digest of Communication] &lt;Fecha del resumen diario&gt;</em></td> 
   <td> Nombre de solicitud<br>Nombre del proyecto<br>Número de referencia<br>Nombre del usuario que respondió a su solicitud<br>Fecha y hora en que se hizo el comentario<br>Texto del comentario hecho en su solicitud<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada solicitud<br>*<strong>[!UICONTROL See All Notifications]</strong> botón<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se publica un comentario en mi solicitud</strong> </p> <p>El contacto principal de un problema recibe una notificación por correo electrónico cuando se publica un comentario en una solicitud de [!UICONTROL Help Desk], a menos que el usuario que publicó el comentario también sea el contacto principal del problema.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comment on] &lt;Nombre de solicitud&gt; en &lt;Nombre de proyecto&gt; (ref# &lt;Número de referencia de solicitud&gt;)</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Digest of Communication] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de solicitud<br>Nombre del proyecto<br>Número de referencia<br>Nombre del usuario que respondió a su solicitud<br>Fecha y hora en que se hizo el comentario<br>Texto del comentario realizado en su solicitud<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada solicitud<br>*Nombre del proyecto<br>*<strong>[!UICONTROL See All Notifications]</strong> botón<br>*Fecha del resumen diario<br></td> 
   <td> <p><strong>Instante</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se añadió un comentario en mi documento</strong> </p> <p>El propietario de un documento de [!DNL Adobe Workfront] recibe una notificación por correo electrónico cuando se publica un comentario en el documento, a menos que el usuario que publicó el comentario también sea el propietario del documento.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current]. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comment on] &lt;Nombre de solicitud&gt; en &lt;Nombre de proyecto&gt; (ref# &lt;Número de referencia de solicitud&gt;)</em></p> <p> El asunto de la notificación de resumen diario es:<em> [!UICONTROL Digest of Communication] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td>Nombre de documento<br>Nombre de proyecto, tarea o problema<br>Número de referencia<br>Nombre del usuario que respondió a su solicitud<br>Fecha y hora en que se hizo el comentario<br>Texto del comentario hecho en el documento</td> 
   <td> <p><strong>Instante</strong> </p> <p><strong>y diarios</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien añade un comentario a un hilo en el cual participo</strong> </p> <p>Los participantes del hilo y los usuarios incluidos en un mensaje directo reciben una notificación por correo electrónico cuando un usuario hace un comentario en el hilo.</p> <p>Los usuarios deben tener acceso a [!UICONTROL View] para recibir una notificación.</p> <p>Los siguientes usuarios no reciben una notificación:</p> 
    <ul> 
     <li>Equipos incluidos en un mensaje directo</li> 
     <li>El propietario de la nota</li> 
     <li>El contacto principal</li> 
    </ul> <p><strong>El asunto del correo electrónico de la notificación instantánea es: <em>[!UICONTROL RE: Comment on] &lt;Object Name&gt;&lt;Object Type&gt; en &lt;Project Name&gt;(ref# &lt;Object Reference Number&gt;</em>)</strong> </p> <p><strong>El asunto de la notificación del resumen diario es:<em> [!UICONTROL Digest of Communication] &lt;Fecha del resumen diario&gt;</em></strong> </p> </td> 
   <td> Nombre de objeto<br>Nombre de objeto principal<br>Nombre del usuario que realizó comentarios en el hilo<br>Texto del comentario realizado en el hilo<br>Fecha y hora en que se realizó el comentario<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Nombre del proyecto<br>* Botón <strong>[!UICONTROL See All Notifications]</strong> <br>*Fecha del resumen diario </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien añade comentarios a uno de mis elementos de trabajo</strong> </p> <p>El usuario asignado del elemento de trabajo recibe una notificación por correo electrónico cada vez que un usuario añade una actualización a un elemento de trabajo, a menos que el usuario que añade la actualización también sea el asignado. </p> <p>Cuando se publica un comentario en una solicitud, es necesario enviarla por correo electrónico al autor del problema.</p> <p>El contacto principal de un problema recibe una notificación por correo electrónico cuando se publica un comentario en una solicitud, a menos que el usuario que publicó el comentario también sea el contacto principal del problema.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>El asunto del correo electrónico de la notificación instantánea es: <em>[!UICONTROL Comment on] &lt;Work Item Name&gt; en &lt;Project Name (ref# &lt;Work Item Reference Number&gt;)</em></p> <p> El asunto de la notificación del resumen diario es:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nombre del elemento de trabajo<br>Nombre del proyecto<br>Número de referencia del elemento de trabajo<br>Nombre del usuario que realizó comentarios sobre el elemento de trabajo<br>Texto del comentario realizado sobre el elemento de trabajo<br>Fecha y hora en que se realizó el comentario<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Nombre del proyecto<br>*<strong>[!UICONTROL See All Notifications]</strong><br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien incluye a mi equipo en una actualización dirigida</strong> </p> <p>Una actualización dirigida es cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a>.</p> <p>En este caso, cualquier miembro del equipo incluido en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico solo se envía a los usuarios que tienen derechos de acceso al objeto.</p> <p>Si el usuario que envía la actualización dirigida es miembro del equipo que se incluye, el usuario que envía la actualización no recibe una notificación por correo electrónico.</p> <p>El asunto del mensaje del correo electrónico de notificación instantánea es:[!UICONTROL Comment on] &lt;Object name&gt; en &lt;Parent Object Name&gt; (ref# &lt;Object Reference Number&gt;)</p> <p> El asunto de la notificación del resumen diario es:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>Nombre del objeto<br>Nombre del objeto principal<br>Número de referencia del objeto<br>Nombre del usuario que realizó la actualización dirigida<br>Nombre de todos los equipos y usuarios incluidos en la actualización dirigida<br>Fecha y hora en que se realizó la actualización dirigida<br>Texto de la actualización dirigida Botón <br><strong>[!UICONTROL Comment]</strong><br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Nombre de proyecto<br>*Botón <strong>[!UICONTROL See All Notifications]</strong><br>*Fecha de resumen diario </p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando se añade un comentario al usuario</strong> </p> <p>Puede realizar un comentario sobre un usuario en la pestaña [!UICONTROL Updates] del objeto de usuario. También puede realizar un comentario sobre un usuario cuando esté editando la configuración del usuario. El usuario sobre el que se realiza el comentario recibe un correo electrónico en el que se le notifica este comentario. </p> <p>Debe tener permisos para al menos [!UICONTROL View] el usuario e introducir una actualización en la pestaña [!UICONTROL Updates] de este. Debe tener permisos de [!UICONTROL Edit] en el usuario para poder editar la configuración de este. </p> <p>Para obtener más información acerca de cómo realizar comentarios sobre los usuarios en la pestaña Actualizaciones, vea <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a>.</p> <p>Para obtener más información sobre cómo escribir un comentario sobre un usuario al editar su configuración, vea <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis opciones</a>.</p> <p>El asunto del correo electrónico de la notificación instantánea es: <em>&lt;User Name&gt; [!UICONTROL wanted you to know]</em></p> <p>El asunto de la notificación del resumen diario es:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Su nombre de usuario<br>Nombre del usuario que añadió el comentario<br>Texto del comentario<br>Fecha y hora en que se hizo el comentario<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Botón <strong>[!UICONTROL See All Notifications]</strong><br>*Fecha del resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diario</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
