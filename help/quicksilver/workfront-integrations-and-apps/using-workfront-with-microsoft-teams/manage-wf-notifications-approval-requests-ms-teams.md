---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Administrar [!DNL Adobe Workfront] notificaciones en [!DNL Microsoft] equipos
description: Puedes recibir notificaciones de  [!DNL Adobe Workfront] acerca de los artículos que necesitas aprobar, las asignaciones que te han dado o los comentarios y cambios en los artículos con los que estás asociado.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Administrar [!DNL Adobe Workfront] notificaciones en [!DNL Microsoft Teams]

>[!NOTE]
>
>Actualmente, la integración de Adobe Workfront para Microsoft Teams solo es compatible con la experiencia clásica de Microsoft Teams.

Puede recibir notificaciones de [!DNL Adobe Workfront] acerca de los elementos que necesita aprobar, las asignaciones que se le han dado o los comentarios y cambios en los elementos con los que está asociado.

Estas notificaciones contienen [!DNL Workfront] acciones que puede realizar en [!DNL Microsoft Teams] sin salir de [!DNL Microsoft Teams] para realizarlas.

>[!NOTE]
>
>[!DNL Microsoft Teams] ya no admite [!DNL Internet Explorer]. Para usar [!DNL Adobe Workfront for Microsoft Teams integration], debe usar un explorador web que no sea [!DNL Internet Explorer].


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Trabajo], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos para recibir notificaciones de [!DNL Workfront] en [!DNL Microsoft Teams]

Puede recibir [!DNL Workfront] notificaciones en [!DNL Microsoft Teams] si se cumplen las siguientes condiciones:

