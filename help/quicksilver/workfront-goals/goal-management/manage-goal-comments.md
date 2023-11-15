---
product-previous: workfront-goals
navigation-topic: goal-management
title: Administrar comentarios sobre metas en Adobe Workfront Goals
description: Puede agregar comentarios a todas las metas que puede ver en Adobe Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 90c730bbab2e62bcc60bee37272edb1219b2afb4
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Administrar comentarios sobre metas en Adobe Workfront Goals

<!--consider retiring this article when goals and all objects are in parity - after the new commenting experience goes to production GA-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

Puede agregar comentarios a todas las metas que puede ver en Adobe Workfront Goals.

<!--drafted for P&P:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para acceder a la funcionalidad de Adobe Workfront Goals que se describe en este artículo. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para utilizar Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver los objetivos o acceder a ellos</p> <p><b>NOTA</b><p>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concesión de acceso a Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <div> 
     <p>Ver permisos superiores en las metas</p> 
     <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área de Objetivos en el menú principal.

## Administrar comentarios de metas

Puede agregar comentarios a los objetivos en la sección Actualizaciones de la página de un objetivo.

Puede responder a un comentario que usted u otras personas agregaron en esta área o marcarlo como me gusta.

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha, o la **Menú principal** icono ![](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible, haga clic en **Metas**.
Se abrirá la lista de metas.
1. Busque la meta a la que desee agregar comentarios y, a continuación, haga clic en su nombre para abrir la página de la meta.
1. Clic  **Actualizaciones** en el panel izquierdo.
<!--
1. (Optional) To locate an existing comment, start typing a keyword or a user's name in the **Search** box in the upper-right corner of the Updates section. You can search for comment owner's names or for users who are tagged on comments. 

   ![](assets/search-field-in-updates-tab-goals.png)

   The keyword or user you searched for is highlighted and the comments that contain it display at the top of the Updates section. 

      >[!TIP]
      >
      >   Searching for a comment is not available for system activity updates. -->

1. Haga clic en **x** en el campo buscar para borrar los resultados de la búsqueda y volver a la página completa.
1. Haga clic en **Comentarios** en la esquina superior izquierda del área de Actualizaciones.
1. Comience a escribir un comentario en **Nuevo comentario** cuadro.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Si sale de la sección Actualizaciones antes de terminar de escribir y enviar un comentario, el comentario en la página se mantiene en modo de borrador incluso después de cerrar la sesión y volver a iniciarla. Todas las imágenes que se agreguen al comentario también se guardarán en el borrador. Los borradores se guardan durante 7 días después de los cuales se descartan y no se pueden recuperar. Los comentarios redactados solo son visibles para el usuario que los escribe.

1. (Opcional) Para deshacer o rehacer un cambio, utilice las siguientes teclas de método abreviado:
   * CTRL + Z (⌘ + z para Mac) para deshacer un cambio
   * CTRL + Y (⌘ + y para Mac) para rehacer un cambio
1. (Opcional) Para agregar formato de texto enriquecido a la actualización, a un hipervínculo o a una imagen, utilice las opciones de la barra de herramientas Texto enriquecido o los iconos adyacentes. Para obtener más información, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Opcional) En el **Etiquetar personas o equipos** , empiece a escribir el nombre o el correo electrónico de un usuario o equipo que desee incluir en este comentario y, a continuación, selecciónelo cuando se muestre en la lista.
1. Seleccione el **Privado para mi compañía** alterne para que el comentario solo sea visible para las personas de la compañía.

   >[!TIP]
   >
   >Debe tener una Compañía especificada en el perfil para que esta opción esté disponible en el área de Actualizaciones.

