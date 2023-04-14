---
content-type: reference
navigation-topic: notifications
title: '''Notificaciones: Comunicación"'
description: Las siguientes notificaciones le avisan sobre la comunicación, como un comentario de actualización, que se produce en un elemento de trabajo con el que esté involucrado. Para obtener información sobre la configuración de las notificaciones que recibe, consulte Activación o desactivación de sus propias notificaciones de evento.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 2af2a1f7d1a4d0b06cf4e7bfd2b9997ff8b9a6bf
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 4%

---

# Notificaciones: Comunicación

Las siguientes notificaciones le avisan sobre la comunicación, como un comentario de actualización, que se produce en un elemento de trabajo con el que esté involucrado. Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Estas notificaciones le avisan de todos los comentarios que se han publicado en un elemento específico. Por este motivo, debe seleccionar o anular la selección de todas las notificaciones al mismo tiempo para enviarlas en un correo electrónico de resumen diario. Si desea que se le notifique sobre ciertos comentarios solo a medida que ocurran, puede especificar que las notificaciones individuales sean para envío instantáneo.

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
   <td> <p><strong>Alguien me incluye en una actualización dirigida</strong> </p> <p>Una actualización dirigida se produce cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Actualizaciones de [!UICONTROL Etiquete otros en]</a>.</p> <p>En este caso, el usuario incluido en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico se envía únicamente si el usuario tiene derechos de acceso al objeto .</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL quería que lo supiera]</em></p> <p>El tema de la notificación diaria de compendio es: <em>[!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del objeto donde se realizó la actualización<br>Nombre del objeto principal<br>Número de referencia del objeto<br>Nombres de todos los usuarios y equipos incluidos en la actualización dirigida<br>Fecha y hora en que se realizó la actualización<br>Texto de la actualización dirigida<br><strong>[!UICONTROL Comentario]</strong> botón<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario<br></td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien responde a mi solicitud</strong> </p> <p>Después de que un usuario envía una solicitud de trabajo y otro usuario responde a esa solicitud de trabajo, el usuario que la envió recibe una notificación por correo electrónico.</p> <p>No se envía una notificación por correo electrónico si:</p> 
    <ul> 
     <li> <p>El usuario que responde es el mismo usuario que realizó la solicitud</p> </li> 
     <li> <p>El usuario no tiene acceso para ver la nota</p> </li> 
    </ul><strong>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comentario en] &lt;request name=""&gt; en &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></strong> El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> Nombre de la solicitud<br>Nombre del proyecto<br>Número de referencia<br>Nombre del usuario que respondió a su solicitud<br>Fecha y hora en que se realizó el comentario<br>Texto del comentario realizado sobre la solicitud<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada solicitud<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se publica un comentario que he solicitado</strong> </p> <p>El contacto principal de un problema recibe una notificación por correo electrónico cuando se publica un comentario en una solicitud del [!UICONTROL Help Desk], a menos que el usuario que publicó el comentario también sea el contacto principal del problema.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comentario en] &lt;request name=""&gt; en &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la solicitud<br>Nombre del proyecto<br>Número de referencia<br>Nombre del usuario que respondió a su solicitud<br>Fecha y hora en que se realizó el comentario<br>Texto del comentario realizado sobre la solicitud<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada solicitud<br>*Nombre del proyecto<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario<br></td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un comentario en mi documento</strong> </p> <p>El propietario de un documento de [!DNL Adobe Workfront] recibe una notificación por correo electrónico cuando se publica un comentario en el documento, a menos que el usuario que publicó el comentario también sea el propietario del documento.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current]. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comentario en] &lt;request name=""&gt; en &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>Nombre del documento<br>Proyecto, tarea o nombre del problema<br>Número de referencia<br>Nombre del usuario que respondió a su solicitud<br>Fecha y hora en que se realizó el comentario<br>Texto de las observaciones formuladas en el documento</td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien agrega un comentario a un hilo en el cual participo</strong> </p> <p>Los participantes en el subproceso y los usuarios incluidos en un mensaje directo reciben una notificación por correo electrónico cuando un usuario hace un comentario en el subproceso.</p> <p>Los usuarios deben tener acceso a [!UICONTROL View] para recibir una notificación.</p> <p>Los siguientes usuarios no reciben una notificación:</p> 
    <ul> 
     <li>Equipos que se incluyen en un mensaje directo</li> 
     <li>El propietario de la Nota</li> 
     <li>El contacto principal</li> 
    </ul> <p><strong>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL RE: Comentar en] &lt;object name=""&gt;&lt;object type=""&gt; en &lt;project name=""&gt;(ref# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> Nombre del objeto<br>Nombre del objeto principal<br>Nombre del usuario que comentó el subproceso<br>Texto del comentario realizado en el hilo<br>Fecha y hora en que se realizó el comentario<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Nombre del proyecto<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien agrega comentarios a uno de mis elementos de trabajo</strong> </p> <p>El usuario asignado del elemento de trabajo recibe una notificación por correo electrónico cada vez que un usuario agrega una actualización a un elemento de trabajo, a menos que el usuario que agrega la actualización también sea el usuario asignado. </p> <p>Cuando se publique un comentario en una solicitud, envíe un correo electrónico al contacto principal del problema.</p> <p>El contacto principal de un problema recibe una notificación por correo electrónico cuando se publica un comentario en una solicitud, a menos que el usuario que publicó el comentario también sea el contacto principal del problema.</p> <p>Los usuarios que estén directamente incluidos en el comentario también recibirán una notificación por correo electrónico.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Comentario en] &lt;work item="" name=""&gt; en &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del elemento de trabajo<br>Nombre del proyecto<br>Número de referencia del elemento de trabajo<br>Nombre del usuario que comentó el elemento de trabajo<br>Texto del comentario sobre el elemento de trabajo<br>Fecha y hora en que se realizó el comentario<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Nombre del proyecto<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien incluye a mi equipo en una actualización dirigida</strong> </p> <p>Una actualización dirigida se produce cuando un usuario incluye específicamente a otro usuario en una actualización, tal como se describe en <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar otros en actualizaciones</a>.</p> <p>En este caso, cualquier miembro del equipo incluido en la actualización dirigida recibe una notificación por correo electrónico sobre la actualización.</p> <p>La notificación por correo electrónico solo se envía a los usuarios que tienen derechos de acceso al objeto.</p> <p>Si el usuario que envía la actualización dirigida es miembro del equipo que se incluye, el usuario que envía la actualización no recibe una notificación por correo electrónico.</p> <p>El asunto del correo electrónico de notificación instantánea es: [!UICONTROL Comentario en] &lt;object name=""&gt; en &lt;parent object="" name=""&gt; (ref# &lt;object reference="" number=""&gt;)</p> <p> El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del objeto<br>Nombre del objeto principal<br>Número de referencia del objeto<br>Nombre del usuario que realizó la actualización dirigida<br>Nombre de todos los equipos y usuarios incluidos en la actualización dirigida<br>Fecha y hora en que se realizó la actualización dirigida<br>Texto de la actualización dirigida<br><strong>[!UICONTROL Comentario]</strong> botón<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*Nombre del proyecto<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario </p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuando se agregue un comentario al usuario</strong> </p> <p>Puede realizar un comentario sobre un usuario en la ficha [!UICONTROL Actualizaciones] del objeto de usuario. También puede hacer un comentario sobre un usuario cuando esté editando la configuración del usuario. El usuario contra el que se realiza el comentario recibe un correo electrónico para notificarles este comentario. </p> <p>Debe tener permisos de al menos [!UICONTROL View] al usuario para introducir una actualización en la pestaña [!UICONTROL Updates] del usuario. Debe tener permisos de [!UICONTROL Edit] en el usuario para poder editar la configuración del usuario. </p> <p>Para obtener más información sobre cómo realizar comentarios en los usuarios de la ficha Actualizaciones , consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a>.</p> <p>Para obtener más información sobre cómo introducir un comentario en un usuario al editar la configuración del usuario, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis ajustes</a>.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;user name=""&gt; [!UICONTROL quería que lo supiera]</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de comunicación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Su nombre de usuario<br>Nombre del usuario que agregó el comentario<br>Texto del comentario<br>Fecha y hora en que se realizó el comentario<br>*Número total de comentarios recibidos<br>*Número de comentarios recibidos para cada objeto<br>*<strong>[!UICONTROL Ver todas las notificaciones]</strong> botón<br>*Fecha del compendio diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
