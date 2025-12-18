---
title: Agregar una página de registros conectados a un registro
description: Puede ver información de registros u objetos conectados agregando una ficha para una página Registros conectados a un registro. Esto agrega los registros conectados en una vista de tabla a la ficha.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1776'
ht-degree: 3%

---


# Agregar una página Registros conectados a un registro

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Puede ver información de registros u objetos conectados agregando una ficha para una página Registros conectados a un registro en Adobe Workfront Planning. Esto agrega los registros conectados en una vista de tabla a la ficha.

Tenga en cuenta lo siguiente al agregar una página Registros conectados a un registro:

* Puede agregar una página Registros conectados a un registro después de conectar tipos de registro u objeto al tipo de registro desde la vista de tabla de un tipo de registro.

* Puede agregar una página Registros conectados desde el área de vista previa de un registro o desde la página del registro.

* Las páginas Registros conectados sólo muestran los objetos o registros conectados de un tipo de objeto o registro. La página no muestra todos los registros de ese tipo.

* Puede mostrar los objetos en una página de registros conectada en la vista de tabla.

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

* Puede agregar páginas Registros conectados para los siguientes tipos de registros u objetos conectados:

   * Tipos de registros de Workfront Planning
   * Proyectos Workfront

     Puede ver los proyectos de Workfront conectados incluso cuando no tenga permisos para acceder a ellos en Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p>
<p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
<tr>
<td> 
   <p> Productos adicionales</p> </td> 
   <td> 
   <p> Además de Adobe Workfront, debe tener lo siguiente si desea agregar una página de registro conectada para objetos de las siguientes aplicaciones:</p>
   <ul><li><p>Licencia de Adobe Experience Manager Assets e integración entre AEM Assets y Workfront para conectar recursos de AEM con tipos de registros de Planning.</p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront para Experience Manager Assets y Assets Essentials: índice de artículo</a>. </p></li>
   <li><p> Licencia de Adobe GenStudio for Performance Marketing para conectar tipos de registros con marcas de GenStudio</p>
   <p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Introducción a Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <p>Permisos de contribución o superiores para un espacio de trabajo y tipo de registro </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> 
  </td>
  </tr>   
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Agregar una página Registros conectados a un registro

Primero debe conectar los tipos de registros con otros tipos de registros o proyectos de Workfront antes de agregar una página de registros conectada a un registro.

