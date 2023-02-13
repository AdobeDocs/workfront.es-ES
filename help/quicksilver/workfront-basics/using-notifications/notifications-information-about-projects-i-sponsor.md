---
content-type: reference
navigation-topic: notifications
title: '''Notificaciones: Información sobre los proyectos que patrocino'
description: Las siguientes notificaciones le avisan de las actividades que se producen en un proyecto que patrocina.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1316'
ht-degree: 6%

---

# Notificaciones: Información sobre los proyectos que patrocino

Las siguientes notificaciones le avisan de las actividades que se producen en un proyecto que patrocina.

Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al agregar un documento.</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un documento al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] y si el documento no es [!UICONTROL Private].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Documento agregado a] &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de proyectos patrocinados] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del documento<br>Nombre del usuario que agregó el documento<br>Nombre del documento<br>Se agregó en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos agregados<br>*Nombre del documento<br>*Nombre del usuario que agregó el documento<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se finaliza una tarea de hito en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se completa una tarea de hitos en un proyecto que patrocina.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p>Nota: Si la tarea se cambia a un estado igual a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Complete]".<br></p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de proyectos patrocinados por usted &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Nuevo estado de tarea<br>Fecha y hora en que se completó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando el proyecto se retrasa. Un proyecto está retrasado cuando el estado de progreso es "[!UICONTROL At Risk]" o "[!UICONTROL In Trouble]".</p> <p>Los usuarios con una licencia de [!UICONTROL Review] no reciben una notificación.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Cambio de progreso del proyecto]: &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es: <em>[!UICONTROL Resumen de proyectos patrocinados] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del progreso del proyecto<br>Proyecto [!UICONTROL Fecha de inicio planeada]<br>Proyecto [!UICONTROL Fecha de finalización planeada]<br>Proyecto [!UICONTROL Fecha de inicio prevista]<br>Proyecto [!UICONTROL Fecha de finalización prevista]<br>Porcentaje completado del proyecto<br>Estado del proyecto<br>Propietario del proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del progreso del proyecto<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se finaliza una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p> <p>Nota: Si la tarea se cambia a un estado igual a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Complete]".</p> </p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de proyectos patrocinados por usted &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Estado de la tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de tarea anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se retrasa una tarea en un proyecto que patrocino</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando una tarea del proyecto se retrasa en la programación. Una tarea está retrasada cuando el estado de progreso es "[!UICONTROL At Risk]" o "[!UICONTROL Behind]" o "[!UICONTROL Late]"."</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Task Progress Change]: &lt;task name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de proyectos patrocinados] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nuevo estado de progreso de tarea<br>Tarea [!UICONTROL Fecha de inicio planeada]<br>Tarea [!UICONTROL Fecha de finalización planeada]<br>Tarea [!UICONTROL Fecha de inicio prevista]<br>Tarea [!UICONTROL Fecha de finalización prevista]<br>Porcentaje de tarea completado<br>Estado de la tarea<br>Asignado a nombre<br>Introducido Por Nombre<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas que están atrasadas<br>*Nombre de tarea<br>*Nombre del usuario que ha introducido la tarea<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al agregar un problema.</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Problema añadido a] &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es: <em>[!UICONTROL Resumen de proyectos patrocinados] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que ha agregado el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de introducción<br>Prioridad del problema<br>Asignado a nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del compendio diario<br><br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al resolver un problema</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;issue name=""&gt; en &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> Resumen de proyectos patrocinados por usted &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que ha completado el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Enviar mensaje de correo electrónico al patrocinador del proyecto al agregar un problema no asignado.</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando se agrega un problema sin asignar al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Quién debe asignarse a este nuevo problema el] &lt;project name=""&gt;?</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de proyectos patrocinados] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que ha agregado el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de introducción<br>Prioridad del problema<br>Nombre asignado a (vacío)<br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que ha añadido el problema<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me asigna como patrocinador de un proyecto</strong> </p> <p>El patrocinador del proyecto recibe una notificación por correo electrónico cuando está establecido como patrocinador de un proyecto.<br></p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Patrocinador de proyectos]: &lt;project name=""&gt;</em></p> <p>El siguiente texto se incluye en el cuerpo de la notificación por correo electrónico:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL te ha hecho patrocinador de] &lt;project name=""&gt;. [!UICONTROL Como patrocinador del proyecto, puede recibir notificaciones por correo electrónico adicionales sobre la actividad del proyecto o participar en la aprobación del trabajo relacionado con el proyecto. Disfrútelo.]</em> </p> <p>El tema de la notificación diaria de compendio es: <em>Resumen de proyectos patrocinados por usted &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Fecha de finalización planeada para el proyecto<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del compendio diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
