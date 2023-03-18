---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Actualizar trabajo
description: Puede añadir una actualización en un objeto de Adobe Workfront (proyecto, tarea o problema) para comunicar el progreso del objeto. Los usuarios asignados o suscritos al objeto pueden ver la actualización. También puede etiquetar a los usuarios para que pongan su atención en la actualización.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 1%

---

# Actualizar trabajo

<!-- Drafted for commenting experience: 

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the way you update work when using the Updates section of an object. 
>You can access the new design by enabling the commenting Beta. 
>Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

Puede agregar comentarios a la mayoría de los objetos de Adobe Workfront en la sección Actualizaciones . Para obtener más información sobre los objetos que muestran la sección Actualizaciones , consulte [Información general sobre la sección Actualizaciones](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

Puede añadir una actualización en un objeto de Workfront (proyecto, tarea o problema) para comunicar el progreso del objeto, al comentar el objeto. Los usuarios asignados o suscritos al objeto pueden ver la actualización. También puede etiquetar a los usuarios para que pongan su atención en la actualización. Los usuarios etiquetados recibirán una notificación en la aplicación y un correo electrónico sobre su actualización.

La información de esta página describe cómo se pueden comentar los objetos de Workfront y cómo se actualizan los proyectos, las tareas y los problemas. Para obtener información sobre cómo comentar objetivos, consulte [Administrar comentarios de objetivo en objetivos de Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md). Debe tener una licencia adicional para acceder a los objetivos de Workfront.


Puede agregar una actualización a proyectos, tareas y problemas desde las siguientes áreas de Workfront:

* Desde un objeto Workfront, en la sección Actualizaciones
* Desde el área de inicio (para tareas y problemas)
* Desde el panel Resumen de una lista de objetos (para tareas y problemas)
* Desde el parte de horas (para tareas y problemas)

## Requisitos de acceso

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td> <p>Ver o editar acceso para el objeto en el que se encuentra la actualización</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar una actualización a un elemento de trabajo

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects

Adding an update to a work item differs depending on what version of the Updates section and what object you choose. 

### Add an update to a work item in the current Updates section

>[!NOTE]
>
>The following functionality is available for all objects except for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. Vaya al elemento de trabajo para el que desea proporcionar una actualización (como un proyecto, una tarea o un problema).
1. Haga clic en el **Actualizaciones** para obtener más información.
1. Haga clic en **Iniciar una nueva actualización,** a continuación, escriba la actualización.
1. (Opcional) Use texto enriquecido o agregue emojis, vínculos o imágenes a la actualización para mejorar el contenido. Para obtener más información, consulte la sección &quot;Usar texto enriquecido en una actualización de Workfront&quot; en este artículo
1. (Opcional) Actualice cualquiera de la siguiente información sobre el elemento de trabajo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notificar</strong></td> 
      <td>Identifique a los usuarios a los que se debe notificar la actualización. Los usuarios asignados o suscritos al objeto reciben automáticamente una notificación cuando se realiza una actualización.<br><p>Para obtener información sobre cómo incluir otros en una actualización, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar otros en actualizaciones</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de confirmación</strong></td> 
      <td>En el selector de fechas, seleccione la fecha en la que se ha comprometido a completar el elemento de trabajo. Para obtener información sobre la fecha de confirmación, consulte <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Resumen de la fecha de confirmación</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condición</strong></td> 
      <td>Seleccione una nueva condición para la tarea o el problema. Para obtener información sobre cómo seleccionar una condición, consulte <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Actualizar condición para tareas y problemas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong></td> 
      <td>Haga clic en la flecha situada junto al estado actual y, a continuación, seleccione el estado que desee en el menú desplegable. Para obtener información sobre la configuración de un estado, consulte <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Actualizar estado de tarea</a>.<p>Actualizar el estado de un elemento de trabajo no cambia automáticamente el estado de un proyecto. Según la configuración del proyecto, es posible que tenga que actualizar el estado del proyecto por separado. Para obtener más información sobre los distintos tipos de actualizaciones del proyecto, consulte <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p><p><b>NOTA</b>

   No se puede cambiar el estado de un elemento de trabajo mientras esté en estado Pendiente de aprobación.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Barra de finalización</strong></td> 
      <td>(Solo disponible en las tareas) Indique el porcentaje de trabajo completado deslizando la barra de progreso al porcentaje deseado. También puede hacer doble clic en la barra de finalización e introducir el porcentaje completado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Privado para mi compañía</strong></td> 
      <td> <p>Deshabilite esta opción para evitar que los usuarios fuera de la empresa tengan acceso a esta actualización.</p> 
      <p><b>NOTA</b></p>
      <p>Esta opción solo se muestra cuando el usuario está asociado con una empresa.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Actualizar** para agregar la actualización al objeto Workfront.

   >[!NOTE]
   >
   >Después de hacer clic en , aparecerá una pequeña ventana emergente durante siete segundos **Actualizar**, lo que le permite deshacer la actualización y volver al panel de edición antes de publicar la actualización. La actualización se publicará si descarta la ventana emergente de deshacer, espera a que desaparezca o sale de la página.
   >
   >Si el administrador de Workfront selecciona el ajuste &quot;No permitir que los usuarios eliminen comentarios&quot; en el nivel de acceso, no podrá deshacer ningún comentario. Para obtener más información, consulte [Crear y modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Para responder a una actualización, consulte [Responder a las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--

### Add an update to a work item using the commenting Beta experience


>[!NOTE]
>
>The functionality described in this section is available for the following objects:
>
>* <span class="preview">Issues, when you enable the commenting Beta experience.</span>
>
>   <span class="preview">This functionality is available only for the Updates section of issues, and it is not available for the following areas:</span>
>
>   * <span class="preview">Home</span>
>   * <span class="preview">Summary panel in lists</span>
>   * <span class="preview">Summary panel in timesheets</span>
>* Goals
>
>   The commenting experience Beta is the default current experience for goals.
>   You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


1. Locate the object you want to update, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Click **Try out the commenting Beta** button in the lower-right corner of the Updates area, then click **Agree** on the Beta agreement. This switches the Updates area to the commenting Beta experience. 
   The **Comments** tab is selected by default. 
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any of the following options from the **Rich Text** toolbar to enhance your text: 

   * Bold
   * Italics
   * Underline
   * Link
   * Bulleted List
   * Numbered List
   * Add attachment (mark this parenthesis as draft: ************ this might be renamed)
   
   For more information, see the "Use Rich Text in a Workfront update" section in this article.

   >[!TIP]
   >
   >   If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
   >
   > ![](assets/real-time-new-red-indicator-unified-commenting.png)



1. Click **Submit** to add the update to the Workfront object. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment, or remove any of the tagged users. 
   You can edit your comment within 15 from submitting it. An "Edited" indicator is added to the left of the date stamp that displays when the comment was updated. 

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********). For information about replying to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Optional) Click the **Like** icon![](assets/like-icon.png). The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When the object or any of its children are updated, Workfront generates a note about that update and displays it in the System Activity tab. 

   For more information see [Updates section  overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >You cannot add a comment to a system update.
-->


## Usar texto enriquecido en una actualización de Workfront

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.

>[!NOTE]
>
>Some of the options in the Rich Text toolbar are not available for the commenting Beta experience.-->


Puede mejorar las actualizaciones mediante el uso de texto enriquecido o agregándole varios elementos, como emojis, vínculos o imágenes.

1. Vaya al área Actualizaciones y empiece a escribir un comentario.
1. (Opcional) Para agregar formato de texto enriquecido a la actualización, utilice cualquier atributo de la variable **Texto enriquecido** mientras escribe.

   | **Atributo** | **Botón de barra de herramientas** | **Teclas de acceso directo de Mac** | **Teclas de acceso directo de PC** |
   |---|---|---|---|
   | Negrita | ![mceclip10.png](assets/mceclip10.png) | función + b | Ctrl + B |
   | Cursiva | ![mceclip9.png](assets/mceclip9.png) | función + i | Ctrl + I |
   | Subrayado | ![mceclip8.png](assets/mceclip8.png) | Alt + u | Ctrl + U |
   | Hipervínculo | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl + K |
   | Lista con viñetas | ![mceclip6.png](assets/mceclip6.png) | Ctrl + Mayús + 8 | Ctrl + Mayús + 8 |
   | Lista numerada | ![mceclip5.png](assets/mceclip5.png) | Ctrl + Mayús + 7 | Ctrl + Mayús + 7 |
   | Cita en bloqueo | ![](assets/block-quote-icon-large.png) | Ctrl + Mayús + 9 | Ctrl + Mayús + 9 |

   Para detener el formato de texto, anule la selección del atributo en la **Texto enriquecido** barra de herramientas.

   >[!NOTE]
   >
   >* El formato también se muestra en cualquier notificación de correo electrónico que los usuarios reciban con la actualización.
   >* El formato de texto enriquecido aplicado a una actualización en un correo electrónico no se muestra en la actualización cuando se ve en la pestaña Actualizaciones .
   >* Si su organización utiliza Workfront con Internet Explorer, cualquier texto con formato pegado en una actualización perderá su formato de texto enriquecido y se mostrará como texto sin formato. Puede cambiar el formato del texto con los atributos de la barra de herramientas Texto enriquecido.
   >* El formato de texto enriquecido no está disponible para las actualizaciones realizadas en el área Hojas de horas ni para los objetos Nota y Última condición que se ven en un informe.


1. (Opcional) Si desea incluir texto de actualizaciones anteriores o de otras fuentes y distinguirlo de su propia actualización, puede marcarlo como una cotización de bloque. Haga clic en el **Comilla de bloque** icono ![](assets/block-quote-small.png) y escriba el texto que desea citar. El texto citado aparece marcado con una línea gris vertical. Haga clic en el **Comilla de bloque** para volver al formato normal.

   ![](assets/block-quote-marked-350x144.png)

1. (Opcional) Añada emojis a su actualización.

   >[!NOTE]
   >
   >* Workfront no reemplaza los emoticonos de puntuación como :) por emojis.
   >* Los emoticonos no están disponibles para las actualizaciones realizadas en el área Hojas de horas ni para los objetos Nota y Última condición que se ven en un informe.
   >* La función emoji de Workfront utiliza caracteres Unicode y, como tal, solo se muestra en navegadores y sistemas operativos que admiten puntos de código Unicode. Es posible que los usuarios de una plataforma, navegador o versión de sistema operativo diferente a la suya no tengan acceso a los mismos emojis.
   >* Un emoji no compatible se representa mediante una caja en blanco o negro.
   >* Windows 7 solo admite emojis en blanco y negro.
   >* Los emoticones aplicados a una actualización realizada por correo electrónico no se muestran en la actualización cuando se ven en el área Actualizaciones .


1. (Opcional) Para agregar un vínculo URL a fuentes de información adicionales:

   1. Haga clic en la actualización donde desee insertar un vínculo.
   1. En el **Texto enriquecido** , haga clic en la barra de herramientas **Hipervínculo** icono. ![](assets/link-icon.png)

   1. En el **Crear vínculo** que aparece, en **URL**, escriba o pegue la dirección URL del origen al que desea vincular.

   1. En **Texto para mostrar**, escriba o pegue el texto del vínculo.
   1. Haga clic en **Guardar**.

1. (Opcional) Para adjuntar una imagen a la actualización, haga clic en el **Imagen** icono ![](assets/addimageicon-35x32.png) y busque la imagen en el equipo.\
   O\
   Arrastre la imagen al área de actualización.

   >[!NOTE]
   >
   >* El administrador de Workfront debe habilitar la adición de imágenes para poder ver el icono Imagen .
   >* El tamaño máximo del archivo de imagen es de 7 MB. Los tipos de archivo de imagen admitidos son .jpg, .gif y .png.
   >* Las imágenes solo son accesibles desde la ficha Actualizaciones de un objeto y no están disponibles en la ficha Documentos.
   >* Puede enviar una actualización con una imagen sin texto.

1. Haga clic en **Actualizar**  <!--<span class="preview">or **Submit**</span>, in the commenting Beta experience-->.


## Copiar información de actualización

<!--drafted for beta release toggle - remove when copying an update will be available: 

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

Existen varias formas de copiar una actualización. Después de copiar un vínculo, puede compartir el vínculo con otros para dirigirlos a la actualización.

* [Copiar la actualización](#copy-the-update)
* [Copiar el vínculo del subproceso](#copy-the-thread-link)
* [Copiar el vínculo de actualización](#copy-the-update-link)

### Copiar la actualización {#copy-the-update}

Esta opción copia el texto de una actualización específica en el portapapeles.

1. Vaya a la actualización o a la respuesta que desee copiar.
1. Haga clic en el **Más** a continuación, haga clic en **Copiar texto del cuerpo**.

   ![Seleccionar Copiar texto del cuerpo](assets/update-stream-copy-body-text-350x152.png)

### Copiar el vínculo del subproceso {#copy-the-thread-link}

Esta opción copia el vínculo de subproceso completo en el portapapeles para que pueda compartir el subproceso con otros usuarios.

1. Vaya al subproceso de actualización que desea copiar.
1. Haga clic en el **Más** a continuación, haga clic en **Copiar vínculo de subproceso**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Copiar el vínculo de actualización {#copy-the-update-link}

Esta opción copia un vínculo de actualización específico en el portapapeles. Cuando comparte el vínculo de actualización, el usuario que lo sigue ve un borde alrededor de la actualización.

1. Vaya a la actualización o a la respuesta que desee copiar.
1. Haga clic en el **Más** junto a la actualización individual y, a continuación, haga clic en **Copiar vínculo de actualización**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Eliminar una actualización o una respuesta

Según el acceso que le proporcione el administrador de Workfront, es posible que pueda eliminar las actualizaciones añadidas en la ficha Actualizaciones de un objeto. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) en el artículo [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Ningún usuario de Workfront (incluido el administrador de Workfront) puede eliminar las actualizaciones realizadas por otro usuario. Sin embargo, si el nivel de acceso de un usuario le permite eliminar sus propias actualizaciones, el administrador de Workfront puede iniciar sesión como ese usuario y eliminar las actualizaciones que haya realizado. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) y [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Vaya a la actualización o a la respuesta que desee eliminar.
1. Haga clic en el **Más** al lado de la actualización o respuesta que desee eliminar y luego haga clic en **Eliminar**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. En el mensaje que aparece, haga clic en **Confirmar** <!--<span class="preview">or **Delete**</span>, in the commenting Beta experience-->.

>[!NOTE]
>
>Al eliminar una actualización con una imagen adjunta, se eliminan el comentario y la imagen.

## Agregar una actualización a un parte de horas

1. Vaya a un parte de horas en el que desee actualizar.
1. Haga clic en el parte de horas para abrirlo.
1. En la parte inferior del parte de horas, haga clic en **Incluir un comentario**.
1. En el cuadro que aparece en la parte inferior del parte de horas, escriba una actualización.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Condicional) Para guardar la actualización sin enviar el parte de horas para su aprobación, haga clic en **Guardar para después**.

   O

   Para guardar la actualización y enviar el parte de horas para su aprobación, haga clic en **Enviar para aprobación**.

   O

   Si el parte de horas no está configurado con un aprobador, haga clic en **Guardar y cerrar parte de horas** para guardar la actualización.

## Habilitar o deshabilitar actualizaciones del sistema

<!--remove preview with 23.2 production: 

<div class="preview">
>[!NOTE]
>
>It is not possible to disable system updates when using the Beta commenting experience. 
>The information in this section refers only to functionality available in the current Updtes section. 
>For more information about system updates in the Beta version, see [Updates section overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md) 
</div>
-->

La sección Actualizaciones de un objeto Workfront muestra dos tipos de información:

* **Actualizaciones de usuario:** Las actualizaciones de usuario son comentarios que usted y otros usuarios del sistema introducen.

   ![](assets/user-update-cl-350x277.png)

* **Actualizaciones del sistema:** Las actualizaciones del sistema registran la eliminación de recursos, la adición o eliminación de versiones, la incorporación o eliminación de una solicitud de aprobación, así como cualquier edición o cambio realizado en los documentos del objeto.

   ![](assets/system-updates-cl-350x277.png)

Según la licencia de Workfront, las actualizaciones del sistema podrían estar habilitadas de forma predeterminada. Los administradores de Workfront pueden determinar el seguimiento que se realiza en las actualizaciones del sistema, tal como se explica en [Actualizaciones rastreadas por el sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). También puede filtrar actualizaciones del sistema o actividades para que solo vea actualizaciones del usuario para todos los objetos.

Para obtener más información sobre la diferencia entre las actualizaciones de usuario y sistema, consulte [Actualizaciones rastreadas por el sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Para habilitar o deshabilitar las actualizaciones del sistema:

1. Haga clic en el **Actualizaciones** en un objeto.
1. Haga clic en **Mostrar actualizaciones del sistema** para deslizar el conmutador a la izquierda (desactivado) o a la derecha (activado).

   ![](assets/show-system-updates-qs-350x55.png)

   Esta opción es persistente en todos los objetos de Workfront y permanece en la posición seleccionada, incluso si se cierra la sesión de Workfront.

