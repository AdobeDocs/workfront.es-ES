---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Actualizar trabajo
description: Puede agregar una actualización a un objeto de Adobe Workfront (proyecto, tarea o problema) para comunicar el progreso del objeto. Los usuarios asignados o suscritos al objeto pueden ver la actualización. También puede etiquetar usuarios para que llamen su atención sobre la actualización.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 73f339b54985b725f265d582992a43b9f80dbd7c
workflow-type: tm+mt
source-wordcount: '3075'
ht-degree: 0%

---

# Actualizar trabajo

<!-- Audited: 1/2024 -->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>  (*****for all customers or in Production for customers who enabled fast releases-->

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

<!--info for April 11: hide the "Important" box below-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span>
-->

Puede agregar una actualización a un objeto de Adobe Workfront agregándole un comentario para informar a otros usuarios sobre el estado o el progreso del objeto, o para solicitar más información o recursos adicionales.

Para obtener más información sobre los objetos a los que se pueden agregar actualizaciones en Workfront, consulte [Información general sobre la sección Actualización](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

La información de este artículo describe cómo puede realizar comentarios sobre proyectos, tareas y problemas. Los usuarios asignados al objeto o suscritos a él pueden ver la actualización. También puede etiquetar usuarios para que llamen su atención sobre la actualización.

Agregar comentarios a otros objetos de Workfront es similar a actualizar proyectos, tareas y problemas.

Para obtener información adicional sobre cómo comentar tarjetas, objetivos y registros en Workfront Planning, consulte los siguientes artículos:

* [Administrar comentarios sobre metas en Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).

  Debe tener una licencia adicional para acceder a los objetivos de Workfront.

* [Añadir una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)

* [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)

* [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
   <p>Actual: Solicitud o superior para problemas y documentos; Revisar o superior para todos los demás objetos</p>
   <p>Nuevo: Colaborador o superior para problemas y documentos: Ligero o superior para todos los demás objetos</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Acceso de visualización o edición para el objeto en el que se encuentra la actualización</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre los comentarios en objetos

* Puede agregar comentarios a la mayoría de los objetos de Adobe Workfront en la sección Actualizaciones. Para obtener más información acerca de los objetos que muestran la sección Actualizaciones, vea [Información general sobre la sección Actualizaciones](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Puede agregar comentarios a objetos de Workfront desde otras aplicaciones integradas con Workfront o desde la aplicación móvil de Workfront.

  No todas las aplicaciones integradas con Workfront pueden agregar comentarios a objetos de Workfront.

  No todas las funciones disponibles en la sección Actualizaciones de un objeto de Workfront están disponibles en otras aplicaciones al acceder a objetos de Workfront desde la aplicación. Por ejemplo, es posible que las funciones de texto enriquecido o hacer que un comentario sea privado para la compañía de otra persona no estén disponibles cuando se agregan comentarios a un objeto de Workfront desde una aplicación de terceros.

* Puede comunicar el progreso de un objeto de Workfront (proyecto, tarea o problema) mientras realiza comentarios sobre el objeto. Los usuarios asignados o suscritos al objeto pueden recibir una notificación sobre la actualización. Cualquier persona con acceso de tipo Ver en el objeto puede ver la actualización.

* Puede etiquetar a los usuarios para que presten atención a la actualización. Los usuarios etiquetados reciben una notificación en la aplicación y un correo electrónico sobre su actualización.

  >[!TIP]
  >
  >Los propietarios de los comentarios se etiquetan automáticamente. Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).


* Puede agregar un comentario a un objeto que pueda ver, o bien puede iniciar sesión como Workfront o administrador de grupo y agregar un comentario en nombre de otro usuario. Para obtener más información, vea [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Puede agregar una actualización a proyectos, tareas y problemas desde las siguientes áreas de Workfront:

   * Desde un objeto de Workfront, en la sección Actualizaciones (para proyectos, tareas y problemas)
   * Desde el área de Inicio (para tareas y problemas)

     Para obtener más información, consulta [Administrar tu trabajo con el widget Mi trabajo](/help/quicksilver/workfront-basics/using-home/new-home/my-work-widget.md).
   * En el panel Resumen, en las siguientes áreas (para tareas, problemas y documentos):

      * Una lista de objetos
      * Una hoja de horas
      * Inicio
      * Distribuidor de cargas de trabajo

     Para obtener más información, consulte los siguientes artículos:

      * [Resumen, descripción general](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
      * [Actualizar los elementos de trabajo en el Distribuidor de cargas de trabajo mediante el Resumen](/help/quicksilver/resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

<!--info for April 11: hide the section below: add an update to a work item-->

<!--
## Add an update to a work item

Adding an update to a work item differs depending on what version of the Updates section you use.

You can add updates to the following objects: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--info for April 11: hide the section below completely:-->

<!--
### Add an update to a work item in the legacy Updates section

>[!IMPORTANT]
>
>The information on this page describes how you update projects, tasks, and issues.

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. (Conditional) If it is enabled, click the **New commenting** option in the upper-right corner of the Updates section to disable it and enable the legacy commenting experience.
1. Click **Start a new update,** then type your update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the [Use Rich Text in a Workfront update](#use-rich-text-in-a-workfront-update) section in this article.
1. (Optional) Update any of the following information about the work item:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who must be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> 
      <p><b>NOTE</b></p>
      <p>This option displays only when the user is associated with a Company.</p>
      <p>This option is not available in all areas where you can add updates from. For example, this is not available in third-party applications where you can add updates from. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update is posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
-->

<!--info for April 11: reword the title of this section to: "Add an update to a work item"; take out the step that says you need to enable the "New commenting" toggle (I think it is step 3??)-->

## Agregar un comentario a un elemento de trabajo

Este artículo describe cómo actualizar proyectos, tareas o problemas. La actualización de la mayoría de los demás objetos es similar.

1. Busque el objeto al que desea agregar un comentario y, a continuación, haga clic en su nombre para abrir la página del objeto.
1. Haga clic en **Actualizaciones** en el panel izquierdo.
La ficha **Comentarios** está seleccionada de forma predeterminada.

1. Empiece a escribir un comentario en el cuadro **Nuevo comentario**.

   ![Nuevo cuadro de comentarios](assets/comment-box-all-tabs.png)

   >[!TIP]
   >
   >Si sale de la sección Actualizaciones antes de terminar de escribir y enviar un comentario, el comentario en la página se mantiene en modo de borrador incluso después de cerrar la sesión y volver a iniciarla. Todas las imágenes que se agreguen al comentario también se guardarán en el borrador. Los borradores se guardan durante 7 días después de los cuales se descartan y no se pueden recuperar. Los comentarios redactados solo son visibles para el usuario que los escribe.

1. (Opcional) Para deshacer o rehacer un cambio, utilice las siguientes teclas de método abreviado:
   * CTRL + Z (⌘ + z para Mac) para deshacer un cambio
   * CTRL + Y (⌘ + y para Mac) para rehacer un cambio

1. (Opcional) En el área **Etiquetar personas o equipos**, empiece a escribir el nombre o el correo electrónico de un usuario o equipo que desee incluir en este comentario y, a continuación, selecciónelo cuando se muestre en la lista.
1. (Opcional) Utilice las opciones de la barra de herramientas Texto enriquecido para dar formato al texto, agregar emojis, vínculos o imágenes a la actualización para mejorar el contenido. Para obtener más información, consulte la sección [Usar texto enriquecido en una actualización de Workfront](#use-rich-text-in-a-workfront-update) en este artículo.

   >[!TIP]
   >
   >Si otro usuario envía un comentario al mismo elemento que está actualizando, existe una línea roja con un indicador &quot;Nuevo&quot; para informarle de los comentarios más recientes.
   >
   >El indicador solo se muestra después de que se haya enviado el comentario sobre el elemento y no cuando el comentario aún está compuesto.
   >
   >El indicador &quot;Nuevo&quot; solo se muestra cuando el usuario que ha introducido una nueva actualización, así como el usuario que está introduciendo una actualización, están utilizando la nueva experiencia de comentarios.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Haga clic en **Enviar** para agregar la actualización al objeto de Workfront.
1. (Opcional) Para editar un comentario, haga clic en el menú **Más** ![](assets/more-menu.png) en la esquina superior derecha del comentario y luego haga clic en **Editar**.

   >[!IMPORTANT]
   >
   >Solo puede editar su comentario en los 15 minutos siguientes al envío.

1. Edite la información del comentario, añada o elimine imágenes, o bien elimine cualquiera de los usuarios etiquetados. Se agrega un indicador &quot;Editado&quot; a la izquierda de la marca de fecha que se muestra cuando se introdujo el comentario.

   >[!TIP]
   >
   >Los comentarios del año actual no muestran el año en el sello de fecha. Al pasar el ratón por encima de una marca de tiempo, se muestra la fecha completa, incluido el año.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Se genera un correo electrónico para notificar a los usuarios de su actualización solo cuando envía la actualización original. No se genera ningún correo electrónico después de editar la actualización.
   >* La marca de fecha que aparece junto al comentario es la fecha del comentario original, no la fecha de la última edición.
   >* Cuando agrega un comentario en nombre de otro usuario (cuando inicia sesión como otro usuario como Workfront o administrador de grupo), no puede editar el comentario si ha iniciado sesión como el otro usuario. Solo puede editar el comentario después de cerrar la sesión como usuario y volver a iniciarla como usuario.

1. (Opcional) Haga clic en **Responder** o empiece a escribir un comentario en el área **Agregar respuesta...** para responder a un comentario existente y, a continuación, siga los pasos del 3 al 7 anteriores. <!--(**************insure this stays accurate***********)--> Para obtener información acerca de cómo responder a una actualización, vea [Responder a actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

1. (Condicional y opcional) Si otros usuarios han agregado comentarios que se muestran fuera del área visible en la sección Actualizaciones mientras agregaba los comentarios, haga clic en **Ver** dentro del **titular de comentarios nuevos** azul en la parte inferior de la pantalla para mostrar estos comentarios.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Los comentarios adicionales se muestran en la parte inferior de la pantalla.

1. (Opcional) Haga clic en el icono **Me gusta**![](assets/like-icon.png). El icono se actualiza con el número de me gusta.
1. (Condicional y opcional) Si ha incluido más personas en el comentario, haga clic en el número de miembros incluidos en la actualización para mostrar una lista de entidades con las que se comparte el comentario que ha escrito.

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >Los nombres de las dos primeras entidades etiquetadas se muestran junto a sus avatares. Si se etiquetan más de dos entidades, solo se mostrará el nombre de la primera y el número de entidades adicionales.

1. (Opcional) Haga clic en el nombre de un comentarista para ver su nombre, función y dirección de correo electrónico en un cuadro de información. Vuelva a hacer clic en el nombre del comentarista en el cuadro de información para abrir su perfil de usuario.
1. (Opcional) Haga clic en la ficha **Actividad del sistema** para ver las actualizaciones registradas por el sistema. Cuando se actualiza el objeto o cualquiera de sus elementos secundarios, Workfront genera una nota sobre esa actualización y la muestra en la pestaña Actividad del sistema.

   Para obtener más información, consulte [Información general sobre la sección de actualizaciones](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

   >[!TIP]
   >
   >No puede agregar un comentario a una actualización del sistema. Sin embargo, todas las respuestas que se realizaron a los registros de actividad del sistema en la experiencia de comentarios heredada se agregaron a la pestaña Actividad del sistema como de solo lectura. La experiencia de comentarios heredada se eliminó de Workfront el 11 de abril de 2024.

1. (Opcional) Haga clic en la ficha **Todos** para ver los comentarios del usuario y los comentarios de la actividad del sistema en un solo lugar. Esta es una pestaña de solo vista.

   >[!TIP]
   >
   >No puede responder a comentarios ni etiquetar a otros usuarios en comentarios existentes en la pestaña Todos. Para responder a un comentario en la ficha Todos, haga clic en **Responder en Comentarios** para abrir el comentario en la ficha Comentarios.

## Utilizar texto enriquecido en un comentario de Workfront{#use-rich-text-in-a-workfront-comment}

Puede mejorar los comentarios mediante Texto enriquecido o agregándole varios elementos, como emojis, vínculos o imágenes.

1. Vaya al área de **Actualizaciones** de un objeto de Workfront, abra la pestaña **Comentarios** y empiece a escribir un comentario.
1. (Opcional) Para agregar formato de texto enriquecido al comentario, utilice los atributos de la barra de herramientas **Texto enriquecido** mientras escribe.

   ![](assets/rich-text-toolbar.png)

   | **Atributo** | **Botón Barra de herramientas** | **Teclas de método abreviado de Mac** | **Teclas de método abreviado de Windows** |
   |---|---|---|---|
   | Negrita | ![](assets/mceclip10.png) | ⌘ + b | Ctrl + B |
   | Cursiva | ![mceclip9.png](assets/mceclip9.png) | ⌘ + i | Ctrl + I |
   | Subrayado | ![mceclip8.png](assets/mceclip8.png) | ⌘ + u | Ctrl + U |
   | Hipervínculo | ![mceclip7.png](assets/mceclip7.png) | <br>Para abrir el cuadro Agregar vínculos: ⌘+K</br> <br>Para pegar un vínculo sobre el texto seleccionado: ⌘+V</br> | <br>Para abrir el cuadro Agregar vínculos: Ctrl+K</br> <br>Para pegar un vínculo sobre el texto seleccionado: Ctrl+V</br> |
   | Lista con viñetas | ![mceclip6.png](assets/mceclip6.png) | ⌘ + Mayús + 8 | Ctrl + Mayús + 8 |
   | Lista numerada | ![mceclip5.png](assets/mceclip5.png) | ⌘ + Mayús + 7 | Ctrl + Mayús + 7 |

   <!--| Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |<br>Ctrl+Shift+9</br> <br>This is not available in the new commenting experience. </br> |-->

   <!--remove the last row when we remove legacy from the system-->

   Para detener el formato del texto, anule la selección del atributo en la barra de herramientas **Texto enriquecido**.


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* El formato también se muestra en cualquier notificación por correo electrónico que reciban los usuarios y que contenga la actualización.
   >* El formato de texto enriquecido aplicado a una actualización en un correo electrónico no se muestra en la actualización cuando se ve en la pestaña Actualizaciones.
   >* Si su organización utiliza Workfront con Internet Explorer, cualquier texto con formato pegado en una actualización perderá su formato de texto enriquecido y se mostrará como texto sin formato. Puede cambiar el formato del texto mediante los atributos de la barra de herramientas Texto enriquecido.
   >* El formato de texto enriquecido no está disponible para las actualizaciones realizadas en el área Plantillas de horas ni para los objetos Nota y Última condición visualizados en un informe.

   <!--1. (Optional and conditional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting. This is not available in the new commenting experience.-->

   <!--remove this picture below and the bullet above when we remove legacy-->

   <!--![](assets/block-quote-marked-350x144.png)-->

1. (Opcional) Haga clic en el icono **emoji** ![](assets/emoji-icon.png) para agregar emojis a la actualización.

   >[!NOTE]
   >
   >* Workfront no reemplaza los emoticonos de puntuación como :) por emojis.
   >* Los emojis no están disponibles para los objetos Nota y Última condición que se vieron en un informe.
   >* La función emoji de Workfront utiliza caracteres Unicode y, como tal, solo se muestra en navegadores y sistemas operativos que admiten puntos de código Unicode. Es posible que los usuarios con una versión de plataforma, explorador o sistema operativo diferente a la tuya no tengan acceso a los mismos emojis.
   >* Un emoji no admitido se representa mediante una caja negra o blanca.
   >* Windows 7 solo admite emojis en blanco y negro.
   >* Los emojis que se aplican a una actualización realizada por correo electrónico no se muestran en la actualización cuando se ven en el área de Actualizaciones.

1. (Opcional) Para agregar un vínculo URL a fuentes de información adicionales:

   1. Haga clic en la actualización en la que desee insertar un vínculo.
   1. En la barra de herramientas **Texto enriquecido**, haga clic en el icono **Hipervínculo** ![](assets/link-icon.png).

   1. En el cuadro **Crear vínculo**, en **URL**, escriba o pegue la URL del origen al que desea vincular.

   1. En **Texto para mostrar**, escriba o pegue el texto del vínculo.
   1. Haga clic en **Guardar**.

1. (Opcional) Para adjuntar una imagen a la actualización, realice una de las siguientes acciones:

   * Guarde la imagen en el equipo y arrástrela y suéltela en el área Nuevo comentario.
   * Copie una captura de pantalla del equipo y péguela en el comentario.
   * Haga clic en el icono **Agregar imagen** ![](assets/add-image-mountain-with-plus-icon.png) y busque la imagen en su equipo.


   >[!NOTE]
   >
   >**IMPORTANTE**
   >
   ><!--<span class="preview">You cannot add images to goals or ad-hoc cards on boards.</span> -->
   >
   >* El administrador de Workfront debe habilitar la adición de imágenes en la sección Actualizar preferencias de fuentes del área de Interfaz de Workfront para que pueda ver los iconos Imagen o Agregar datos adjuntos. Para obtener más información, consulte [Configurar preferencias para actualizaciones de usuarios](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* El tamaño máximo de archivo de imagen es de 7 MB. Los tipos de archivo de imagen admitidos son .jpg, .gif y .png.
   >* Se puede acceder a las imágenes desde la sección Actualizaciones de un objeto y también están disponibles en el área Documentos del menú principal.
   >Puede copiar una captura de pantalla del equipo mediante una combinación de teclas o, por ejemplo, la función Imprimir pantalla (en equipos con Windows).
   >* Puede pegar la imagen haciendo clic con el botón secundario en el nuevo comentario y luego haciendo clic en **Pegar**, o presionando CTRL+V para Windows (o ⌘+V para Mac) en el teclado.
   >* Puede enviar una actualización con una imagen y sin texto.
   >* Cuando elimina un comentario que contiene una imagen, la imagen se quita de la sección Actualizaciones y del área Documentos. La imagen también se elimina del área Documentos cuando edita un comentario y elimina la imagen.
   >* Cuando alguien elimina una imagen adjunta a un comentario del área Documentos, también se elimina del comentario.

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. (Opcional) Para ver una imagen en la actualización existente, realice una de las siguientes acciones:

   * Haga clic en el icono **Vista previa** ![](assets/previewimageicon-31x31.png) de la miniatura de la imagen para abrir la imagen a tamaño completo en una nueva pestaña del explorador.
   * Haga clic en el icono **Descargar** ![](assets/downloadimageicon.png) de la miniatura de la imagen para descargar la imagen.

1. Haga clic en **Enviar** para agregar su comentario.

## Buscar una actualización

Puede buscar un comentario o una respuesta en la sección Actualizaciones de un objeto.

1. Vaya a la sección **Actualizaciones** de un objeto.
1. Empiece a escribir una palabra clave <!--or a user's name --> en el cuadro **Buscar** de la esquina superior derecha de la ficha **Comentarios**.

   <!--Add this tip or note instead of the note below - when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   >[!NOTE]
   >
   >Solo puede buscar palabras que pertenezcan al texto de un comentario o respuesta. No puede buscar nombres de usuarios o equipos etiquetados en una actualización.

   ![Buscar en actualizaciones](assets/updates-all-tabs-with-search-field.png)

   La palabra clave <!--or user--> que buscó se resalta y los comentarios que la contienen se muestran en la parte superior de la sección Actualizaciones.

   Workfront busca en todo el flujo de actualización del objeto, fuera de los comentarios visibles en la pantalla.

1. Haga clic en el icono **x** en el campo de búsqueda para borrar los resultados de búsqueda y volver a todos los comentarios.

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## Copiar comentarios

Hay varias formas de copiar un comentario.

Puede copiar un vínculo al comentario o copiar el contenido del comentario para utilizarlo en una nueva actualización.

<!--Copying an update differs depending on which commenting experience you use.-->

<!--info for April 11: take the sentence above out and reword the section title below to: Copy an update-->

### Copiar un comentario

Para copiar información de un comentario existente, siga uno de estos procedimientos:

* [Copiar vínculo](#copy-link)
* [Copiar el texto del cuerpo](#copy-body-text)
* [Cita respuesta](#quote-reply)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### Copiar vínculo a un comentario

La opción Copiar vínculo copia el comentario o el vínculo de subproceso en el portapapeles para que pueda compartir el comentario o todo el subproceso con otros usuarios.

1. Vaya al comentario cuyo vínculo desee copiar.

1. Haga clic en el menú **Más** y luego haga clic en **Copiar vínculo**.

1. Pegue el vínculo copiado en el paso anterior en un correo electrónico u otra aplicación para compartirlo con otros usuarios. El vínculo compartido abre el comentario desde el que compartió el vínculo.

   >[!TIP]
   >
   >Cuando comparte el vínculo de una conversación sobre un objeto secundario desde un objeto de mayor clasificación, el vínculo abre el subproceso en el área Actualizaciones del objeto de mayor clasificación.
   >
   >Por ejemplo, si copia el vínculo de un comentario de tarea desde el área de Actualizaciones del proyecto, el comentario abre la página del proyecto.

#### Copiar el texto del cuerpo

La opción Copiar texto del cuerpo copia el texto de un comentario específico en el portapapeles.

1. Vaya al comentario o la respuesta que desee copiar.
1. Haga clic en el menú **Más** y, a continuación, haga clic en **Copiar texto principal**.

#### Cita respuesta

La opción Respuesta de oferta copia el comentario original en una nueva respuesta como una cita de bloque.

1. Vaya al comentario o la respuesta que desee copiar.
1. Haga clic en el menú **Más** y, a continuación, haga clic en **Citar respuesta**.

   Se abre un nuevo cuadro de comentarios y la respuesta citada se incluye en el nuevo comentario y se marca como una cita de bloque.

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)


1. Continúa agregando tu actualización y haz clic en **Enviar** para agregar el comentario.

<!--info for April 11: hide the entire section below - notice that there are several sub-sub sections below this main section - hide them all, all the way up to "Delete an update"-->

<!--
### Copy an update in the legacy commenting experience

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)
* [Quote Reply](#quote-reply)

   >[!TIP]
   >
   >When you copy and share the link of a conversation on a child object from a higher-ranking object, the link opens the thread in the child object's Updates area. 
   >
   >For example, if you copy the link of a task comment from the project's Updates area, the comment opens the task page.

#### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.

1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png) 

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/copy-update-link-old-ui.png)

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Quote Reply  

The Quote Reply option copies the original comment to a new reply as a block quote. 

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Quote Reply**.

   A new comment box opens and the quoted reply is included in the new comment and marked as a block quote.

1. Continue adding your update and click **Reply** to add the comment.
-->

## Eliminar un comentario o una respuesta

Según el acceso que le proporcione el administrador de Workfront, es posible que pueda eliminar los comentarios que haya agregado en la sección Actualizaciones de un objeto.

Para obtener más información, vea [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) en el artículo [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Ningún usuario de Workfront (incluido el administrador de Workfront) puede eliminar las actualizaciones realizadas por otro usuario. Sin embargo, si el nivel de acceso de un usuario le permite eliminar sus propias actualizaciones, el administrador de Workfront puede iniciar sesión como ese usuario y eliminar las actualizaciones que haya realizado. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) e [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Vaya al comentario o la respuesta que desee eliminar.
1. Haga clic en el menú **Más** que está junto al comentario o la respuesta que desea eliminar y, a continuación, haga clic en **Eliminar**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. En el mensaje que aparece, haga clic en **Eliminar**.

   >[!NOTE]
   >
   >Al eliminar una actualización con una imagen adjunta, se eliminan el comentario y la imagen. Para obtener más información, consulte la sección [Usar texto enriquecido en una actualización de Workfront](#use-rich-text-in-a-workfront-update) en este artículo.

   Cuando el comentario que elimina tiene respuestas asociadas a él, existe una indicación de que el comentario se eliminó con el nombre del usuario que lo eliminó.

   ![](assets/removed-comment-indicator-new-experience.png)

   Los comentarios eliminados se eliminan inmediatamente de Workfront. Un usuario que utiliza la sección Actualizaciones ve un comentario que otro usuario elimina en tiempo real.


## Revisar actualizaciones del sistema

La sección Actualizaciones de un objeto de Workfront muestra dos tipos de información:

* **Actualizaciones de usuarios:** Las actualizaciones de usuarios son comentarios que usted y otros usuarios de su sistema escriben. Las actualizaciones de usuario se muestran en las pestañas Comentarios y Todas de la sección Actualizaciones.

  ![](assets/user-update-cl-350x277.png)

* **Actualizaciones del sistema:** Las actualizaciones del sistema registran la eliminación de tareas o problemas, la adición o eliminación de versiones de documentos, el adjuntado o la eliminación de una solicitud de aprobación, así como las modificaciones o cambios realizados en el objeto. Las actualizaciones del sistema se muestran en las pestañas Actividad del sistema y Todas de la sección Actualizaciones.

  ![](assets/system-updates-cl-350x277.png)

  Los administradores de Workfront pueden determinar qué se rastrea en las actualizaciones del sistema, tal como se explica en [Actualizaciones rastreadas por el sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). También puede filtrar las actualizaciones o actividades del sistema para ver solo las actualizaciones de los usuarios de todos los objetos.

  Los objetos siguientes no tienen actualizaciones generadas por el sistema:

   * Equipo
   * Plantilla
   * Tarea de plantilla
   * Tarjeta ad hoc

Para obtener más información sobre las actualizaciones de usuarios y sistemas y cómo se muestran en la sección Actualizaciones de los objetos de Workfront, consulte [Información general de la sección Actualizaciones](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->