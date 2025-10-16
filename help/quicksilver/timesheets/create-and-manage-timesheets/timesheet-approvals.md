---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Aprobar una hoja de horas
description: El proceso de aprobación de plantillas de horas proporciona a los administradores visibilidad sobre las horas de trabajo de sus informes directos. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período.
author: Lisa
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 60%

---

# Aprobación de una plantilla de horas

<!--Audited: 8/2024-->

El proceso de aprobación de plantillas de horas proporciona a los administradores visibilidad sobre las horas de trabajo de sus informes directos. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas para el período.

Adobe Workfront permite configurar las aprobaciones de plantillas de horas para que sean compatibles en esta área.

Para obtener información sobre cómo enviar una plantilla de horas, consulte [Enviar una plantilla de horas para su aprobación](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Acceso administrativo a hojas de horas y horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Designar aprobadores de plantillas de horas

Normalmente, los administradores funcionales o el personal de recursos humanos aprueban las plantillas de horas. Los administradores del proyecto no suelen aprobar las plantillas de horas. Los administradores del proyecto pueden aprobar los proyectos con registro de tiempo, aunque son los administradores de equipo o de Recursos Humanos los que deben aprobar las plantillas de horas.

Se define un aprobador de plantilla de horas al crear el perfil de plantilla de horas. Debe contar con una licencia de planificación para ser designado como aprobador.

Para obtener más información sobre cómo designar aprobadores de plantillas de horas, consulte la sección [Crear o editar un perfil de plantilla de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) en el artículo [Crear, editar y asignar perfiles de plantilla de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Aprobación de una plantilla de horas

Puede aprobar todas las plantillas de horas que se hayan enviado donde haya sido designado como aprobador. Cuando se envía una hoja de horas para su aprobación, la hoja de horas se enumera en el widget **Mis aprobaciones** del área de **Inicio**. Para obtener más información, consulte [Aprobación de trabajo](../../review-and-approve-work/manage-approvals/approving-work.md).

Si se establece la siguiente configuración de notificación, el usuario que envía la plantilla de horas para su aprobación recibe un correo electrónico una vez aprobada la plantilla de horas:

* El administrador de Workfront ha habilitado la Aprobación de plantilla de horas para el usuario y el Rechazo de plantilla de horas para los controladores de eventos del usuario. Para obtener información acerca de cómo habilitar las notificaciones de eventos, vea [Tipos de notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* Se aprueba la hoja de horas Mi notificación personal está habilitada en la página de perfil del usuario. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Aprobar una hoja de horas desde el área Hojas de horas

{{step1-to-timesheets}}

Se abre el área **Plantillas de horas**.

1. (Condicional) Si la última vez que accedió a se abre, haga clic en **Volver a las hojas de horas** en la esquina superior izquierda de la pantalla.

1. Seleccione **Mis aprobaciones de plantillas de horas** en la esquina superior derecha de la página para ver solamente las plantillas de horas que usted apruebe

   O

   Seleccione el filtro **Mis aprobaciones de plantillas de horas** en la parte superior de la lista de plantillas de horas.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >La opción Mis aprobaciones de hojas de horas no se muestra en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo quitó el filtro Mis aprobaciones de hojas de horas de los controles de lista del área Configuración o de la plantilla Diseño.
   >
   >Para obtener más información, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Opcional) Haga clic en el icono **buscar** ![](assets/search-icon.png) en la parte superior de la lista de plantilla de horas y escriba una palabra clave para buscar una plantilla de horas específica. Puede buscar un lapso de tiempo o el nombre de un propietario o aprobador.
1. Haga clic en el lapso de tiempo de la plantilla de horas que desee aprobar. Se abre la plantilla de horas.

   >[!TIP]
   >
   >Las plantillas de horas que esperan aprobación tienen un estado de [!UICONTROL Enviado].


1. Haga clic en **Aprobar**

   O

   Si desea rechazar la plantilla de horas, haga clic en **Rechazar** en la esquina inferior izquierda de la plantilla de horas.

   Si se aprueba, el estado de la plantilla de horas cambiará a **Cerrado**.

   Si se rechaza, el estado de la plantilla de horas cambia a **Rechazado**.

### Aprobar una hoja de horas desde el área de Inicio

{{step1-to-home}}

Se abre el área de Inicio.

1. Asegúrese de que ha agregado el widget **Mis aprobaciones** al área de inicio. Para obtener más información, consulte [Agregar, editar o quitar widgets en la nueva página de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).
1. Busque una aprobación de plantilla de horas en el widget Mis aprobaciones.
1. (Opcional) Expanda el menú desplegable a la derecha de los botones Aprobar o Rechazar para agregar un comentario sobre su decisión y luego haga clic en **Agregar**.
1. Haga clic en uno de los siguientes botones para tomar la decisión de aprobación:

   * Aprobar
   * Reject

   La aprobación se eliminó del widget **Mis aprobaciones**.


