---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: metas'
description: 'Notificaciones: metas'
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 99%

---

# Notificaciones: metas

Puede habilitar las notificaciones por correo electrónico de los eventos que se producen en [!DNL Adobe Workfront Goals] en su perfil. Un usuario con licencia [!UICONTROL Plan] también puede habilitarlas para otros usuarios. Para obtener más información, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

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
   <td role="rowheader"><strong>Producto</strong></td> 
   <td>[!DNL Workfront Goals] <p>Para obtener información acerca de [!DNL Workfront Goals], consulte <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] Información general</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL View] a [!DNL Goals] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede cambiar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación y modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

El usuario cuyas notificaciones de [!DNL Goals] se hayan actualizado debe tener lo siguiente:

* Plantilla de diseño que incluye el área [!DNL Goals] en el [!UICONTROL menú principal].
* Acceso a la nueva experiencia [!DNL Adobe Workfront].

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!DNL Goals] notificaciones en el área [!UICONTROL perfil de usuario]

Las notificaciones enumeradas en la siguiente tabla le avisan de los eventos que ocurren en [!DNL Workfront Goals], como que alguien le asigne una meta, resultado o actividad o que alguien realice una actualización en una meta, resultado o actividad de su propiedad. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![Preferencias de notificaciones](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>Las notificaciones instantáneas de [!DNL Goals] están deshabilitadas de manera predeterminada. No puede activar o desactivar las notificaciones diarias y no recibe correos electrónicos de resumen diario para los eventos de esta categoría. Puede habilitar o deshabilitar notificaciones instantáneas individuales para la categoría [!DNL Goals].

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
   <td> <p>El nombre de la persona que le asignó el resultado o la actividad</p> <p>El periodo de la meta para el resultado o la actividad</p> <p>El nombre del resultado o actividad</p> <p>El botón <strong>[!UICONTROL Open in web app]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>El botón <strong>[!UICONTROL Change Notifications Settings]</strong> que le permite administrar las notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Alguien me ha creado una nueva meta personal</strong> </td> 
   <td> <p>Nombre de la persona que asignó la meta</p> <p>El periodo de la meta</p> <p>Nombre de la meta</p> <p>El botón <strong>[!UICONTROL Open in web app]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>El botón <strong>[!UICONTROL Change Notifications Settings]</strong> que le permite administrar las notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Alguien ha dejado un comentario sobre mi meta</strong></td> 
   <td> <p>El nombre de la persona que dejó el comentario</p> <p>El periodo de la meta </p> <p>Nombre de la meta</p> <p>Texto del comentario</p> <p>El botón <strong>[!UICONTROL Open in web app]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>El botón <strong>[!UICONTROL Change Notifications Settings]</strong> que le permite administrar las notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>A alguien le ha gustado mi comentario sobre una meta</strong></td> 
   <td> <p>Nombre de la persona a la que le ha gustado el comentario</p> <p>El periodo de la meta </p> <p>Nombre de la meta</p> <p>Texto del comentario </p> <p>El botón <strong>[!UICONTROL Open in web app]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>El botón <strong>[!UICONTROL Change Notifications Settings]</strong> que le permite administrar las notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>A alguien le ha gustado una actualización de mi meta</strong></td> 
   <td> <p>Recibes un correo electrónico cuando a alguien le gusta un comentario que has hecho en una meta o cuando actualizas el progreso de tus resultados o actividades en la meta. </p> <p>El nombre de la persona a la que le gustó la actualización</p> <p>El periodo de la meta </p> <p>Nombre de la meta</p> <p>El botón <strong>[!UICONTROL Open in web app]</strong> que abre el panel [!UICONTROL Goal Details]</p> <p>El botón <strong>[!UICONTROL Change Notifications Settings]</strong> que le permite administrar las notificaciones.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
