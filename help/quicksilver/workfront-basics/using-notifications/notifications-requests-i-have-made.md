---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Solicitudes que he realizado"
description: Las siguientes notificaciones le permiten conocer las solicitudes que ha realizado en Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 7%

---

# Notificaciones: Solicitudes que he realizado

Las siguientes notificaciones le permiten conocer las solicitudes que ha realizado en [!DNL Adobe Workfront].

Para obtener información sobre cómo configurar qué notificaciones recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Solicitudes que he hecho</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación de documento</strong> </p> <p>El usuario que solicitó una aprobación de un documento recibe una notificación por correo electrónico cuando se completa la solicitud de aprobación del documento.</p> <p>El asunto del correo electrónico de notificación instantánea es:<em> &lt;approver name=""&gt; tiene &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; este documento.</em></p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </td> 
   <td> Nombre de documento<br>Nombre del aprobador </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha cambiado o subido un documento en un problema en el cual soy el autor</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se carga o cambia un documento en el problema, a menos que el usuario que cargó o cambió el documento también sea el contacto principal.</p> <p>Sólo se enviará una notificación si el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitudes]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Documento añadido a &lt;issue name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>Resumen de sus solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del objeto donde se cargó el documento<br>Nombre del objeto principal<br>Número de referencia del documento<br>Nombre del usuario que cargó el documento<br>Nombre de documento<br>Añadido el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de documentos cargados<br>*Nombre del documento<br>*Nombre del objeto principal<br>*Nombre del usuario que agregó el documento<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una solicitud de subir documento</strong> </p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se completa una solicitud de carga de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Su solicitud de documento de] &lt;user name=""&gt; se ha cumplido</em></p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </td> 
   <td> <p>Nombre del usuario que cargó el documento<br>Nombre del objeto donde se cargó el documento<br>Nombre de documento<br><br></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha completado una tarea personal que había asignado a otro usuario</strong> </p> <p>Se envía una notificación al usuario que asignó una tarea ad hoc a otra persona cuando se completa esa tarea. </p> <p>Para obtener más información sobre las tareas ad hoc, consulte <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Crear elementos de trabajo desde el área de [!UICONTROL Home]</a>.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Finalización de tarea: &lt;task name=""&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto predeterminado (proyecto personal del usuario que recibió la tarea personal)<br>Número de referencia de tarea<br>Nombre del propietario de tarea<br>Estado de nueva tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br><br><br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar correo electrónico al creador del problema cuando se resuelva el problema</strong> </p> <p>El contacto principal de un problema recibe una notificación cuando se resuelve el problema.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Resolución de problemas]: &lt;issue name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que ha completado el problema<br>Nuevo estado<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario que ha completado el problema<br>*Fecha del resumen diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Agrego un problema a un proyecto</strong> </p> <p>El contacto principal de un problema recibe una notificación cuando añade un problema en un proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema enviado]: &lt;issue name=""&gt; el &lt;project name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia de problema<br>Su nombre<br>Nombre de problema<br>Fecha de ingreso<br>Prioridad de problema<br>Estado del problema<br>Asignado a nombre<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas añadidos<br>*Nombre del problema<br>*Fecha del resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y a diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Yo envío una solicitud (confirmación)</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando envía un problema.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] y si el proyecto está configurado como una [!UICONTROL Cola de solicitudes de ayuda] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitudes]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Solicitud enviada]: &lt;request name=""&gt; el &lt;project request="" queue="" name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre de proyecto (nombre de cola de solicitudes)<br>Nombre del Portfolio<br>Número de referencia de problema<br>Nombre de problema<br>Fecha de ingreso<br>Prioridad de problema<br>Estado del problema<br>Asignado a nombre<br>Contacto principal<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>* Número total de solicitudes enviadas<br>*Nombre de la solicitud<br>*Solicitar prioridad<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y a diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mi solicitud se ha cerrado (confirmación)</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se cierra la solicitud.</p> <p>Sólo se enviará una notificación si el estado del proyecto es Actual y si el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Su solicitud se ha cerrado]:"&lt;request name=""&gt;"</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de solicitud<br>Nombre de proyecto<br>Número de referencia de solicitud<br>Nombre del usuario que cerró la solicitud<br>Estado del problema<br>Fecha y hora de cierre de la solicitud<br>Estado de solicitud anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>* Número total de solicitudes cerradas<br>*Nombre de la solicitud<br>*Nombre del usuario que cerró la solicitud<br>*Fecha del resumen diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien está asignado a mi solicitud</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se asigna un usuario al problema, a menos que el contacto principal y el usuario asignado sean el mismo usuario.</p> <p>Sólo se enviará una notificación si el estado del proyecto es Actual y si el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitudes]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL se ha asignado a su solicitud]: "&lt;request name=""&gt;"</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre de solicitud<br>Tipo de solicitud<br>Fecha de ingreso<br>Prioridad de problema<br>Contacto principal<br>Fecha planificada de finalización<br>Estado del problema<br><strong>Ver más detalles</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de solicitudes asignadas<br>*Nombre de la solicitud<br>*Asignado a nombre<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia el estado de un proyecto que he creado</strong> </p> <p>El usuario que ha creado el proyecto recibe una notificación por correo electrónico cuando cambia el estado del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de estado del proyecto]: &lt;project name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado del proyecto<br>Estado anterior del proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Nuevo estado del proyecto<br>*Nombre del usuario que ha cambiado el estado del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en mi solicitud</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando cambia el estado del problema, a menos que el usuario que ha cambiado el estado también sea el contacto principal.</p> <p>Sólo se enviará una notificación si el estado del proyecto es Actual y el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitudes]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;request name=""&gt; es &lt;new status=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de solicitud<br>Nombre de proyecto<br>Número de referencia de solicitud<br>Nombre del usuario que ha cambiado el estado de la solicitud<br>Nuevo estado<br>Fecha y hora en que se cambió el estado de la solicitud<br>Estado de solicitud anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de solicitudes cuyo estado ha cambiado<br>*Nombre de la solicitud<br>*Estado de solicitud anterior<br>*Nuevo estado de la solicitud<br>*Nombre del usuario que ha cambiado el estado<br>*Fecha del resumen diario<br></td> 
   <td> <p><strong>Diariamente</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
