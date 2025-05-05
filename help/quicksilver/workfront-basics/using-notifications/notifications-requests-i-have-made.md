---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Solicitudes que he realizado"
description: Las siguientes notificaciones le permiten conocer las solicitudes que ha realizado en Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Notificaciones: Solicitudes que he realizado

Las siguientes notificaciones le permiten conocer las solicitudes que ha realizado en [!DNL Adobe Workfront].

Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se completó una solicitud de aprobación de documento</strong> </p> <p>El usuario que solicitó una aprobación de un documento recibe una notificación por correo electrónico cuando se completa la solicitud de aprobación del documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em> &lt;Nombre de aprobador&gt; tiene &lt;Decisión de aprobación ([!UICONTROL aprobada], [!UICONTROL aprobada con cambios], [!UICONTROL rechazado])&gt; este documento.</em></p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </td> 
   <td> Nombre de documento<br>Nombre de aprobador </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha cambiado o subido un documento en un problema en el cual soy el contacto principal</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se carga o cambia un documento en el problema, a menos que el usuario que cargó o cambió el documento también sea el contacto principal.</p> <p>Solo se envía una notificación si el proyecto está configurado como una [!UICONTROL Cola de solicitudes de ayuda] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitudes]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Documento agregado a &lt;Nombre del problema&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>Resumen de sus solicitudes &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del objeto donde se cargó el documento<br>Nombre del objeto principal<br>Número de referencia del documento<br>Nombre del usuario que cargó el documento<br>Nombre del documento<br>Añadido en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Vista previa]</strong> y <strong>[!UICONTROL Descarga]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos cargados<br>*Nombre del documento<br>*Nombre del objeto principal&rbrace;*Nombre del usuario que agregó el documento<br>*Fecha del resumen diario<br> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de carga de documento</strong> </p> <p>El solicitante del documento recibe una notificación por correo electrónico cuando se completa una solicitud de carga de documento.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Su solicitud de documento de] &lt;Nombre de usuario&gt; se ha completado</em></p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </td> 
   <td> <p>Nombre del usuario que subió el documento<br>Nombre del objeto donde se subió el documento<br>Nombre del documento<br><br></p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea personal que asigné a otra persona</strong> </p> <p>Se envía una notificación al usuario que asignó una solicitud de trabajo personal a otra persona cuando se completa esa solicitud. </p>  <p>El asunto del correo electrónico de notificación instantánea es: <em>Finalización de tarea: &lt;Nombre de tarea&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto predeterminado (proyecto personal del usuario que recibió la tarea personal)<br>Número de referencia de la tarea<br>Nombre del propietario de la tarea<br>Nuevo estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br><br><br></td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha resuelto un problema en el cual soy el contacto principal</strong> </p> <p>El contacto principal de un problema recibe una notificación cuando se resuelve el problema.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Resolución del problema]: &lt;Nombre del problema&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;Fecha del resumen diario&gt;</em></p> <p> </p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que completó el problema<br>Nuevo estado<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario que completó el problema<br>*Fecha del resumen diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Agrego un problema a un proyecto</strong> </p> <p>El contacto principal de un problema recibe una notificación cuando añade un problema en un proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema enviado]: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del problema<br>Nombre del problema<br>Fecha de introducción<br>Prioridad del problema<br>Estado del problema<br>Asignado a nombre<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Fecha del resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envío una solicitud (confirmación)</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando envía un problema.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y si el proyecto está configurado como una [!UICONTROL Cola de solicitudes de ayuda] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Crear una cola de solicitudes]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Solicitud enviada]: &lt;Nombre de solicitud&gt; en &lt;Nombre de proyecto (cola de solicitud)&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre de proyecto (nombre de cola de solicitud)<br>Nombre de Portfolio<br>Número de referencia del problema<br>Nombre de problema<br>Fecha de introducción<br>Prioridad del problema<br>Estado del problema<br>Asignado a nombre<br>Contacto principal<br>*Número de referencia del proyecto<br>*Nombre de proyecto<br>*Número total de solicitudes enviadas<br>*Nombre de solicitud<br>*Prioridad de solicitud<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha cerrado mi solicitud (confirmación)</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se cierra la solicitud.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Su solicitud se ha cerrado]:"&lt;Nombre de solicitud&gt;"</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de solicitud<br>Nombre de proyecto<br>Número de referencia de solicitud<br>Nombre del usuario que cerró la solicitud<br>Estado del problema<br>Fecha y hora en que se cerró la solicitud<br>Estado de solicitud anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de solicitudes cerradas<br>*Nombre de solicitud<br>*Nombre del usuario que cerró la solicitud<br>*Fecha del resumen diario </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha asignado a alguien a mi solicitud</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando se asigna un usuario al problema, a menos que el contacto principal y el usuario asignado sean el mismo usuario.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y si el proyecto está configurado como una [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;Nombre del usuario asignado a su solicitud&gt; [!UICONTROL se ha asignado a su solicitud]: "&lt;Nombre de solicitud&gt;"</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre de solicitud<br>Tipo de solicitud<br>Fecha de introducción<br>Prioridad del problema<br>Contacto principal<br>Fecha planificada de finalización<br>Estado del problema<br><strong>Ver más detalles</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de solicitudes asignadas<br>*Nombre de solicitud<br>*Asignado al nombre<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en un proyecto que he creado</strong> </p> <p>El usuario que ha creado el proyecto recibe una notificación por correo electrónico cuando cambia el estado del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de estado del proyecto]: &lt;Nombre de proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de sus solicitudes] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que cambió el estado<br>Nuevo estado<br>Fecha y hora en que se cambió el estado del proyecto<br>Estado anterior del proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Nuevo estado del proyecto<br>*Nombre del usuario que cambió el estado del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en mi solicitud</strong> </p> <p>El contacto principal del problema recibe una notificación por correo electrónico cuando cambia el estado del problema, a menos que el usuario que ha cambiado el estado también sea el contacto principal.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual y el proyecto está configurado como [!UICONTROL Help Request Queue] (como se describe en <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;Nombre de solicitud&gt; es &lt;Nuevo estado&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de sus solicitudes &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de solicitud<br>Nombre de proyecto<br>Número de referencia de solicitud<br>Nombre del usuario que cambió el estado de la solicitud<br>Nuevo estado<br>Fecha y hora en que se cambió el estado de la solicitud<br>Estado de solicitud anterior<br><strong>[!UICONTROL Ver más detalles]</strong> button<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de solicitudes cuyo estado cambió<br>*Nombre de solicitud<br>*Estado de solicitud anterior<br>*Nuevo estado de solicitud<br>*Nombre del usuario que cambió el estado<br> Fecha del resumen diario<br></td> 
   <td> <p><strong>Diariamente</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
