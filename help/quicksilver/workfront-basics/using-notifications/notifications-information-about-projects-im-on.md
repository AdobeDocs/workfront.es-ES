---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Información sobre proyectos en los que participo'
description: Las siguientes notificaciones le avisan sobre las actividades que tienen lugar en los proyectos en los que está trabajando.
author: Courtney
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 100%

---

# Notificaciones: Información sobre proyectos en los que participo

Las siguientes notificaciones le avisan sobre las actividades que tienen lugar en los proyectos en los que está trabajando.

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
   <td> <p><strong>Se añade un documento a un proyecto en el que participo</strong> </p> <p>Los integrantes de un equipo de proyectos reciben una notificación por correo electrónico cuando se añade un documento al proyecto, salvo el usuario que lo ha añadido.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] y el documento no es privado.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p>El asunto de la notificación de resumen diario es <em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del documento<br>Nombre del usuario que ha añadido el documento<br>Nombre del documento<br>Se añadió el día<br>Detalles del documento (formato, tamaño, número de versión)<br>Miniatura del documento <br><strong>Botones [!UICONTROL Preview]</strong> y <strong>[!UICONTROL Download]</strong><br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de documentos añadidos<br>*Nombre del documento<br>*Nombre del usuario que ha subido el documento<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una tarea de hito en un proyecto en el que participo</strong> </p> <p>Los integrantes de un equipo de proyecto reciben una notificación cuando se completa una tarea de hito en el proyecto. Las notificaciones no se envían cuando se completa una tarea personal.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>La línea de asunto es <em>[!UICONTROL Complete]: &lt;Task Name&gt; en &lt;Project Name&gt;</em></p> <p>El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que ha completado la tarea<br>Estado de la tarea<br>Fecha y hora en que se completó la tarea<br>Estado de la tarea anterior<br><strong>Botón [!UICONTROL See More Details]</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del resumen diario<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se activa un proyecto en el que participo</strong> </p> <p>Los integrantes de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto se establece en [!UICONTROL Current].</p> <p>Nota: Los usuarios deben aparecer en la pestaña Dotación de personal de un proyecto para recibir una notificación cuando el estado de un proyecto se establezca en [!UICONTROL Current]. Para obtener información sobre cómo se añaden usuarios a un equipo de proyecto, consulte <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Administrar el equipo del proyecto</a>.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es <em>&lt;Project Name&gt; [!UICONTROL is Current - Go to your project and see your tasks!]</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Estado del proyecto<br> [!UICONTROL Planned Completion Date] del proyecto<br>Propietario del proyecto<br>Lista de tareas que se le han asignado o que se han asignado a una de sus funciones de trabajo o a uno de sus equipos<br><strong>Botón [!UICONTROL See More Details]</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Se activa un proyecto en el que participa mi equipo</strong> <p>Los integrantes de un equipo reciben una notificación por correo electrónico cuando se activa un proyecto. El equipo debe estar asignado al menos a una tarea para recibir la notificación.</p><p>Si a un usuario individual y a un equipo se les asigna una tarea del proyecto, el equipo no recibirá ninguna notificación.</p><p>El asunto del mensaje de correo electrónico de notificación instantánea es <i>&lt;Project Name&gt; [!UICONTROL is Active - Go to your project and see your tasks!]</i></p><p>El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p></td> 
   <td>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Estado del proyecto<br>[!UICONTROL Planned Completion Date] del proyecto <br>Propietario del proyecto<br>Lista de tareas asignadas a su equipo<br><strong>Botón [!UICONTROL See More Details]</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario</td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa un proyecto en el que participo</strong> </p> <p>Los integrantes de un equipo de proyecto reciben una notificación por correo electrónico cuando el estado del proyecto es [!UICONTROL Complete].</p> <p>Sugerencia: Si los proyectos se completan con regularidad, habilitar esta opción puede crear mucho correo electrónico para los usuarios que tienen un número limitado de tareas en muchos proyectos.</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Project Status Change]: &lt;Project Name&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Nombre del usuario que ha completado el proyecto<br>Estado del proyecto<br>Fecha y hora en que se completó el proyecto<br>Estado anterior del proyecto<br><strong>Botón [!UICONTROL See More Details]</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completa una tarea en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo del proyecto reciben una notificación por correo electrónico cuando se completa una tarea en su proyecto. <br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Complete]: &lt;Nombre de la tarea&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> <p>Nota: Si se cambia el estado de la tarea a un estado equivalente a [!UICONTROL Complete], el asunto del correo electrónico seguirá mostrando “[!UICONTROL Complete]”.</p> </p> <p><em>El asunto de la notificación de resumen diario es: [!UICONTROL Digest of Projects You're On] &lt;Fecha del resumen diario&gt; </em> </p> </td> 
   <td> <p>Nombre de tarea<br>Nombre del proyecto<br>Número de referencia de la tarea<br>Nombre del usuario que ha completado la tarea<br>Estado de la tarea<br>Fecha y hora en que se cambió el estado de la tarea<br>Estado de la tarea anterior<br><strong>botón Ver más detalles</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de tareas completadas<br>*Nombre de la tarea<br>*Nombre del usuario que ha completado la tarea<br>*Fecha del resumen diario<br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se añade un problema a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo del proyecto reciben una notificación por correo electrónico cuando se añade un problema al proyecto.</p> <p>Se envía una notificación solo si el estado del proyecto es Actual.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Issue added to] &lt;Nombre del proyecto&gt;</em></p> <p> </p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del problema<br>Nombre del usuario que ha añadido el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos al proyecto<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se resuelve un problema en un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyectos reciben una notificación por correo electrónico cuando se resuelve un problema en su proyecto.<br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL Complete]: &lt;Nombre del problema&gt; en &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del problema<br>Nombre del proyecto<br>Nombre del usuario que ha completado el problema<br>Estado del problema<br>Fecha y hora en que se completó el problema<br>Estado del problema anterior<br><strong>Botón[!UICONTROL See More Details]</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas completados<br>*Nombre del problema<br>*Nombre del usuario asignado al problema<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se añade un problema no asignado a un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyecto reciben una notificación por correo electrónico cuando se añade un problema no asignado al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>¿[!UICONTROL Who should be assigned to this new issue on] &lt;Nombre de proyecto&gt;?</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del problema<br>Nombre del usuario que ha añadido el problema<br>Nombre del problema<br>Tipo de problema<br>Fecha de entrada<br>Prioridad del problema<br>Asignado al nombre (vacío) <br>Estado del problema<br>Contacto principal<br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Número total de problemas añadidos<br>*Nombre del problema<br>*Nombre del usuario que ha añadido el problema<br>*Fecha del resumen diario<br></td> 
   <td> <p><strong>Instantáneo</strong> </p> <p><strong>y diariamente</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me añade a un proyecto</strong> </p> <p>El usuario que se ha añadido al proyecto recibe una notificación por correo electrónico cuando se añade, a menos que el usuario se haya añadido a sí mismo al proyecto.</p> <p>Solo se envía una notificación si el estado del proyecto es [!UICONTROL Current].</p> <p>El asunto del correo electrónico de notificación instantánea es <em>[!UICONTROL You've been added to the project] &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Nombre del usuario que le ha añadido al proyecto<br>[!UICONTROL Planned Start Date] del proyecto<br>[!UICONTROL Planned Completion Date] del proyecto<br>Porcentaje completado del proyecto<br>Nombres de otros usuarios en el proyecto<br>Propietario del proyecto<br><strong>Botón Ver más detalles</strong><br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Fecha del resumen diario</p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cambia el estado de un proyecto en el que participo</strong> </p> <p>Los miembros de un equipo de proyectos reciben una notificación por correo electrónico cuando cambia el estado del proyecto. <br>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>[!UICONTROL Project Status Change]: &lt;Nombre del proyecto&gt;</em></p> <p> El asunto de la notificación de resumen diario es <em> [!UICONTROL Digest of Projects You're On] &lt;Fecha del resumen diario&gt; </em></p> </td> 
   <td> Nombre del proyecto<br>Nombre del portafolio<br>Número de referencia del proyecto<br>Nombre del usuario que ha cambiado el estado del proyecto<br>Nuevo estado del proyecto<br>Fecha y hora en que cambió el estado del proyecto<br>Estado anterior del proyecto<br><strong>Botón [!UICONTROL See More Details]</strong> <br>*Nombre del proyecto<br>*Número de referencia del proyecto<br>*Estado del proyecto<br>*Fecha del resumen diario </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
 </tbody> 
</table>
