---
title: Configuración de notificaciones de recordatorio
description: Configuración de notificaciones de recordatorio
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 1%

---

# Configuración de notificaciones de recordatorio

Las notificaciones del recordatorio envían correos electrónicos a los destinatarios según los criterios especificados. Como administrador de Adobe Workfront o usuario con un nivel de acceso de Planificador y acceso administrativo a las notificaciones de recordatorio, puede asociar manualmente las notificaciones de recordatorio con los elementos de trabajo, como proyectos, tareas, problemas y hojas de tiempo.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Planificador o superior, con acceso administrativo a las notificaciones de recordatorio</p> <p>Para obtener información sobre cómo conceder acceso administrativo a un usuario del Plan, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Personalización del correo electrónico del recordatorio

Puede personalizar la notificación del recordatorio con un correo electrónico personalizado que incluya un asunto y un cuerpo de correo electrónico personalizados. El cuerpo del correo electrónico puede contener un HTML personalizado.

O bien, puede utilizar el correo electrónico predeterminado incluido con la notificación del recordatorio. El correo electrónico predeterminado utiliza el nombre de notificación del recordatorio como asunto del correo electrónico y el nombre del objeto en el cuerpo del correo electrónico, incluido el evento que activó la notificación.

Si desea personalizar el correo electrónico recordatorio, debe crear una plantilla de correo electrónico y adjuntarla a la notificación del recordatorio.

