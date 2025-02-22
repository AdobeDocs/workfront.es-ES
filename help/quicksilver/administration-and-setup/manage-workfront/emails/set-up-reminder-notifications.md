---
title: Configuración de notificaciones de recordatorio
description: Las notificaciones de recordatorio generan correos electrónicos que se envían a los usuarios en función de criterios específicos. Las notificaciones de recordatorio recuerdan a los usuarios de una acción que deben realizar para una tarea, un problema, un proyecto o una hoja de horas.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1232'
ht-degree: 7%

---

# Configurar notificaciones de recordatorio

<!-- Audited: 1/2024 -->

Como administrador de Workfront, puede crear notificaciones de recordatorio para los usuarios y asociarlos a objetos a los que desee que presten especial atención.

Las notificaciones de recordatorio generan correos electrónicos que se envían a los usuarios en función de criterios específicos. Las notificaciones de recordatorio recuerdan a los usuarios de una acción que deben realizar para una tarea, un problema, un proyecto o una hoja de horas.

Después de crear las notificaciones de recordatorio, los usuarios pueden asociarlas manualmente a elementos de trabajo, como proyectos, tareas, problemas y plantillas de horas. Para obtener más información, vea [Adjuntar una notificación de aviso a un objeto](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar </p>
 <p>o</p> 
<p>Actual: plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Planificador o superior, con acceso administrativo a las notificaciones de recordatorio</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar el correo electrónico del recordatorio

Puede personalizar el asunto, el cuerpo y el HTML en el correo electrónico de notificación de recordatorio.

O bien, puede utilizar el correo electrónico predeterminado incluido con la notificación de recordatorio. El correo electrónico predeterminado utiliza el nombre de la notificación de recordatorio como asunto del correo electrónico y el nombre del objeto en el cuerpo del correo electrónico, incluido el evento que activó la notificación.

Si desea personalizar el correo electrónico del recordatorio, debe crear una plantilla de correo electrónico y adjuntarla a la notificación del recordatorio.

Para obtener información sobre cómo crear una plantilla de correo electrónico, consulte [Configurar plantillas de correo electrónico](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Crear una notificación de recordatorio

{{step-1-to-setup}}

1. Haga clic en **Correo electrónico** > **Notificaciones** > **Notificaciones de recordatorio**.

   ![Ficha Notificaciones de recordatorio](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Haga clic en **Nueva notificación de recordatorio**.

1. En la lista desplegable, haga clic en el tipo de objeto que desee asociar a la notificación de recordatorio.

   Por ejemplo, si desea adjuntar una notificación de recordatorio a una hoja de horas, haga clic en **Hoja de horas**.

1. En el cuadro **Nueva notificación de recordatorio** que aparece, especifique la siguiente información.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de la notificación de recordatorio</td> 
      <td>Especifique un nombre para la notificación de recordatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Período de calificación</td> 
      <td> <p>Especifique el número de horas, días laborables, días (días del calendario), semanas o meses antes o después de la fecha en el campo <strong>Intervalos</strong>.</p> <p><b>NOTA</b>:  
        <ul> 
         <li> <p>Las notificaciones de recordatorio comienzan 24 horas después de la fecha especificada y una vez que se cumplen todos los criterios.</p> </li> 
         <li> <p>Notificaciones de recordatorio para proyectos, tareas y problemas déclencheur todas las noches a medianoche, hora de la montaña de EE. UU. Todos los objetos que cumplen los requisitos para recibir una notificación de recordatorio a partir de ese día déclencheur una notificación a los usuarios designados poco después de esa hora.</p> </li> 
         <li> <p>Las notificaciones de recordatorio para las hojas de horas se envían a la hora especificada en función de su zona horaria y de la fecha de finalización, fecha de inicio o fecha de última actualización de la hoja de horas.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intervalo</td> 
      <td> <p>Seleccione el evento que almacena en déclencheur la notificación de recordatorio que se va a programar.</p> <p>Si la notificación de recordatorio está destinada a proyectos, tareas o problemas, las opciones disponibles están relacionadas con la Fecha de finalización o Fecha de inicio. La notificación de recordatorio tiene en cuenta la marca de tiempo de las fechas de finalización y de inicio de los proyectos, las tareas y los problemas.</p>

   <p>Si la notificación de recordatorio está destinada a hojas de horas, las opciones disponibles están relacionadas con la fecha de finalización, la fecha de inicio o la fecha de última actualización. La notificación de recordatorio para las plantillas de horas tiene en cuenta la marca de tiempo de las fechas de finalización, inicio y última actualización de la plantilla de horas. La plantilla de horas comienza a medianoche del día de la fecha de inicio (12:00 a.m.) y finaliza justo antes de la medianoche de la fecha de finalización (11:59 p.m.).</p>

   <p><b>NOTA</b></p>
      <p>Las notificaciones de recordatorio de hoja de horas solo se distribuyen una vez cada 24 horas.</p> <p>Cuando configura varias notificaciones de recordatorio en un periodo de 24 horas, Workfront envía un correo electrónico de notificación con todos los recordatorios incluidos en esa notificación.</p>
      <p>Por ejemplo, si configura tres notificaciones de recordatorio para que se almacenen en déclencheur 10 horas antes, 2 horas antes y 1 hora antes de una fecha de vencimiento, los tres recordatorios se combinarán en la misma notificación si se producen durante el mismo día.</p> <p>Sin embargo, si establece una notificación de recordatorio para 26 horas antes y otra para 1 hora antes de una fecha de vencimiento, los usuarios recibirán dos notificaciones independientes. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criterios</td> 
      <td> <p>Seleccione los criterios para calificar la notificación de recordatorio para que se programe. Las notificaciones de recordatorio no están programadas a menos que se cumpla la selección de criterios.</p> <p>Las siguientes opciones de criterios están disponibles, según el tipo de objeto seleccionado en el paso 4:</p> 
       <ul> 
        <li><strong>Incompleto en proyectos actuales:</strong> <i>(disponible para recordatorios de tareas y problemas)</i> La notificación de recordatorio está programada para enviarse solamente cuando el estado del objeto con el que está asociada la notificación de recordatorio no es Completo y el estado del proyecto es Actual.</li> 
        <li><strong>Todo en proyectos actuales:</strong> <i>(disponible para recordatorios de tareas y problemas)</i> La notificación de recordatorio está programada para enviarse independientemente del estado del objeto y solo cuando el estado del proyecto con el que está asociada la notificación de recordatorio es Actual.</li> 
        <li><strong>Proyectos incompletos:</strong> <i>(disponible para recordatorios de proyectos)</i> La notificación de recordatorio está programada para enviarse cuando el estado del proyecto sea cualquier cosa menos Completado.</li> 
        <li><strong>Todos los proyectos:</strong> <i>(disponible para recordatorios de proyectos)</i> La notificación de recordatorio está programada para enviarse independientemente del estado del proyecto.</li> 
        <li><strong>Abrir hojas de horas:</strong> <i>(disponible para recordatorios de hojas de horas)</i> Se ha programado el envío de la notificación de recordatorio cuando el estado de la hoja de horas sea Abierto.</li> 
        <li><strong>Hojas de horas enviadas:</strong> <i>(disponible para recordatorios de hojas de horas)</i> La notificación de recordatorio está programada para enviarse cuando se envíe el estado de la hoja de horas.</li> 
        <li><strong>Abrir hoja de horas o menos de 40 horas a la semana:</strong> <i>(disponible para recordatorios de hojas de horas)</i> La notificación de recordatorio está programada para enviarse cuando el estado de la hoja de horas es Abierta o cuando la hoja de horas tiene menos de 40 horas registradas.</li> 
        <li><strong>Plantilla de correo electrónico:</strong> En la lista desplegable, seleccione una plantilla de correo electrónico para adjuntarla al recordatorio.<br>Para obtener información sobre cómo generar una plantilla de correo electrónico, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurar plantillas de correo electrónico</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinatarios</td> 
      <td><p>Según el objeto para el que sea la notificación de recordatorio, seleccione entre los siguientes tipos de usuarios que desea que reciban la notificación:</p>
      <ul>
      <li>Asignado a</li>
      <li>Introducido por</li>
      <li>Equipo del proyecto (todos los usuarios del equipo del proyecto reciben el recordatorio)</li>
      <li>Usuarios asignados a tareas dependientes (los usuarios asignados a tareas dependientes reciben el recordatorio)</li>
      <li>Propietario del proyecto</li>
      <li>Asignado a (los usuarios asignados a una tarea o a un problema reciben el recordatorio)</li>
      <li>Propietario de hoja de horas</li>
      <li>Aprobador de hoja de horas</li>
      <li>Gerente de propietario de hoja de horas</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
1. Adjuntar la notificación de recordatorio a un elemento de trabajo, como se describe en [Adjuntar una notificación de recordatorio a un objeto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Recibir una notificación de recordatorio

Cuando se cumple la condición en el elemento que tiene adjunta la notificación de recordatorio, se activa una notificación por correo electrónico al usuario definido en la notificación de recordatorio.

Para obtener más información sobre cómo recibir notificaciones de recordatorio, consulte la sección [Notificaciones de recordatorio](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) en [Notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Envío de notificación de recordatorio de prueba

Déclencheur de notificaciones de recordatorio todas las noches a medianoche, hora de la montaña. Todos los objetos que cumplen los requisitos para una notificación de recordatorio almacenan en déclencheur una notificación a los usuarios designados poco después de esa fecha.

Para que las notificaciones de recordatorio entren en déclencheur manualmente, primero debe cumplirse la condición del recordatorio.\
Por ejemplo, si un recordatorio se establece en déclencheur una hora después de la fecha planificada de finalización de un proyecto, ese tiempo debe haber pasado entre el momento en que se estableció el recordatorio y ahora. Los proyectos en los que se haya aprobado la fecha planificada de finalización antes de activar el recordatorio no almacenarán en déclencheur notificaciones.

Para que una notificación de recordatorio se almacene en déclencheur manualmente:

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Diagnóstico** en la esquina inferior izquierda de Workfront.

1. Haga clic en **Enviar notificaciones de recordatorio** y espere a que se confirme en la parte superior de la pantalla que se han enviado.

   Los usuarios designados en la notificación de recordatorio recibirán un correo electrónico.

![Prueba de notificación de recordatorio](assets/reminder-test.png)
