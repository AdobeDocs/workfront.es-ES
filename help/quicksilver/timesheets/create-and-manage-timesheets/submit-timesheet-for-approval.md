---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enviar hoja de horas para su aprobación
description: Enviar su hoja de horas para su aprobación le da a su gerente visibilidad de sus horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período de tiempo.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
TQID: https://experienceleague.adobe.com/uxfkWowkcyC9zeX1vNaZaY-i3AFCHMngvflZ8-REnac
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 20%
---
# Enviar plantilla de horas para su aprobación

<!--Audited: 8/2024-->

Enviar su hoja de horas para su aprobación le da a su gerente visibilidad de sus horas de trabajo. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período de tiempo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
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

## Enviar plantilla de horas para su aprobación

* [Enviar plantilla de horas para su aprobación](#submit-a-timesheet-for-approval)
* [Ver el estado de una hoja de horas enviada](#view-the-status-of-a-submitted-timesheet)

### Enviar plantilla de horas para su aprobación

Después de establecer un aprobador de hoja de horas (como se describe en la sección [Designar aprobadores de hoja de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) del artículo [Aprobar una hoja de horas](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), el botón **Cerrar** de la parte inferior de la hoja de horas cambia a un botón **Enviar para aprobación**.

Para enviar una hoja de horas para su aprobación:

1. Vaya a una hoja de horas configurada para tener un aprobador.
1. Registrar tiempo, como se describe en [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Haga clic en **Enviar para aprobación** para iniciar el proceso de aprobación de hojas de horas.

   ![Botón Enviar para aprobación](assets/submit-for-approval-button-on-timesheet.png)

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

{{step1-to-timesheets}}

De forma predeterminada, se muestran todas las hojas de horas a las que tiene acceso para ver.

![Lista de hojas de horas](assets/list-of-all-timesheets.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solamente las hojas de horas que usted apruebe,

     O

     Seleccione **Mis plantillas de horas** para ver solamente sus plantillas de horas.

     Esto aplica los filtros **Mis aprobaciones de hojas de horas** o **Mi hoja de horas** a la lista de hojas de horas.

   * Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png) para aplicar un filtro o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado esos filtros de los controles de lista en el área de Configuración o de la plantilla de diseño. Para obtener más información, consulte [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condicional) Si seleccionó **Mis hojas de horas**, asegúrese de que se aplique la vista **Estándar** y observe la columna **Estado**.

   Las plantillas de horas pueden tener los siguientes estados:

   | Estado | Descripción |
   | --------- | ---------- |
   | Abrir | <p>Su hoja de horas está abierta actualmente y puede registrar las horas.</p><p>Aparece una hoja de horas recuperada con el estado Abierto. Para obtener más información, consulte la sección [Recuperar una hoja de horas](#recall-a-timesheet) en este artículo.</p> |
   | Enviado | Ha enviado su hoja de horas para su aprobación, pero aún no se ha aprobado. Puede recuperar una hoja de horas enviada para seguir editándola. Para obtener más información, consulte la sección [Recuperar una hoja de horas](#recall-a-timesheet) en este artículo. |
   | Cerrado | <p>Se dan los siguientes escenarios:</p><ul><li>Si la plantilla de horas no tiene aprobador, ha guardado el tiempo y lo ha cerrado.</li><li>Si la hoja de horas tiene un aprobador, la ha enviado para su aprobación y se ha aprobado.</li></ul> |
   | Rechazado | Ha enviado la hoja de horas para su aprobación y el aprobador la ha rechazado. |

## Recuperar una hoja de horas {#recall-a-timesheet}

Puede recuperar una hoja de horas que ya se haya enviado para su aprobación. Solo se pueden recuperar las hojas de horas que no se hayan aprobado.

Para recuperar una hoja de horas:

{{step1-to-timesheets}}

1. Haga clic en **Mis hojas de horas** en la esquina superior derecha de la pantalla, o bien seleccione **Mis hojas de horas** del menú desplegable **Filtrar** ![Icono de filtro](assets/filter-nwepng.png).
1. Haga clic en el lapso de tiempo de una hoja de horas con un estado de **Enviado**.
1. Haga clic en **Recuperar**.

   La hoja de horas vuelve a poder editarse y su estado cambia a **Abrir**.
