---
title: Administrar la vista de cronología
description: Puede mostrar registros en una vista de escala de tiempo al acceder a la página de tipo de registro en Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---


# Administrar la vista de cronología

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede mostrar registros en una vista de escala de tiempo al acceder a la página de tipo de registro en Adobe Maestro.

Para obtener información acerca de las vistas Maestro, vea [Administrar vistas de registros en Adobe Maestro](../views/manage-record-views.md).

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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Administrar una vista de cronología {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Al crear una vista de escala de tiempo, todos los registros del tipo de registro seleccionado se muestran en una escala de tiempo cronológica.

Tenga en cuenta lo siguiente:

* Sólo puede crear una vista Cronología si tiene al menos dos campos de fecha asociados a un tipo de registro. Cuando hay uno o ningún campo de fecha asociado a un tipo de registro, la opción de vista Cronología aparece atenuada.
* Según las fechas asociadas con los registros, es posible que algunos registros no se muestren en la vista de escala de tiempo en los siguientes casos:

   * Cuando las fechas de inicio y finalización no tienen valores
   * Cuando las fechas de inicio y finalización no tienen valor
   * Cuando la fecha de inicio es posterior a la fecha de finalización

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

Al crear una vista de escala de tiempo, todos los registros del tipo de registro seleccionado se muestran en una escala de tiempo como barras de forma predeterminada.

Para administrar una vista de cronología:

1. Vaya a la página del tipo de registro cuya cronología desea ver.
1. Cree una vista de cronología, tal como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Los registros asociados con el tipo de registro seleccionado se muestran en una cronología cronológica en forma de barras.

1. Realice una de las siguientes acciones para navegar por la cronología:

   * Haga clic en los iconos izquierdo y derecho o utilice el desplazamiento horizontal para moverse hacia atrás y hacia adelante en la cronología.
   * Clic **Hoy** para centrar la cronología en la fecha actual.
   * Seleccione una de las siguientes opciones del menú desplegable lapso de tiempo para actualizar los incrementos de tiempo:

      * Año
      * Trimestre
      * Mes
1. Clic **Cambiar a estándar** vista para mostrar registros en líneas independientes <!--check to see if they updated the name of the setting here-->

   O

   Clic **Cambiar a la vista Compacta** para mostrar los registros cuyas fechas no se cruzan en la misma línea. <!--check to see if they updated the name of the setting here-->

   Los registros se muestran en la vista Compacta de forma predeterminada.

1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Filtros](#add-filters)
   * [Agrupación](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [Configuración](#edit-the-timeline-view-settings)

### Añadir filtros

Los filtros le ayudan a reducir la cantidad de información que se muestra en la pantalla.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de cronología:

<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para la vista de cronología funcionarán de forma independiente de los filtros de la vista de tabla cuando se apliquen al mismo tipo de registro.

* Los filtros son exclusivos de la vista seleccionada. Dos vistas de escala de tiempo del mismo tipo de registro pueden tener diferentes filtros aplicados. Dos usuarios que ven la misma vista de cronología ven el mismo filtro que se aplica actualmente.

* No puede asignar nombres a los filtros que genere y aplique a una vista de cronología.

* Al eliminar los filtros, se eliminan de todos los usuarios que tienen acceso al mismo tipo de registro que usted y que utilizan la misma vista que utiliza.

Añadir filtros en la vista de cronología es idéntico a añadir filtros en la vista de tabla.

Para obtener más información, consulte la sección &quot;Agregar filtros&quot; en el artículo [Administrar la vista de tabla](../views/manage-the-table-view.md).

### Agregar agrupación

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


Puede agrupar registros por información similar al aplicar una agrupación a una vista.

Tenga en cuenta lo siguiente al trabajar con agrupaciones en la vista de cronología:

* Puede aplicar agrupaciones tanto en las vistas de tabla como de escala de tiempo. Las agrupaciones de la vista de tabla son independientes de las de la vista de escala de tiempo del mismo tipo de registro.
* Puede aplicar tres niveles de agrupación en una vista Maestro. Los registros se agrupan en el orden de agrupaciones que seleccione.
* Puede aplicar hasta 4 niveles de agrupación al utilizar la API.

Para agregar una agrupación:

1. Cree una vista de cronología, tal como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).
1. Clic **Agrupación**.

   ![](assets/grouping-ui-timeline-view.png)

1. Haga clic en uno de los campos sugeridos o en **Elija un campo diferente** y busque un campo diferente y, a continuación, haga clic en él cuando se muestre en la lista.

   >[!TIP]
   >
   >No se pueden seleccionar campos vinculados.

   La agrupación se aplica automáticamente a la cronología y los registros se muestran dentro del cuadro de agrupación. El número de elementos de una agrupación se muestra en la línea de agrupación.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Opcional) Repita los pasos anteriores para agregar hasta 3 agrupaciones.

   El número de agrupaciones aplicadas se muestra a la izquierda del icono Agrupación en la esquina superior derecha de la barra de herramientas.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Opcional) Haga clic en **x** a la derecha de una agrupación para eliminar la agrupación

   O

   Clic **Borrar todo** para quitar todas las agrupaciones.

1. Haga clic fuera de **Agrupar registros por** para cerrarlo.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Editar la configuración de vista de cronología {#edit-the-timeline-view-settings}

Actualice la configuración de vista de escala de tiempo para indicar qué información se muestra en la sección de escala de tiempo de la vista.

1. Cree una vista de cronología, tal como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).
1. Clic **Configuración**.
1. Clic **Fecha y hora** en el panel izquierdo, seleccione una **Fecha de inicio** y un **Fecha de finalización** para mostrar en la cronología. Puede elegir las fechas de inicio y finalización predeterminadas, o bien puede elegir cualquier campo de fecha disponible. Las barras que representan los registros comienzan en la fecha que se indica para la fecha Start y finalizan en la fecha correspondiente a End date.

   >[!NOTE]
   >
   >    Los registros que no tienen valores para las fechas Start o End o que tienen una fecha Start posterior a End no se muestran en la vista de escala de tiempo.


1. Clic **Registrar detalles** para indicar qué campos desea mostrar en los tableros de registros.

   El campo Name está seleccionado de forma predeterminada.

1. Clic **Añadir campo** para agregar hasta 4 campos a las barras de registros.
1. Haga clic dentro de **Campos de búsqueda** y haga clic en el campo que desee añadir.

   >[!TIP]
   >
   >   * Debe crear los campos para poder agregarlos a las barras de registros.
   > 
   >   * Debe haber seleccionado al menos un campo. **Nombre** está seleccionado de forma predeterminada.

   A la derecha aparece una vista previa del aspecto que tendrán las barras en la cronología.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Haga clic en **Guardar**.

   Los registros se muestran en la vista de escala de tiempo con las especificaciones seleccionadas.


