---
title: Administrar el diseño de página de registro
description: Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '1913'
ht-degree: 45%

---


# Administrar el diseño de página de registro

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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
<p>Cualquiera</p>
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p>
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
   <p>Aportar o permisos superiores a un espacio de trabajo <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal y el área de Planning para proyectos, portafolios y programas. </p> Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Información general sobre el acceso a Adobe Planning</a>. </p>  </p>  
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

   <div class="preview">

   ![Cuadro de detalles](assets/details-box.png)

   </div>

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

   <div class="preview">

   ![Cuadro de detalles](assets/details-box.png)

   </div>

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![Abrir cuadro de detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una ficha nueva.

   La ficha **Detalles** del registro se abre de manera predeterminada.

   <div class="preview">

   ![Página de detalles](assets/details-page.png)

   </div>

1. En la ficha de registro **Detalles**, haga clic en el icono **agarrar** ![Icono de agarrar](assets/grab-icon.png) a la izquierda del nombre de un campo y, a continuación, arrástrelo y suéltelo en el lugar deseado.

   >[!TIP]
   >
   >Puede arrastrar y soltar campos en otra sección.
   >Debe haber al menos un portafolio en el sistema.
   >

   La nueva posición del campo se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios en el diseño de la vista previa o la página del registro se guardan automáticamente.

## Agregar una página de vista Conexión a la página de un registro

<!--suggested a new name for this type of page: "Connected records details" - check to see if this changed-->

Tenga en cuenta lo siguiente al agregar una vista Conexión a la página de un registro:

* Puede agregar una página de vista Conexión a la página de un registro.

* No se puede agregar una página de vista Conexión al área de vista previa de un registro.

* Las páginas de vista de conexión muestran una página de registro conectada en la vista de tabla. La vista de tabla es de solo lectura. <!--more views might be added in the future-->

* Puede agregar una página Vista de conexión por cada tipo de registro conectado.  <!--edit this when we can remove fields from this page-->

* Después de agregar una página de vista Conexión a la página de un registro, la ficha Página se puede ver desde el área de vista previa del registro. Debe ir a la página completa para ver la vista de tabla del registro conectado. <!--this might have changed? check and take disclaimer out-->

Para agregar una página Vista de conexión:

1. En una vista de página de registro, haga clic en el nombre de un registro para abrirlo y, a continuación, haga clic en el icono **Abrir en ficha nueva** ![Abrir detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la página de vista previa.
1. Haga clic en **Agregar página** > **Vista de conexión**.

   ![Agregar modal de página de vista de conexión](assets/add-connection-view-page-modal.png)
1. Agregue **Nombre de página**, haga clic en **Vista de conexión** y, a continuación, haga clic en **Crear**.

   Se agrega una nueva pestaña a la página del registro.
1. Busque o haga clic en el nombre de un tipo de objeto o registro conectado en la lista.
Se muestra la vista de tabla del tipo de registro seleccionado y los registros conectados se muestran en la vista de tabla.
Todos los campos del registro conectado se muestran en la vista de tabla de la ficha del registro conectado.

   <span class="preview">Al acceder a Workfront Planning desde el entorno de vista previa, los primeros cinco campos de la tabla de registro conectada se muestran de forma predeterminada. No se muestran campos de búsqueda de forma predeterminada.</span>

   La vista de tabla es de solo lectura.

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   <div class="preview">

   ![Vista de tabla conectada a la audiencia con detalles de campaña](assets/audience-connected-table-view-under-campaign-details-page.png)

   </div>

1. (Opcional) Haga doble clic en el nombre de la pestaña

   O

   Pase el ratón sobre el nombre de la ficha, luego haga clic en **Más** ![Menú más](assets/more-menu.png), luego haga clic en **Cambiar nombre** para cambiar el nombre a la nueva ficha Vista conectada.
1. (Opcional) Utilice cualquiera de los siguientes elementos de vista de la barra de herramientas para administrar la vista de tabla:

   * Filtros
   * Ordenar
   * Agrupación
   * <span class="preview">Campos, para mostrar, ocultar o reorganizar campos</span>

   <!--Add to the list above from the list below - and condition these for Preview only: Hide fields, rearrange fields-->

   Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   No puede realizar ninguna de las siguientes acciones en la vista de tabla de la ficha de un registro conectado:
   >
   >   * Ocultar o reorganizar campos. <span class="preview">Puede ocultar y reorganizar campos en el entorno de vista previa.</span>
   >   * Crear, editar o eliminar campos
   >

1. <span class="preview">Haga clic en **Conectar** para agregar o quitar registros. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md)</span>
1. (Opcional) Pase el ratón sobre el nombre de la pestaña Vista de conexión, haga clic en **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Eliminar** para quitar a la nueva pestaña Vista conectada.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



