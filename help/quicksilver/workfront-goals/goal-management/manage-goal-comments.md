---
product-previous: workfront-goals
navigation-topic: goal-management
title: Administrar comentarios de objetivos en Objetivos de Adobe Systems Workfront
description: Puede añadir comentarios a todas las metas que puede ver en Adobe Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 71%

---

# Administrar comentarios de metas en Adobe Workfront Goals

<!--Audited for P&P only: 04/2025-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

Puede agregar comentarios a todos los objetivos que puede vista en Adobe Systems Objetivos de Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> 
   <p>Para la nueva estructura de plan y licencias:
  <ul><li>Un plan Ultimate </li></ul>
   </p>
<p>Para la estructura actual de plan y licencias: 
<ul><li> Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront</td>
 <td>
 <p>Cualquiera</td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito del producto: Workfront</p>
 O
 <p>Requisitos actuales del producto: Además de una licencia de Workfront, debe comprar una licencia para Adobe Systems objetivos de Workfront. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Configuración de nivel de acceso</td>
 <td> <p>Acceso de visualización o superior a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Acceso de visualización o superior a la meta</p>
  <p>De forma predeterminada, los usuarios no tienen acceso a las metas </p>
 <p>Para obtener información acerca de cómo compartir metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Metas en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar comentarios de metas

Puede añadir comentarios a las metas en la sección Actualizaciones de la página de una meta.

1. Haz clic en el icono](assets/main-menu-icon.png) del menú principal en la esquina superior derecha o en el icono ![del **menú** principal Líneas](assets/lines-main-menu.png) del menú principal en la esquina superior izquierda, si están disponibles, y haz clic en **Objetivos******![
Se abrirá la lista de metas.
1. Busque la meta a la que desee añadir comentarios y, a continuación, haga clic en su nombre para abrir la página de la meta.
1. Haga clic en **Actualizaciones** en el panel izquierdo. 

   Para obtener más información acerca de la administración de comentarios para objetos Workfront, consulte Actualización [del trabajo](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--   
1. (Optional) To locate an existing comment, start typing a keyword (*****or a user's name********) in the **Search** box in the upper-right corner of the **Comments** tab. 
   
   ![Search field](assets/search-field-in-updates-tab-goals.png)

   The keyword (****or user****) you searched for is highlighted and the comments that contain it display at the top of the Updates section. 


      >[!NOTE]
      >
      >You must search for a word included in a comment or reply. You cannot search for a tagged user or team.
   
   For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. Click the **x** icon in the search field to clear the search results and return to the complete update.
1. Click the **Comments** tab in the upper-left corner of the Updates area.
1. Start entering a comment in the **New comment** box.
         
   ![Comment box](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.

1. (Optional) To undo or redo a change, use the following shortcut keys:
      * CTRL + Z (⌘+z for Mac) to undo a change 
      * CTRL + Y (⌘+y for Mac) to redo a change 
1. (Optional) To add rich-text formatting to your update, a hyperlink, or an emoji, use any options on the Rich Text toolbar or the icons adjacent to it. For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 
1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. Select the **Private to my company** toggle to make the comment visible only to people in your company. 

      >[!TIP]
      >
      >You must have a Company specified in your profile to have this option available in the Updates area. 

1. Click **Submit**. 

      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments, as well as a blue notification at the bottom of the screen indicating the number of new comments. 
      >
      >The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >![Real time new red indicator](assets/real-time-new-red-indicator-unified-commenting-copy.png)
      
1. (Optional) To edit a comment, click the **More** menu ![More icon](assets/more-icon.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment or remove any of the tagged users. 
   You can edit your comment within 15 minutes from submitting it. An "edited" indicator is added to the left of the date stamp that displays when the comment was updated.

   ![Edited tag on comment](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
   >
   > * The date stamp is the date of the original comment and not the date of the latest update. 

1. (Optional) Click the **More** menu ![More icon](assets/more-icon.png), then click any of the following options to copy information from a comment to the clipboard or into a new reply:

      * **Copy link** to copy the link of an update, without the replies.
      * **Copy body text** to copy the text of an update. 
      * **Quote reply** to open a new comment box where the original comment is quoted in a new reply and is marked as a block quote.

         For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

1. (Optional) Click the **More** menu ![More icon](assets/more-icon.png) to the right of a comment, then click **Delete** to delete a comment you added. For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-9 above. For more information about replying to updates, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). (**********insure this stays accurate*********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Updates section, click **View** inside the blue **new comments banner** at the bottom of the screen  to display these comments.
   
   ![Blue comments banner](assets/blue-new-comments-banner-with-view-button.png)
   
   Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon![Like icon](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes.

1. (Optional) Click the **System Activity** tab to view updates logged by the system. When a goal is updated, Workfront generates a note about that update that and displays it in the System Activity tab. Workfront also records a system update when a result, activity, or project is added to the goal or when it is updated. (*********ensure the casing on the tab has not changed**********)-->


