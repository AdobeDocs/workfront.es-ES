---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Aprobar un parte de horas
description: El proceso de aprobación de las hojas de horas proporciona a los administradores visibilidad sobre las horas de trabajo de sus informes directos. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas durante el período.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Aprobar un parte de horas

El proceso de aprobación de las hojas de horas proporciona a los administradores visibilidad sobre las horas de trabajo de sus informes directos. Los aprobadores pueden verificar que todo el tiempo registrado se ha asignado en las áreas correctas y que se ha registrado un número suficiente de horas durante el período.

Adobe Workfront permite configurar las aprobaciones de hojas de horas para que sean compatibles con esta área.

Para obtener información sobre el envío de un parte de horas, consulte [Enviar un parte de horas para su aprobación](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Designar aprobadores de hojas de horas

Por lo general, las hojas de horas son aprobadas por administradores funcionales o personal de recursos humanos. (Normalmente, los administradores de proyectos no aprueban las hojas de horas).

Se define un aprobador de parte de horas al crear el perfil de parte de horas. Debe tener una licencia del Plan para ser designado como aprobador.

Para obtener más información sobre la designación de aprobadores de hojas de horas, consulte la sección [Crear o editar un perfil de hoja de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) en el artículo [Crear, editar y asignar perfiles de parte de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Aprobar un parte de horas

Puede aprobar cualquier hoja de tiempo que se haya enviado donde haya sido designado aprobador. Cuando se envía un parte de horas para su aprobación, este se enumera en la sección **Aprobaciones** del área **Página principal**  página. Para obtener más información, consulte [Aprobación del trabajo](../../review-and-approve-work/manage-approvals/approving-work.md).

Si el administrador de Workfront ha habilitado la aprobación de parte de horas para el usuario y el rechazo de parte de horas para los controladores de eventos de usuario, se le notifica después de aprobar o rechazar el parte de horas. Para obtener información sobre cómo activar las notificaciones de eventos, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para aprobar un parte de horas:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Hojas de tiempo**.
1. Seleccione el **Aprobaciones de Mi parte de horas** en la esquina superior derecha de la página para ver solo las partes de horas que aprueba

   O

   Seleccione el **Aprobaciones de Mi parte de horas** en la parte superior de la lista de hojas de horas.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >La opción Mis aprobaciones de parte de horas no se muestra en la parte superior de la lista de parte de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo ha eliminado el filtro Mis aprobaciones de parte de horas de los controles de lista del área Configuración o de la plantilla de diseño. Para obtener más información, consulte los siguientes artículos:
   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Haga clic en el **búsqueda** icono ![](assets/search-icon.png) en la parte superior de la lista de parte de horas y escriba una palabra clave para localizar un parte de horas específico. Puede buscar un lapso de tiempo, o el nombre de un propietario o aprobador.
1. Haga clic en el lapso de tiempo para el parte de horas que desee aprobar. Se abre el parte de horas.

   >[!TIP]
   Las hojas de tiempo en espera de aprobación tienen un estado de [!UICONTROL Enviado].


1. Haga clic en **Aprobar**

   O

   Si desea rechazar el parte de horas, haga clic en **Rechazar** en la esquina inferior izquierda del parte de horas.

   Si se aprueba, el estado del parte de horas cambia a **Cerrado**.

   Si se rechaza, el estado del parte de horas cambia a **Rechazado**.
