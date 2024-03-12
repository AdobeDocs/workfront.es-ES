---
title: Administrar la vista de tabla
description: Puede mostrar los registros y sus campos en una vista de tabla al acceder a la página de tipo de registro en las funciones de planificación de Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 4c62b567fa1ebec37fc64831757eb67d4a048c1f
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 3%

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

{{maestro-important-intro}}

Puede mostrar los registros y sus campos en una vista de tabla al acceder a la página de tipo de registro en las funciones de planificación de Adobe Workfront.

Para obtener información sobre las vistas de registros y cómo administrarlas, consulte [Administrar vistas de registros](../views/manage-record-views.md).

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
<p>Su organización debe estar inscrita en el programa beta cerrado de capacidades de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td role="rowheader">Configuración del nivel de acceso</td>
   <td> <p>No hay controles de nivel de acceso para las capacidades de planificación de Adobe de Workfront </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos de la vista</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Administración de una vista de tabla {#manage-a-table-view}

<!--insert screen shot of table view-->

Al crear una vista de tabla, todos los registros del tipo seleccionado se muestran en una tabla. Cada fila es un registro único y cada columna es un campo de registro. Todos los campos y todos los registros se muestran de forma predeterminada.

Para administrar una vista de tabla:

1. Cree una vista de tabla como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. (Opcional) Haga clic en **Altura de fila**, luego seleccione entre las siguientes opciones para modificar la altura de las filas de la tabla:
   * Baja
   * Media
   * Alta

1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Columnas (o campos)](#add-columns-or-fields)
   * [Filas (o registros)](#add-rows-or-records)
   * [Filtros](#add-filters)
   * [Agrupación](#add-groupings)
   * [Ordenar](#add-a-sort)


### Agregar columnas (o campos) {#add-columns}

Los encabezados de columna de una vista de tabla muestran los campos asociados a los registros de la vista. Los mismos campos mostrados en la vista de tabla también se muestran en la sección Detalles de un registro. Para obtener más información, consulte [Edición de registros](../records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

Añadir columnas a una vista es idéntico a añadir campos a un tipo de registro.

Puede agregar hasta 500 campos (o columnas) en una vista de tabla.

1. Vaya a una página de tipo de registro y seleccione un **Tabla** vista desde el menú desplegable vista.

   <!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. Empiece a agregar campos (o columnas), tal como se describe en el artículo [Creación de campos](../fields/create-fields.md).

   Las columnas que agregue serán visibles para todos los usuarios que tengan acceso al tipo de registro y se agregarán como campos nuevos en la página Detalles de los registros del tipo de registro seleccionado.

1. Realice una de las siguientes acciones para reordenar las columnas de la tabla:

   * Coja el encabezado de la columna y arrástrela y suéltela en la posición deseada. La columna que ha movido aparece brevemente con un fondo azul hasta que realice otros ajustes en la tabla.

   * Clic **Campos** en la barra de herramientas de la tabla, arrastre y suelte los campos en el orden deseado y, a continuación, haga clic fuera de **Visibilidad y orden de los campos** para cerrarlo.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* El campo Nombre es siempre el primer campo de la vista de tabla, de forma predeterminada. Se considera un campo principal.
     >
     >* No puede mover el campo Nombre a otra posición, a menos que designe otro campo como campo principal. Para obtener más información, continúe con el paso 4. <!--accurate?-->
     >
     >* No se puede ocultar ni eliminar un campo principal.
     >
     >* El campo principal está congelado y no forma parte del desplazamiento horizontal.

   * Reemplace el campo de la primera columna por otro campo cambiando el campo principal. Para obtener más información, siga con el paso 4. <!--accurate?-->

1. (Opcional) Pase el ratón sobre un nombre de campo en el encabezado de columna de cualquier campo que no se muestre en la primera columna de la tabla, haga clic en la flecha hacia abajo a la derecha del nombre del campo y, a continuación, haga clic en **Establecer como campo principal**.

   ![](assets/set-as-primary-field-option-table-view.png)

1. Clic **Definir campo** para confirmar.

   El campo se convierte en un campo principal, lo que significa que se muestra como la primera columna de la vista de tabla. El campo principal anterior se desplaza a la segunda columna.

   >[!NOTE]
   >
   >   * Solo pueden ser campos principales los campos de los siguientes tipos:
   >
   >       * Texto de línea única
   >       * Número
   >       * Fórmula
   >
   >   * El campo principal siempre está congelado y no se puede mover. Puede seleccionar otro campo para reemplazar un campo principal si necesita moverlo a otra posición.
   >
   >   * Cambiar el campo principal en la vista de tabla afecta a la vista de todos los demás usuarios que lo elijan.
   >
   >   * Cambiar el campo principal en una vista de tabla afecta a todas las vistas de tabla.
   >
   >   * No se puede eliminar ni ocultar un campo principal.
   >
   >   * El valor enumerado en el campo principal siempre tiene un hipervínculo a la página Detalles del registro.

1. Haga clic en las líneas de separación de columnas, arrástrelas y suéltelas en el lugar deseado para aumentar el ancho de las columnas.

   >[!TIP]
   >
   >Los cambios que realice en el ancho y el orden de las columnas son permanentes y visibles para todos los usuarios que tengan acceso al tipo de registro.

1. Pase el ratón sobre el encabezado de la columna, haga clic en la flecha hacia abajo y luego haga clic en **Ocultar campo**

   O

   Clic **Campos** en la barra de herramientas de la tabla, deshabilite la opción asociada a los campos (o columnas) que desee ocultar. El **Visibilidad y orden de los campos** aparece el cuadro.

   >[!TIP]
   >
   >El número de campos ocultos se muestra a la izquierda del icono Campos de la barra de herramientas.


1. Haga clic en **Campos** y active la opción asociada a los campos que desea mostrar en las columnas de la tabla. Todos los campos se muestran de forma predeterminada.

1. Haga lo siguiente para buscar rápidamente registros que coincidan con una palabra clave:

   1. Haga clic en **Buscar** icono ![](assets/search-icon.png) y empiece a escribir una palabra clave asociada a cualquier campo de un registro que se muestra en la pantalla. El número de coincidencias correctas se muestra junto al elemento de búsqueda y el campo con la coincidencia correcta está resaltado.

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      Puede utilizar cualquier palabra o carácter especial que esté visible en la pantalla.

      No se pueden utilizar palabras clave asociadas a campos que están ocultos en la vista de tabla.

   1. Prensa **Entrar** en el teclado para ir al siguiente campo encontrado.

   1. (Opcional) Si hay más de una coincidencia, haga clic en las flechas arriba y abajo a la derecha de la palabra clave de búsqueda para encontrar todas las coincidencias de la tabla.

   1. Haga clic en **x** en el cuadro de búsqueda para borrar la palabra clave de búsqueda.


### Agregar filas (o registros) {#add-rows}

Las filas de una vista de tabla muestran registros individuales del tipo de registro seleccionado.

Puede tener hasta 50 000 registros (o filas) para un tipo de registro S.

1. Vaya a una página de tipo de registro y seleccione un **Tabla** vista desde el menú desplegable vista.

<!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. Empiece a agregar registros (o filas), tal como se describe en el artículo [Creación de registros](../records/create-records.md).

   Los registros que agregue a la vista de tabla se guardan inmediatamente y son visibles para todos los usuarios que tengan permisos de Vista o superiores en el área de trabajo.

1. (Opcional) Agregue una miniatura a cada registro y haga clic en **Campos** en la esquina superior derecha de la tabla, seleccione la opción para **Miniatura** para mostrarlo a la izquierda del campo principal. De forma predeterminada, no está seleccionada.

   Para obtener más información, consulte [Añadir miniaturas a los registros](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

1. (Opcional) Seleccione uno o varios registros de una fila y, a continuación, arrastre y suelte el **manipular** icono ![](assets/handle-icon.png) a la izquierda del nombre del registro para reordenar las filas.

   >[!NOTE]
   >
   >No puede reordenar filas si aplica al menos una ordenación a la vista de tabla.

   <!-- this is not possible right now:

    1. To reorder the rows, click the row header, drag and drop it in the desired location. 

        The changes you make to the row order are permanent and visible to all users who access the record type
    -->

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Añadir filtros {#add-filters}

Los filtros le ayudan a reducir la cantidad de información que se muestra en la pantalla.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de tabla:
<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para la vista de tabla funcionan de forma independiente de los filtros de la vista de cronología cuando se aplican al mismo tipo de registro.

* Los filtros son exclusivos de la vista seleccionada. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes filtros aplicados. Dos usuarios que ven la misma vista de tabla ven el mismo filtro que se aplica actualmente.

* No puede asignar un nombre a los filtros que genere y aplique a una vista de tabla.

* Al eliminar los filtros, se eliminan de todos los que tengan acceso al mismo tipo de registro que usted y utilicen la misma vista que utiliza.

* Añadir filtros a la vista de tabla es idéntico a añadir filtros a la vista de cronología.

* Puede filtrar por campos de registro conectados o campos de búsqueda, pero no por los campos que permiten la vinculación a varios registros.

Para agregar un filtro a una vista de tabla:

1. Cree una vista de tabla para una página de tipo de registro, tal como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).
1. Seleccione una vista de tabla y haga clic en **Filtros** en la esquina superior derecha de la tabla.
1. Clic **Añadir condición** y añada la siguiente información:

   * Seleccione un campo por el que desee filtrar <!-- the tip below might change-->

   * Seleccione una opción (o un modificador de filtro) para definir qué tipo de condición debe cumplir el campo

     La tabla siguiente muestra los modificadores disponibles para cada tipo de campo.

     <table>
        <thead>
        <tr>
            <th><b>Tipo de campo</b></th>
            <th><b>Modificadores</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Una línea, párrafo, fórmula </td>
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
            <td>Selección múltiple, Personas</td>
            <td><p>Tiene cualquiera de</p>
            <p>Tiene todas de</p>
            <p>Es exactamente</p>
            <p>No tiene ninguno de</p>
            <p>Está vacío</p>
            <p>No está vacío</p></td>
        </tr>
        <tr>
            <td>Número, Porcentaje, Moneda</td>
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
            <p>Es anterior a</p>
            <p>Está entre</p><p>No está entre</p>
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

### Agregar agrupaciones {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Puede agrupar registros por información similar al aplicar una agrupación a una vista.

Agregar agrupaciones en la vista de tabla es similar a agregar agrupaciones a la vista de escala de tiempo.

Tenga en cuenta lo siguiente:

* Puede aplicar agrupaciones tanto en las vistas de tabla como de escala de tiempo. Las agrupaciones de la vista de tabla son independientes de las de la vista de escala de tiempo del mismo tipo de registro.
* Se pueden aplicar 3 niveles de agrupación en una vista. Los registros se agrupan en el orden de agrupaciones que seleccione.
&lt;!—* Puede aplicar hasta 4 niveles de agrupación al utilizar la API. —comprobando este por ahora—>
* Las agrupaciones son únicas para la vista que seleccione. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes agrupaciones aplicadas. Dos usuarios que ven la misma vista de tabla ven la misma agrupación que se aplica actualmente.
* No puede asignar un nombre a las agrupaciones que genere para una vista de tabla.
* Al quitar las agrupaciones, se quitan de cualquier usuario que tenga acceso al mismo tipo de registro que usted y que muestre la misma vista que usted.
* Puede editar los registros enumerados bajo una agrupación.
* Puede agrupar por campos de registro conectados o campos de búsqueda, pero no para los campos que permiten la vinculación a varios registros.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Para agregar una agrupación:

1. Cree una vista de cronología para un tipo de registro, tal como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).
1. Clic **Agrupación** en la esquina superior derecha de la vista de tabla.

   ![](assets/grouping-ui-table-view-with-linked-fields.png)

1. Haga clic en uno de los campos sugeridos o en **Elija un campo diferente**, busque un campo diferente y, a continuación, haga clic en él cuando se muestre en la lista.

   La agrupación se aplica automáticamente a la tabla y los registros se muestran bajo la línea de separación de agrupación.

1. (Opcional) Repita los pasos anteriores para agregar hasta 3 agrupaciones.

   El número de campos seleccionados para la agrupación se muestra junto al icono Grouping.

   ![](assets/grouping-applied-in-table-view.png)

1. (Opcional) Dentro de **Agrupar registros por** , haga clic en **x** a la derecha de un campo seleccionado para que la agrupación elimine la agrupación

   O

   Clic **Borrar todo** para eliminar todos los campos.

1. Haga clic fuera de **Agrupar registros por** para cerrarlo.
1. (Opcional) Haga clic en **+ Nuevo &lt; Nombre del tipo de registro >** al final de cualquier agrupación para agregar nuevos registros, actualice la página para agregar el nuevo registro a la agrupación adecuada. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

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

* Los campos vinculados solo se pueden ordenar si permiten valores únicos o valores de selección múltiple con la opción de resumen seleccionada (suma, promedio, máximo, mínimo).

* Al quitar los criterios de ordenación, se quitan de cualquier usuario que tenga acceso al mismo tipo de registro que usted y utilice la misma vista que utiliza.

* Puede ordenar por campos de registro conectados o campos de búsqueda, pero no por los campos que permiten la vinculación a varios registros.

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

1. (Opcional) En el **Ordenar registros por** , haga clic en **x** a la derecha de un campo de clasificación para eliminar la clasificación

   O

   Clic **Borrar todo** para eliminar todos los campos de la ordenación.

1. Haga clic fuera de **Ordenar registros por** para cerrarlo.

   ![](assets/sorting-in-table-view.png)

   La información mostrada en la tabla se ordena según los criterios seleccionados.

   Los campos seleccionados para la ordenación muestran un icono de ordenación seguido de un número que indica el orden en que se aplica la ordenación.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->
