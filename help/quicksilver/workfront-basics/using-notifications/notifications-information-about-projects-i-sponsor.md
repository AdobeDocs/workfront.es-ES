---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: información sobre los proyectos que patrocino'
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.
author: Courtney
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 100%

---

# Notificaciones: información sobre los proyectos que patrocino

Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.

Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se añade un documento a un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se añade un documento al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] y si el documento no es [!UICONTROL Private].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Document added to] &lt;Nombre del proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolios<br>Número de referencia del documento<br>Nombre del usuario que añadió el documento<br>Nombre del documento<br>Se añadió el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>Botones [!UICONTROL Preview]</strong> y <strong>[!UICONTROL Download]</strong><br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos añadidos<br>*Nombre del documento<br>*Nombre del usuario que añadió el documento<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha finalizado una tarea de hito en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se completa una tarea de hito en un proyecto que patrocina.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando “[!UICONTROL Complete]”.<br></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea<br>Nuevo estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>Botón [!UICONTROL See More Details]</strong><br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un proyecto que patrocino se retrasa</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa con respecto a la programación. Un proyecto se retrasa con respecto a lo programado cuando el estado del progreso es “[!UICONTROL At Risk]” o “[!UICONTROL In Trouble]”.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Project Progress Change]: &lt;Nombre del proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Digest of Projects You Sponsor] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Estado del progreso del proyecto<br>[!UICONTROL Planned Start Date] del proyecto<br>[!UICONTROL Planned Completion Date] del proyecto<br>[!UICONTROL Projected Start Date] del proyecto<br>[!UICONTROL Projected Completion Date] del proyecto<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha completado una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre de la tarea&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando “[!UICONTROL Complete]”.</p> </p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea<br>Estado de la tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de la tarea anterior<br><strong>botón Ver más detalles</strong><br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación. Una tarea se retrasa con respecto a lo programado cuando el estado del progreso es “[!UICONTROL At Risk]”, “[!UICONTROL Behind]” o “[!UICONTROL Late]”.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Task Progress Change]: &lt;Nombre de la tarea&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de la tarea<br>Nuevo estado de progreso de la tarea<br>[!UICONTROL Planned Start Date] de la tarea<br>[!UICONTROL Planned Completion Date] de la tarea<br>[!UICONTROL Projected Start Date] de la tarea<br>[!UICONTROL Projected Completion Date] de la tarea<br>Porcentaje completado de la tarea<br>Estado de la tarea<br>Asignado al nombre<br>Introducido por nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas que retrasadas<br>*Nombre de la tarea<br>*Nombre del usuario que ha introducido la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha añadido un problema a un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Issue added to] &lt;Nombre del proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Digest of Projects You Sponsor] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del problema<br>Nombre del usuario que añadió el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha completado un problema en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que completó el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>Botón Ver más detalles</strong><br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha añadido un problema no asignado a un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se añade un problema no asignado al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>¿[!UICONTROL Who should be assigned to this new issue on] &lt;Nombre de proyecto&gt;?</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del problema<br>Nombre del usuario que añadió el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado a nombre (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que añadió el problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me ha asignado como patrocinador de un proyecto</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se le asigna el patrocinio de un proyecto.<br></p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Project Sponsor]: &lt;Nombre del proyecto&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hi] &lt;Su nombre&gt;,</em> </p> <p><em>&lt;Nombre del usuario que le asignó como patrocinador del proyecto&gt; [!UICONTROL made you the sponsor of] &lt;Nombre del proyecto&gt;. [!UICONTROL As the Project Sponsor, you might receive additional email notifications about project activity or be involved in approving work related to the project.  Enjoy.]</em> </p> <p>El asunto de la notificación del resumen diario es: <em>Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Fecha planificada de finalización del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
