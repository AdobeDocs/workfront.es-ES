---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información sobre proyectos que patrocino"
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 0%

---

# Notificaciones: Información sobre proyectos que patrocino

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
   <td> <p><strong>Se agrega un documento a un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y si el documento no es [!UICONTROL Privado].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Documento agregado a] &lt;Nombre de proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de proyectos que patrocina] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del documento<br>Nombre del usuario que agregó el documento<br>Nombre del documento<br>Se agregó el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Download]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos agregados<br>*Nombre del documento<br>*Nombre del usuario que agregó el documento<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea de hito en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se completa una tarea de hito en un proyecto que patrocina.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".<br></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Nuevo estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa con respecto a la programación. Un proyecto está retrasado con respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]" o "[!UICONTROL con problemas]".</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio en progreso de proyecto]: &lt;Nombre de proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Resumen de los proyectos que patrocina] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del progreso del proyecto<br>Fecha planificada de inicio del proyecto [!UICONTROL]<br>Fecha planificada de finalización del proyecto [!UICONTROL]<br>Fecha proyectada de inicio del proyecto [!UICONTROL]<br>Fecha proyectada de finalización del proyecto [!UICONTROL]<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL completo]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> </p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea<br>Estado de la tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de la tarea anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación. Una tarea está retrasada respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]" o "[!UICONTROL detrás]" o "[!UICONTROL retrasado]"."</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio en progreso de tarea]: &lt;Nombre de tarea&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de proyectos que patrocina] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nuevo estado de progreso de la tarea<br>Fecha planificada de inicio de la tarea [!UICONTROL]<br>Fecha planificada de finalización de la tarea [!UICONTROL]<br>Fecha proyectada de inicio de la tarea [!UICONTROL]<br>Fecha proyectada de finalización de la tarea [!UICONTROL]<br>Porcentaje completado de la tarea<br>Estado de la tarea<br>Asignado al nombre<br>Introducido por el nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto*Número de proyecto<br>*Número total de tareas que se retrasan las tareas<br>*Número de tareas 4}*Nombre de tarea<br>*Nombre del usuario que ha introducido la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agregó un problema a un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema agregado a] &lt;Nombre de proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Resumen de los proyectos que patrocina] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que agregó el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se resuelve un problema en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL completado]: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que completó el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema no asignado a un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL ¿A quién se debe asignar este nuevo problema en] &lt;Nombre de proyecto&gt;?</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de proyectos que patrocina] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que agregó el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado a nombre (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estoy establecido como patrocinador de un proyecto</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se le asigna el patrocinio de un proyecto.<br></p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Patrocinador de proyecto]: &lt;Nombre de proyecto&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hola] &lt;Su nombre&gt;,</em> </p> <p><em>&lt;Nombre del usuario que le asignó como patrocinador del proyecto&gt; [!UICONTROL le convirtió en patrocinador de] &lt;Nombre del proyecto&gt;. [!UICONTROL Como patrocinador del proyecto, podría recibir otras notificaciones de correo electrónico en cuanto a la actividad del proyecto o podría participar en la aprobación de trabajo relacionado con el proyecto. Disfrútelo.]</em> </p> <p>El asunto de la notificación de resumen diario es: <em>Resumen de los proyectos que patrocina &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre de Portfolio<br>Número de referencia del proyecto<br>Fecha planificada de finalización del proyecto<br>*Nombre de proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
