---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información sobre proyectos en los que estoy"
description: Las siguientes notificaciones le avisan de las actividades que se producen en proyectos en los que esté trabajando.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 6%

---

# Notificaciones: Información sobre proyectos en los que estoy

Las siguientes notificaciones le avisan de las actividades que se producen en proyectos en los que esté trabajando.

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
   <td> <p><strong>Se agrega un documento a proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se agrega un documento al proyecto, excepto para el usuario que lo ha agregado.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] y el documento no es privado.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Documento agregado a] &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es <em>[!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del documento<br>Nombre del usuario que agregó el documento<br>Nombre del documento<br>Se agregó en la fecha<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Preview]</strong> y <strong>[!UICONTROL Descargar]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos agregados<br>*Nombre del documento<br>*Nombre del usuario que cargó el documento<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una tarea de hito en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación cuando se completa una tarea de hito en el proyecto. Las notificaciones no se envían cuando se completa una tarea personal.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>La línea de asunto es <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de tarea anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se activa un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto está establecido en [!UICONTROL Actual].</p> <p>Nota: Los usuarios deben aparecer en la ficha Dotación de personal de un proyecto para recibir notificaciones cuando el estado de un proyecto esté establecido en [!UICONTROL Actual]. Para obtener información sobre cómo agregar usuarios a un equipo de proyecto, consulte <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Administrar el equipo del proyecto</a>.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>&lt;project name=""&gt; [!UICONTROL es actual - Vaya a su proyecto y vea sus tareas!]</em></p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del proyecto<br>Proyecto [!UICONTROL Fecha de finalización planeada]<br>Propietario del proyecto<br>Una lista de tareas asignadas a usted, a una de sus funciones de trabajo o a uno de sus equipos<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del compendio diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Se activa un proyecto en el que participa mi equipo</strong> <p>Los miembros de un equipo reciben una notificación por correo electrónico cuando un proyecto se activa. El equipo debe estar asignado a al menos una tarea para recibir la notificación.</p><p>Si un usuario individual y un equipo están asignados a una tarea del proyecto. el equipo no recibirá una notificación.</p><p>El asunto del correo electrónico de notificación instantánea es <i>&lt;project name=""&gt; [!UICONTROL está activo - Vaya a su proyecto y vea sus tareas!]</i></p><p>El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del proyecto<br>Proyecto [!UICONTROL Fecha de finalización planeada]<br>Propietario del proyecto<br>Una lista de tareas asignadas a su equipo<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del compendio diario</td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto es [!UICONTROL Complete].</p> <p>Sugerencia: Si los proyectos se completan con regularidad, la activación de esta opción puede crear un montón de correos electrónicos para los usuarios que tienen un número limitado de tareas en muchos proyectos.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Cambio de estado del proyecto]: &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que ha completado el proyecto<br>Estado del proyecto<br>Fecha y hora en que se completó el proyecto<br>Estado del proyecto anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se finaliza una tarea en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se completa una tarea en su proyecto. <br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Complete]: &lt;task name=""&gt; en &lt;project name=""&gt;</em></p> <p> <p>Nota: Si la tarea se cambia a un estado igual a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Complete]".</p> </p> <p><em> El tema de la notificación diaria de compendio es: [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Estado de la tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de tarea anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del compendio diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es Actual.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Problema añadido a] &lt;project name=""&gt;</em></p> <p> </p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que ha agregado el problema<br>Tipo de problema<br>Nombre del problema<br>Fecha de introducción<br>Prioridad del problema<br>Asignado a nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del compendio diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se resuelve un problema en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se completa un problema en su proyecto.<br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Complete]: &lt;issue name=""&gt; en &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Nombre del usuario que ha completado el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema no asignado a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se añade un problema sin asignar al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Quién debe asignarse a este nuevo problema el] &lt;project name=""&gt;?</em></p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que ha agregado el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de introducción<br>Prioridad del problema<br>Nombre asignado a (vacío) <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que ha añadido el problema<br>*Fecha del compendio diario<br></td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y Diario</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me agrega a un proyecto</strong> </p> <p>El usuario que se añadió al proyecto recibe una notificación por correo electrónico cuando se añade, a menos que el usuario se añada al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Se ha añadido al proyecto] &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que lo agregó al proyecto<br>Proyecto [!UICONTROL Fecha de inicio planeada]<br>Proyecto [!UICONTROL Fecha de finalización planeada]<br>Porcentaje completado del proyecto<br>Nombres de otros en el proyecto <br>Propietario del proyecto<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del compendio diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia el estado de un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando cambia el estado del proyecto. <br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Cambio de estado del proyecto]: &lt;project name=""&gt;</em></p> <p> El tema de la notificación diaria de compendio es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que ha cambiado el estado del proyecto<br>Nuevo estado del proyecto<br>Fecha y hora en que cambió el estado del proyecto<br>Estado del proyecto anterior<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del compendio diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
