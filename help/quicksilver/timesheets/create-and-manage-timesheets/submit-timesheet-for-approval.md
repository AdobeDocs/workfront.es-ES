---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar hoja de horas para su aprobación
description: Enviar su hoja de horas para su aprobación le da a su gerente visibilidad de sus horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período de tiempo.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 33%

---

# Enviar hoja de horas para su aprobación

<!--Audited: 8/2024-->

Enviar su hoja de horas para su aprobación le da a su gerente visibilidad de sus horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período de tiempo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Ligero o superior </p>
   <p>Revisión o superior </p>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a tareas y problemas </p> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Ver los permisos o superiores de la plantilla de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enviar hoja de horas para su aprobación

* [Enviar plantilla de horas para su aprobación](#submit-a-timesheet-for-approval)
* [Ver el estado de una hoja de horas enviada](#view-the-status-of-a-submitted-timesheet)

### Enviar hoja de horas para su aprobación

Después de establecer un aprobador de hoja de horas (como se describe en la sección [Designar aprobadores de hoja de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) del artículo [Aprobar una hoja de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), el botón **Cerrar** de la parte inferior de la hoja de horas cambia a un botón **Enviar para aprobación**.

Para enviar una hoja de horas para su aprobación:

1. Vaya a una hoja de horas configurada para tener un aprobador.
1. Registrar tiempo, como se describe en [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Haga clic en **Enviar para aprobación** para iniciar el proceso de aprobación de hojas de horas.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   El botón **Enviar para aprobación** se ha reemplazado por los botones **Aprobar**, **Rechazar** y **Recuperar**. El estado de la hoja de horas cambia a **Enviado**.

   Cuando la hoja de horas se envía para su aprobación, el aprobador la ve en la hoja de horas enumerada en el widget **Mis aprobaciones** del área **Inicio**. Pueden ocurrir lo siguiente:

   * Si lo aprueban, el botón **Recuperar** cambia a **Volver a abrir** y el estado de la hoja de horas se actualiza a **Abrir**.
   * Si lo rechazan, el botón **Enviar para aprobación** reemplaza el botón **Recuperar** y el estado de la hoja de horas se actualiza a **Rechazado**.

1. (Opcional) Haga clic en **Recuperar** si necesita volver a abrir la hoja de horas y actualizar la hora. Para obtener más información, consulte la sección [Recuperar una hoja de horas](#recall-a-timesheet) en este artículo.

### Ver el estado de una hoja de horas enviada {#view-the-status-of-a-submitted-timesheet}

Puede ver el estado de una plantilla de horas después de enviarla.

Si el administrador de Workfront ha habilitado la Aprobación de plantilla de horas para el usuario y el Rechazo de plantilla de horas para los controladores de eventos del usuario, se le notificará una vez aprobada o rechazada la plantilla de horas. Para obtener información acerca de cómo habilitar las notificaciones de eventos, vea [Tipos de notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sin estas notificaciones, puede obtener más información sobre el estado de las hojas de horas enviadas en el área Hoja de horas de Workfront.

Para ver el estado de una plantilla de horas:

1. Haga clic en el icono de **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Plantilla de horas**. El filtro **Todos** está seleccionado de manera predeterminada.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Aprobaciones de Mis plantillas de horas** en la esquina superior derecha de la página para ver solamente las plantillas de horas que usted apruebe

     O

     Seleccione **Mis plantillas de horas** para ver solamente sus plantillas de horas.

     Esto es válido para los filtros Aprobaciones de Mis hojas de horas o de Mis hojas de horas a la lista de hojas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono de Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Aprobaciones de Mis hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si su administrador de Workfront o su administrador de grupos ha eliminado los filtros Aprobaciones de Mis hojas de horas y Mis hojas de horas de Controles de Lista en el área Configuración o de la Plantilla de diseño. Para obtener más información, consulte los siguientes artículos:
   >
   >   
   >   
   >   * [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Condicional) Si seleccionó **Mis hojas de horas**, asegúrese de que se aplique la vista **Estándar** y observe la columna **Estado**.

   Las plantillas de horas pueden tener los siguientes estados:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abrir</td> 
      <td> <p>Su hoja de horas está abierta actualmente y puede registrar las horas. </p> <p>Aparece una hoja de horas recuperada con el estado Abierto. Para obtener más información, consulte la sección <a href="#recall-a-timesheet" class="MCXref xref">Recuperar una hoja de horas</a> en este artículo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviado</td> 
      <td>Ha enviado su hoja de horas para su aprobación, pero aún no se ha aprobado. Puede recuperar una hoja de horas enviada para seguir editándola. Para obtener más información, consulte la sección <a href="#recall-a-timesheet" class="MCXref xref">Recuperar una hoja de horas</a> en este artículo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerrado</td> 
      <td> <p>Se dan los siguientes escenarios:</p> 
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

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Plantillas de horas**.
1. Haga clic en **Mis hojas de horas** en la esquina superior derecha de la pantalla o seleccione **Mis hojas de horas** del menú desplegable **Filtrar** ![](assets/filter-nwepng.png).
1. Haga clic en el lapso de tiempo de una hoja de horas con un estado de **Enviado**.
1. Haga clic en **Recuperar**.

   La hoja de horas vuelve a poder editarse y su estado cambia a **Abrir**.
