---
title: Administrar comentarios de registro
description: Puede colaborar en los registros de Adobe Maestro agregando comentarios o respuestas en el área Comentarios de un registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---


# Administrar comentarios de registro

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. </span>

<span class="preview">Para obtener más información sobre la programación actual de versiones, consulte [Información general sobre la versión del primer trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

Puede colaborar en los registros de Adobe Maestro agregando comentarios o respuestas en el área Comentarios de un registro.

## Consideraciones acerca de los comentarios en un registro

* Puede agregar comentarios y respuestas a registros operativos y taxonomías en Maestro, en la sección Comentarios de un registro.

* Los comentarios agregados a los registros vinculados no se muestran en los registros desde los que está vinculando. Por ejemplo, si comenta un registro de producto de Maestro que está vinculado a un registro de Campaign, el comentario sólo se mostrará en el registro de producto de Maestro y no en el registro de campaña desde el que está vinculando.

* Puede agregar comentarios a los registros de Maestro creados como resultado de una conexión entre un registro de Maestro y un objeto de otra aplicación.

  Por ejemplo, puede realizar comentarios en el registro de Project Maestro después de conectar proyectos de Workfront con registros de Maestro. Para obtener más información, consulte [Conectar registros](/help/quicksilver/maestro/records/connect-records.md).

* Los comentarios agregados a objetos vinculados en otras aplicaciones no se muestran en Maestro y los comentarios agregados a objetos vinculados en Maestro no se muestran en otras aplicaciones.

  Por ejemplo, los comentarios agregados a proyectos en Workfront no se muestran en el mismo proyecto vinculado a una campaña en Maestro y los comentarios agregados al registro de proyecto Maestro no se muestran en Workfront.

* Puede etiquetar a los usuarios para que presten atención a una actualización. Los usuarios etiquetados no reciben una notificación dentro de la aplicación ni un correo electrónico sobre su actualización. <!--this might change??-->

* Puede agregar una actualización a los registros desde las siguientes áreas de Maestro:

   * En la página Detalles.

  <!--* From the table view.-->

## Requisitos de acceso

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
   <p> Product</p> </td>
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
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso en Maestro. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Ver permisos superiores a un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de Workfront o de grupo debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Administración de comentarios en registros

{{step1-to-maestro}}

El último espacio de trabajo al que se accede se abre de forma predeterminada.
1. Elija una vista de tabla de la **Ver** menú desplegable.
1. Haga clic en el nombre de un registro en la vista de tabla.

   El registro es... **Detalles** se abre la página. El área Comentarios se abre de forma predeterminada en el panel derecho.

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

1. <span class="preview">(Opcional y condicional) Para buscar un comentario existente, empiece a escribir una palabra clave en el cuadro de búsqueda situado en la esquina superior derecha de la etiqueta **Comentarios** área.</span>

   <span class="preview">![](assets/search-box-for-comments-area.png)</span>

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

