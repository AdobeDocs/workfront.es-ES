---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información sobre proyectos de mi propiedad"
description: Las siguientes notificaciones le avisan sobre las actividades que se realizan en un proyecto de su propiedad. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte Modificación de sus propias notificaciones por correo electrónico.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 6%

---

# Notificaciones: Información sobre proyectos de mi propiedad

Las siguientes notificaciones le avisan sobre las actividades que se realizan en un proyecto de su propiedad. Para obtener información sobre cómo configurar qué notificaciones recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se agrega un documento a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el usuario que agregó el documento también sea el propietario del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y el documento no es Privado.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se agregó un documento [!UICONTROL a] &lt;project name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó el documento<br>Nombre de documento<br>Añadido el día<br>Detalles del documento (formato, tamaño, número de versión)<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de documentos añadidos<br>*Nombre del documento<br>*Nombre del usuario que agregó el documento<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una tarea de hito en un proyecto de mi propiedad</strong> </p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt; el &lt;project name=""&gt;</em></p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Estado de nueva tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa mi proyecto</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando el proyecto está retrasado. Un proyecto está retrasado con respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]", "[!UICONTROL retrasado]" o "[!UICONTROL retrasado]".</p> <p>Una práctica recomendada es mantener esta notificación activa. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de avance del proyecto]: &lt;project name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado de progreso del proyecto<br>Proyecto [!UICONTROL Fecha planificada de inicio]<br>Proyecto [!UICONTROL Fecha planificada de finalización]<br>Proyecto [!UICONTROL Fecha proyectada de inicio]<br>Proyecto [!UICONTROL Fecha proyectada de finalización]<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario de proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema a mi proyecto</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema añadido a] &lt;project name=""&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia de problema<br>Nombre del usuario que agregó el problema<br>Nombre de problema<br>Tipo de problema<br>Fecha de ingreso<br>Prioridad de problema<br>Asignado a nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas añadidos al proyecto<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y a diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Finalización de una tarea de un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación cuando se completa una tarea en su proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt; el &lt;project name=""&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea <br>Estado de tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas <br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación. Una tarea está retrasada respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]" o "[!UICONTROL detrás]" o "[!UICONTROL retrasado]"."</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de progreso de tarea]: &lt;task name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Estado del progreso de la nueva tarea<br>Tarea [!UICONTROL Fecha planificada de inicio]<br>Tarea [!UICONTROL Fecha planificada de finalización]<br>Tarea [!UICONTROL Fecha proyectada de inicio]<br>Tarea [!UICONTROL Fecha proyectada de finalización]<br>Porcentaje completado de tarea<br>Estado de tarea<br>Asignado a nombre<br>Introducido por nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas que están retrasadas con respecto a la programación<br>*Nombre de tarea<br>*Asignado a nombre<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se resuelve un problema en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se resuelve un problema en su proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;issue name=""&gt; el &lt;project name=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que ha completado el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas resueltos<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema no asignado a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Quién debe recibir este nuevo problema el] &lt;project name=""&gt;?</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> Resumen de los proyectos de su propiedad &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia de problema<br>Nombre del usuario que agregó el problema<br>Nombre de problema<br>Tipo de problema<br>Fecha de ingreso<br>Prioridad de problema<br>Asignado a nombre (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y a diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me asigna como propietario de un nuevo proyecto</strong> </p> <p>Cuando se asigna a un usuario como propietario de un proyecto, ese usuario recibe una notificación por correo electrónico.</p> <p>Si el propietario del proyecto es el mismo usuario que realizó la asignación, no se envía una notificación por correo electrónico.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>Active esta opción porque se les está asignando a algo. </p> <p> Asignar algo, compartir algo, obtener acceso para algo.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Usted ahora es propietario del proyecto] &lt;project name=""&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL le convirtió en propietario de] &lt;project name=""&gt;. [!UICONTROL Como propietario del proyecto, es posible que reciba otras notificaciones de correo electrónico en cuanto a la actividad del proyecto, que se le pida que apruebe horas en el proyecto o que participe en la aprobación de trabajo relacionado con el proyecto. Es todo tuyo.]</em> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Fecha de finalización del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia la fecha de confirmación de una tarea en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de una tarea del proyecto, a menos que el usuario que ha cambiado la fecha de confirmación también sea el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de confirmación para] &lt;task name=""&gt; [!UICONTROL está ahora] &lt;new commit="" date=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen de los proyectos de su propiedad &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Tarea [!UICONTROL Fecha planificada de finalización]<br>Información sobre cómo se ve afectada la escala de tiempo del proyecto por este cambio<br>Asignado a nombre<br>Introducido por nombre<br>Propietario de proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas cuya fecha de confirmación ha cambiado.<br>*Nombre de tarea<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Si cambia la fecha de confirmación de un problema en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de un problema del proyecto, a menos que el usuario que cambia la fecha de confirmación sea el mismo usuario que el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de confirmación para] &lt;issue name=""&gt; [!UICONTROL está ahora] &lt;new commit="" date=""&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Fecha planificada de finalización de problema<br>Asignado a nombre<br>Introducido por nombre<br>Propietario de proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas cuya fecha de confirmación ha cambiado<br>*Nombre del problema<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