Para obtener información sobre cómo crear una plantilla de correo electrónico, consulte [Configuración de plantillas de correo electrónico](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Creación de una notificación de recordatorio

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Correo electrónico** > **Notificaciones**.

1. Haga clic en el **Notificaciones de recordatorio** a continuación, haga clic en **Nueva notificación de recordatorio**.

1. En la lista desplegable, haga clic en el tipo de objeto que desee asociar a la notificación de recordatorio.

   Por ejemplo, si desea adjuntar una notificación de recordatorio a un parte de horas, haga clic en **Hoja de horas**.

1. En el **Nueva notificación de recordatorio** que aparece, especifique la siguiente información.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de la notificación de recordatorio</td> 
      <td>Especifique un nombre para la notificación del recordatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Período de calificación</td> 
      <td> <p>Especifique el número de horas, días laborables, días (días del calendario), semanas o meses antes o después de la fecha en la variable <strong>Temporización</strong> campo .</p> <p><b>NOTA</b>:  
        <ul> 
         <li> <p>Las notificaciones de recordatorio comienzan 24 horas después de la fecha especificada y una vez que se cumplen todos los criterios.</p> </li> 
         <li> <p>Avisos para proyectos, tareas y déclencheur de emisiones todas las noches a la medianoche, hora de las montañas de EE. UU. Todos los objetos que cumplen los requisitos para recibir un recordatorio a partir de ese día déclencheur una notificación a los usuarios designados poco después de esa hora.</p> </li> 
         <li> <p>Las notificaciones de recordatorio para hojas de horas se envían a la hora especificada en función de la zona horaria y la fecha de finalización, la fecha de inicio o la fecha de última actualización del parte de horas.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intervalo</td> 
      <td> <p>Seleccione el evento que déclencheur la notificación de recordatorio a programarse.</p> <p>Si la notificación del recordatorio está pensada para proyectos, tareas o problemas, las opciones disponibles están relacionadas con la fecha de finalización o la fecha de inicio. La notificación del recordatorio tiene en cuenta la marca de tiempo de las fechas de finalización e inicio de los proyectos, tareas y problemas.</p> <p>Si la notificación del recordatorio está pensada para partes de horas, las opciones disponibles están relacionadas con la fecha de finalización, la fecha de inicio o la fecha de última actualización. La notificación de recordatorio para Hojas de horas tiene en cuenta la marca de tiempo de las fechas de finalización, inicio y última actualización del parte de horas. El parte de horas comienza a medianoche del día de la fecha de inicio (12:00 AM) y finaliza justo antes de la medianoche en la fecha de finalización (23:59 PM).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criterios</td> 
      <td> <p>Seleccione los criterios para calificar la notificación de recordatorio que se va a programar. Las notificaciones de recordatorio no están programadas a menos que se cumpla la selección de criterios.</p> <p>Las siguientes opciones de criterios están disponibles, según el tipo de objeto seleccionado en el paso 4:</p> 
       <ul> 
        <li><strong>Incompleto en proyectos actuales:</strong> (Disponible para recordatorios de problemas y tareas) La notificación del recordatorio está programada para enviarse solo cuando el estado del objeto con el que está asociada la notificación del recordatorio no ha finalizado y el estado del proyecto es Actual.</li> 
        <li><strong>Todo en proyectos actuales:</strong>(Disponible para recordatorios de problemas y tareas) La notificación del recordatorio está programada para enviarse independientemente del estado del objeto y solo cuando el estado del proyecto con el que está asociada la notificación del recordatorio es Actual.</li> 
        <li><strong>Proyectos incompletos:</strong> (Disponible para recordatorios de proyecto) La notificación del recordatorio está programada para enviarse cuando el estado del proyecto es cualquier cosa menos Completado.</li> 
        <li><strong>Proyectos completos:</strong> (Disponible para recordatorios de proyecto) La notificación del recordatorio está programada para enviarse cuando se complete el estado del proyecto.</li> 
        <li><strong>Abrir partes de horas:</strong> (Disponible para recordatorios de parte de horas) La notificación del recordatorio está programada para enviarse cuando el estado del parte de horas es Abierta.</li> 
        <li><strong>Hojas de horas enviadas:</strong> (Disponible para recordatorios de parte de horas) La notificación del recordatorio está programada para enviarse cuando se envía el estado del parte de horas.</li> 
        <li><strong>Abrir parte de horas o menos de 40 horas por semana:</strong> (Disponible para recordatorios de parte de horas) La notificación del recordatorio está programada para enviarse cuando el estado del parte de horas es Open o cuando el parte de horas tiene menos de 40 horas registradas.</li> 
        <li><strong>Plantilla de correo electrónico:</strong> En la lista desplegable , seleccione una plantilla de correo electrónico para adjuntarla al recordatorio.<br>Para obtener información sobre cómo crear una plantilla de correo electrónico, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configuración de plantillas de correo electrónico</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinatarios</td> 
      <td>Seleccione los tipos de usuarios que desea que reciban la notificación. Seleccione entre varias partes interesadas del objeto, como propietario, aprobador o usuario asignado.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
1. Adjuntar la notificación del recordatorio a un elemento de trabajo, tal como se describe en [Adjuntar una notificación recordatoria a un objeto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Recibir una notificación de recordatorio

Cuando se cumple la condición en el elemento que tiene adjunta la notificación de recordatorio, se activa una notificación por correo electrónico para el usuario definido en la notificación de recordatorio.

Para obtener más información sobre la recepción de notificaciones de recordatorio, consulte la [Notificaciones recordatorias](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) en [Notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Envío de notificaciones de recordatorio de prueba

Aviso déclencheur todas las noches a medianoche, hora de montaña. Todos los objetos que cumplen los requisitos para una notificación recordatoria déclencheur una notificación a los usuarios designados poco después.

Para que las notificaciones de recordatorio se déclencheur manualmente, primero debe cumplirse la condición para el recordatorio.\
Por ejemplo, si se establece un recordatorio en déclencheur una hora después de la fecha de finalización planeada de un proyecto, ese tiempo debe haber transcurrido entre el momento en que se configuró el recordatorio y ahora. Los proyectos que hayan pasado fechas de finalización previstas antes de que se activara el recordatorio no se déclencheur una notificación.

Para hacer que una notificación recordatoria se déclencheur manualmente:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Diagnóstico** en la esquina inferior izquierda de Workfront.

1. Haga clic en **Enviar notificaciones de recordatorio** y espere a que se confirme en la parte superior de la pantalla que se han enviado.

   Los usuarios designados en la notificación recordatoria reciben un correo electrónico.
