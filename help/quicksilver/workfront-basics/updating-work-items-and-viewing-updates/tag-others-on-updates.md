---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Etiquetar otros en actualizaciones
description: Al proporcionar comentarios de actualización en un objeto de Adobe Workfront, todos los usuarios del proyecto pueden ver la información enviada. Sin embargo, es posible que a veces los usuarios que no están en el proyecto se beneficien de ver esta información. En lugar de incluir a esos usuarios en el proyecto, puede etiquetarlos en la actualización para compartirlos con ellos. Los usuarios etiquetados reciben una notificación de evento.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Etiquetar otros en actualizaciones

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
Puede etiquetar a los usuarios al realizar una actualización de un objeto si desea llamar su atención sobre un objeto que de otra manera no seguirían.
En lugar de incluir a esos usuarios en el objeto asignándolos o haciendo que se suscriban a él, puede etiquetarlos en la actualización para compartirlos con ellos. Los usuarios etiquetados reciben una notificación sobre la actualización que introduzca.

>[!NOTE]
>
>Se debe activar una notificación de evento para que un usuario reciba la notificación por correo electrónico. Los administradores pueden activar notificaciones para todo el sistema o para un grupo de nivel superior. Un usuario también puede habilitar y deshabilitar notificaciones de eventos individuales en su propio perfil de usuario. Para obtener más información, consulte lo siguiente:
>
>* [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Ver y configurar notificaciones de eventos para un grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


Para obtener información sobre cómo agregar actualizaciones a objetos de Workfront, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Cuando un problema se convierte en un proyecto o tarea, las actualizaciones se copian en el nuevo proyecto o tarea, pero los usuarios etiquetados no. Para continuar con la conversación, debe etiquetar a los participantes de nuevo.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitar o superior problemas y documentos; Revisar o superior para todos los demás objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Solicitante o superior para problemas y documentos; Revisor o superior para todos los demás objetos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Etiquetar otros en actualizaciones

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. Comience a actualizar un elemento de trabajo, tal como se describe en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. En el **Notificar** , empiece a escribir el nombre del usuario o equipo que desea incluir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   O

   Escriba el símbolo @ en la variable **Iniciar una nueva actualización** , empiece a escribir el nombre del usuario o equipo que desea incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   >
   >Para identificar el usuario correcto cuando hay usuarios con nombres similares o idénticos, fíjese en el avatar, la función principal del usuario o su dirección de correo electrónico. Los usuarios deben estar asociados con al menos una función de trabajo para verla al etiquetarlos en una actualización.

   ![](assets/tag-users-in-update.png)

1. (Opcional) Para que la actualización sea privada, active **Privado para mi empresa** en la esquina inferior derecha del cuadro de actualización. Esto hace que la actualización sea visible solo para los usuarios de su empresa.

   >[!NOTE]
   >
   >Los usuarios etiquetados fuera de la empresa aún podían recibir una notificación o un correo electrónico en la aplicación, aunque no vieran los comentarios privados en la pestaña Actualizaciones . Se recomienda no etiquetar a los usuarios externos en una actualización si no desea compartir la información con ellos.

1. (Opcional) Para agregar varios usuarios y equipos, repita el paso 2.

   >[!NOTE]
   >
   >Todos los usuarios y miembros del equipo que aparecen en el campo Notificar reciben una notificación en la aplicación para la actualización y podrían recibir un correo electrónico, en función de la configuración de sus ajustes de notificación por correo electrónico. Los usuarios que se etiquetan en un comentario o respuesta reciben una notificación para ese comentario o respuesta y pueden ver su nombre en el campo Notificar durante el resto del subproceso, pero no reciben otra notificación a menos que se etiqueten de nuevo. Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) y [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Haga clic en **Actualizar**.\
   A los usuarios incluidos en la actualización se les concede automáticamente el permiso Ver al objeto y pueden ver y responder a las actualizaciones realizadas en el objeto.

   Puede ver quién ha sido etiquetado en cada respuesta en la parte superior del subproceso de actualización. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o una respuesta en el objeto.

   ![](assets/tagging-transparency-350x192.png)

   Para obtener información sobre la funcionalidad adicional disponible al actualizar un elemento de trabajo, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->