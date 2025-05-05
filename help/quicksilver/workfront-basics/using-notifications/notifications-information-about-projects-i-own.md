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
ht-degree: 1%

---

# Notificaciones: Información sobre proyectos de mi propiedad

Las siguientes notificaciones le avisan sobre las actividades que se realizan en un proyecto de su propiedad. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Se agrega un documento a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto, a menos que el usuario que agregó el documento también sea el propietario del proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y el documento no es Privado.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Documento agregado a] &lt;Nombre de proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que agregó el documento<br>Nombre del documento<br>Se agregó el día<br>Detalles del documento (formato, tamaño, número de versión)<br><strong>[!UICONTROL Vista previa]</strong> y <strong>[!UICONTROL Descarga]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos agregados<br>*Nombre del documento<br>*Nombre del usuario que agregó el documento<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea de hito en un proyecto de mi propiedad</strong> </p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Nuevo estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa mi proyecto</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando el proyecto está retrasado. Un proyecto está retrasado con respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]", "[!UICONTROL retrasado]" o "[!UICONTROL retrasado]".</p> <p>Una práctica recomendada es mantener esta notificación activa. </p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio en progreso de proyecto]: &lt;Nombre de proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del progreso del proyecto<br>Fecha planificada de inicio del proyecto <br>Fecha planificada de finalización del proyecto <br>Fecha prevista de inicio del proyecto <br>Fecha prevista de finalización del proyecto <br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema a mi proyecto</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema agregado a] &lt;Nombre de proyecto&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que agregó el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados al proyecto<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario</p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación cuando se completa una tarea en su proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea <br>Estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas <br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación. Una tarea está retrasada respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]" o "[!UICONTROL detrás]" o "[!UICONTROL retrasado]"."</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio en progreso de tarea]: &lt;Nombre de tarea&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nuevo estado de progreso de la tarea<br>Fecha planificada de inicio de la tarea <br>Fecha planificada de finalización de la tarea <br>Fecha proyectada de inicio de la tarea <br>Fecha proyectada de finalización de la tarea <br>Porcentaje completado de la tarea<br>Estado de la tarea<br>Asignado al nombre<br>Introducido por el nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto*Número de proyecto<br>*Número total de tareas que se retrasan las tareas<br>*Número de tareas 4&rbrace;*Nombre de tarea<br>*Asignado a nombre<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha resuelto un problema en un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se resuelve un problema en su proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL completado]: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que completó el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema no asignado a un proyecto de mi propiedad</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL ¿A quién se debe asignar este nuevo problema en] &lt;Nombre de proyecto&gt;?</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es: <em> Resumen de proyectos de su propiedad &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que agregó el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado a nombre (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me ha asignado como propietario de un nuevo proyecto</strong> </p> <p>Cuando se asigna a un usuario como propietario de un proyecto, ese usuario recibe una notificación por correo electrónico.</p> <p>Si el propietario del proyecto es el mismo usuario que realizó la asignación, no se envía una notificación por correo electrónico.</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>Active esta opción porque se les está asignando a algo. </p> <p> Asignar algo, compartir algo, obtener acceso para algo.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Usted ahora es propietario del proyecto] &lt;Nombre de proyecto&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:<em><br></em></p> <p><em>[!UICONTROL Hola] &lt;Su nombre&gt;,<br></em><em>&lt;Nombre del usuario que le asignó como propietario del proyecto&gt; [!UICONTROL le convirtió en propietario de] &lt;Nombre del proyecto&gt;. [!UICONTROL Como propietario del proyecto, es posible que reciba otras notificaciones de correo electrónico en cuanto a la actividad del proyecto, que se le pida que apruebe horas en el proyecto o que participe en la aprobación de trabajo relacionado con el proyecto. Es todo tuyo.]</em> </p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> <p> </p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre de Portfolio<br>Número de referencia del proyecto<br>Fecha de finalización del proyecto<br>*Nombre de proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia la fecha de confirmación de una tarea en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de una tarea del proyecto, a menos que el usuario que ha cambiado la fecha de confirmación también sea el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de confirmación para] &lt;Nombre de tarea&gt; [!UICONTROL es ahora] &lt;Nueva fecha de confirmación&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> Resumen de proyectos de su propiedad &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Fecha planificada de finalización de la tarea<br>Información sobre cómo se ve afectada la escala de tiempo del proyecto por este cambio<br>Asignado a nombre<br>Introducido por nombre<br>Propietario del proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas cuya fecha de confirmación ha cambiado<br> Nombre<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong> y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia la fecha de confirmación de un problema en uno de mis proyectos</strong> </p> <p>El propietario del proyecto recibe una notificación por correo electrónico cuando cambia la fecha de confirmación de un problema del proyecto, a menos que el usuario que cambia la fecha de confirmación sea el mismo usuario que el propietario del proyecto.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Fecha de confirmación para] &lt;Nombre del problema&gt; [!UICONTROL es ahora] &lt;Nueva fecha de confirmación&gt;</em></p> <p> El asunto de la notificación de resumen diario es: <em> [!UICONTROL Resumen de los proyectos de su propiedad] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que cambió la fecha de confirmación<br>Nueva fecha de confirmación<br>Fecha planificada de finalización del problema<br>Asignada al nombre<br>Introducida por el nombre<br>Propietario del proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas cuya fecha de confirmación ha cambiado<br>*Nombre del problema<br>*Fecha del resumen diario<br></p> </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong> y [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
