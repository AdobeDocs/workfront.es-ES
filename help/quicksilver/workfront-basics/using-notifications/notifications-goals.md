---
content-type: reference
navigation-topic: notifications
title: '''Notificaciones: Objetivos'
description: '''Notificaciones: Objetivos'
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 6%

---

# Notificaciones: Objetivos

Puede activar las notificaciones por correo electrónico para los eventos que se producen en [!DNL Adobe Workfront Goals] en su perfil. Un usuario con un [!UICONTROL Plan] licencia también puede habilitarlas para otros usuarios. Para obtener más información, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

## Requisitos de acceso

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Product</strong></td> 
   <td>[!DNL Workfront Goals] <p>Para obtener información sobre [!DNL Workfront Goals], consulte <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] información general</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL View] a [!DNL Goals] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

El usuario cuyo [!DNL Goals] las notificaciones se actualizan deben tener lo siguiente:

* Una plantilla de diseño que incluye el [!DNL Goals] en el [!UICONTROL Menú principal].
* Acceso al nuevo [!DNL Adobe Workfront] experiencia.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!DNL Goals] notificaciones en el [!UICONTROL perfil de usuario] area

Las notificaciones enumeradas en la siguiente tabla le avisan de los eventos que se producen en [!DNL Workfront Goals], como alguien que le asigne un objetivo, un resultado o una actividad, o alguien que actualice un objetivo, un resultado o una actividad de su propiedad. Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>Notificaciones instantáneas para [!DNL Goals] están desactivados de forma predeterminada. No puede activar ni desactivar las notificaciones diarias y no recibe correos electrónicos resumidos diarios para los eventos de esta categoría. Puede activar o desactivar notificaciones instantáneas individuales para la variable [!DNL Goals] categoría.

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Notificación</strong></td> 
   <td> <p><strong>Campos incluidos</strong> </p> <p><strong>*Solo notificaciones instantáneas</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Alguien me ha asignado un resultado o una actividad</strong></td> 
   <td> <p>El nombre de la persona que le asignó el resultado o la actividad</p> <p>El periodo del objetivo para el resultado o la actividad</p> <p>Nombre del resultado o actividad</p> <p>La variable <strong>[!UICONTROL Abrir en aplicación web]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>La variable <strong>[!UICONTROL Cambiar configuración de notificaciones]</strong> que le permite administrar sus notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Alguien ha creado una nueva meta personal para mí</strong> </td> 
   <td> <p>Nombre de la persona que asignó el objetivo</p> <p>El periodo del objetivo</p> <p>Nombre del objetivo</p> <p>La variable <strong>[!UICONTROL Abrir en aplicación web]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>La variable <strong>[!UICONTROL Cambiar configuración de notificaciones]</strong> que le permite administrar sus notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Alguien ha dejado un comentario sobre mi meta</strong></td> 
   <td> <p>Nombre de la persona que abandonó el comentario</p> <p>El periodo del objetivo </p> <p>Nombre del objetivo</p> <p>Texto del comentario</p> <p>La variable <strong>[!UICONTROL Abrir en aplicación web]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>La variable <strong>[!UICONTROL Cambiar configuración de notificaciones]</strong> que le permite administrar sus notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>A alguien le ha gustado mi comentario sobre una meta</strong></td> 
   <td> <p>Nombre de la persona a la que le gustó el comentario</p> <p>El periodo del objetivo </p> <p>Nombre del objetivo</p> <p>Texto del comentario </p> <p>La variable <strong>[!UICONTROL Abrir en aplicación web]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>La variable <strong>[!UICONTROL Cambiar configuración de notificaciones]</strong> que le permite administrar sus notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>A alguien le ha gustado una actualización de mi meta</strong></td> 
   <td> <p>Recibe un correo electrónico cuando a alguien le gusta un comentario que haya hecho sobre un objetivo o cuando actualiza el progreso de sus resultados o actividades en el objetivo. </p> <p>Nombre de la persona a la que le gustó la actualización</p> <p>El periodo del objetivo </p> <p>Nombre del objetivo</p> <p>La variable <strong>[!UICONTROL Abrir en aplicación web]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>La variable <strong>[!UICONTROL Cambiar configuración de notificaciones]</strong> que le permite administrar sus notificaciones.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
