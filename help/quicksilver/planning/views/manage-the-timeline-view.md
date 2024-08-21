---
title: Administrar la vista de cronología
description: Acceda y edite registros en una vista de cronología de la página de tipo de registro de Adobe Workfront Planning. Personalice la cronología con filtros, agrupaciones y ajustes. Utilice la función Desglose para mostrar los registros conectados.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '1941'
ht-degree: 0%

---

# Administrar la vista de cronología

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Puede mostrar registros en una vista de cronología al acceder a la página de tipo de registro en Adobe Workfront Planning.

Para obtener información sobre las vistas de registros, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   O
   <p>Actual: plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> No hay controles de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en una vista</p>  
   <p>Ver permisos de una vista para cambiar temporalmente su configuración</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--EDIT PERMISSIONS AND ACCESS AND REPLACE THE table above with the following table at Planning GA release: 
## Access requirements

You must have the following to be able to access Workfront Planning: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following new Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td>
   <td>
<p>Any of the following Workfront Planning plans:</p>
<ul><li>Planning</li>
<li>Planning Plus</li>
</ul>
<p>For more information about what is included in each Workfront Planning plan, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Standard, to create workspaces</p></li></ul>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a> and and <a href="../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md">Assign users to a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

*********ensure that the link ^^^^^^^^above^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************

-->


## Administrar una vista de cronología {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Al crear una vista de escala de tiempo, todos los registros del tipo de registro seleccionado se muestran en una escala de tiempo cronológica.

Tenga en cuenta lo siguiente:

* Sólo puede crear una vista Cronología si tiene al menos dos campos de fecha asociados a un tipo de registro. Cuando hay uno o ningún campo de fecha asociado a un tipo de registro, la opción de vista Cronología aparece atenuada.

  Puede seleccionar los siguientes campos de fecha al crear una vista de cronología:

   * Registrar fechas
   * Registrar campos generados por el sistema: fecha de creación, fecha de la última modificación
   * Buscar fechas de tipos de objeto o registro conectados.
* Según las fechas asociadas con los registros, es posible que algunos registros no se muestren en la vista de escala de tiempo en los siguientes casos:

   * Cuando las fechas de inicio y finalización no tienen valores
   * Cuando las fechas de inicio y finalización no tienen valor
   * Cuando la fecha de inicio es posterior a la fecha de finalización

Para administrar una vista de cronología:

1. Vaya a la página del tipo de registro cuya cronología desea ver.
1. Cree una vista de escala de tiempo, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Los registros asociados con el tipo de registro seleccionado se muestran como barras en una cronología y se ordenan en orden cronológico de su fecha de inicio de forma predeterminada.

   >[!TIP]
   >
   >    La ordenación de los registros de la cronología no es visible en la vista Compacta.

1. (Opcional y condicional) Cuando el nombre del registro esté truncado, pase el ratón sobre una barra de registros para mostrar el nombre completo del registro y la información adicional.

1. Realice una de las siguientes acciones para navegar por la cronología:

   * Haga clic en los iconos izquierdo y derecho o utilice el desplazamiento horizontal para moverse hacia atrás y hacia adelante en la cronología. Al actualizar la página, se conserva el lapso de tiempo seleccionado.
   * Haga clic en **Hoy** para centrar la escala de tiempo en la fecha de hoy.
   * Seleccione una de las siguientes opciones del menú desplegable lapso de tiempo para actualizar los incrementos de tiempo:

      * Año
      * Trimestre
      * Mes
1. Haga clic en **Cambiar a la vista Estándar** para mostrar los registros en líneas independientes <!--check to see if they updated the name of the setting here-->

   O

   Haga clic en **Cambiar a la vista compacta** para mostrar los registros cuyas fechas no se cruzan en la misma línea. <!--check to see if they updated the name of the setting here-->

   Los registros se muestran en la vista Compacta de forma predeterminada.

