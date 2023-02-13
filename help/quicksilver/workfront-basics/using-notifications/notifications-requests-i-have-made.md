---
content-type: reference
navigation-topic: notifications
title: '''Notificaciones: Solicitudes que he hecho'
description: Las siguientes notificaciones le permiten conocer las solicitudes realizadas en Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 6%

---

# Notificaciones: Solicitudes que he formulado

Las siguientes notificaciones le permiten conocer las solicitudes realizadas en [!DNL Adobe Workfront].

Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se completó una solicitud de aprobación de documento</strong> </p> <p>El usuario que solicitó una aprobación en un documento recibe una notificación por correo electrónico cuando se completa la solicitud de aprobación del documento.</p> <p>El asunto del correo electrónico de notificación instantánea es:<em> &lt;approver name=""&gt; has &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; este documento.</em></p> <p>Nota: No puede configurar esta notificación para un correo electrónico de compendio diario.</p> </td> 
   <td> Nombre del documento<br>Nombre del aprobador </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha cambiado o subido un documento en un problema en el cual soy el autor</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se carga o cambia un documento del problema, a menos que el usuario que cargó o cambió el documento también sea el contacto principal.</p> <p>Solo se envía una notificación si el proyecto está configurado como una [!UICONTROL Help Request Queue] (tal como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitud]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Documento agregado a &lt;issue name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es: <em>Resumen de sus solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del objeto donde se cargó el documento<br>Nombre del objeto principal<br>Número de referencia del documento<br>Nombre del usuario que cargó el documento<br>Nombre del documento<br>Se agregó en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos cargados<br>*Nombre del documento<br>*Nombre del objeto principal<br>*Nombre del usuario que agregó el documento<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una solicitud de subir documento</strong> </p> <p>El Solicitante de documento recibe una notificación por correo electrónico cuando se completa una solicitud de carga de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Su solicitud de documento desde] &lt;user name=""&gt; se cumplió</em></p> <p>Nota: No puede configurar esta notificación para un correo electrónico de compendio diario.</p> </td> 
   <td> <p>Nombre del usuario que cargó el documento<br>Nombre del objeto donde se cargó el documento<br>Nombre del documento<br><br></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha completado una tarea personal que había asignado a otro usuario</strong> </p> <p>Se envía una notificación al usuario que asignó una tarea ad hoc a otra persona cuando se completa dicha tarea. </p> <p>Para obtener más información sobre las tareas ad hoc, consulte <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Crear elementos de trabajo desde el área [!UICONTROL Home]</a>.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Finalización de tarea: &lt;task name=""&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de compendio diario.</p> </p> </td> 
   <td> Nombre de la tarea<br>Nombre de proyecto predeterminado (proyecto personal del usuario que recibió la tarea personal)<br>Número de referencia de tarea<br>Nombre del propietario de la tarea<br>Nuevo estado de tarea<br>Fecha y hora en que se completó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br><br><br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar correo electrónico al creador del problema cuando se resuelva el problema</strong> </p> <p>El contacto principal de un problema recibe una notificación cuando se completa el problema.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema finalizado]: &lt;issue name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de las solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que ha completado el problema<br>Nuevo estado<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario que ha completado el problema<br>*Fecha del compendio diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Agrego un problema a un proyecto</strong> </p> <p>El contacto principal de un problema recibe una notificación cuando agrega un problema en un proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema enviado]: &lt;issue name=""&gt; en &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de las solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Su nombre<br>Nombre del problema<br>Fecha de introducción<br>Prioridad del problema<br>Estado del problema<br>Asignado a nombre<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Fecha del compendio diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Yo envío una solicitud (confirmación)</strong> </p> <p>El contacto principal sobre el problema recibe una notificación por correo electrónico cuando envía un problema.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y si el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitud]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Request Submitted]: &lt;request name=""&gt; en &lt;project request="" queue="" name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de las solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del proyecto (nombre de la cola de solicitud)<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del problema<br>Fecha de introducción<br>Prioridad del problema<br>Estado del problema<br>Asignado a nombre<br>Contacto principal<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de solicitudes enviadas<br>*Nombre de la solicitud<br>*Prioridad de la solicitud<br>*Fecha del compendio diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mi solicitud se ha cerrado (confirmación)</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se cierra la solicitud.</p> <p>Solo se envía una notificación si el estado del proyecto es Current y si el proyecto está configurado como una [!UICONTROL Help Request Queue] (tal como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Se ha cerrado su solicitud]:"&lt;request name=""&gt;"</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la solicitud<br>Nombre del proyecto<br>Número de referencia de solicitud<br>Nombre del usuario que cerró la solicitud<br>Estado del problema<br>Fecha y hora en que se cerró la solicitud<br>Estado de solicitud anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de solicitudes cerradas<br>*Nombre de la solicitud<br>*Nombre del usuario que cerró la solicitud<br>*Fecha del compendio diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguien está asignado a mi solicitud</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se asigna un usuario al problema, a menos que el contacto principal y el usuario asignado sean el mismo usuario.</p> <p>Solo se envía una notificación si el estado del proyecto es Current y si el proyecto está configurado como una [!UICONTROL Help Request Queue] (tal como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitud]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL se ha asignado a su solicitud]: "&lt;request name=""&gt;"</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre de la solicitud<br>Tipo de solicitud<br>Fecha de introducción<br>Prioridad del problema<br>Contacto principal<br>Fecha de finalización planeada<br>Estado del problema<br><strong>Ver más detalles</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de solicitudes asignadas<br>*Nombre de la solicitud<br>*Asignado a nombre<br>*Fecha del compendio diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia el estado de un proyecto que he creado</strong> </p> <p>El usuario que ha creado el proyecto recibe una notificación por correo electrónico cuando cambia el estado del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de estado del proyecto]: &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado del proyecto<br>Estado del proyecto anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Nuevo estado del proyecto<br>*Nombre del usuario que ha cambiado el estado del proyecto<br>*Fecha del compendio diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en mi solicitud</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando cambia el estado del problema, a menos que el usuario que cambió el estado también sea el contacto principal.</p> <p>Solo se envía una notificación si el estado del proyecto es Current y el proyecto está configurado como una [!UICONTROL Help Request Queue] (tal y como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitud]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;request name=""&gt; es &lt;new status=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de las solicitudes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la solicitud<br>Nombre del proyecto<br>Número de referencia de solicitud<br>Nombre del usuario que ha cambiado el estado de la solicitud<br>Nuevo estado<br>Fecha y hora en que se cambió el estado de la solicitud<br>Estado de solicitud anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de solicitudes cuyo estado ha cambiado<br>*Nombre de la solicitud<br>*Estado de solicitud anterior<br>*Nuevo estado de solicitud<br>*Nombre del usuario que ha cambiado el estado<br>*Fecha del compendio diario<br></td> 
   <td> <p><strong>Diariamente</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
