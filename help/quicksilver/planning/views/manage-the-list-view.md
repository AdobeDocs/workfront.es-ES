---
title: Administrar la vista de lista en Adobe Workfront Planning
description: Puede mostrar objetos y sus campos en una vista de lista, al acceder a ellos en la página Registros conectados de un registro, en Adobe Workfront Planning. Este artículo describe cómo se puede crear o editar una vista de lista en la página Registros conectados de un registro.
feature: Workfront Planning
role: User
hidefromtoc: true
hide: true
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '3339'
ht-degree: 67%

---


<!--add these to the metadata above when publishing:

author: Alina
recommendations: noDisplay, noCatalog-->

# Administrar la vista de lista en Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede mostrar objetos y sus campos en una vista de lista, al acceder a ellos en la página Registros conectados de un registro, en Adobe Workfront Planning.

Este artículo describe cómo se puede crear o editar una vista de lista en la página Registros conectados de un registro y cómo se pueden editar los objetos de la vista.

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
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p> Estándar para crear y eliminar vistas</p>
   <p>Colaborador o superior para actualizar los elementos de vista</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración de una vista</p>  
   <p>Ver permisos en una vista para cambiar temporalmente la configuración de la vista o para duplicarla</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Consideraciones sobre las vistas de lista

* No puede ver registros en las páginas de tipo de registro en una vista de lista. Sólo se pueden mostrar los objetos siguientes en una vista de lista cuando se ven en la página Registros conectados de un registro:

   * Proyectos Workfront

  Para obtener información acerca de cómo crear una página de registros conectados, vea [Agregar una página de registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Para poder ver una vista de lista en una página de registros conectada de un registro, debe conectar los proyectos de Workfront con los tipos de registros de Planning. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
* Las vistas de lista son similares a las listas mejoradas. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Administración de una vista de lista {#manage-a-list-view}

{{step1-to-planning}}

1. Haga clic en una tarjeta de espacio de trabajo y, a continuación, haga clic en una tarjeta de tipo de registro.
1. Desde cualquier vista, haga clic en el nombre de un registro para abrir la página de vista previa o de detalles del registro.
1. Agregue una **página Registros conectados** para proyectos conectados como se describe en el artículo [Agregar una página Registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

   La página Registros conectados muestra los proyectos conectados al registro en la vista de lista.

   ![Proyectos en la página de registros conectados en la vista de lista](assets/projects-on-connected-records-page-list-view.png)

<!--BELOW IS ALL FROM TABLE VIEW - EDIT EVERYTHING-->

1. Cree una vista de tabla, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

   ![Ejemplo de vista de tabla](assets/table-view-example.png)

1. (Opcional) Haga clic en **Altura de la fila** y, a continuación, seleccione una de las siguientes opciones para modificar la altura de las filas de la tabla:
   * Baja
   * Media
   * Alta

1. (Opcional) Haga clic en el icono **Pantalla completa** ![Abrir icono de pantalla completa](assets/open-full-screen-icon.png) para abrir la vista en pantalla completa y, a continuación, en el icono **Salir de pantalla completa** ![Salir del icono de pantalla completa](assets/exit-full-screen-icon.png) o Escape del teclado para salir de la pantalla completa.

1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Columnas (o campos)](#add-columns-or-fields)
   * [Filas (o registros)](#add-rows-or-records)
   * [Filtros](#add-filters)
   * [Ordenar](#add-a-sort)
   * [Agrupación](#add-groupings)
   * [Colores de la fila](#add-row-colors)
   * [Indicador de presencia en tiempo real](#enable-the-real-time-presence-indicator)


### Añadir columnas (o campos) {#add-columns}

Los encabezados de columna de una vista de tabla muestran los campos asociados a los registros de la vista. Los campos mostrados en la vista de tabla también se muestran en la sección Detalles de un registro.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

Añadir columnas a una vista es idéntico a añadir campos a un tipo de registro.

Puede añadir hasta 500 campos (o columnas) en una vista de tabla.

1. Vaya a una página de tipo de registro y haga clic en una ficha de vista de tabla, o bien haga clic en **+ Vista** para añadir una nueva vista y, a continuación, elija **Tabla**.

1. Empiece a añadir campos (o columnas), tal como se describe en el artículo [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

   Las columnas que añada serán visibles para todos los usuarios que tengan acceso al tipo de registro y se añadirán como campos nuevos en la página del registro.

1. (Opcional) Haga clic en el icono **Campos** ![Icono de Campos](assets/fields-icon.png) en la barra de herramientas, busque un campo y, a continuación, anule la selección del botón de alternancia a la derecha del nombre del campo para ocultar el campo.

1. Realice una de las siguientes acciones para reordenar las columnas de la tabla:

   * Arrastre el encabezado de la columna y suéltelo en la posición deseada. La columna que ha movido se mostrará brevemente con un fondo azul hasta que realice otros ajustes en la tabla.

   * Haga clic en **Campos** en la barra de herramientas de la tabla, arrastre y suelte los campos en el orden deseado y, a continuación, haga clic fuera del cuadro **Visibilidad y orden de los campos** para cerrarlo.

     ![Campos configurando la barra de herramientas de la vista de tabla expandida](assets/fields-setting-table-view-toolbar-expanded.png)

     >[!TIP]
     >
     >* El campo Nombre es siempre el primer campo de la vista de tabla, de forma predeterminada. Se considera un campo principal
     >
     >* No puede mover el campo Nombre a otra posición, a menos que designe otro como campo principal. Para obtener más información, continúe en el paso 4. <!--accurate?-->
     >
     >

   * Reemplace el campo de la primera columna por otro cambiando el campo principal. Para obtener más información, continúe en el paso 4. <!--accurate?-->

1. (Opcional) Pase el puntero por encima de un nombre de campo en el encabezado de columna de cualquier campo que no se muestre en la primera columna de la tabla, haga clic en la flecha hacia abajo situada a la derecha del nombre del campo y, a continuación, haga clic en **Establecer como campo principal**.

   ![Establecer como opción de campo principal en la vista de tabla](assets/set-as-primary-field-option-table-view.png)

1. Haga clic en **Establecer campo** para confirmar.

   El campo se convertirá en un campo principal, lo que significa que se mostrará como la primera columna de la vista de tabla. El campo principal anterior se desplazará a la segunda columna.

   Los campos principales se convierten en el título del registro y se muestran en el área de encabezado de la página del registro y en cualquier lugar donde se muestren los registros. Por ejemplo, el título del registro se muestra en los campos conectados y en todas las vistas. Para obtener más información acerca de los campos principales, consulte [Información general sobre el campo principal](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Haga clic en las líneas de separación de columnas, y arrástrelas y suéltelas en el lugar deseado para aumentar la anchura de las columnas.

   >[!TIP]
   >
   >Los cambios que realice en la anchura y el orden de las columnas serán permanentes y visibles para todos los usuarios que tengan acceso al tipo de registro.

1. Pase el puntero por encima del encabezado de la columna, haga clic en la flecha que apunta hacia abajo y, a continuación, en **Ocultar campo**

   O

   Haga clic en **Campos** en la barra de herramientas de la tabla y deshabilite el conmutador asociado a los campos (o columnas) que desee ocultar. Se mostrará el cuadro **Visibilidad y orden de los campos**.

   >[!TIP]
   >
   >El número de campos ocultos se muestra a la izquierda del icono Campos de la barra de herramientas.
   >
   ><span class="preview">De forma predeterminada, los campos ocultos no se muestran en el cuadro de vista previa **Detalles** del registro. Todos los campos se muestran en la página Detalles del registro. Para obtener más información, vea [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md)</span>


1. Haga clic en el icono **Campos** y habilite la opción asociada a los campos que desea mostrar en las columnas de la tabla. Todos los campos se mostrarán de forma predeterminada.

1. Haga lo siguiente para buscar rápidamente registros que coincidan con una palabra clave:

   1. En el cuadro **Buscar** ![Icono de búsqueda](assets/search-icon.png) y empiece a escribir una palabra clave asociada a cualquier campo de un registro que se muestra en la pantalla. El número de coincidencias correctas se mostrará junto al elemento de búsqueda y el campo con la coincidencia correcta quedará resaltado.

      ![Cuadro de búsqueda con contorno azul de resultados en la vista de tabla](assets/search-box-with-results-blue-outline-table-view.png)

      Puede utilizar cualquier palabra o carácter especial que esté visible en la pantalla.

      No se pueden utilizar palabras clave asociadas a campos que estén ocultos en la vista de tabla.

   1. Pulse **Intro** en el teclado para ir al siguiente campo encontrado.

   1. (Opcional) Si hay más de una coincidencia, haga clic en las flechas arriba y abajo situadas a la derecha de la palabra clave de búsqueda para encontrar todas las coincidencias de la tabla.

   1. Haga clic en el icono **x** en el cuadro de búsqueda para borrar la palabra clave de búsqueda.


### Añadir filas (o registros) {#add-rows}

Las filas de una vista de tabla muestran registros individuales del tipo de registro seleccionado.

Puede tener hasta 50 000 registros (o filas) para un tipo de registro.

1. Vaya a una página de tipo de registro y haga clic en una ficha de vista de tabla, o bien haga clic en **+ Vista** para añadir una nueva vista y, a continuación, elija **Tabla**.

1. Empiece a añadir registros (o filas), tal como se describe en el artículo [Crear registros](/help/quicksilver/planning/records/create-records.md).

   Los registros que añada a la vista de tabla se guardarán inmediatamente y serán visibles para todos los usuarios que tengan permisos de vista o superiores sobre el área de trabajo.

1. (Opcional) Añada una miniatura a cada registro, haga clic en **Campos** en la esquina superior derecha de la tabla y, a continuación, seleccione el conmutador del campo **Miniatura** para mostrarlo a la izquierda del campo principal. De forma predeterminada, no está seleccionado.

   Para obtener más información, consulte [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Opcional) Seleccione uno o varios registros de una fila y, a continuación, arrastre y suelte el icono **controlador** ![icono de controlador](assets/handle-icon.png) a la izquierda del registro para reordenar las filas.

   >[!NOTE]
   >
   >No se pueden reordenar filas si se aplica al menos una ordenación a la vista de tabla.
   >
   >Los cambios que realice en el orden de filas serán visibles para todos los usuarios que tengan acceso al tipo de registro

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Añadir filtros {#add-filters}

Los filtros le ayudan a reducir la cantidad de información que se muestra en la pantalla.

Tenga en cuenta lo siguiente cuando utilice filtros en la vista de tabla:

<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para la vista de tabla funcionan de forma independiente de los filtros de la vista de cronología cuando se aplican al mismo tipo de registro.

* Los filtros son exclusivos de la vista que seleccione. En dos vistas de tabla con el mismo tipo de registro se pueden aplicar diferentes filtros. Dos usuarios que consulten la misma vista de tabla verán el mismo filtro aplicado en ese momento.

* No puede asignar un nombre a los filtros que genere y aplique a una vista de tabla.

* Al quitar los filtros, se quitarán para todas las personas que tengan acceso al mismo tipo de registro que usted y utilicen la misma vista que utiliza.

* Puede filtrar por campos de registro conectados o por campos de búsqueda.

* Puede filtrar por campos de búsqueda que muestren varios valores.

* Puede hacer referencia a un campo que esté situado a una distancia de hasta 4 niveles del tipo de registro actual. Por ejemplo, si va a crear un filtro para un tipo de registro de actividad y la actividad está conectada al tipo de registro de producto que está conectado al tipo de registro de campaña que está conectado a un proyecto de Workfront, puede hacer referencia al presupuesto del proyecto en el filtro que va a crear para el tipo de registro de actividad.

Para añadir un filtro a una vista de tabla:

1. Cree una vista de tabla para una página de tipo de registro, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Seleccione una vista de tabla y luego haga clic en **Filtros** en la esquina superior derecha de la tabla.
1. Haga clic en **Añadir condición** y añada la siguiente información:

   * Busque un campo y selecciónelo cuando se muestre en la lista cuando.

   * **Seleccione una opción** (o un modificador de filtro) para definir qué tipo de condición debe cumplir el campo

     En la tabla siguiente se muestran los modificadores disponibles para cada tipo de campo.

     <table>
        <thead>
        <tr>
            <th><b>Tipo de campo</b></th>
            <th><b>Modificadores</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Una sola línea, párrafo, fórmula </td>
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

   ![Vista de tabla de IU de filtro](assets/filter-ui-table-view.png)

   No hay límite en cuanto a las condiciones de filtrado que se pueden añadir.

1. (Opcional) Haga clic en **Añadir condición** para añadir otra opción de filtrado y repita los pasos anteriores. El número de filtros aplicados se muestra a la izquierda del icono Filtros.
1. Haga clic en los siguientes operadores para indicar cómo se unen y deberían aplicarse las condiciones de filtro:

   * **AND**: se deben cumplir todas las condiciones especificadas.
   * **OR**: se debe cumplir cualquiera de las condiciones especificadas. Esta es la opción predeterminada.

   1. (Opcional) Agregue operadores **AND** o **OR** adicionales entre varias agrupaciones de condiciones.

      ![Filtros de varios niveles en las vistas](assets/multi-tiered-filters-in-views.png)

   La lista de registros se filtra automáticamente.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Opcional) Haga clic en el icono **x** para quitar una condición de filtro.
1. (Opcional) Haga clic en **Filtros** para cerrar el cuadro de filtros. <!--right now you cannot "clear all" for filters, but this might come later-->

### Añadir una ordenación {#sort-information}

Al aplicar una ordenación, puede organizar la información en un orden determinado.

Puede ordenar la siguiente información:

* Todos los registros de una vista de tabla. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Tenga en cuenta lo siguiente al ordenar registros en la vista de tabla:

<!-- if this is available for the timeline view, update both when you update one-->

* La ordenación es única para la vista que seleccione. En dos vistas de tabla con el mismo tipo de registro se pueden aplicar diferentes criterios de ordenación. Dos usuarios que consulten la misma vista de tabla verán el mismo orden que se aplica en ese momento.

* No puede asignar un nombre a las ordenaciones que genere y aplique a una vista de tabla.

* El orden creado se conservará cuando deje de navegar.

* Puede ordenar por tantos campos como vea en la vista de tabla de un tipo de registro.

* No puede ordenar por los campos de registro conectados, pero puede ordenar por los campos de búsqueda de tipos de registro conectados.

* Al ordenar por los campos de búsqueda con varios valores (que no se hayan resumido con un agregador), se utiliza el primer valor para ordenar.

* Cuando se quitan los criterios de ordenación, se quitan para cualquier usuario que tenga acceso al mismo tipo de registro que el suyo y utilice la misma vista que utiliza.

* Puede hacer referencia a un campo que esté situado a una distancia de hasta 4 niveles del tipo de registro actual. Por ejemplo, si va a crear una ordenación para un tipo de registro de actividad y la actividad está conectada al tipo de registro de producto que está conectado al tipo de registro de campaña que está conectado a un proyecto de Workfront, puede hacer referencia al estado del proyecto en la ordenación que va a crear para el tipo de registro de actividad.

Para ordenar registros <!--ungrouped (add this when sorting for groupings will be available-->, haga lo siguiente:

1. Cree una vista de tabla, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Haga clic en el icono **Ordenar** ![Icono Ordenar](assets/sort-icon.png) en la esquina superior derecha de la tabla

   O

   Pase el puntero por encima del nombre de una columna en la vista de tabla, haga clic en la flecha hacia abajo a la derecha del nombre del encabezado de la columna y, a continuación, haga clic en **Ordenar por este campo**. El campo se añade como una selección de ordenación en el icono de Ordenar de la esquina superior derecha de la vista de tabla.

1. (Condicional) En el cuadro **Ordenar registros por**, haga clic en uno de los campos sugeridos o haga clic en **Elegir un campo diferente** y busque un campo diferente; a continuación, haga clic en él cuando se muestre en la lista.

   El orden se aplicará automáticamente a la vista de tabla y los registros se mostrarán ordenados según los criterios seleccionados.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Opcional) Haga clic en **Añadir condición** y repita los pasos anteriores para ordenar por campos adicionales.

   El número de campos por el que está ordenando se muestra a la izquierda del icono de Ordenar en la esquina superior derecha de la barra de herramientas. Solo puede elegir campos que se muestran en las columnas de la vista de tabla.

1. (Opcional) En el cuadro **Ordenar registros por**, haga clic en el icono **x** a la derecha de un campo de ordenación para quitar la ordenación

   O

   Haga clic en **Borrar todo** para quitar todos los campos de la ordenación.

1. Haga clic fuera del cuadro **Ordenar registros por** para cerrarlo.

   ![Ordenando en la vista de tabla](assets/sorting-in-table-view.png)

   La información mostrada en la tabla se ordena según los criterios seleccionados.

   Los campos seleccionados para la ordenación muestran un icono de ordenación seguido de un número que indica el orden de aplicación de la ordenación.

### Añadir agrupaciones {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Es posible agrupar registros por información similar al aplicar una agrupación a una vista.

Tenga en cuenta lo siguiente:

* Es posible aplicar agrupaciones tanto en las vistas de tabla como de cronología. Las agrupaciones de la vista de tabla son independientes de las de la vista de cronología del mismo tipo de registro.
* Se pueden aplicar 3 niveles de agrupación en una vista. Los registros se agrupan en el orden de agrupaciones que se seleccione.
&lt;!--* Es posible aplicar hasta 4 niveles de agrupación al utilizar la API. --comprobando este ahora-->
* Las agrupaciones son únicas para la vista que se seleccione. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes agrupaciones aplicadas. Dos usuarios que vean la misma vista de tabla verán la misma agrupación que se aplique en ese momento.
* No se puede asignar un nombre a las agrupaciones que se generen para una vista de tabla.
* Al quitar las agrupaciones, se quitarán de cualquier usuario que tenga acceso al mismo tipo de registro y que muestre la misma vista que usted.
* Es posible editar los registros enumerados bajo una agrupación.
* Es posible agrupar por campos de registro conectados o campos de búsqueda.
* Cuando se agrupan por campos de búsqueda con varios valores (que no se hayan resumido por un agregador), los registros se agruparán según cada combinación única de valores de campo.
* Puede hacer referencia a un campo que esté situado a una distancia de hasta 4 niveles del tipo de registro actual. Por ejemplo, si se crea una agrupación para un tipo de registro de actividad y la actividad estuviera conectada al tipo de registro de producto, que está conectado al tipo de registro de campaña, y que está conectado a un proyecto de Workfront, se podrá hacer referencia al estado del proyecto en la agrupación que esté creando para el tipo de registro de actividad.
* Las agrupaciones se muestran en el orden alfabético de sus valores.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

para añadir una agrupación:

1. Cree una vista de cronología para un tipo de registro, tal y como se describe en el artículo [Administración de vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Haga clic en **Agrupación**, en la esquina superior derecha de la vista de tabla.

   ![Vista de tabla de IU de agrupación con campos vinculados](assets/grouping-ui-table-view-with-linked-fields.png)

1. Haga clic en uno de los campos sugeridos o en **Elegir un campo diferente**, busque uno y luego hágale clic cuando se muestre en la lista.

   La agrupación se aplicará automáticamente a la tabla y los registros se mostrarán bajo la línea de separación de la agrupación.

1. (Opcional) Haga clic en **Añadir condición** y repita los pasos anteriores para añadir hasta 3 agrupaciones.

   El número de campos seleccionados para la agrupación se muestra junto al icono de Agrupación.

   ![Agrupación aplicada en la vista de tabla](assets/grouping-applied-in-table-view.png)



1. (Opcional) Dentro del cuadro **Agrupar registros por**, haga clic en el icono **x** a la derecha de un campo seleccionado para la agrupación para quitar la agrupación

   O

   Haga clic en **Borrar todo** para quitar todos los campos.

1. Haga clic fuera del cuadro **Agrupar registros por** para cerrarlo.
1. (Opcional) Haga clic en **+ Nuevo registro** al final de cualquier agrupación para añadir nuevos registros y, a continuación, actualice la página para añadir el nuevo registro a la agrupación adecuada. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

1. Para expandir o contraer agrupaciones, siga uno de estos procedimientos:

   1. Haga clic en el icono **Agrupación**, luego en **Expandir todo** o **Contraer todo**. Esto expande todas las agrupaciones y subagrupaciones de la vista de tabla.

      ![Expandir y contraer todos los botones de la vista de tabla del cuadro de agrupación](assets/expand-collapse-all-buttons-on-grouping-box-table-view.png)

   1. Haga clic con el botón secundario en cualquiera de los encabezados de agrupación de la vista de tabla y, a continuación, haga clic en una de las siguientes opciones:
      * **Expandir grupo**
      * **Contraer grupo**
      * **Expandir todo**
      * **Contraer todo**
      * **Expandir subgrupos**
      * **Contraer subgrupos**

      Según el número de agrupaciones que aplique a la vista, es posible que algunas opciones no estén disponibles.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->

### Agregar colores de fila

1. (Opcional) Haga clic en **Colores de fila** para definir las condiciones y elegir configurar diferentes colores para las filas de la tabla.

1. Haga clic en **Agregar color**, luego busque un campo y selecciónelo cuando se muestre en la lista. Este es el campo cuyo valor desea determinar el color de una fila.

   Por ejemplo, para mostrar campañas con el estado Activo en verde, seleccione **Estado** y, a continuación, elija un modificador y un valor para el campo.

   ![Cuadro de colores de fila con estado Activo seleccionado y opción de color predeterminada](assets/row-colors-box-with-active-status-selected-default-color-choice.png)

1. Haga clic en el menú desplegable del selector de color en la esquina superior izquierda de la condición seleccionada, para elegir el color de la condición y, a continuación, haga clic fuera del cuadro selector de color para cerrarlo.

   ![Menú desplegable del selector de color en el cuadro Colores de fila resaltado](assets/drop-down-color-picker-menu-in-row-colors-box-highlighted.png)

1. (Opcional) Haga clic en **Agregar condición** para agregar más campos y valores al primer conjunto de condiciones

   O

   Haga clic en **Agregar color** para agregar un nuevo conjunto de condiciones e identificar un nuevo color.

   Por ejemplo, puede mostrar las campañas en un estado de Planning en amarillo definiendo un nuevo conjunto de condiciones.

   ![Cuadro de colores de fila con colores personalizados de estado Activo y Planificación](assets/row-colors-box-with-active-and-planning-status-custom-colors.png)

1. (Opcional) Active la opción **Aplicar a toda la fila** en la esquina superior derecha del cuadro Colores de fila. Toda la fila donde se cumple la condición se muestra automáticamente en el color seleccionado.

   >[!NOTE]
   >
   >* Si la configuración Aplicar a toda la fila está desactivada, solo el lado izquierdo del campo Principal muestra un indicador de color estrecho con el color seleccionado. La configuración está desactivada de forma predeterminada.
   >
   >* No se pueden aplicar colores de fila a toda una fila si se ha seleccionado al menos una agrupación en la vista de tabla.

1. Haga clic fuera del cuadro **Colores de fila** para cerrarlo. Los colores se aplican automáticamente.