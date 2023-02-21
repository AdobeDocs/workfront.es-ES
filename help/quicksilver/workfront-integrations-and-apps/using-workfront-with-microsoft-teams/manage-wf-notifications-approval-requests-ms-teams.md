---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Administrar [!DNL Adobe Workfront] notificaciones en [!DNL Microsoft] Equipos
description: Puede recibir notificaciones de [!DNL Adobe Workfront] acerca de los artículos que debe aprobar, las asignaciones que le han sido asignadas, o los comentarios y cambios en los artículos con los que está asociado.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 473a1fe3cb7e247749d9b540e3e5556cbe17a1dd
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# Administrar [!DNL Adobe Workfront] notificaciones en [!DNL Microsoft Teams]

Puede recibir notificaciones de [!DNL Adobe Workfront] acerca de los artículos que debe aprobar, las asignaciones que le han sido asignadas, o los comentarios y cambios en los artículos con los que está asociado.

Estas notificaciones contienen [!DNL Workfront] acciones que puede realizar en [!DNL Microsoft Teams] sin salir de [!DNL Microsoft Teams] para cumplirlos.

>[!NOTE]
>
>[!DNL Microsoft Teams] ya no es compatible [!DNL Internet Explorer]. Para usar la variable [!DNL Adobe Workfront for Microsoft Teams integration], debe utilizar un explorador web que no sea [!DNL Internet Explorer].


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
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos para la recepción [!DNL Workfront] Notificaciones en [!DNL Microsoft Teams]

Puede recibir [!DNL Workfront] notificaciones en [!DNL Microsoft Teams] si se cumplen las condiciones siguientes:

* Un propietario del equipo ha instalado y configurado [!DNL Workfront for Microsoft Teams] para su equipo.
* Ha iniciado sesión [!DNL Workfront] from [!DNL Microsoft Teams].
* Ha habilitado notificaciones instantáneas en [!DNL Workfront]. Para obtener información sobre cómo activar notificaciones instantáneas, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener información sobre la instalación [!DNL Workfront for Microsoft Teams] e inicie sesión en [!DNL Workfront from Microsoft Teams], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Administración [!DNL Workfront] Notificaciones en [!DNL Microsoft Teams]

Cuando la variable [!DNL Workfront for Microsoft Teams] la aplicación está instalada, [!DNL Workfront] el canal de chat se crea en [!DNL Microsoft Teams] para cada miembro de ese equipo. Cuando se realiza una determinada acción en [!DNL Workfront], puede configurar las opciones de [!DNL Workfront for Microsoft Teams] para recibir notificaciones sobre esa acción en el [!DNL Workfront] canal de chat de [!DNL Microsoft Teams].

Tenga en cuenta lo siguiente al trabajar con [!DNL Workfront] notificaciones de [!DNL Microsoft Teams]:

