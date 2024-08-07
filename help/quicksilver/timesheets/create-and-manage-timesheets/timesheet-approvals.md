---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Aprobar una hoja de horas
description: El proceso de aprobación de hojas de horas proporciona a los administradores visibilidad sobre las horas de trabajo de sus informes directos. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Aprobar una hoja de horas

<!--Audited: 8/2024-->

El proceso de aprobación de hojas de horas proporciona a los administradores visibilidad sobre las horas de trabajo de sus informes directos. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período.

Adobe Workfront permite configurar las aprobaciones de plantillas de horas para que sean compatibles en esta área.

Para obtener información sobre cómo enviar una hoja de horas, consulte [Enviar una hoja de horas para su aprobación](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>plan de Adobe Workfront</p></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td> <p>Nuevo: estándar</p>
   <p>Actual: plan </p> 
   <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a hojas de horas y horas </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Designar aprobadores de hojas de horas

Normalmente, los administradores funcionales o el personal de recursos humanos aprueban las hojas de horas. Los jefes de proyecto no suelen aprobar las hojas de horas. Los jefes de proyecto pueden aprobar los proyectos con registro de tiempo, pero los jefes de equipo o de recursos humanos deben aprobar las plantillas de horas.

Se define un aprobador de hoja de horas al crear el perfil de hoja de horas. Debe contar con una licencia de planificación para ser designado como aprobador.

Para obtener más información sobre cómo designar aprobadores de hojas de horas, consulte la sección [Crear o editar un perfil de hoja de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) en el artículo [Crear, editar y asignar perfiles de hoja de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Aprobar una hoja de horas

Puede aprobar todas las hojas de horas que se hayan enviado donde haya sido designado como aprobador. Cuando se envía una hoja de horas para su aprobación, esta se enumera en el área de **Aprobaciones** de la página **Inicio**. Para obtener más información, consulte [Aprobación de trabajo](../../review-and-approve-work/manage-approvals/approving-work.md).

Si el administrador de Workfront ha habilitado la Aprobación de plantilla de horas para el usuario y el Rechazo de plantilla de horas para los controladores de eventos del usuario, se le notificará una vez aprobada o rechazada la plantilla de horas. Para obtener información acerca de cómo habilitar las notificaciones de eventos, vea [Tipos de notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para aprobar una hoja de horas:

{{step1-to-timesheets}}

Se abre el área **Plantillas de horas**.

1. Seleccione **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solamente las hojas de horas que usted apruebe

   O

   Seleccione el filtro **Mis aprobaciones de hojas de horas** en la parte superior de la lista de hojas de horas.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >La opción Mis aprobaciones de hojas de horas no se muestra en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo quitó el filtro Mis aprobaciones de hojas de horas de los controles de lista del área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   >
   >   
   >   
   >   * [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Opcional) Haga clic en el icono **buscar** ![](assets/search-icon.png) en la parte superior de la lista de hojas de horas y escriba una palabra clave para buscar una hoja de horas específica. Puede buscar un lapso de tiempo, o el nombre de un propietario o aprobador.
1. Haga clic en el lapso de tiempo de la hoja de horas que desee aprobar. Se abre la hoja de horas.

   >[!TIP]
   >
   >Las hojas de horas que esperan aprobación tienen un estado de [!UICONTROL Enviado].


1. Haga clic en **Aprobar**

   O

   Si desea rechazar la hoja de horas, haga clic en **Rechazar** en la esquina inferior izquierda de la hoja de horas.

   Si se aprueba, el estado de la hoja de horas cambiará a **Cerrado**.

   Si se rechaza, el estado de la hoja de horas cambia a **Rechazado**.
