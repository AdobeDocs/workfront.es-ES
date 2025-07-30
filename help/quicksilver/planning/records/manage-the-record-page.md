---
title: Administrar el diseño de página de registro
description: Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 567fa8c960f7db47279d6cde1f5e90dc7f38ae79
workflow-type: tm+mt
source-wordcount: '2133'
ht-degree: 40%

---


# Administrar el diseño de página de registro

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.

La vista previa del registro es una vista más pequeña de la página del registro que se muestra en la vista de un tipo de registro.

Al cambiar el diseño de una vista previa y una página de registro, los cambios afectan a los cuadros de vista previa y a las páginas de detalles de todos los registros del mismo tipo.

En este artículo se describe cómo puede cambiar el diseño y el aspecto de un cuadro de vista previa de registro o de una página de registro. Para obtener información sobre la edición de registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Debe crear tipos de registros y registros para poder empezar a editar páginas de registros.

Para obtener más información, consulte los siguientes artículos:

* [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)

* [Crear registros](/help/quicksilver/planning/records/create-records.md)

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
<p>Cualquiera</p>
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
   <td>
   <p>Estándar</p>
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
   <td>
   <p>Permisos de contribución o superiores para un espacio de trabajo y tipo de registro </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> 
  </td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Consideraciones sobre la edición de páginas de registro

* De forma predeterminada, las páginas de detalles y de vista previa de un registro muestran todos los campos asociados al registro.

* No se pueden añadir nuevos campos para un registro en la página de vista previa o de detalles. Debe añadir nuevos campos en la vista de tabla para mostrarlos en las páginas de vista previa y detalles.

* Puede añadir secciones a una vista previa o a una página de detalles del registro para organizar la información según criterios comunes y facilitar su búsqueda.

* Los siguientes cambios afectan a todos los registros del mismo tipo y son visibles para todos los usuarios que acceden a esos registros:

   * Reorganización de campos
   * Añadir o quitar secciones

* Los cambios de visualización que realice en la vista previa del registro se pueden ver inmediatamente en la página de detalles del registro. Los cambios realizados en la página de registro también se pueden ver en el cuadro de vista previa del registro.