* El propietario de un equipo ha instalado y configurado [!DNL Workfront for Microsoft Teams] para su equipo.
* Ha iniciado sesión en [!DNL Workfront] desde [!DNL Microsoft Teams].
* Ha habilitado las notificaciones instantáneas en [!DNL Workfront]. Para obtener información sobre cómo habilitar las notificaciones instantáneas, consulte [Modificar tus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener información sobre cómo instalar [!DNL Workfront for Microsoft Teams] e iniciar sesión en [!DNL Workfront from Microsoft Teams], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Administrando [!DNL Workfront] notificaciones en [!DNL Microsoft Teams]

Cuando la aplicación [!DNL Workfront for Microsoft Teams] está instalada, se crea un canal de chat [!DNL Workfront] en [!DNL Microsoft Teams] para cada miembro de ese equipo. Cuando se realiza una acción determinada en [!DNL Workfront], puede configurar los valores de [!DNL Workfront for Microsoft Teams] para recibir notificaciones sobre esa acción en el canal de chat [!DNL Workfront] de [!DNL Microsoft Teams].

Tenga en cuenta lo siguiente al trabajar con [!DNL Workfront] notificaciones de [!DNL Microsoft Teams]:

* No puede recibir todas las notificaciones, solo un número seleccionado de [!DNL Workfront] en [!DNL Microsoft Teams].
* Todas las notificaciones que reciba de [!DNL Workfront] aparecerán en el canal de chat de bots [!DNL Workfront].

  Para obtener información sobre la instalación del canal de bots [!DNL Workfront], consulte la sección [Iniciar sesión en [!DNL Workfront] desde [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) en el artículo [Instalar [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

* Puede haber un retraso de hasta 5 minutos entre el momento en que se realiza una actualización en [!DNL Workfront] y el momento en que recibe la notificación al respecto en [!DNL Microsoft Teams].
* También recibe una notificación por correo electrónico por cada notificación [!DNL Microsoft Teams].

Para administrar las [!DNL Workfront] notificaciones que puede recibir en [!DNL Microsoft Teams]:

1. Haga clic en el icono **[!UICONTROL Más aplicaciones agregadas]** (tres puntos) en la barra de navegación izquierda de [!DNL Microsoft Teams].

1. Haga clic en [!DNL Workfront] en la lista que aparece.
1. Seleccione la pestaña **[!UICONTROL Configuración]**.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Deshabilite cualquiera de las notificaciones que no desee recibir. Puede habilitar o deshabilitar grupos de notificaciones, como notificaciones de información o de aprobación, o puede administrar las notificaciones individualmente.

   Todas las notificaciones están habilitadas de forma predeterminada.

   La configuración de notificaciones de [!DNL Workfront for Microsoft] equipos se guarda automáticamente.

   >[!NOTE]
   >
   >No se pueden agregar más notificaciones a las que están disponibles de forma predeterminada.

## Respondiendo a [!DNL Workfront] notificaciones y solicitudes de aprobación en [!DNL Microsoft Teams]

1. Iniciar sesión en [!DNL Workfront] desde [!DNL Microsoft Teams].\
   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Vaya al área de **[!UICONTROL Chat]** y haga clic en el canal de bots **[!DNL Workfront]**.\
   Este canal es para su charla personal con el bot [!DNL Workfront]. Aquí se muestran todas las [!DNL Workfront] notificaciones.
1. Según el tipo de notificación que reciba, continúe con la sección correspondiente:

   * [Notificaciones de aprobación](#approval-notifications-approval-notifications)
   * [Notificaciones de asignación](#assignment-notifications-assignment-notifications)
   * [Notificaciones de comentario](#comment-notifications-comment-notifications)
   * [Actualizar notificaciones](#update-notifications-update-notifications)
   * [Notificaciones de cambio de fecha](#date-change-notifications-date-change-notifications)

### Notificaciones de aprobación {#approval-notifications}

Recibirá notificaciones de aprobación cuando se le pida que apruebe un objeto, como una tarea, una plantilla de horas o una prueba. Sin embargo, aún puede realizar comentarios en la notificación. Desde la notificación de aprobación, puede realizar las siguientes acciones:

* **[!UICONTROL Aprobar]**: haga clic para aprobar el elemento.
* **[!UICONTROL Cambiar]**: haga clic para aprobar el elemento con cambios.
* **[!UICONTROL Rechazar]**: haga clic para rechazar el elemento.
* **[!UICONTROL Comentario]**: Haga clic para hacer un comentario. Su comentario también aparece en [!DNL Workfront] como una actualización del objeto del que trata la notificación.
* **[!UICONTROL Ir a la revisión]**: haga clic para abrir la revisión. A continuación, puede tomar una decisión directamente en la prueba. Para obtener más información, consulte [Tomar una decisión sobre una prueba en el visor de pruebas](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Una vez que haya tomado una decisión de aprobación, no puede cambiarla desde la notificación.

#### Acciones disponibles en notificaciones de aprobación específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>[!UICONTROL Aprobar]</th> 
   <th>[!UICONTROL Rechazar]</th> 
   <th> <p>[!UICONTROL Cambio]</p> </th> 
   <th> <p>[!UICONTROL Ir a prueba] </p> </th> 
   <th>[!UICONTROL Comentario]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Debe aprobar un proyecto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Debe aprobar una tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Debe aprobar un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Debe aprobar un documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Debe aprobar el acceso a un objeto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Debe aprobar una plantilla de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien desea que usted apruebe esta revisión</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se rechaza su hoja de horas</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se ha reabierto su hoja de horas</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se aprueba una solicitud de aprobación de documento que ha solicitado</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se aprueba con cambios una solicitud de aprobación de documento solicitada</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se rechazó una solicitud de aprobación de documento que usted solicitó</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se aprueba su hoja de horas</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notificaciones de asignación {#assignment-notifications}

Recibirá notificaciones de asignación cuando usted o un equipo en el que esté, se asignen a una tarea o a un problema en Workfront. Desde la notificación de asignación, puede realizar las siguientes acciones:

* **[!UICONTROL Trabajar en ello]**: seleccione esta opción para comprometerse a trabajar en el elemento. Se muestra brevemente una notificación para confirmar que se ha agregado un nuevo elemento a su lista de trabajos.
* **[!UICONTROL Ver en[!DNL Workfront]]**: seleccione esta opción para ver el problema o la tarea asignados en Workfront, que abre una nueva pestaña.
* **[!UICONTROL Iniciar]**: Haga clic para comenzar a trabajar en el elemento. Se muestra brevemente una notificación para confirmar que se ha agregado un nuevo elemento a su lista de trabajos.
* **[!UICONTROL Comentario]**: haga clic para hacer un comentario sobre el elemento. Su comentario también aparece en el flujo de actualización del elemento en Workfront.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione el nuevo estado del elemento de trabajo en el menú desplegable.

#### Acciones disponibles en notificaciones de asignación específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>[!UICONTROL Iniciar]</th> 
   <th>[!UICONTROL Comentario]</th> 
   <th> <p>[!UICONTROL Estado]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se le ha asignado una tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se le ha asignado un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">El equipo al que esté asignado recibirá una solicitud de trabajo para una tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">El equipo al que esté asignado recibirá una solicitud de trabajo para un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notificaciones de comentario {#comment-notifications}

Recibes una notificación de comunicación cuando alguien comenta un artículo con el que estás asociado o te incluye en una actualización. Desde la notificación de comunicación, puede realizar las siguientes acciones:

* **Reply**: haz clic para responder al comentario o a [!UICONTROL actualizar]. Su respuesta también aparece en el flujo de actualización, donde el comentario aparece en Workfront.
* **[!UICONTROL Ver en Workfront]**: seleccione esta opción para ver el comentario y el elemento en Workfront, que se abre en una nueva pestaña.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione un nuevo estado para el elemento de trabajo sobre el que trata el comentario o la actualización.

#### Acciones disponibles en las notificaciones de comunicaciones específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>[!UICONTROL Responder]</th> 
   <th> <p>[!UICONTROL Estado]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se publica un comentario en su solicitud</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se publica una respuesta en su solicitud de trabajo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien agrega un comentario a un hilo en el que usted se encuentra</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien agrega comentarios a uno de sus elementos de trabajo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien agrega un comentario a una hoja de horas que usted apruebe</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se agrega un comentario en la página de perfil de usuario o al editar varios usuarios por lotes</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se agrega un comentario en una de las actualizaciones</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se agrega un comentario en la hoja de horas</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Actualizar notificaciones {#update-notifications}

Recibirás una notificación cuando haya una actualización de un artículo con el que estés asociado, pero no es necesario que realices ninguna acción sobre el artículo. Desde la notificación de información, puede realizar las siguientes acciones:

* **[!UICONTROL Responder]**: Haz clic para responder a la [!UICONTROL actualización]. Su respuesta también aparece en el flujo de actualizaciones del elemento en Workfront.
* **Ver en Workfront**: seleccione esta opción para ver el comentario y el elemento en Workfront, que se abre en una nueva pestaña.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione el nuevo estado del elemento en el menú desplegable.

#### Acciones disponibles en notificaciones de información específica:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>[!UICONTROL Responder]</th> 
   <th> <p>[!UICONTROL Estado]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se hace una actualización a una tarea, un problema o un proyecto al cual se ha suscrito</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien le incluye en una actualización dirigida</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien incluye a su equipo en una actualización dirigida de [!UICONTROL]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notificaciones de cambio de fecha {#date-change-notifications}

Recibirá una notificación de cambio de fecha cuando cambie la fecha de un elemento de trabajo al que esté asignado. Desde la notificación de cambio de fecha, puede realizar las siguientes acciones.

* **[!UICONTROL Comentario]**: haga clic para hacer un comentario sobre el elemento. Su comentario también aparece en el flujo de actualización del elemento en Workfront.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione el nuevo estado del elemento de trabajo en el menú desplegable.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th> <p>[!UICONTROL Comentario]</p> </th> 
   <th> <p>[!UICONTROL Estado]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Cambia la fecha límite de una tarea a la que está asignado</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
