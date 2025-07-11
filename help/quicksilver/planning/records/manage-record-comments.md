---
title: Administrar comentarios de registro
description: Puede colaborar en registros de Adobe Workfront Planning añadiendo comentarios o respuestas en el panel derecho de un registro. También puede ver otros cambios realizados en el registro y registrados por el sistema en esta área.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 60f2890e431065d0eb034a9254680e43a51ecab8
workflow-type: tm+mt
source-wordcount: '1045'
ht-degree: 54%

---

# Administrar comentarios de registros

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede colaborar en registros de Adobe Workfront Planning añadiendo comentarios o respuestas en el panel derecho de un registro. También puede ver otros cambios realizados en el registro y registrados por el sistema en esta área.

El panel derecho de un registro muestra las siguientes secciones:

* **Comentarios**: muestra comentarios y respuestas que los usuarios añaden a los registros.
* **Historial**: muestra los cambios registrados por el sistema que los usuarios realizan en los campos del registro. Para obtener más información, consulte [Información general sobre la sección Historial](/help/quicksilver/planning/records/history-section-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Licencia de colaborador o superior</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Ver permisos superiores a un área de trabajo <span class="preview"> y tipo de registro </span> </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya las áreas de planificación.</p>
   <div class="preview">
<p> En el entorno de vista previa, a los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.</p>

<p>Los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</p></div>

<p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Crear y administrar plantillas de diseño</a>.</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Consideraciones acerca de los comentarios en un registro

* Puede añadir comentarios y respuestas a registros en Workfront Planning, en la sección Comentarios de un registro.

* Los comentarios añadidos a los registros vinculados no se muestran en los registros desde los que está vinculando. Por ejemplo, si comenta un registro de producto de Workfront Planning vinculado a un registro de campaña, el comentario solo se muestra en el registro de producto de Workfront Planning y no en el registro de campaña desde el que está vinculando.

* Puede añadir comentarios a los registros de Workfront Planning creados como resultado de una conexión entre un registro y un objeto de otra aplicación.

  Por ejemplo, puede realizar comentarios en el registro de Project Workfront Planning después de conectar proyectos de Workfront con registros de Workfront Planning. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Los comentarios añadidos a objetos vinculados en otras aplicaciones no se muestran en Workfront Planning y los comentarios añadidos a objetos vinculados en Workfront Planning no se muestran en otras aplicaciones.

  Por ejemplo, los comentarios añadidos a proyectos en Workfront no se muestran en el mismo proyecto vinculado a una campaña en Workfront Planning y los comentarios añadidos al proyecto en el registro de Workfront Planning no se muestran en Workfront.

* Puede etiquetar usuarios o equipos para que llamen su atención sobre una actualización. Tanto los usuarios etiquetados de forma individual como los usuarios de los equipos etiquetados reciben una notificación dentro de la aplicación y un correo electrónico sobre la actualización.

  >[!NOTE]
  >
  >   Solo los usuarios de clientes que han incorporado con la experiencia unificada de Adobe reciben una notificación dentro de la aplicación y una notificación por correo electrónico. Para determinar si su empresa utiliza la experiencia unificada de Adobe, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Puede añadir una actualización a los registros y revisar el historial de cambios desde las siguientes áreas de Workfront Planning:

   * Desdes la página de detalles del registro.
   * Desde una vista, en el cuadro de detalles del registro.

### Administración de comentarios en registros

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran en tarjetas.

1. Haga clic en una tarjeta de tipo de registro.
Se abre la página de tipo de registro y se muestran todos los registros de ese tipo.

1. Elija una vista de tabla en el menú desplegable **Ver**.
1. Haga clic en el nombre de un registro en la vista de tabla.

   Se abre la página **Detalles** del registro. El área Comentarios se abre de forma predeterminada en el panel derecho.

1. (Condicional) Si el panel derecho no se abre de manera predeterminada, haga clic en el icono **Mostrar comentarios** ![Mostrar icono de comentarios](assets/show-comments-icon.png) en la esquina superior derecha para abrir la sección Comentarios.

1. Empiece a escribir un comentario en el cuadro **Nuevo comentario**.

   ![Cuadro de comentarios vacío en el registro](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Si sale de la sección Comentarios antes de terminar de escribir y enviar un comentario, el comentario en la página se mantiene en modo de borrador incluso después de cerrar la sesión y volver a iniciarla. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Opcional) Para deshacer o rehacer un cambio, utilice las siguientes teclas de método abreviado:
   * CTRL + Z (⌘+z para Mac) para deshacer un cambio
   * CTRL + Y (⌘+y para Mac) para rehacer un cambio
1. (Opcional y condicional) Si la instancia de Workfront forma parte de la experiencia unificada de Adobe, agregue **@** seguido del nombre de un usuario o de un equipo para etiquetarlos en la actualización. Para obtener más información, vea la sección [Consideraciones acerca de comentar un registro](#considerations-about-commenting-on-a-record) en este artículo.

1. (Opcional) Utilice las opciones de la barra de herramientas Texto enriquecido para dar formato al texto, agregar emojis o vínculos a la actualización con el fin de mejorar el contenido.

   >[!TIP]
   >
   >No se pueden agregar imágenes a un comentario de registro.


1. Continúe agregando comentarios al registro.

   Para obtener más información sobre cómo actualizar objetos, incluidos los registros de Workfront Planning, vea [Actualizar trabajo](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Haga clic en el icono **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha del comentario y, a continuación, haga clic en **Eliminar** para eliminar el comentario.
1. (Opcional) Haga clic en el icono **Ocultar comentarios** ![Ocultar comentarios](assets/hide-comments-icon.png) para cerrar el panel derecho.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ..** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## Resumen de la sección Historial

Puede revisar los cambios realizados en el registro en la sección Historial del panel derecho de un registro.

Para obtener más información, consulte [Información general sobre la sección Historial](/help/quicksilver/planning/records/history-section-overview.md).
