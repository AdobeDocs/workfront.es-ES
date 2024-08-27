---
title: Administrar comentarios de registro
description: Puede colaborar en registros de Adobe Workfront Planning agregando comentarios o respuestas en el panel derecho de un registro. También puede ver otros cambios realizados en el registro y registrados por el sistema en esta área.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---

# Administrar comentarios de registro

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

Puede colaborar en registros de Adobe Workfront Planning agregando comentarios o respuestas en el panel derecho de un registro. También puede ver otros cambios realizados en el registro y registrados por el sistema en esta área.

El panel derecho de un registro muestra las siguientes secciones:

* **Comentarios**: Muestra comentarios y respuestas que los usuarios agregan a los registros.
* **Historial**: muestra los cambios registrados por el sistema que los usuarios realizan en los campos de registro. Para obtener más información, consulte [Resumen de la sección de historial](/help/quicksilver/planning/records/history-section-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener lo siguiente para poder acceder a Workfront Planning:

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre lo que se incluye en cada plan de Workfront Planning, consulte <a href="https://business.adobe.com/products/workfront/pricing.html">Precios y empaquetado de Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Colaborador, Ligero o Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Ver permisos superiores a un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

## Consideraciones acerca de los comentarios en un registro

* Puede agregar comentarios y respuestas a registros en Workfront Planning, en la sección Comentarios de un registro.

* Los comentarios agregados a los registros vinculados no se muestran en los registros desde los que está vinculando. Por ejemplo, si comenta un registro de producto de Workfront Planning vinculado a un registro de campaña, el comentario solo se muestra en el registro de producto de Workfront Planning y no en el registro de campaña desde el que está vinculando.

* Puede agregar comentarios a los registros de Workfront Planning creados como resultado de una conexión entre un registro y un objeto de otra aplicación.

  Por ejemplo, puede realizar comentarios en el registro de Project Workfront Planning después de conectar proyectos de Workfront con registros de Workfront Planning. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Los comentarios agregados a objetos vinculados en otras aplicaciones no se muestran en Workfront Planning y los comentarios agregados a objetos vinculados en Workfront Planning no se muestran en otras aplicaciones.

  Por ejemplo, los comentarios agregados a proyectos en Workfront no se muestran en el mismo proyecto vinculado a una campaña en Workfront Planning y los comentarios agregados al proyecto en el registro de Workfront Planning no se muestran en Workfront.

* Puede etiquetar a los usuarios para que presten atención a una actualización. Los usuarios etiquetados no reciben una notificación dentro de la aplicación ni un correo electrónico sobre su actualización. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* Puede agregar una actualización a los registros y revisar el historial de cambios desde las siguientes áreas de Workfront Planning:

   * Desde la página de detalles del registro.
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

1. (Condicional) Si el panel derecho no se abre de forma predeterminada, haga clic en el icono **Mostrar comentarios** ![](assets/show-comments-icon.png) en la esquina superior derecha para abrir la sección Comentarios.

1. Empiece a escribir un comentario en el cuadro **Nuevo comentario**.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Si sale de la sección Comentarios antes de terminar de escribir y enviar un comentario, el comentario en la página se mantiene en modo de borrador incluso después de cerrar la sesión y volver a iniciarla. Todas las imágenes que se agreguen al comentario también se guardarán en el borrador. Los borradores se guardan durante 7 días después de los cuales se descartan y no se pueden recuperar. Los comentarios redactados solo son visibles para el usuario que los escribe.

1. (Opcional) Para deshacer o rehacer un cambio, utilice las siguientes teclas de método abreviado:
   * CTRL + Z (⌘ + z para Mac) para deshacer un cambio
   * CTRL + Y (⌘ + y para Mac) para rehacer un cambio
1. (Opcional) Agregue **@** seguido del nombre de un usuario para etiquetar a alguien en la actualización.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Opcional) Utilice las opciones de la barra de herramientas Texto enriquecido para dar formato al texto, agregar emojis, vínculos o imágenes a la actualización para mejorar el contenido. Para obtener más información, consulte la sección &quot;Usar texto enriquecido en una actualización de Workfront&quot; en el artículo [Trabajo de actualización](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Si otro usuario envía un comentario al mismo elemento que está actualizando, existe una línea roja con un indicador &quot;Nuevo&quot; para informarle de los comentarios más recientes.
   >
   >El indicador solo se muestra después de que se haya enviado el comentario sobre el elemento y no cuando el comentario aún está compuesto.
   >
   >![](assets/new-line-indicator-comments.png)

1. Haga clic en **Enviar** para agregar la actualización al registro.
1. (Opcional) Para editar un comentario, haga clic en el menú **Más** ![](assets/more-menu.png) en la esquina superior derecha del comentario y luego haga clic en **Editar**.

   >[!IMPORTANT]
   >
   >Solo puede editar su comentario en los 15 minutos siguientes al envío.

1. Edite la información del comentario, añada o elimine imágenes, o bien elimine cualquiera de los usuarios etiquetados. Se agrega un indicador &quot;editado&quot; a la izquierda del comentario.

   >[!TIP]
   >
   >Los comentarios del año actual no muestran el año en el sello de fecha. Al pasar el ratón por encima de una marca de tiempo, se muestra la fecha completa, incluido el año.

1. (Opcional y condicional) Para buscar un comentario existente, empiece a escribir una palabra clave en el cuadro de búsqueda situado en la esquina superior derecha del área **Comentarios**.

   ![](assets/search-box-for-comments-area.png)

1. (Opcional) Haga clic en **Responder** o empiece a escribir un comentario en el área **Agregar respuesta...** para responder a un comentario existente y, a continuación, siga los pasos del 4 al 8 anteriores. <!--(**************accurate??***********)-->

1. (Condicional y opcional) Si otros usuarios han agregado comentarios que se muestran fuera del área visible en la sección Comentarios mientras agregaba los comentarios, haga clic en **Ver** dentro del **nuevo titular de comentarios** en la parte inferior de la pantalla para mostrar estos comentarios.

   ![](assets/new-comments-banner-on-record.png)

   Los comentarios adicionales se muestran en la parte inferior de la pantalla.

1. (Opcional) Haga clic en el icono **Me gusta** para que le guste una actualización o para que reconozca que la ha leído. El icono se actualiza con el número de me gusta.
1. (Condicional y opcional) Si ha incluido más personas en el comentario, haga clic en los avatares de los usuarios incluidos en la actualización para mostrar una lista de usuarios con los que se comparte el comentario.
1. (Opcional) Haga clic en el icono **Más** ![](assets/more-menu.png) en la esquina superior derecha del comentario y haga clic en una de las siguientes opciones para copiar la información de un comentario:

   * **Copiar vínculo**: Esto copia un vínculo al comentario en el portapapeles.
   * **Copiar texto principal**: copia el texto del comentario en el portapapeles.
   * **Respuesta de cita**: copia el contenido del comentario en una nueva respuesta. Las imágenes no se incluyen en la respuesta copiada.

   Para obtener más información, consulte [Trabajo de actualización](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Opcional) Haga clic en el icono **Más** ![](assets/more-menu.png) en la esquina superior derecha del comentario y, a continuación, haga clic en **Eliminar** para eliminar el comentario.
1. (Opcional) Haga clic en el icono **Ocultar comentarios** ![](assets/hide-comments-icon.png) para cerrar el panel derecho.

## Resumen de la sección Historial

Puede revisar los cambios realizados en el registro en la sección Historial del panel derecho de un registro.

Para obtener más información, consulte [Resumen de la sección de historial](/help/quicksilver/planning/records/history-section-overview.md).