1. Clic **Enviar**.

   >[!TIP]
   >
   >Si otro usuario envía un comentario al mismo elemento que está actualizando, habrá una línea roja con un indicador &quot;Nuevo&quot; para informarle de los comentarios más recientes, así como una notificación azul en la parte inferior de la pantalla que indica el número de comentarios nuevos.
   >
   >El indicador solo se muestra después de que el comentario se haya enviado sobre el elemento, y no cuando el comentario aún está compuesto.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. (Opcional) Para editar un comentario, haga clic en **Más** menú ![](assets/more-icon.png) a la derecha del icono Like y, a continuación, haga clic en **Editar**.
1. Edite la información del comentario, añada o elimine imágenes, o quite usuarios etiquetados.
Puede editar su comentario en un plazo de 15 minutos a partir del envío. Se agrega un indicador &quot;editado&quot; a la izquierda de la marca de fecha que muestra cuándo se actualizó el comentario.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * Se genera un correo electrónico para notificar a los usuarios de su actualización solo cuando envía la actualización original. No se genera ningún correo electrónico después de editar la actualización.
   >
   > * La marca de fecha es la fecha del comentario original y no la fecha de la última actualización.

   1. (Opcional) Haga clic en **Más** menú ![](assets/more-icon.png)A continuación, haga clic en cualquiera de las siguientes opciones para copiar información de un comentario en el portapapeles:

      * **Copiar vínculo** para copiar el vínculo de una actualización, sin las respuestas.
      * **Copiar el texto del cuerpo** para copiar el texto de una actualización.

        Para obtener más información, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Haga clic en **Más** menú ![](assets/more-icon.png) a la derecha de un comentario y haga clic en **Eliminar** para eliminar un comentario que ha agregado. Para obtener más información, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Opcional) Haga clic en **Responder** para responder a un comentario existente, siga los pasos del 5 al 9 anteriores. Para obtener más información sobre cómo responder a las actualizaciones, consulte [Responder a las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). <!--insure this stays accurate-->
1. (Condicional y opcional) Si otros usuarios han agregado comentarios que se muestran fuera del área visible en la sección Actualizaciones, haga clic en **Ver** dentro del azul **titular de nuevos comentarios** en la parte inferior de la pantalla para mostrar estos comentarios.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Los comentarios adicionales se muestran en la parte inferior de la pantalla.
1. (Opcional) Haga clic en **Like** icono![](assets/like-icon.png) para que le guste un comentario que otra persona haya agregado. El icono se actualiza con el número de me gusta.

1. (Opcional) Haga clic en **Actividad del sistema** para ver las actualizaciones registradas por el sistema. Cuando se actualiza un objetivo, Workfront genera una nota sobre esa actualización que se muestra en la pestaña Actividad del sistema. Workfront también registra una actualización del sistema cuando se agrega un resultado, una actividad o un proyecto al objetivo o cuando se actualiza. <!--ensure the casing on the tab has not changed-->

<!--BELOW IS OLD, ATIIM/ WORKFRONT GOALS INFORMATION ABOUT COMMENTS: 

## Add comments to goals in the Check-in section

<div class="preview">

The Check-in section has been removed from the Preview environment. You can update goals by accessing the goal page. For information, see 
[Update goals in the Goal details section in Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md). 


</div>

>[!TIP]
>
>You must have access to Edit Goals in your access level to view the Check-in section.

You can add comments to goals in the Check-in section of Workfront Goals, as part of updating your list of goals. For information about updating goals, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

You can also like goal comments that other users have added to mark your approval of them in the Check-in section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   ( Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner))

   This opens the Workfront Goals area. 

1. Click the **Check-in** section in the left panel.

   ![](assets/check-in-icon-left.png)

   Goals assigned to you or that have results and activities that are assigned to you display in this area. 

1. (Optional) Click the right-pointing arrow to the left of the goal name to expand the goal, if the goal is not already expanded. 
1. Type your comment in the **Add a comment to this goal (optional)** field, then click **Post**.

   Two most recent comments display by default under each goal.

1. Click **Show all comments** to display all comments on a goal. A number of total comments for the goal also displays. Comments display in the order they were entered, with the most recent first. 
1. (Optional) Click the **Like icon** ![](assets/like-icon.png) to like a comment. The icon updates with the number of likes. 

