---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Información sobre proyectos que tengo'
description: Las siguientes notificaciones le avisan de las actividades que se están realizando en un proyecto que posea. Para obtener información sobre la configuración de las notificaciones que recibe, consulte Activación o desactivación de sus propias notificaciones de evento.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# Notificaciones: Información sobre proyectos que tengo

Las siguientes notificaciones le avisan de las actividades que se están realizando en un proyecto que posea. Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se agrega un documento a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el usuario que agregó el documento también sea el propietario del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] y el documento no es privado.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Documento agregado a] &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó el documento<br>Nombre del documento<br>Se agregó en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos agregados<br>*Nombre del documento<br>*Nombre del usuario que agregó el documento<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una tarea de hijo en un proyecto de mi propiedad</strong> </p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p>Nota: Si la tarea se cambia a un estado igual a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Complete]".</p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Nuevo estado de tarea<br>Fecha y hora en que se completó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando el proyecto está atrasado. Un proyecto está retrasado cuando el estado de progreso es "[!UICONTROL At Risk]", "[!UICONTROL Behind]" o "[!UICONTROL Late]".</p> <p>Se recomienda mantener activa esta notificación. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de progreso del proyecto]: &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del progreso del proyecto<br>Proyecto [!UICONTROL Fecha de inicio planeada]<br>Proyecto [!UICONTROL Fecha de finalización planeada]<br>Proyecto [!UICONTROL Fecha de inicio prevista]<br>Proyecto [!UICONTROL Fecha de finalización prevista]<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del compendio diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema añadido a] &lt;project name=""&gt;</em></p> <p> </p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que ha agregado el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de introducción<br>Prioridad del problema<br>Asignado a nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados al proyecto<br>*Nombre del problema<br>*Nombre del usuario que ha añadido el problema<br>*Fecha del compendio diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Finalización de una tarea de un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación cuando una tarea finaliza en su proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p> <p>Nota: Si la tarea se cambia a un estado igual a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Complete]".</p> </p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea <br>Estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas <br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa en la programación. Una tarea está retrasada cuando el estado de progreso es "[!UICONTROL At Risk]" o "[!UICONTROL Behind]" o "[!UICONTROL Late]"."</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Task Progress Change]: &lt;task name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nuevo estado de progreso de tarea<br>Tarea [!UICONTROL Fecha de inicio planeada]<br>Tarea [!UICONTROL Fecha de finalización planeada]<br>Tarea [!UICONTROL Fecha de inicio prevista]<br>Tarea [!UICONTROL Fecha de finalización prevista]<br>Porcentaje de tarea completado<br>Estado de la tarea<br>Asignado a nombre<br>Introducido Por Nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas que están atrasadas<br>*Nombre de tarea<br>*Asignado a nombre<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se resuelve un problema en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se completa un problema en el proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben una notificación. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;issue name=""&gt; en &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que ha completado el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema no asignado a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema sin asignar al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Quién debe asignarse a este nuevo problema el] &lt;project name=""&gt;?</em></p> <p> </p> <p> El tema de la notificación diaria de compendio es: <em> Resumen de proyectos que posee &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que ha agregado el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de introducción<br>Prioridad del problema<br>Nombre asignado a (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que ha añadido el problema<br>*Fecha del compendio diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me asigna como propietario de un nuevo proyecto</strong> </p> <p>Cuando se asigna a un usuario como propietario de un proyecto, este recibe una notificación por correo electrónico.</p> <p>Si el propietario del proyecto es el mismo usuario que realizó la asignación, no se envía una notificación por correo electrónico.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben una notificación.</p> <p>Enciéndelo porque están siendo asignados a algo. </p> <p> Asignar algo, compartir algo, obtener acceso para algo.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Ahora es el propietario del proyecto de] &lt;project name=""&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL le ha hecho propietario de] &lt;project name=""&gt;. [!UICONTROL Como propietario del proyecto, puede recibir notificaciones por correo electrónico adicionales sobre la actividad del proyecto, ser necesario para aprobar horas del proyecto o participar en la aprobación del trabajo relacionado con el proyecto. Es todo tuyo.]</em> </p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Fecha de finalización del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del compendio diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia la fecha de confirmación de una tarea en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de una tarea del proyecto, a menos que el usuario que cambió la fecha de confirmación también sea el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de confirmación] &lt;task name=""&gt; [!UICONTROL es ahora] &lt;new commit="" date=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> Resumen de proyectos que posee &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Tarea [!UICONTROL Fecha de finalización planeada]<br>Información sobre cómo se ve afectada la línea de tiempo del proyecto por este cambio<br>Asignado a nombre<br>Introducido Por Nombre<br>Propietario del proyecto<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas cuya fecha de confirmación ha cambiado<br>*Nombre de tarea<br>*Fecha del compendio diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Si cambia la fecha de confirmación de un problema en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de un problema del proyecto, a menos que el usuario que cambie la fecha de confirmación sea el mismo usuario que el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de confirmación] &lt;issue name=""&gt; [!UICONTROL es ahora] &lt;new commit="" date=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es: <em> [!UICONTROL Resumen de proyectos que posee] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Fecha de finalización planeada del problema<br>Asignado a nombre<br>Introducido Por Nombre<br>Propietario del proyecto<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas cuya fecha de confirmación ha cambiado<br>*Nombre del problema<br>*Fecha del compendio diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
