---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: información sobre proyectos de mi propiedad'
description: Las siguientes notificaciones avisan sobre las actividades que se realizan en un proyecto de su propiedad. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte Modificación de sus propias notificaciones por correo electrónico.
author: Courtney
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 100%

---

# Notificaciones: información sobre proyectos de mi propiedad

Las siguientes notificaciones avisan sobre las actividades que se realizan en un proyecto de su propiedad. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se añade un documento a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se añade un documento al proyecto, a menos que el usuario que añadió el documento también sea el propietario del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] y el documento no es privado.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Document added to] &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Nombre del usuario que añadió el documento<br>Nombre del documento<br>Se añadió el día<br>Detalles del documento (formato, tamaño y número de versión)<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Download]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos añadidos<br>*Nombre del documento<br>*Nombre del usuario que añadió el documento<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una tarea de hito en un proyecto de mi propiedad</strong> </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando “[!UICONTROL Complete]”.</p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea<br>Nuevo estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL See More Details]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa mi proyecto</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa. Un proyecto se encuentra retrasado con respecto a la programación cuando el estado del progreso es “[!UICONTROL At Risk]”, “[!UICONTROL Behind]” o “[!UICONTROL Late]”.</p> <p>Una práctica recomendada consiste en mantener esta notificación activa. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Project Progress Change]: &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Estado del progreso del proyecto<br>[!UICONTROL Planned Start Date] del proyecto<br>[!UICONTROL Planned Completion Date] del proyecto<br>[!UICONTROL Projected Start Date] del proyecto<br>[!UICONTROL Projected Completion Date] del proyecto<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado de progreso del proyecto<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema a mi proyecto</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Issue added to] &lt;Nombre del proyecto&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del problema<br>Nombre del usuario que añadió el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos al proyecto<br>*Nombre del problema<br>*Nombre del usuario que añadió el problema<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Finalización de una tarea de un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación cuando se completa una tarea del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre de la tarea&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando “[!UICONTROL Complete]”.</p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea <br>Estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL See More Details]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas <br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación. Una tarea se retrasa con respecto a lo programado cuando el estado del progreso es “[!UICONTROL At Risk]”, “[!UICONTROL Behind]” o “[!UICONTROL Late]”.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Task Progress Change]: &lt;Task Name&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nuevo estado de progreso de la tarea<br>Tarea [!UICONTROL Planned Start Date]<br>Tarea [!UICONTROL Planned Completion Date]<br>Tarea [!UICONTROL Projected Start Date]<br>Tarea [!UICONTROL Projected Completion Date]<br>Porcentaje completado de la tarea<br>Estado de la tarea<br>Asignado al nombre<br>Introducido por el nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas con retraso<br>*Nombre de tarea<br>*Asignado a nombre<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se resuelve un problema en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se resuelve un problema en su proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Issue Name&gt; en &lt;Project Name&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que completó el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL See More Details]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se añade un problema no asignado a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se añade un problema no asignado al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Who should be assigned to this new issue on] &lt;Project Name&gt;?</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> Resumen de proyectos de su propiedad &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que añadió el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado a nombre (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados<br>*Nombre del problema<br>*Nombre del usuario que añadió el problema<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me asigna como propietario de un nuevo proyecto</strong> </p> <p>Cuando se asigna a un usuario como propietario de un proyecto, ese usuario recibe una notificación por correo electrónico.</p> <p>Si el propietario del proyecto es el mismo usuario que realizó la asignación, no se envía una notificación por correo electrónico.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>Active esta opción porque se les está asignando a algo. </p> <p> Asignar algo, compartir algo, obtener acceso para algo.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL You're now the project owner of] &lt;Project Name&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;Your Name&gt;,<br></em><em>&lt;Name of the user who assigned you as the Project Owner&gt; [!UICONTROL made you the owner of] &lt;Project Name&gt;.  [!UICONTROL As the Project Owner, you might receive additional email notifications about project activity, be required to approve hours for the project, or be involved in approving work related to the project.  It's all yours.]</em> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> <p> </p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre de portatfolio<br>Número de referencia del proyecto<br>Fecha de finalización del proyecto<br>*Nombre de proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia la fecha de compromiso de una tarea en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de una tarea del proyecto, a menos que el usuario que la haya cambiado también sea el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Commit date for] &lt;Task Name&gt; [!UICONTROL is now] &lt;New Commit Date&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen de proyectos de su propiedad &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Tarea [!UICONTROL Planned Completion Date]<br>Información sobre cómo se ve afectada la línea de tiempo del proyecto por este cambio<br>Asignado a nombre<br>Introducido por nombre<br>Propietario del proyecto<br><strong>[!UICONTROL See More Details]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas cuya fecha de confirmación ha cambiado<br>*Nombre de tarea<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong> y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Si cambia la fecha de compromiso de un problema en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de un problema del proyecto, a menos que el usuario que cambia la fecha de confirmación sea el mismo usuario que el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Commit date for] &lt;Issue Name&gt; [!UICONTROL is now] &lt;New Commit Date&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Fecha planificada de finalización del problema<br>Asignada al nombre<br>Introducida por nombre<br>Propietario del proyecto<br><strong>[!UICONTROL See More Details]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas cuya fecha de confirmación ha cambiado<br>*Nombre del problema<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong> y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