1. Haga lo siguiente para buscar rápidamente registros que coincidan con una palabra clave:

   1. Haga clic en el icono **Search** ![](assets/search-icon.png) y empiece a escribir una palabra clave asociada a cualquier campo de un registro que se muestra en la pantalla. El número de coincidencias correctas se muestra junto al elemento de búsqueda y el registro con la coincidencia correcta se resalta.

      ![](assets/search-box-and-results-timeline-view.png)

      Puede utilizar cualquier palabra o carácter especial que esté visible en la pantalla.

      No se pueden utilizar palabras clave asociadas a campos que no se muestran en la vista de cronología.

   1. Pulse Enter en el teclado para ir al siguiente campo encontrado.
   1. (Opcional) Si hay más de una coincidencia, haga clic en las flechas arriba y abajo a la derecha de la palabra clave de búsqueda para encontrar todas las coincidencias de la tabla.
   1. Haga clic en el icono **x** en el cuadro de búsqueda para borrar la palabra clave de búsqueda.

1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Filtros](#add-filters)
   * [Agrupación](#add-grouping)
   * [Configuración](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Añadir filtros

Puede reducir la cantidad de información que se muestra en la pantalla mediante filtros.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de cronología:

<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para una vista de cronología funcionarán de forma independiente de los filtros de cualquier otra vista aplicada al mismo tipo de registro.

* Los filtros son exclusivos de la vista seleccionada. Dos vistas de escala de tiempo del mismo tipo de registro pueden tener diferentes filtros aplicados.

* Dos usuarios que ven la misma vista de cronología ven el mismo filtro que se aplica actualmente.

* No puede asignar un nombre a los filtros que genere para una vista de cronología.

* Al eliminar los filtros, se eliminan de todos los que tengan acceso al mismo tipo de registro que usted y que muestren la misma vista que usted.

* Añadir filtros en la vista de cronología es idéntico a añadir filtros en la vista de tabla.

  Para obtener más información, consulte la sección &quot;Agregar filtros&quot; en el artículo [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Puede filtrar por campos de registro conectados o campos de búsqueda.
* Puede filtrar por campos de búsqueda que muestren varios valores.


### Agregar agrupación

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Puede agrupar registros por información similar al aplicar una agrupación a una vista.

Agregar agrupaciones en la vista de escala de tiempo es similar a agregar agrupaciones a la vista de tabla.

Tenga en cuenta lo siguiente al trabajar con agrupaciones en la vista de cronología:

* Puede aplicar agrupaciones tanto en las vistas de tabla como de escala de tiempo. Las agrupaciones de la vista de tabla son independientes de las de la vista de escala de tiempo del mismo tipo de registro.
* Se pueden aplicar 3 niveles de agrupación en una vista. Los registros se agrupan en el orden de agrupaciones que seleccione.
&lt;!—* Puede aplicar hasta 4 niveles de agrupación al utilizar la API. —comprobando este por ahora—>
* Las agrupaciones son únicas para la vista que seleccione. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes agrupaciones aplicadas. Dos usuarios que ven la misma vista de tabla ven la misma agrupación que se aplica actualmente.
* No puede asignar un nombre a las agrupaciones que genere para una vista de tabla.
* Al quitar las agrupaciones, se quitan de cualquier usuario que tenga acceso al mismo tipo de registro que usted y que muestre la misma vista que usted.
* Puede editar los registros enumerados bajo una agrupación.
* Puede agrupar por campos de registro conectados o campos de búsqueda.
* Cuando se agrupan por campos de búsqueda con varios valores (que no se han resumido con un agregador), los registros se agrupan por cada combinación única de valores de campo.
* Puede hacer referencia a un campo que esté situado a una distancia de hasta 4 niveles del tipo de registro actual. Por ejemplo, si está creando una agrupación para un tipo de registro de actividad y la actividad está conectada al tipo de registro de producto conectado al tipo de registro de campaña conectado a un proyecto de Workfront, puede hacer referencia al estado del proyecto en la agrupación que está creando para el tipo de registro de actividad.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Para agregar una agrupación en la vista de escala de tiempo:

1. Cree una vista de escala de tiempo para un tipo de registro, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Haga clic en **Agrupación** en la esquina superior derecha de la vista de escala de tiempo.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Haga clic en uno de los campos sugeridos o haga clic en **Elija un campo diferente**, busque un campo diferente y, a continuación, haga clic en él cuando se muestre en la lista.

   La agrupación se aplica automáticamente a la cronología y los registros se muestran dentro del cuadro de agrupación.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Opcional) Repita los pasos anteriores para agregar hasta 3 agrupaciones.

   El número de campos seleccionados para la agrupación se muestra junto al icono Grouping.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Opcional) Dentro del cuadro **Agrupar registros por**, haga clic en el icono **x** a la derecha de un campo seleccionado para la agrupación para quitar la agrupación

   O

   Haga clic en **Borrar todo** para eliminar todos los campos.

1. Haga clic fuera del cuadro **Agrupar registros por** para cerrarlo.
1. (Opcional) Haga clic en **Configuración** y, a continuación, en **Color** para añadir agrupaciones con códigos de color. Para obtener más información, consulte la sección [Editar la configuración de la vista de la cronología](#edit-the-timeline-view-settings) en este artículo.
   <!--1. (Optional) Click **Breakdown** to display connected records on the timeline. For information, see the section [Use the Breakdown feature to display connected records in the timeline view](#break-down-connected-records-in-the-timeline-view)-->

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Editar la configuración de vista de cronología {#edit-the-timeline-view-settings}

Actualice la configuración de vista de escala de tiempo para indicar qué información se muestra en la sección de escala de tiempo de la vista y cómo.

1. Cree una vista de escala de tiempo para un tipo de registro, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Haga clic en **Configuración**.
1. Haga clic en **Fecha y hora** en el panel izquierdo, luego seleccione una **fecha de inicio** y una **fecha de finalización** para mostrar en la cronología. Puede elegir las fechas de inicio y finalización predeterminadas, o bien puede elegir cualquier campo de fecha disponible. Las barras que representan los registros comienzan en la fecha que se indica para la fecha Start y finalizan en la fecha correspondiente a End date.

   >[!NOTE]
   >
   >Los registros que no tienen valores para las fechas Start o End o que tienen una fecha Start posterior a End no se muestran en la vista de escala de tiempo.

1. Haga clic en **Estilo de barra** en el panel izquierdo para indicar qué campos desea mostrar en las barras de registros.

   El campo principal (o título) del registro, tal como se define en la vista de tabla del registro, está seleccionado de forma predeterminada. <!--adjust this when the primary field is released??-->

1. (Opcional y condicional) Si ha agregado miniaturas a los registros, seleccione la opción Miniatura para mostrar la imagen asociada a los registros en la barra de registros.

   >[!NOTE]
   >
   >    Primero debe agregar miniaturas en la vista de tabla para poder mostrarlas en la vista de escala de tiempo. Para obtener más información, vea [Agregar una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Haga clic en **Agregar campo** para agregar hasta 4 campos a las barras de registros.
1. Haga clic dentro del cuadro **Buscar campos** y haga clic en el campo que desee agregar.

   >[!TIP]
   >
   >   * Debe crear los campos para poder agregarlos a las barras de registros.
   > 
   >   * Debe haber seleccionado al menos un campo. **Nombre** está seleccionado de manera predeterminada.

   A la derecha aparece una vista previa del aspecto que tendrán las barras en la cronología.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Haga clic en **Color** en el panel izquierdo para personalizar los colores de los registros y agrupaciones en la cronología.

   ![](assets/color-tab-timeline-view.png)

1. (Condicional y opcional) Si agregó una agrupación a la vista de escala de tiempo, seleccione entre las siguientes opciones para establecer un color para la agrupación en la sección **Establecer color de agrupación**:

   * **Predeterminado (gris)**: el color de las agrupaciones está establecido en gris. Esta es la opción predeterminada.
   * **Valores de campo**: El color de las agrupaciones coincide con el color del campo por el que se agrupa.

     >[!NOTE]
     >
     >    * Puede hacer coincidir el color solo con campos con opciones codificadas por colores. Por ejemplo, puede hacer coincidir el color con los campos de Estado o con las opciones asociadas con los colores.
     >    
     >    * No se puede hacer coincidir el color con los campos de búsqueda de tipos de objeto o registro vinculados.


   Por ejemplo, los campos de selección múltiple o de selección única pueden tener opciones codificadas por colores.

   Si agrupa por campos sin opciones codificadas por colores, el color de agrupación permanece gris.

   >[!TIP]
   >
   >Si no ha agregado agrupaciones a la vista de cronología, esta sección no se muestra.

1. En la sección **Establecer color de registro**, seleccione entre las siguientes opciones para establecer un color para los registros:

   * **Tipo de registro**: El color de los registros coincide con el color del tipo de registro seleccionado. Esta es la opción predeterminada.
   * **Valores de campo**: El color de los registros coincide con el color de un campo que especifique. Continúe con el paso 10. <!--ensure this stays accurate-->
   * **Agrupación**: El color de los registros coincide con el color indicado para las agrupaciones. Esta opción aparece atenuada cuando no se han aplicado agrupaciones a la vista de escala de tiempo.
   * **Ninguno**: los registros se muestran en una barra blanca.

1. (Condicional) Si seleccionó **Valores de campo** para los colores de registro, seleccione un campo en el menú desplegable **Coincidir el color del registro con**.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   En el menú desplegable solo se muestran los campos con opciones codificadas por colores.

   Por ejemplo, los campos de selección múltiple o de selección única pueden tener opciones codificadas por colores.

   Si no tiene ningún campo con opciones codificadas por colores para el tipo de registro seleccionado, esta opción aparece atenuada.

1. Haga clic en **Guardar**.

   Los registros se muestran en la vista de escala de tiempo con las especificaciones seleccionadas.

<!--
### Use the Breakdown feature to display connected records in the timeline view

You can display connected records in a record's timeline view by using the Breakdown feature. Breaking down records by their connections allows you to view the timelines of other connected records and understand how they might affect the performance and deadlines of your records. 

#### Considerations when using the Breakdown feature

* You can display connected records or objects under the records of the selected record type in the timeline view. 
* You can display the following in the timeline view, using the Breakdown feature:
    * Workfront Planning records connected to the selected record type. 
    * Workfront (*************or AEM Assets*************)  object types connected to the selected record type.
    * Workfront Planning records or objects from other application that are connected to records connected to the selected record type. 
    
        For example, you might connect campaigns to portfolios. In addition, you might connect  another record type, products, with projects, as well as with campaigns. When you build the campaign timeline view, you can break down the campaigns by portfolios, products, and projects. 

* You cannot display object types that are connected only to Workfront objects in Workfront, but are not connected to a Workfront Planning record type. You can only display object or record types that are connected in Workfront Planning. 

    For example, tasks, are connected to projects in Workfront. Using the Breakdown feature, you can display projects that are connected to campaigns in Planning, but not tasks connected to projects in Workfront. 

    If you want to display both portfolios and projects in the timeline view of a Workfront Planning record type, both the portfolios and the projects must be connected to the Planning record or to a record connected to the Planning record whose timeline view you are managing.
* You can only display record types that are associated with at least two date fields. 
* The date fields for the record types you want to display in the timeline view must be visible in the table view of the selected record type, as lookup fields. 
* The Start and End dates of the record types you want to display in the timeline view must by in chronological order. For example, if a record has a Start date of January 31 and an End date of January 1, it does not display in the timeline view. For more information, see the section [Manage a timeline view](#manage-a-timeline-view) in this article. 
* There is a limit of 5 record types that you can include in a record's breakdown. 


#### Break down connected records in the timeline view

1. Create a timeline view for a record type, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Click **Breakdown**.
1. Expand the **Select a linked record type** box and select a connected record type. (**************add new screen shot***************)

    ![](assets/breakdown-picker-and-button-on-timeline.png)

    >[!TIP]
    >
    >    If you do not have any connected records, or if the connected records do not have at least two date fields, the **Select a linked record type** box is not available.

1. Choose a **Start date** and an **End date field**.

    >[!TIP]
    >
    >    The Start and End dates must be sequential. If the End date is before the Start date, no records will display in the timeline. 

    A right-pointing arrow displays on the selected record's bar in the timeline, if they they are connected with other records. 

    ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)    


1. (Optional) Repeat the steps above to add more connected records. 

    >[!TIP]
    >
    >    You can add up to 5 connected records in a timeline using the Breakdown feature. 


-->