* No puede recibir todo, pero solo un número seleccionado de [!DNL Workfront] notificaciones en [!DNL Microsoft Teams].
* Todas las notificaciones recibidas de [!DNL Workfront] aparecen en la [!DNL Workfront] canal de chat de bot.

   Para obtener información sobre cómo instalar la variable [!DNL Workfront] canal de bots, consulte la [Iniciar sesión en [!DNL Workfront] from [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) en [Instalación [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) artículo.

* Puede haber hasta 5 minutos de retraso entre el momento en que se realiza una actualización en [!DNL Workfront] y cuando reciba la notificación sobre él en [!DNL Microsoft Teams].
* Para cada [!DNL Microsoft Teams] , también recibirá una notificación por correo electrónico.

Para administrar el [!DNL Workfront] notificaciones que puede recibir en [!DNL Microsoft Teams]:

1. Haga clic en el **[!UICONTROL Más]** icono de aplicaciones (tres puntos) en la barra de navegación izquierda de [!DNL Microsoft Teams].

1. Haga clic en [!DNL Workfront] en la lista que aparece.
1. Seleccione el **[!UICONTROL Configuración]** pestaña .

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Deshabilite cualquiera de las notificaciones que no desee recibir. Puede habilitar o deshabilitar grupos de notificaciones, como notificaciones de información o aprobación, o puede administrar las notificaciones de forma individual.

   Todas las notificaciones están habilitadas de forma predeterminada.

   La configuración de notificaciones de [!DNL Workfront for Microsoft] Los equipos se guardan automáticamente.

   >[!NOTE]
   >
   >No puede agregar más notificaciones a las que están disponibles de forma predeterminada.

## Respondiendo a [!DNL Workfront] Notificaciones y solicitudes de aprobación en [!DNL Microsoft Teams]

1. Iniciar sesión en [!DNL Workfront] from [!DNL Microsoft Teams].\
   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Vaya a la **[!UICONTROL Chat]** y haga clic en el botón **[!DNL Workfront]** canal de bots.\
   Este canal es para su conversación personal con el [!DNL Workfront] bot. Todo [!DNL Workfront] aquí se muestran las notificaciones.
1. En función del tipo de notificación que reciba, diríjase a la sección correspondiente:

   * [Notificaciones de aprobación](#approval-notifications-approval-notifications)
   * [Notificaciones de asignación](#assignment-notifications-assignment-notifications)
   * [Notificaciones de comentarios](#comment-notifications-comment-notifications)
   * [Actualizar notificaciones](#update-notifications-update-notifications)
   * [Notificaciones de cambio de fecha](#date-change-notifications-date-change-notifications)

### Notificaciones de aprobación {#approval-notifications}

Recibe notificaciones de aprobación cuando se le pide que apruebe un objeto, como una tarea, un parte de horas o una prueba. Sin embargo, aún puede comentar la notificación. Desde la notificación de aprobación, puede realizar las siguientes acciones:

* **[!UICONTROL Aprobar]**: Haga clic en para aprobar el elemento.
* **[!UICONTROL Cambiar]**: Haga clic en para aprobar el elemento con los cambios.
* **[!UICONTROL Rechazar]**: Haga clic en para rechazar el elemento.
* **[!UICONTROL Comentario]**: Haga clic en para realizar un comentario. El comentario también aparece en [!DNL Workfront] como actualización del objeto sobre el que se envía la notificación.
* **[!UICONTROL Vaya a Prueba]**: Haga clic en para abrir la prueba. A continuación, puede tomar una decisión directamente en la prueba. Para obtener más información, consulte [Tome una decisión sobre una prueba en el visor de pruebas](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

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
   <td role="rowheader">Debe aprobar un parte de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien quiere que apruebe esta prueba</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">El parte de horas se rechaza</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se vuelve a abrir el parte de horas</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se aprueba una solicitud de aprobación de documento que solicitó</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Una solicitud de aprobación de documento que solicitó se aprobó con cambios</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se rechaza una solicitud de aprobación de documento que solicitó</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Su parte de horas está aprobada</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notificaciones de asignación {#assignment-notifications}

Recibe notificaciones de asignación cuando usted, o el equipo en el que esté, estén asignados a una tarea o problema en Workfront. Desde la notificación de asignación, puede realizar las siguientes acciones:

* **[!UICONTROL Trabaje en él]**: Seleccione para comprometerse a trabajar en el elemento. Se muestra brevemente una notificación para confirmar que se ha añadido un nuevo elemento a la lista de trabajo.
* **[!UICONTROL Ver en[!DNL Workfront]]**: Seleccione para ver el problema o la tarea asignados en Workfront, que abre una nueva pestaña.
* **[!UICONTROL Inicio]**: Haga clic en para comenzar a trabajar en el elemento. Se muestra brevemente una notificación para confirmar que se ha añadido un nuevo elemento a la lista de trabajo.
* **[!UICONTROL Comentario]**: Haga clic en para realizar un comentario sobre el elemento. El comentario también aparece en el flujo de actualización del elemento en Workfront.
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
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comentario]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se le asigna una tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se le asigna un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un equipo al que esté asignado recibe una solicitud de trabajo para una tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un equipo al que esté asignado recibe una solicitud de trabajo para un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notificaciones de comentarios {#comment-notifications}

Recibe una notificación de comunicación cuando alguien comenta sobre un elemento con el que está asociado o lo incluye en una actualización. Desde la notificación de comunicación, puede realizar las siguientes acciones:

* **Reply**: Haga clic en para responder al comentario o [!UICONTROL actualizar]. La respuesta también aparece en el flujo de actualización, donde el comentario aparece en Workfront.
* **[!UICONTROL Ver en Workfront]**: Seleccione para ver el comentario y el elemento en Workfront, que se abre en una pestaña nueva.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione un nuevo estado para el elemento de trabajo del que trata el comentario o la actualización.

#### Acciones disponibles en notificaciones de comunicación específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>[!UICONTROL Respuesta]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se publica un comentario en la solicitud</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se publica una respuesta en su solicitud de trabajo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien comenta en un hilo en el que estás</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien comenta sobre uno de sus elementos de trabajo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien comenta en un parte de horas que apruebe</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se añade un comentario en la página de perfil de usuario o editando masivamente varios usuarios</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se añade un comentario en una de las actualizaciones</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se añade un comentario en el parte de horas</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Actualizar notificaciones {#update-notifications}

Recibe una notificación de información cuando hay una actualización de un artículo con el que está asociado, pero no necesita realizar ninguna acción sobre el artículo. Desde la notificación de información, puede realizar las siguientes acciones:

* **[!UICONTROL Responder]**: Haga clic en para responder a la [!UICONTROL actualizar]. La respuesta también aparece en el flujo de actualización del elemento en Workfront.
* **Ver en Workfront**: Seleccione para ver el comentario y el elemento en Workfront, que se abre en una pestaña nueva.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione el nuevo estado del elemento en el menú desplegable.

#### Acciones disponibles en notificaciones de información específicas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>[!UICONTROL Respuesta]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se realiza una actualización de una tarea, un problema o un proyecto al que está suscrito</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien te incluye en una actualización dirigida</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alguien incluye a su equipo en una [!UICONTROL actualización dirigida]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notificaciones de cambio de fecha {#date-change-notifications}

Recibirá una notificación de cambio de fecha cuando la fecha cambie en un elemento de trabajo al que esté asignado. Desde la notificación de cambio de fecha, puede realizar las siguientes acciones.

* **[!UICONTROL Comentario]**: Haga clic en para realizar un comentario sobre el elemento. El comentario también aparece en el flujo de actualización del elemento en Workfront.
* **[!UICONTROL Estado]**: Haga clic en y, a continuación, seleccione el nuevo estado del elemento de trabajo en el menú desplegable.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th> <p>[!UICONTROL Comentario]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">La fecha de vencimiento cambia en una tarea a la que está asignado</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
