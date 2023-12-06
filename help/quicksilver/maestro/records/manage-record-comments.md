---
title: Administrar comentarios de registro
description: Puede colaborar en los registros de Adobe Maestro agregando actualizaciones y formulando preguntas o respuestas en el área Comentarios de un registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Administrar comentarios de registro

Puede colaborar en los registros de Adobe Maestro agregando actualizaciones y formulando preguntas o respuestas en el área Comentarios de un registro.

## Consideraciones acerca de los comentarios en un registro

* Puede agregar comentarios y respuestas a registros operativos y taxonomías en Maestro, en la sección Comentarios de un registro.

* Los comentarios agregados a los registros vinculados no se muestran en los registros desde los que está vinculando. Por ejemplo, si comenta un proyecto vinculado a un registro de campaña, el comentario sólo se mostrará en el registro de proyecto de Maestro y no en el registro de campaña desde el que está vinculando.

* Los comentarios agregados a objetos vinculados en otras aplicaciones no se muestran en Maestro.
Los comentarios agregados a objetos vinculados en Maestro no se muestran en otras aplicaciones.\
  Por ejemplo, los comentarios agregados a proyectos en Workfront no se muestran en el mismo proyecto vinculado a una campaña en Maestro.

* Puede etiquetar a los usuarios para que presten atención a una actualización. Los usuarios etiquetados no reciben una notificación dentro de la aplicación ni un correo electrónico sobre su actualización. No puede etiquetar equipos en un comentario de Maestro.

  >[!TIP]
  >
  >* Los propietarios de los comentarios no se etiquetan automáticamente en una actualización.
  >
  >* No puede quitar usuarios etiquetados de una actualización cuando responde a ella.

* Puede agregar una actualización a los registros desde las siguientes áreas de Maestro:

   * En la página Detalles.

  <!--* From the table view.-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> producto de Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Maestro. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Cualquiera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nivel de acceso</td>
   <td> <p>Cualquiera</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/grant-access.md">Conceder acceso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### Administración de comentarios en registros

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](assets/dots-main-menu.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Maestro]**.

   El último espacio de trabajo al que se accede se abre de forma predeterminada.
1. Elija una vista de tabla de la **Ver** menú desplegable.
1. Haga clic en el nombre de un registro en la vista de tabla.

   El registro es... **Detalles** se abre la página.

1. Comience a escribir un comentario en **Nuevo comentario** cuadro.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Si sale de la sección Comentarios antes de terminar de escribir y enviar un comentario, el comentario en la página se mantiene en modo de borrador incluso después de cerrar la sesión y volver a iniciarla. Todas las imágenes que se agreguen al comentario también se guardarán en el borrador. Los borradores se guardan durante 7 días después de los cuales se descartan y no se pueden recuperar. Los comentarios redactados solo son visibles para el usuario que los escribe.

1. (Opcional) Para deshacer o rehacer un cambio, utilice las siguientes teclas de método abreviado:
   * CTRL + Z (⌘ + z para Mac) para deshacer un cambio
   * CTRL + Y (⌘ + y para Mac) para rehacer un cambio
1. (Opcional) Añadir **@** seguido del nombre de un usuario para etiquetar a alguien en la actualización.
1. (Opcional) Utilice las opciones de la barra de herramientas Texto enriquecido para dar formato al texto, agregar emojis, vínculos o imágenes a la actualización para mejorar el contenido. Para obtener más información, consulte la sección &quot;Uso de texto enriquecido en una actualización de Workfront&quot; en el artículo [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Si otro usuario envía un comentario al mismo elemento que está actualizando, existe una línea roja con un indicador &quot;Nuevo&quot; para informarle de los comentarios más recientes.
   >
   >El indicador solo se muestra después de que se haya enviado el comentario sobre el elemento y no cuando el comentario aún está compuesto.
   >
   >![](assets/new-line-indicator-comments.png)

1. Clic **Enviar** para agregar la actualización al registro.
1. (Opcional) Para editar un comentario, haga clic en **Más** menú ![](assets/more-menu.png) en la esquina superior derecha del comentario y haga clic en **Editar**.

   >[!IMPORTANT]
   >
   >Solo puede editar su comentario en los 15 minutos siguientes al envío.

1. Edite la información del comentario, añada o elimine imágenes, o bien elimine cualquiera de los usuarios etiquetados. Se agrega un indicador &quot;editado&quot; a la izquierda del comentario.

   >[!TIP]
   >
   >Los comentarios del año actual no muestran el año en el sello de fecha. Al pasar el ratón por encima de una marca de tiempo, se muestra la fecha completa, incluido el año.

1. (Opcional y condicional) Para buscar un comentario existente, empiece a escribir una palabra clave en el cuadro de búsqueda situado en la esquina superior derecha de la etiqueta **Comentarios** área.

   ![](assets/search-box-for-comments-area.png)

1. (Opcional) Haga clic en **Responder** o empiece a escribir un comentario en la **Añadir respuesta...** , para responder a un comentario existente, siga los pasos 4-8 anteriores. <!--(**************accurate??***********)-->

1. (Condicional y opcional) Si otros usuarios han agregado comentarios que se muestran fuera del área visible en la sección Comentarios mientras agregaba los comentarios, haga clic en **Ver** dentro de **titular de nuevos comentarios** en la parte inferior de la pantalla para mostrar estos comentarios.

   ![](assets/new-comments-banner-on-record.png)

   Los comentarios adicionales se muestran en la parte inferior de la pantalla.

1. (Opcional) Haga clic en **Like** para que le guste una actualización o reconozca que la ha leído. El icono se actualiza con el número de me gusta.
1. (Condicional y opcional) Si ha incluido más personas en el comentario, haga clic en los avatares de los usuarios incluidos en la actualización para mostrar una lista de usuarios con los que se comparte el comentario.
1. (Opcional) Haga clic en **Más** icono ![](assets/more-menu.png) en la esquina superior derecha del comentario y haga clic en una de las siguientes opciones para copiar información de un comentario:

   * **Copiar vínculo**: copia un vínculo al comentario en el portapapeles.
   * **Copiar texto del cuerpo** t: copia el texto del comentario en el portapapeles.
   * **Cita respuesta**: copia el contenido del comentario en una nueva respuesta. Las imágenes no se incluyen en la respuesta copiada.

   Para obtener más información, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Opcional) Haga clic en **Más** icono ![](assets/more-menu.png) en la esquina superior derecha del comentario y haga clic en **Eliminar** para eliminar el comentario.