1. Haga clic en el nombre del registro para abrirlo desde cualquier vista de una página de tipo de registro.
1. Haga clic en **Agregar página** en una de las siguientes áreas:

   * Ventana de vista previa del registro
   * La página de detalles del registro, después de hacer clic en el icono **Abrir en ficha nueva** ![Abrir detalles en icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la página de vista previa.

   Se abre el cuadro **Crear página**.

   ![Agregar página de registros conectados modal](assets/add-connection-view-page-modal.png)

1. Agregue **Nombre de página**, haga clic en **Página de registros conectados** para el **Tipo de página** y, a continuación, haga clic en **Crear**.
1. (Opcional) Haga clic en el nombre de un registro conectado o tipo de objeto en la lista, o búsquelo y, a continuación, haga clic en él cuando aparezca en la lista para crear la página para ese registro o tipo de objeto.

1. (Opcional y condicional) Si se muestra más de un campo conectado del tipo de registro u objeto para el que está creando la página, haga clic en el campo cuyos registros u objetos desee mostrar en la página de registros conectados de la lista **Seleccionar campo de referencia**.

   ![Seleccionar lista de campos de referencia](assets/select-reference-field-list-on-connected-records-page.png)

   Se agrega una de las siguientes páginas a la página registros conectados:

   * La vista de tabla de un tipo de registro
   * La vista de lista de un tipo de objeto de proyecto

   Los registros o proyectos conectados al registro actual se muestran en la vista de tabla o lista.

   >[!TIP]
   >
   >Debe agregar registros conectados en la tabla o en el área Detalles de un registro para poder mostrarlos en una página de registros conectados. De lo contrario, la tabla o la lista estarán vacías.

   Los cinco primeros campos de los registros conectados se muestran de forma predeterminada. <!--No lookup fields display by default.-->

   ![Vista de tabla conectada a la audiencia con detalles de campaña](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Condicional) Según el tipo de registros que muestre en la página de registros conectada, realice una de las siguientes acciones:

   * Administrar la vista de tabla de los registros
Para obtener más información, vea la sección [Administrar la vista de tabla de registros en la página de registros conectados](#manage-the-record-table-view-in-the-connected-records-page) en este artículo.
   * Administrar la vista de lista de proyectos
Para obtener más información, consulte la sección [Administrar la vista de lista de proyectos en la página de registros conectados](#manage-the-project-list-view-in-the-connected-records-page) en este artículo.

1. (Opcional) Haga doble clic en el nombre de la ficha **Página de registros conectados**

   O

   Pase el ratón sobre el nombre de la ficha, luego haga clic en **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Cambiar nombre** para cambiar el nombre a la nueva ficha de página de registros conectados.


   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Opcional) Pase el ratón sobre el nombre de la pestaña de la página de registros conectados, haga clic en **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Eliminar** para quitar a la pestaña.

### Administrar la vista de tabla de registros en la página de registros conectada

Cuando cree una página de registros conectados para registros conectados de Planning, haga lo siguiente: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Vaya a una página de tipo de registro y haga clic en el nombre de un registro. Se abre la página de vista previa del registro.
1. Haga clic en la ficha de una página de registros conectados que muestra registros de Planning.
Los registros conectados al registro seleccionado se muestran en la vista de tabla.
1. Haga clic en **Conectar** en la parte inferior de la vista de tabla para conectar los registros existentes, selecciónelos en el cuadro de conexión y, a continuación, haga clic fuera del cuadro para cerrarlo. Los registros se agregan automáticamente a la tabla y se conectan al registro seleccionado. Los registros deben existir antes de que pueda agregarlos.

   Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Edite cualquier información de los registros conectados en línea en la vista de tabla.
1. Pase el ratón sobre el nombre de un registro conectado y luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png)

   O

   Seleccione uno de los registros y, a continuación, haga clic en una de las siguientes opciones de la barra azul situada en la parte inferior de la lista:

   * **Ver** para abrir la página de registros en una nueva pestaña
   * **Copiar vínculo** para copiar un vínculo a la página de registro
   * **Editar miniatura** para abrir el cuadro **Grabar miniatura** y editar la imagen en miniatura del registro
   * **Duplicate** para duplicar el registro conectado. El registro duplicado también está conectado al registro actual.
   * **Inserte un registro por encima o por debajo de** para agregar nuevos registros al tipo de registro conectado. Los registros nuevos agregados aquí también están conectados al registro actual. Esta opción no está disponible en la barra azul al seleccionar un registro de la tabla.
   * **Eliminar** para eliminar el registro. Al eliminar un registro conectado, se elimina de su tipo de registro y de cualquier lugar donde esté conectado. Los registros eliminados se mueven al grupo **Eliminados recientemente** de su tipo de registro.

     Para obtener información acerca de cómo editar registros en la vista de tabla, vea [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >Puede seleccionar más de un registro u objeto para eliminarlos.

1. Edite en línea cualquiera de los registros de la tabla de la página de registros conectados.
1. Utilice cualquiera de los siguientes elementos de vista en la barra de herramientas de una página de registro conectada para administrar la vista de tabla:

   * **Filtros**
   * **Ordenar**
   * **Agrupación**
   * **Campos**, para mostrar, ocultar o reorganizar campos
   * **Altura de fila**
   * **Búsqueda**

   Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >No puede crear, editar ni eliminar campos en la vista de tabla de la ficha de un registro conectado.

   <!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      >[!TIP]
      >
      >You can select more than one record or object to disconnect them.
      -->

### Administrar la vista de lista de proyectos en la página de registros conectados

Cuando cree una página de registros conectados para proyectos conectados de Workfront, haga lo siguiente:

1. Vaya a una página de tipo de registro y haga clic en el nombre de un registro. Se abre la página de vista previa del registro.
1. Haga clic en la ficha de una página de registros conectada que muestre proyectos de Workfront.
Los proyectos conectados al registro seleccionado se muestran en la vista de lista.
1. Haga clic en **Conectar registros** en la esquina superior derecha de la página de registros conectada para conectar proyectos existentes.

   Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Editar en línea la información del proyecto en la tabla.
1. Haga clic en **Nueva fila** para crear un proyecto sin plantilla. El nuevo proyecto se conecta automáticamente al registro actual.

   Para obtener más información, vea [Crear objetos de Workfront desde Workfront Planning a medida que los conecta a registros](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
1. Pase el ratón sobre un nombre de proyecto en la lista y haga clic en el menú **Más** [Menú más](assets/more-menu.png)

   O

   Seleccione uno o varios proyectos, observe la barra azul en la parte inferior de la lista y, a continuación, haga clic en uno de los siguientes:

   * **Eliminar** para eliminar el proyecto. Al eliminar un proyecto, se desconecta del registro y se mueve a la papelera de reciclaje de Workfront. Los administradores de Workfront pueden recuperar los proyectos eliminados hasta 30 días después de haberlos eliminado.
   * **Desconectar** para desconectar el proyecto del registro. Al desconectar un proyecto, éste y todos los valores de sus campos de búsqueda se eliminan del registro actual.

   >[!TIP]
   >
   >Puede seleccionar más de un proyecto para desconectarlos o eliminarlos.
1. Haga clic en el menú desplegable de vistas y, a continuación, haga clic en **Nueva vista** para agregar una nueva vista para la página y, a continuación, haga lo siguiente:
   1. Agregar **nombre de vista**.
   1. Seleccione **Lista** del área **Tipo de vista**.
   1. Haga clic en **Crear**.
Se agrega una nueva vista de lista al menú desplegable de vistas.
   1. (Opcional) Pase el ratón sobre el nombre de una vista que haya creado, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en una de las siguientes opciones:
      * **Cambiar nombre**, para agregar un nuevo nombre para la vista.
      * <span class="preview">**Compartir**</span>

        Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >No puede compartir una vista predeterminada creada por Workfront.

      * **Eliminar**
Para obtener más información, consulte [Eliminar vistas de registros](/help/quicksilver/planning/views/delete-record-views.md).


        ![](assets/view-more-menu-projects-connected-records-page.png)
   1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) y use el filtro para mostrar proyectos específicos.

      >[!TIP]
      >
      ><span class="preview">Para campos de tipo personas, como **Propietario** o **Patrocinador**, puede usar un comodín para mostrar proyectos donde el usuario que ha iniciado sesión esté asignado a estos roles.</span>
      >
      >![Filtro con comodín de usuario para la página de registros conectados al proyecto](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >
   1. Haga clic en el icono **Columnas** ![Icono de Columnas](assets/columns-icon.png) para ocultar o mostrar columnas en la lista.
   1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla para agregar campos existentes a la tabla. Los campos deben existir antes de poder agregarlos.

      Se abre el cuadro **Administrador de columnas**. Haga lo siguiente:

      1. Busque un campo de objeto existente en la columna **Disponible** y, a continuación, haga clic en **+** a la derecha del nombre del campo para agregarlo a la columna **Seleccionado**.

         Los campos que seleccione se agregarán a la vista de tabla de la página registros conectados.
      1. Haga clic en **-** a la derecha de un campo en la columna **Seleccionado** para quitarlo de la vista de tabla.
      1. Haga clic en **Guardar** para guardar la vista de tabla de páginas de registros conectados.


<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->