1. (Optional) Click the number of likes next to a comment and a list with the names of the users who liked the comment displays in the right panel.

   ![](assets/list-of-likes-users-350x121.png)

1. (Conditional) Click **Back to Updates** to return to the Updates tab of the Goal Details panel, or click the **X icon** in the upper-right corner to close the right panel.

## Add comments to goals in the Pulse section


<div class="preview">

The Pulse section has been removed from the Preview environment. You can update goals by accessing the goal page. For information, see 
[Update goals in the Goal details section in Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md). 

</div>

You can add comments to goals in the Pulse section of Workfront Goals, as part of reviewing goals that might affect yours. For information about reviewing goals in the Pulse section, see [Review goals in the Adobe Workfront Goals Pulse section](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goals-in-pulse.md).

You can also like goal comments that other users have added to mark your approval of them in the Pulse section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner))

   This opens the Workfront Goals area. 

1. Click the Pulse section in the left panel.

   ![](assets/pulse-icon-left.png)

   All current goals display in this section, regardless of their status.

1. Click **Add a comment**, then type your comment in the **Add a comment to this goal (optional)** field.
1. Click **Post**.

   Three comments display by default under each goal.

1. Click **Show all updates** to display all comments on a goal. A number of total comments for the goal also displays. Comments display in the order they were entered, with the most recent first. 
1. (Optional) Click the **Like icon** ![](assets/like-icon.png) to like a comment. The icon updates with the number of likes. 

1. (Optional) Click the number of likes next to a comment and a list with the names of the users who liked the comment displays in the right panel.

   ![](assets/list-of-likes-users-350x121.png)

1. (Conditional) Click **Back to Updates** to return to the Updates tab of the Goal Details panel, or click the **X icon** in the upper-right corner to close the right panel.

-->

<!--
Locating goal comments differs depending on what environment you use. 

### Locate goal comments in the Production environment

You can add comments to goals in the following areas of Workfront Goals:

* The Goal Details panel
* The Check-in section 
* The Pulse section

Although the process for adding comments to goals is similar in these areas, there are differences in being able to edit, delete, or react to a comment when using one area versus another. When you enter a comment in any of these areas, the comment is visible in all areas where goal comments display.

>[!NOTE]
>
>You cannot add comments to results and activities.

-->

<!--
## Add comments to goals in the Goal Details panel

Adding comments to goals differs depending on what environment you use.

### Add comments to goals in the Production environment


You can add comments to goals in the Goal Details panel, as part of updating an individual goal.

You can edit or delete a comment that you entered in this area, or you can like comments.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner))
   

   This opens the Workfront Goals area. 

1. Locate the goal you want to add comments to, then click its name to open the Goal Details panel to the right. 
1. Click the **Updates** tab.
1. Type your comment in the **Comment here** field, then click **Post**. 
1. (Optional and conditional) Select the **Comments** option at the top of the list to view your comment at the top of the list. It is enabled by default and comments display here with the most recent comment first. 
1. (Optional) Click **Edit** to edit your comment, then click **Save** to save your changes, or **Cancel** to revert to the original update.

   >[!TIP]
   >
   >* You can only edit comments you entered. 
   >* There is no time limit for how long after you enter a comment you are allowed to edit it.

1. (Optional) Click **Delete** to delete your comment, then click **Yes, Delete** to confirm.

   >[!TIP]
   >
   >* You can only delete comments you entered. 
   >* There is no time limit for how long after you enter a comment you are allowed to delete it.

1. (Optional) Click the **Like icon** ![](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes. 

1. (Optional) Click the number of likes next to a comment and a list with the names of the users who liked the comment displays in the right panel.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this functionality might change)</p>
   

   ![](assets/list-of-likes-users-350x121.png)

1. (Conditional) Click **Back to Updates** to return to the Updates tab of the Goal Details panel, or click the **X icon** in the upper-right corner to close the right panel.

-->