---
title: Administrar la vista de tabla
description: Puede mostrar los registros y sus campos en una vista de tabla al tener acceso a la página de tipo de registro en Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: 4a3cf7211eef2b161a29b74e8e9b2b12c21eaf4d
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 5%

---


# Administrar la vista de tabla

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta cerrado que está abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede mostrar los registros y sus campos en una vista de tabla al tener acceso a la página de tipo de registro en Adobe Maestro.

Para obtener información acerca de las vistas de Maestro y cómo administrarlas, vea [Administrar vistas de registros](../views/manage-record-views.md).

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

## Administración de una vista de tabla {#manage-a-table-view}

<!--insert screen shot of table view-->

Al crear una vista de tabla, todos los registros del tipo seleccionado se muestran en una tabla. Cada fila es un registro único y cada columna es un campo de registro. Todos los campos y todos los registros se muestran de forma predeterminada.

Para administrar una vista de tabla:

1. Cree una vista de tabla como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Columnas (o campos)](#add-columns-or-fields)
   * [Filas (o registros)](#add-rows-or-records)
   * [Filtros](#add-filters)
   * [Agrupación](#add-groupings)
   * [Ordenar](#sort-information)


### Agregar columnas (o campos) {#add-columns}

Los encabezados de columna de una vista de tabla de Maestro muestran los campos asociados a los registros de la vista. Los mismos campos mostrados en la vista de tabla también se muestran en la sección Detalles de un registro Maestro. Para obtener más información, consulte [Edición de registros](../records/edit-records.md).

<!-- this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. -->

Añadir columnas a una vista es idéntico a añadir campos a un tipo de registro.

Puede agregar hasta 500 campos (o columnas) en una vista de tabla.

1. Vaya a una página de tipo de registro y seleccione un **Tabla** vista desde el menú desplegable vista.
1. Empiece a agregar campos (o columnas), tal como se describe en el artículo [Creación de campos](../architecture-and-fields/create-fields.md).

   Las columnas que agregue serán visibles para todos los usuarios que tengan acceso al tipo de registro y se agregarán como campos nuevos en la página Detalles de los registros del tipo de registro seleccionado.

1. Para reordenar las columnas de la tabla, siga uno de estos procedimientos:

   * Coja el encabezado de la columna y arrástrela y suéltela en la posición deseada. La columna que ha movido aparece brevemente con un fondo azul hasta que realice otros ajustes en la tabla.

   * Clic **Campos** en la barra de herramientas de la tabla, arrastre y suelte los campos en el orden deseado y, a continuación, haga clic fuera de **Visibilidad de campos y cuadro de orden** para cerrarlo.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)

   >[!TIP]
   >
   >* El campo Nombre es siempre el primer campo de la vista de tabla.
   >
   >* No se puede mover el campo Nombre a otra posición.
   >
   >* No puede ocultar el campo Nombre.
   >
   >* El campo Nombre está inmovilizado y no forma parte del desplazamiento horizontal.

1. Para aumentar el ancho de las columnas, haga clic y arrastre las líneas de separación de columnas y suéltelas en el lugar deseado.

   >[!TIP]
   >
   >Los cambios que realice en el ancho y el orden de las columnas son permanentes y visibles para todos los usuarios que tengan acceso al tipo de registro.

1. Para ocultar una columna, pase el ratón sobre el encabezado de la columna, haga clic en la flecha hacia abajo y, a continuación, haga clic en **Ocultar campo**

   O

   Clic **Campos** en la barra de herramientas de la tabla y desactive la opción asociada a los campos que desea ocultar.

   >[!TIP]
   >
   >El número de campos ocultos se muestra a la izquierda del icono Campos de la barra de herramientas.


1. Desde el **Campos** , active la opción asociada a los campos que desea mostrar en las columnas de la tabla. Todos los campos se muestran de forma predeterminada.

### Agregar filas (o registros) {#add-rows}

Las filas de una vista de tabla de Maestro muestran registros individuales del tipo de registro seleccionado.

Puede tener hasta 10.000 registros (o filas) para un tipo de registro en Maestro.

Agregar filas a una vista de tabla de Maestro es idéntico a crear registros en una tabla.

Para obtener más información, consulte [Creación de registros](../records/create-records.md).

<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### Añadir filtros {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

Los filtros le ayudan a reducir la cantidad de información que se muestra en la pantalla.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de tabla:
<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para la vista de tabla funcionan de forma independiente de los filtros de la vista de cronología cuando se aplican al mismo tipo de registro.

* Los filtros son exclusivos de la vista seleccionada. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes filtros aplicados. Dos usuarios que ven la misma vista de tabla ven el mismo filtro que se aplica actualmente.

* No puede asignar un nombre a los filtros que genere y aplique a una vista de tabla.

* Al eliminar los filtros, se eliminan de todos los que tengan acceso al mismo tipo de registro que usted y utilicen la misma vista que utiliza.

* Añadir filtros a la vista de tabla es idéntico a añadir filtros a la vista de cronología.

Para agregar un filtro a una vista de tabla:

1. Cree una vista de tabla para una página de tipo de registro, tal como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).
1. Seleccione una vista de tabla y haga clic en **Filtros** en la esquina superior derecha de la tabla.
1. Clic **Añadir condición** y añada la siguiente información:

   * Seleccione un campo por el que desee filtrar <!-- the tip below might change-->

   * Seleccione una opción (o un modificador de filtro) para definir qué tipo de condición debe cumplir el campo

     La tabla siguiente muestra los modificadores disponibles para cada tipo de campo.

     >[!TIP]
     >
     > No se pueden seleccionar campos vinculados. Para obtener más información, consulte [Creación de campos](../architecture-and-fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>Tipo de campo</b></th>
            <th><b>Modificadores</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Párrafo de una sola línea </td>
            <td><p>Contiene</p>
            <p>No contiene</p>
            <p>Es</p>
            <p>No es</p>
            <p>Está vacío</p>
            <p>No está vacío</p></td>
        </tr>
        <tr><td>Selección única</td>
            <td><p>Es</p>
            <p>No es</p>
            <p>Es cualquiera de</p>
            <p>No es ninguno de</p>
            <p>Está vacío</p>
            <p>No está vacío</p></td>
        </tr>
        <tr>
            <td>Selección múltiple</td>
            <td><p>Tiene cualquiera de</p>
            <p>Tiene todas de</p>
            <p>Es exactamente</p>
            <p>No tiene ninguno de</p>
            <p>Está vacío</p>
            <p>No está vacío</p></td>
        </tr>
        <tr>
            <td>Numérico, porcentaje, moneda</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Está vacío</p>
            <p>No está vacío</p></td>
        </tr>
        <tr>
            <td>Fecha</td>
            <td><p>Es</p>
            <p>No es</p>
            <p>Es después de</p>
            <p>Es anterior</p>
            <p>Es entre</p><p>No está entre</p>
            <p>Está vacío</p><p>No está vacío</p></td>
        </tr>

     <tr>
            <td>Casilla de verificación</td>
            <td><p>Es</p>
        </tr>
        </tbody>
        </table>

   * Seleccione un valor para el campo seleccionado.

   ![](assets/filter-ui-table-view.png)

   No hay límite en cuanto a las condiciones de filtrado que se pueden añadir.

1. (Opcional) Haga clic en **Añadir condición** para añadir otra opción de filtrado y repita los pasos anteriores. El número de filtros aplicados se muestra a la izquierda del icono Filtros.
1. Haga clic en los siguientes operadores para indicar cómo se unen y deben aplicarse las condiciones de filtro:

   * **Y**: se deben cumplir todas las condiciones especificadas.
   * **O**: se debe cumplir cualquiera de las condiciones especificadas. Esta es la opción predeterminada.

   La lista de registros se filtra automáticamente.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Opcional) Haga clic en **Filtros**, luego haga clic en **x** para eliminar un filtro. <!--right now you cannot "clear all" for filters, but this might come later-->

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. (***************check on this; this might be true for timeline, but not for table??? One dev said in a demo that there are unlimited groupings in a table - check *********************)
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. 
    
        >[!TIP]
        >
        > You cannot select linked fields. For information, see [Create fields](../architecture-and-fields/create-fields.md).  
    The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

-->

### Agregar un orden {#sort-information}

Al aplicar una ordenación, puede organizar la información en un orden determinado.

Puede ordenar la siguiente información:

* Todos los registros de una vista de tabla. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Tenga en cuenta lo siguiente al ordenar registros en la vista de tabla:

<!-- if this is available for the timeline view, update both when you update one-->

* La ordenación es única para la vista seleccionada. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes criterios de ordenación aplicados. Dos usuarios que ven la misma vista de tabla ven el mismo orden que se aplica actualmente.

* No puede asignar un nombre a las ordenaciones que genere y aplique a una vista de tabla.

* El orden que cree se conservará cuando se aleje.

* Puede ordenar por tantos campos como vea mostrados en la vista de tabla de un tipo de registro.

* Al quitar los criterios de ordenación, se quitan de cualquier usuario que tenga acceso al mismo tipo de registro que usted y utilice la misma vista que utiliza.

Para ordenar <!--ungrouped (add this when sorting for groupings will be available--> Registros, haga lo siguiente:

1. Cree una vista de tabla como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).
1. Haga clic en **Ordenar** icono ![](assets/sort-icon.png) en la esquina superior derecha de la tabla

   O

   Pase el ratón sobre el nombre de una columna en la vista de tabla, haga clic en la flecha hacia abajo a la derecha del nombre del encabezado de la columna y, a continuación, haga clic en **Ordenar por este campo**. El campo se agrega como una selección de ordenación en el icono Ordenar de la esquina superior derecha de la vista de tabla.
1. En el **Ordenar registros por** , haga clic en uno de los campos sugeridos o en **Elija un campo diferente** y busque un campo diferente y, a continuación, haga clic en él cuando se muestre en la lista.

   El orden se aplica automáticamente a la vista de tabla y los registros se muestran ordenados según los criterios seleccionados.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Opcional) Repita los pasos anteriores para ordenar por campos adicionales.

   El número de campos por el que está ordenando se muestra a la izquierda del icono Ordenar en la esquina superior derecha de la barra de herramientas. Sólo puede elegir campos que se muestran en las columnas de la vista de tabla.

   >[!TIP]
   >
   > No se pueden seleccionar campos vinculados. Para obtener más información, consulte [Creación de campos](../architecture-and-fields/create-fields.md).

1. (Opcional) En el **Ordenar registros por** , haga clic en **x** a la derecha de un campo de clasificación para eliminar la clasificación

   O

   Clic **Borrar todo** para eliminar todos los campos de la ordenación.

1. Haga clic fuera de **Ordenar registros por** para cerrarlo.

   La información mostrada en la tabla se ordena según los criterios seleccionados.

   Los campos seleccionados para la ordenación muestran un icono de ordenación seguido de un número que indica el orden en que se aplica la ordenación.

   ![](assets/sorting-in-table-view.png)


<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->