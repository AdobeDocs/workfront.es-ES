---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar un parte de horas para su aprobación
description: El envío del parte de horas para su aprobación proporciona al administrador visibilidad sobre las horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas durante el período de tiempo.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Enviar un parte de horas para su aprobación

El envío del parte de horas para su aprobación proporciona al administrador visibilidad sobre las horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas durante el período de tiempo.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a Tareas y problemas</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores en tareas y problemas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Enviar un parte de horas para su aprobación

* [Enviar un parte de horas para su aprobación](#submit-a-timesheet-for-approval)
* [Ver el estado de un parte de horas enviado](#view-the-status-of-a-submitted-timesheet)

### Enviar un parte de horas para su aprobación

Después de configurar un aprobador de parte de horas (como se describe en la sección [Designar aprobadores de hojas de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) en el artículo [Aprobar un parte de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), el **Cerrar** en la parte inferior del parte de horas cambia a **Enviar para aprobación** botón.

Para enviar un parte de horas para su aprobación:

1. Vaya a un parte de horas configurado para tener un aprobador.
1. Tiempo de registro, tal como se describe en [Tiempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Haga clic en **Enviar para aprobación** para iniciar el proceso de aprobación del parte de horas.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   La variable **Enviar para aprobación** se reemplaza por la función **Aprobar**, **Rechazar** y **Recordar** botones. El estado del parte de horas cambia a **Enviado**.

   Cuando se envía el parte de horas para su aprobación, el aprobador ve el parte de horas enumerado en la **Aprobaciones** en el **Página principal** página. Puede ocurrir lo siguiente:

   * Si lo aprueban, la variable **Recordar** cambia a **Volver a abrir** y el estado del parte de horas se actualiza a **Apertura**.
   * Si lo rechazan, la variable **Enviar para aprobación** reemplaza a la función **Recordar** y el estado del parte de horas se actualiza a **Rechazado**.

1. (Opcional) Haga clic en **Recordar** si necesita volver a abrir el parte de horas y actualizar su hora. Para obtener más información, consulte la [Recuperar un parte de horas](#recall-a-timesheet) en este artículo.

### Ver el estado de un parte de horas enviado {#view-the-status-of-a-submitted-timesheet}

Puede ver el estado de un parte de horas después de enviarlo.

Si el administrador de Workfront ha habilitado la aprobación de parte de horas para el usuario y el rechazo de parte de horas para los controladores de eventos de usuario, se le notifica después de aprobar o rechazar el parte de horas. Para obtener información sobre cómo activar las notificaciones de eventos, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sin estas notificaciones, puede obtener información sobre el estado de las hojas de horas enviadas en el área Hoja de horas de Workfront.

Para ver el estado de un parte de horas:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Hojas de tiempo**. La variable **Todo** está seleccionado de forma predeterminada.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de partes de horas:

   * Select **Aprobaciones de Mi parte de horas** en la esquina superior derecha de la página para ver solo las partes de horas que aprueba

      O

      Select **Mis hojas de hora** para ver solo sus partes de horas.

      Esto aplica los filtros Mis aprobaciones de parte de horas o Mi parte de horas a la lista de partes de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de parte de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo han eliminado los filtros Mis aprobaciones de parte de horas y Mis hojas de horas de los controles de lista del área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   >
   >   
   >   
   >   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Condicional) Si ha seleccionado **Mis hojas de hora**, asegúrese de que **Estándar** se aplica la vista y observe la **Estado** para abrir el Navegador.

   Las hojas de tiempo pueden tener los siguientes estados:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abrir</td> 
      <td> <p>El parte de horas está abierto y es posible que registre la hora. </p> <p>Se muestra un parte de horas recuperada con el estado Abrir. Para obtener más información, consulte la <a href="#recall-a-timesheet" class="MCXref xref">Recuperar un parte de horas</a> en este artículo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviado</td> 
      <td>Ha enviado el parte de horas para su aprobación, pero aún no se ha aprobado. Puede recordar un parte de horas enviado para seguir editándolo. Para obtener más información, consulte la <a href="#recall-a-timesheet" class="MCXref xref">Recuperar un parte de horas</a> en este artículo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerrado</td> 
      <td> <p>Existen los siguientes escenarios:</p> 
       <ul> 
        <li> <p>Si el parte de horas no tiene aprobador, guardó el tiempo y lo cerró.</p> </li> 
        <li> <p>Si el parte de horas tiene un aprobador, lo ha enviado para su aprobación y se ha aprobado.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechazado</td> 
      <td>Ha enviado el parte de horas para su aprobación y el aprobador lo ha rechazado.</td> 
     </tr> 
    </tbody> 
   </table>

## Recuperar un parte de horas {#recall-a-timesheet}

Puede recordar un parte de horas que ya se ha enviado para aprobación. Solo se pueden recuperar las partes de horas que no se hayan aprobado.

Para recuperar un parte de horas:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Hojas de tiempo**.
1. Haga clic en **Mis hojas de hora** en la esquina superior derecha de la pantalla o seleccione **Mis hojas de hora** de la variable **Filtro** ![](assets/filter-nwepng.png) menú desplegable.
1. Haga clic en el lapso de tiempo de un parte de horas con un estado de **Enviado**.
1. Haga clic en **Recordar**.

   El parte de horas se vuelve editable de nuevo y su estado cambia a **Apertura**.
