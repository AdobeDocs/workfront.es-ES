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
ht-degree: 6%

---

# Notificaciones: Información sobre proyectos que patrocino

Las siguientes notificaciones le avisan sobre las actividades que se producen en un proyecto que patrocina.

Para obtener información sobre cómo configurar qué notificaciones recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al agregar un documento.</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y si el documento no es [!UICONTROL Privado].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se agregó un documento [!UICONTROL a] &lt;project name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de los proyectos que patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del documento<br>Nombre del usuario que agregó el documento<br>Nombre de documento<br>Añadido el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de documentos añadidos<br>*Nombre del documento<br>*Nombre del usuario que agregó el documento<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se finaliza una tarea de hito en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se completa una tarea de hito en un proyecto que patrocina.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt; el &lt;project name=""&gt;</em></p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".<br></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Estado de nueva tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa con respecto a la programación. Un proyecto está retrasado con respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]" o "[!UICONTROL con problemas]".</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben ninguna notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de avance del proyecto]: &lt;project name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Resumen de los proyectos que patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado de progreso del proyecto<br>Proyecto [!UICONTROL Fecha planificada de inicio]<br>Proyecto [!UICONTROL Fecha planificada de finalización]<br>Proyecto [!UICONTROL Fecha proyectada de inicio]<br>Proyecto [!UICONTROL Fecha proyectada de finalización]<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario de proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se finaliza una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;task name=""&gt; el &lt;project name=""&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> </p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Estado de tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de la tarea anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa con respecto a la programación. Una tarea está retrasada respecto a la programación cuando el estado del progreso es "[!UICONTROL en riesgo]" o "[!UICONTROL detrás]" o "[!UICONTROL retrasado]"."</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de progreso de tarea]: &lt;task name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de los proyectos que patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Estado del progreso de la nueva tarea<br>Tarea [!UICONTROL Fecha planificada de inicio]<br>Tarea [!UICONTROL Fecha planificada de finalización]<br>Tarea [!UICONTROL Fecha proyectada de inicio]<br>Tarea [!UICONTROL Fecha proyectada de finalización]<br>Porcentaje completado de tarea<br>Estado de tarea<br>Asignado a nombre<br>Introducido por nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas que están retrasadas con respecto a la programación<br>*Nombre de tarea<br>*Nombre del usuario que ha introducido la tarea<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al agregar un problema.</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema añadido a] &lt;project name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es: <em>[!UICONTROL Resumen de los proyectos que patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia de problema<br>Nombre del usuario que agregó el problema<br>Nombre de problema<br>Tipo de problema<br>Fecha de ingreso<br>Prioridad de problema<br>Asignado a nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas añadidos al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al resolver un problema</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Completo]: &lt;issue name=""&gt; el &lt;project name=""&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> Resumen de los proyectos que patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de problema<br>Nombre de proyecto<br>Número de referencia de problema<br>Nombre del usuario que ha completado el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas resueltos<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al agregar un problema no asignado.</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Quién debe recibir este nuevo problema el] &lt;project name=""&gt;?</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de los proyectos que patrocina] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia de problema<br>Nombre del usuario que agregó el problema<br>Nombre de problema<br>Tipo de problema<br>Fecha de ingreso<br>Prioridad de problema<br>Asignado a nombre (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>* Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me asigna como patrocinador de un proyecto</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se le asigna el patrocinio de un proyecto.<br></p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Patrocinador de proyecto]: &lt;project name=""&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL le convirtió en patrocinador de] &lt;project name=""&gt;. [!UICONTROL Como patrocinador del proyecto, podría recibir otras notificaciones de correo electrónico en cuanto a la actividad del proyecto o podría participar en la aprobación de trabajo relacionado con el proyecto. Disfrútelo.]</em> </p> <p>El asunto de la notificación de resumen diario es: <em>Resumen de los proyectos que patrocina &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre de proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Fecha planificada de finalización del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