* Añadir una imagen de portada o una miniatura a un registro no forma parte del diseño general de la vista previa o la página del registro. Puede añadir imágenes de portada o miniaturas únicas a cada registro. Para obtener más información, consulte [Añadir una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) y [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Añadir secciones a una vista previa o página de registro

Tenga en cuenta lo siguiente al añadir secciones a una página de registro:

* No hay límite en cuanto a la cantidad de secciones que puede haber en una página.
* No puede tener una sección vacía. Debe haber al menos un portafolio en el sistema.
* Puede arrastrar y soltar campos de una sección a otra. Para obtener más información, consulte la sección [Reorganización de campos en la vista previa o en la página de detalles del registro](#rearrange-fields-in-the-record-preview-or-details-page) de este artículo.
* Al eliminar todos los campos de una sección, ésta se elimina automáticamente y no se puede recuperar.

Para añadir una sección a una vista previa o a una página del registro:

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla, haga clic en el icono **Abrir detalles** ![Abrir detalles en el campo de nombre de tabla](assets/open-details-icon-in-table-name-field.png) de la primera columna.

   La vista previa del registro se abrirá en la vista.

   ![Cuadro de detalles](assets/details-box.png)

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![Abrir detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una ficha nueva.

   Se abre la página de registro. La pestaña Detalles se abre de forma predeterminada.

   ![Página de detalles](assets/details-page.png)

1. En la pestaña **Detalles** de la página o vista previa del registro, pasa el ratón sobre el espacio en blanco a la izquierda de los campos y, a continuación, haz clic en el icono **Agregar sección** ![Agregar icono de sección](assets/add-section-icon.png) para agregar una sección.
1. Haga clic dentro del nombre de la sección y reemplace **Sección sin título** por un nombre; a continuación, haga clic en Entrar. Los campos que se muestran en la sección forman parte automáticamente de la nueva sección.
1. Empiece a arrastrar y soltar campos en la nueva sección, tal como se describe en la sección [Reorganización de los campos en la vista previa o en la página de detalles del registro](#rearrange-fields-in-the-record-preview-or-details-page) de este artículo.

1. (Opcional) Pase el ratón sobre el nombre de una sección y haga clic en el menú **Más** ![Menú más](assets/more-menu.png).

   ![Más opciones de menú para la sección de la página de registros](assets/more-menu-options-for-section-on-record-page.png)
1. (Opcional) Realice una de las siguientes acciones para editar la sección:

   * Haga clic en **Cambiar nombre** para cambiar el nombre de la sección

     >[!TIP]
     >
     > Puede cambiar el nombre de una sección en línea haciendo clic en él.

   * Haga clic en **Subir** para subir la sección una posición

     O

     Haga clic en **Bajar** para bajar la sección una posición.
Todos los campos de la sección se mueven con la sección.

   * Haga clic en **Eliminar** para eliminar la sección. La sección se elimina y no se puede recuperar. Todos los usuarios que accedan a los registros de este tipo ya no verán la sección eliminada.

1. Haga clic en la flecha hacia abajo situada a la izquierda del nombre de la sección para contraerla o en la flecha hacia la derecha para expandirla.
Todas las secciones se expanden de forma predeterminada.

1. (Opcional) Haga clic en el icono **asidero** ![Icono de asidero](assets/grab-icon.png) a la izquierda del nombre de una sección, luego arrástrela y suéltela en el lugar que desee.

   La nueva posición de la sección se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios realizados en las secciones y el orden de los campos se guardan automáticamente.

1. (Opcional) Haga clic en el icono **Exportar** del menú ![Exportar en la página de detalles del registro](assets/export-icon-in-record-details-page.png) para exportar la pestaña Detalles a un archivo de Word o PDF. Para obtener más información, vea [Exportar los detalles de un registro](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Opcional) Haga clic en la ficha **Conexiones** junto a la ficha **Detalles**. Es posible que tenga que hacer clic en **Más** antes de hacer clic en la ficha **Conexiones**.

   Todos los registros u objetos conectados al registro seleccionado se muestran bajo los nombres del tipo de registro o de la aplicación a la que pertenecen.

   ![Ficha Conexiones registrada en Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Opcional) Seleccione la opción **Mostrar todos los registros** en la esquina superior derecha de la pestaña Conexiones. Se muestran todos los tipos de registros conectados, incluidos los que aún no tienen registros conectados. De forma predeterminada, la opción no está seleccionada y los tipos de registro sin registros conectados están ocultos.

1. (Opcional) Haga clic en **Conectar** para agregar más registros a los tipos de registros conectados. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

1. (Opcional) Pase el ratón sobre una tarjeta de registro, haga clic en el icono de registro de desconexión **-** y, a continuación, haga clic en **Desconectar**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Ocurren lo siguiente:
   * El registro ya no está conectado al objeto Workfront.
   * El objeto Workfront también se quita del campo conectado del registro de Workfront Planning.
   * También se eliminan los valores de los campos de búsqueda de Workfront conectados al registro de Planning.

## Reorganizar campos en la pestaña Detalles del registro

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla, haga clic en el icono **Abrir detalles** ![Abrir detalles en el campo de nombre de tabla](assets/open-details-icon-in-table-name-field.png) de la primera columna.

   La vista previa del registro se abrirá en la vista.

   ![Cuadro de detalles](assets/details-box.png)

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![Abrir cuadro de detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una ficha nueva.

   La ficha **Detalles** del registro se abre de manera predeterminada.

   ![Página de detalles](assets/details-page.png)

1. En la ficha de registro **Detalles**, haga clic en el icono **agarrar** ![Icono de agarrar](assets/grab-icon.png) a la izquierda del nombre de un campo y, a continuación, arrástrelo y suéltelo en el lugar deseado.

   >[!TIP]
   >
   >Puede arrastrar y soltar campos en otra sección.
   >Debe haber al menos un portafolio en el sistema.
   >

   La nueva posición del campo se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios en el diseño de la vista previa o la página del registro se guardan automáticamente.

## Agregar una página Registros conectados a un registro

Puede ver información de registros u objetos conectados agregando una ficha para una página Registros conectados a un registro.

La información de los registros conectados se puede editar en la vista de tabla. La información de los objetos conectados desde otra aplicación no se puede editar en la vista de tabla.

Tenga en cuenta lo siguiente al agregar una página Registros conectados a un registro:

* Puede agregar una página Registros conectados a un registro después de conectar tipos de registro u objeto al tipo de registro desde la vista de tabla de un tipo de registro.

* No se puede agregar una página Registros conectados al área de vista previa de un registro. <!--take this out when we release connected record pages to the record preview area-->

* Las páginas Registros conectados muestran sólo los objetos o registros conectados de un tipo de objeto o registro en una vista de tabla. La página no muestra todos los registros de ese tipo en la vista de tabla.

* Después de agregar una página Registros conectados a un registro, la ficha de página es visible desde el área de vista previa del registro, pero está en blanco. Debe ir a la página completa para ver la vista de tabla del registro conectado. &lt;!—esto cambiará con el lanzamiento de las páginas conectadas al área de previsualización— comprobar y eliminar la exención de responsabilidad—>

* Puede agregar páginas Registros conectados para los siguientes tipos de registros u objetos conectados:

   * Tipos de registros de Workfront Planning
   * Proyectos, programas, portafolios, grupos o compañías de Workfront. Puede ver los objetos de Workfront conectados incluso cuando no tenga permisos para acceder a ellos en Workfront.

  >[!NOTE]
  >
  >   No puede agregar una página Registros conectados para registros de AEM Assets conectados.

Para agregar una página Registros conectados:

<!--replace the first 2 steps with these steps when we release connected record page to the record preview area, if this goes both to Preview and Prod: 

1. Click the name of the record to open it. 
1. Click **Add page** from one of the following areas: 

   * The record's preview window
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

-->

1. En una vista de página de registro, haga clic en el nombre de un registro para abrirlo y, a continuación, haga clic en el icono **Abrir en ficha nueva** ![Abrir detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la página de vista previa.
1. Haga clic en **Agregar página**.

   Se abre el cuadro **Crear página**.

   ![Agregar página de registros conectados modal](assets/add-connection-view-page-modal.png)

1. Agregue **Nombre de página**, haga clic en **Página de registros conectados** y, a continuación, haga clic en **Crear**.

   Se agrega una nueva pestaña a la página del registro.
1. Busque o haga clic en el nombre de un tipo de objeto o registro conectado en la lista.
La vista de tabla del tipo de registro seleccionado se muestra en la nueva página y los registros conectados se muestran en la vista de tabla.
Todos los campos del registro conectado se muestran en la vista de tabla de la ficha del registro conectado.

   Los cinco primeros campos de la tabla de registros conectada se muestran de forma predeterminada. De forma predeterminada, no se muestran campos de búsqueda.

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   ![Vista de tabla conectada a la audiencia con detalles de campaña](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Opcional) En la vista de tabla de los registros conectados, realice una de las siguientes acciones:

   * Haga clic en el nombre de un registro. Se abre la página del registro en una nueva ficha.

     Se abre la página de vista previa del registro. Haga clic en el icono **Abrir en una ficha nueva** ![Abrir en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha para abrir la página del registro conectado.

   * Haga clic en **Conectar** para conectar más registros y, a continuación, haga clic fuera del cuadro de conexión para cerrarlo. Los registros nuevos se agregan automáticamente a la tabla.
   * Edite cualquier información de los registros conectados dentro de la vista de tabla.

   * Pase el ratón sobre el nombre de un registro conectado, luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) y, a continuación, haga clic en una de las siguientes opciones:
      * Ver
      * Copiar vínculo
      * Editar miniatura
      * Duplicar
      * Insertar registro arriba o abajo
      * Eliminar
   * Seleccione uno de los registros y haga clic en una de las siguientes opciones de la barra azul de la parte inferior de la pantalla:
      * Ver
      * Copiar vínculo
      * Editar miniatura
      * Duplicar
      * Eliminar. Eliminar es la única opción disponible cuando se selecciona más de un registro.

     Para obtener información acerca de cómo editar registros en la vista de tabla, vea [Editar registros](/help/quicksilver/planning/records/edit-records.md).

   * Edite en línea cualquiera de los registros de la tabla en la página Registros conectados. Los objetos de Workfront se muestran en una vista de tabla de solo lectura y no se pueden editar.

1. (Opcional) Haga doble clic en el nombre de la ficha de la página Registros conectados

   O

   Pase el ratón sobre el nombre de la ficha, luego haga clic en **Más** ![Menú más](assets/more-menu.png), luego haga clic en **Cambiar nombre** para cambiar el nombre a la nueva ficha Vista conectada.
1. (Opcional) Utilice cualquiera de los siguientes elementos de vista de la barra de herramientas para administrar la vista de tabla:

   * Filtros
   * Ordenar
   * Agrupación
   * Campos, para mostrar, ocultar o reorganizar campos

   Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   No puede crear, editar ni eliminar campos en la vista de tabla de la ficha de un registro conectado.
   >

1. Haga clic en **Conectar** para agregar o quitar registros. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
1. (Opcional) Pase el ratón sobre el nombre de la ficha de la página Registros conectados, haga clic en **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Eliminar** para quitar a la ficha.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



