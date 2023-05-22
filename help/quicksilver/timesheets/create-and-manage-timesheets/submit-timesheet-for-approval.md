---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar hoja de horas para su aprobación
description: Enviar su hoja de horas para su aprobación le da a su gerente visibilidad de sus horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período de tiempo.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Enviar hoja de horas para su aprobación

Enviar su hoja de horas para su aprobación le da a su gerente visibilidad de sus horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período de tiempo.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver el acceso o superior a Tareas y problemas</p> <p>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores en tareas y problemas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Enviar hoja de horas para su aprobación

* [Enviar hoja de horas para su aprobación](#submit-a-timesheet-for-approval)
* [Ver el estado de una hoja de horas enviada](#view-the-status-of-a-submitted-timesheet)

### Enviar hoja de horas para su aprobación

Después de establecer un aprobador de hoja de horas (como se describe en la sección ). [Designar aprobadores de hojas de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) en el artículo [Aprobar una hoja de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), el **Cerrar** botón situado en la parte inferior de la plantilla de horas cambia a **Enviar para aprobación** botón.

Para enviar una hoja de horas para su aprobación:

1. Vaya a una hoja de horas configurada para tener un aprobador.
1. Registrar tiempo, tal como se describe en [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Clic **Enviar para aprobación** para iniciar el proceso de aprobación de plantillas de horas.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   El **Enviar para aprobación** se reemplaza por el botón **Aprobar**, **Rechazar**, y **Recordar** botones. El estado de la plantilla de horas cambia a **Enviado**.

   Cuando la plantilla de horas se envía para su aprobación, el aprobador la ve enumerada en la **Aprobaciones** en el área **Inicio** página. Pueden ocurrir lo siguiente:

   * Si lo aprueban, el **Recordar** el botón cambia a **Volver a abrir** y el estado de la plantilla de horas se actualiza a **Abrir**.
   * Si lo rechazan, el **Enviar para aprobación** reemplaza el botón de **Recordar** y el estado de la plantilla de horas se actualiza a **Rechazado**.

1. (Opcional) Haga clic en **Recordar** si necesita volver a abrir la plantilla de horas y actualizar la hora. Para obtener más información, consulte [Recuperar una hoja de horas](#recall-a-timesheet) de este artículo.

### Ver el estado de una hoja de horas enviada {#view-the-status-of-a-submitted-timesheet}

Puede ver el estado de una plantilla de horas después de enviarla.

Si el administrador de Workfront ha habilitado la Aprobación de plantilla de horas para el usuario y el Rechazo de plantilla de horas para los controladores de eventos del usuario, se le notificará una vez aprobada o rechazada la plantilla de horas. Para obtener información sobre la activación de notificaciones de eventos, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sin estas notificaciones, puede obtener más información sobre el estado de las hojas de horas enviadas en el área Hoja de horas de Workfront.

Para ver el estado de una plantilla de horas:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Clic **Plantillas de horas**. El **Todo** El filtro está seleccionado de forma predeterminada.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccionar **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solo las plantillas de horas que apruebe

      O

      Seleccionar **Mis hojas de horas** para ver únicamente las hojas de horas.

      Esto aplica los filtros Mis aprobaciones de hojas de horas o Mis hojas de horas a la lista de hojas de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Creación o edición de filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado los filtros Mis aprobaciones de hojas de horas y Mis hojas de horas de los controles de Lista en el área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   >
   >   
   >   
   >   * [Personalización de filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Condicional) Si ha seleccionado **Mis hojas de horas**, asegúrese de que las variables **Standard** se aplique la vista y observe el **Estado** columna.

   Las plantillas de horas pueden tener los siguientes estados:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abrir</td> 
      <td> <p>Su hoja de horas está abierta actualmente y puede registrar las horas. </p> <p>Aparece una hoja de horas recuperada con el estado Abierto. Para obtener más información, consulte <a href="#recall-a-timesheet" class="MCXref xref">Recuperar una hoja de horas</a> de este artículo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviado</td> 
      <td>Ha enviado su hoja de horas para su aprobación, pero aún no se ha aprobado. Puede recuperar una hoja de horas enviada para seguir editándola. Para obtener más información, consulte <a href="#recall-a-timesheet" class="MCXref xref">Recuperar una hoja de horas</a> de este artículo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerrado</td> 
      <td> <p>Existen los siguientes escenarios:</p> 
       <ul> 
        <li> <p>Si la plantilla de horas no tiene aprobador, ha guardado el tiempo y lo ha cerrado.</p> </li> 
        <li> <p>Si la hoja de horas tiene un aprobador, la ha enviado para su aprobación y se ha aprobado.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechazado</td> 
      <td>Ha enviado la hoja de horas para su aprobación y el aprobador la ha rechazado.</td> 
     </tr> 
    </tbody> 
   </table>

## Recuperar una hoja de horas {#recall-a-timesheet}

Puede recuperar una hoja de horas que ya se haya enviado para su aprobación. Solo se pueden recuperar las hojas de horas que no se hayan aprobado.

Para recuperar una hoja de horas:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Clic **Plantillas de horas**.
1. Clic **Mis hojas de horas** en la esquina superior derecha de la pantalla o seleccione **Mis hojas de horas** desde el **Filtrar** ![](assets/filter-nwepng.png) menú desplegable.
1. Haga clic en el lapso de tiempo de una hoja de horas con un estado de **Enviado**.
1. Clic **Recordar**.

   La plantilla de horas vuelve a poder editarse y su estado cambia a **Abrir**.
