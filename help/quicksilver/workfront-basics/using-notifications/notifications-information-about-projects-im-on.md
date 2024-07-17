---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información sobre proyectos en los que participo"
description: Las siguientes notificaciones le avisan sobre las actividades que se producen en los proyectos en los que está trabajando.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 0%

---

# Notificaciones: Información sobre proyectos en los que participo

Las siguientes notificaciones le avisan sobre las actividades que se producen en los proyectos en los que está trabajando.

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
   <td> <p><strong>Se agrega un documento a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se agrega un documento al proyecto, excepto por el usuario que lo agregó.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual] y el documento no es Privado.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Documento agregado a] &lt;Nombre de proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es <em>[!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del documento<br>Nombre del usuario que agregó el documento<br>Nombre del documento<br>Se agregó el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento<br><strong>[!UICONTROL Vista previa]</strong> y <strong>[!Descarga UICONTROL]</strong> botones<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos agregados<br>*Nombre del documento<br>*Nombre del usuario que subió el documento<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea de hito en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación cuando se completa una tarea de hito en el proyecto. Las notificaciones no se envían cuando se completa una tarea personal.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>La línea de asunto es <em>[!UICONTROL completado]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p>El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que completó la tarea<br>Estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>[!UICONTROL Diariamente]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se activa un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto se establece en [!UICONTROL Actual].</p> <p>Nota: los usuarios deben aparecer en la ficha Asignación de personal de un proyecto para recibir una notificación cuando el estado de un proyecto se establezca en [!UICONTROL Actual]. Para obtener información sobre cómo agregar usuarios a un equipo del proyecto, vea <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Administrar el equipo del proyecto</a>.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es <em>&lt;Nombre de proyecto&gt; [!UICONTROL está actualizado - Vaya al proyecto y vea las tareas!]</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Estado del proyecto<br>Fecha planificada de finalización del proyecto [!UICONTROL]<br>Propietario del proyecto<br>Lista de tareas asignadas a usted, a uno de sus roles o a uno de sus equipos<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Se activa un proyecto en el que se encuentra mi equipo</strong> <p>Los miembros de un equipo reciben una notificación por correo electrónico cuando se activa un proyecto. El equipo debe estar asignado al menos a una tarea para recibir la notificación.</p><p>Si a un usuario individual y a un equipo se les asigna una tarea en el proyecto. el equipo no recibirá ninguna notificación.</p><p>El asunto del mensaje de correo electrónico de notificación instantánea es <i>&lt;Nombre de proyecto&gt; [!UICONTROL está activo: vaya al proyecto y vea las tareas!]</i></p><p>El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p></td> 
   <td>Nombre de proyecto<br>Nombre de Portfolio<br>Número de referencia del proyecto<br>Estado del proyecto<br>Fecha planificada de finalización del proyecto [!UICONTROL]<br>Propietario del proyecto<br>Lista de tareas asignadas a su equipo<br><strong>[!UICONTROL Ver más detalles]</strong> button<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario</td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto es [!UICONTROL Completado].</p> <p>Sugerencia: si los proyectos se finalizan con regularidad, activar esta opción puede crear mucho correo electrónico para los usuarios que tienen un número limitado de tareas en muchos proyectos.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Cambio de estado del proyecto]: &lt;Nombre de proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que completó el proyecto<br>Estado del proyecto<br>Fecha y hora en que se completó el proyecto<br>Estado anterior del proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una tarea en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se completa una tarea en su proyecto. <br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Resumen del equipo del proyecto</a>.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es <em>[!UICONTROL completado]: &lt;Nombre de tarea&gt; en &lt;Nombre de proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Completado], el asunto del correo electrónico seguirá mostrando "[!UICONTROL Completado]".</p> </p> <p><em> El asunto de la notificación de resumen diario es: [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em> </p> </td> 
   <td> <p>Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que completó la tarea<br>Estado de la tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de la tarea anterior<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que completó la tarea<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agregó un problema a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se agrega un problema al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Problema agregado a] &lt;Nombre de proyecto&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que agregó el problema<br>Tipo de problema<br>Nombre del problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha resuelto un problema en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se resuelve un problema en su proyecto.<br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Resumen del equipo del proyecto</a>.</p> <p>Sólo se enviará una notificación si el estado del proyecto es [!UICONTROL Actual] o [!UICONTROL Planificación].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL completado]: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Nombre del usuario que completó el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agrega un problema no asignado a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se agrega un problema no asignado al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL ¿A quién se debe asignar este nuevo problema el] &lt;Nombre de proyecto&gt;?</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del problema<br>Nombre del usuario que agregó el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre (vacío) <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas agregados<br>*Nombre del problema<br>*Nombre del usuario que agregó el problema<br>*Fecha del resumen diario<br></td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diarios</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me agrega a un proyecto</strong> </p> <p>El usuario que se añadió al proyecto recibe una notificación por correo electrónico cuando se añade, a menos que el usuario se haya añadido a sí mismo al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Actual].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Se le ha agregado al proyecto] &lt;Nombre de proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que lo agregó al proyecto<br>Fecha planificada de inicio del proyecto [!UICONTROL]<br>Fecha planificada de finalización del proyecto [!UICONTROL]<br>Porcentaje completado del proyecto<br>Nombres de otros en el proyecto <br>Propietario del proyecto<br><strong>Ver más detalles</strong> botón<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>El estado cambia en un proyecto en el que estoy</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando cambia el estado del proyecto. <br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Resumen del equipo del proyecto</a>.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Cambio de estado del proyecto]: &lt;Nombre de proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Resumen de proyectos en los que se encuentra] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del Portfolio<br>Número de referencia del proyecto<br>Nombre del usuario que cambió el estado del proyecto<br>Nuevo estado del proyecto<br>Fecha y hora en que cambió el estado del proyecto<br>Estado anterior del proyecto<br><strong>[!UICONTROL Ver más detalles]</strong> button<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
