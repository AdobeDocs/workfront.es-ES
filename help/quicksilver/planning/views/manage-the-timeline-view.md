---
title: Administrar la vista de cronología
description: Acceda y edite registros en una vista de cronología de la página de tipo de registro de Adobe Workfront Planning. Este artículo describe cómo crear una vista de escala de tiempo y editar o eliminar una existente. Personalice la cronología con filtros, agrupaciones y ajustes. Utilice la función Desglose para mostrar los registros conectados.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '2874'
ht-degree: 62%

---

# Administrar la vista de cronología

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede mostrar registros en una vista de línea de tiempo al acceder a la página de tipo de registro en Adobe Workfront Planning.

Para obtener información sobre las vistas de registros, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

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
<p>Cualquiera </p> 
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
   <td><p> Estándar </p>
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
   <td>   <p>Permisos de administración de una vista</p>  
   <p>Permisos de visualización de una vista para cambiar temporalmente su configuración</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya Planning.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar una vista de línea de tiempo {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Al crear una vista de línea de tiempo, todos los registros del tipo de registro seleccionado se muestran en una línea de tiempo cronológica.

Tenga en cuenta lo siguiente:

* Solo puede crear una vista de línea de tiempo si tiene al menos dos campos de fecha asociados a un tipo de registro. Cuando hay uno o ningún campo de fecha asociado a un tipo de registro, la opción de vista de línea de tiempo aparece atenuada.

  Puede seleccionar los siguientes campos de fecha al crear una vista de cronología:

   * Registrar fechas
   * Registrar campos generados por el sistema: fecha de creación, fecha de la última modificación
   * Buscar fechas de tipos de objeto o registro conectados.
* Según las fechas asociadas a los registros, es posible que algunos no se muestren en la vista de línea de tiempo en los siguientes casos:

   * Cuando las fechas de inicio y finalización no tienen valores
   * Cuando las fechas de inicio y finalización no tienen valor
   * Cuando la fecha de inicio es posterior a la fecha de finalización

Para administrar una vista de línea de tiempo:

1. Vaya a la página del tipo de registro cuya línea de tiempo desea ver.
1. Cree una vista de línea de tiempo, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

   ![Ejemplo de vista de escala de tiempo](assets/timeline-view-example.png)

   Los registros asociados al tipo de registro seleccionado se muestran como barras en una línea de tiempo y se ordenan en orden cronológico según su fecha de inicio de forma predeterminada.

   >[!TIP]
   >
   >    La ordenación de los registros en la línea de tiempo no es visible en la vista compacta.

1. (Opcional y condicional) Cuando el nombre del registro esté truncado, pase el ratón sobre una barra de registros para mostrar el nombre completo del registro y la información adicional.

1. Realice una de las siguientes acciones para navegar por la línea de tiempo:

   * Haga clic en los iconos izquierdo y derecho o utilice el desplazamiento horizontal para moverse hacia atrás y hacia adelante en la línea de tiempo. Al actualizar la página, se conserva el lapso de tiempo seleccionado.
   * Haga clic en **Hoy** para centrar la línea de tiempo en la fecha de hoy.
   * Seleccione una de las siguientes opciones del menú desplegable de lapso de tiempo para actualizar los incrementos de tiempo:

      * Año
      * Trimestre
      * Mes
1. Haga clic en **Cambiar a vista estándar** para mostrar los registros en líneas independientes <!--check to see if they updated the name of the setting here-->

   O

   Haga clic en **Cambiar a la vista compacta** para mostrar los registros cuyas fechas no se cruzan en la misma línea. <!--check to see if they updated the name of the setting here-->

   Los registros se muestran en la vista Compacta de forma predeterminada.

1. Haga lo siguiente para buscar rápidamente registros que coincidan con una palabra clave:

   1. Haga clic en el icono **Buscar** ![Icono de búsqueda](assets/search-icon.png) y empiece a escribir una palabra clave asociada a cualquier campo de un registro que se muestra en la pantalla. El número de coincidencias correctas se muestra junto al elemento de búsqueda y el registro con la coincidencia correcta se resalta.

      ![Vista de cuadro de búsqueda y escala de tiempo de resultados](assets/search-box-and-results-timeline-view.png)

      Puede utilizar cualquier palabra o carácter especial que esté visible en la pantalla.

      No se pueden utilizar palabras clave asociadas a campos que no se muestran en la vista de línea de tiempo.

   1. Pulse Intro en el teclado para ir al siguiente campo encontrado.
   1. (Opcional) Si hay más de una coincidencia, haga clic en las flechas arriba y abajo situadas a la derecha de la palabra clave de búsqueda para encontrar todas las coincidencias de la tabla.
   1. Haga clic en el icono **x** en el cuadro de búsqueda para borrar la palabra clave de búsqueda.

1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Filtros](#add-filters)
   * [Agrupación](#add-grouping)
   * [Configuración](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. (Opcional) Haga clic en **Desglose** para mostrar los registros conectados en la cronología.

   Para obtener más información, vea la sección [Usar la característica Desglose para mostrar los registros conectados en la vista de escala de tiempo](#break-down-connected-records-in-the-timeline-view)

### Añadir filtros

Puede reducir la cantidad de información que se muestra en la pantalla mediante filtros.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de línea de tiempo:

<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para una vista de línea de tiempo funcionarán de forma independiente de los filtros de cualquier otra vista aplicada al mismo tipo de registro.

* Los filtros son exclusivos de la vista que seleccione. Dos vistas de línea de tiempo del mismo tipo de registro pueden tener diferentes filtros aplicados.

* Dos usuarios que ven la misma vista de línea de tiempo ven el mismo filtro que se aplica actualmente.

* No puede asignar un nombre a los filtros que genere para una vista de línea de tiempo.

* Al eliminar los filtros, se eliminan de todos los usuarios que tengan acceso al mismo tipo de registro que usted y que muestren la misma vista que usted.

* Añadir filtros en la vista de línea de tiempo es idéntico a añadir filtros en la vista de tabla.

  Para obtener más información, consulte la sección “Añadir filtros” del artículo [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Puede filtrar por campos de registro conectados o por campos de búsqueda.
* Puede filtrar por campos de búsqueda que muestren varios valores.


### Agregar agrupación

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Es posible agrupar registros por información similar al aplicar una agrupación a una vista.

Añadir agrupaciones en la vista de línea de tiempo es similar a añadir agrupaciones a la vista de tabla.

Tenga en cuenta lo siguiente al trabajar con agrupaciones en la vista de línea de tiempo:

* Es posible aplicar agrupaciones tanto en las vistas de tabla como de línea de tiempo. Las agrupaciones de la vista de tabla son independientes de las de la vista de línea de tiempo del mismo tipo de registro.
* Se pueden aplicar 3 niveles de agrupación en una vista. Los registros se agrupan en el orden de agrupaciones que se seleccione.
&lt;!--* Es posible aplicar hasta 4 niveles de agrupación al utilizar la API. --comprobando este ahora-->
* Las agrupaciones son únicas para la vista que se seleccione. Dos vistas de tabla del mismo tipo de registro pueden tener diferentes agrupaciones aplicadas. Dos usuarios que vean la misma vista de tabla verán la misma agrupación que se aplique en ese momento.
* No se puede asignar un nombre a las agrupaciones que se generen para una vista de tabla.
* Al quitar las agrupaciones, se quitarán de cualquier usuario que tenga acceso al mismo tipo de registro y que muestre la misma vista que usted.
* Es posible editar los registros enumerados bajo una agrupación.
* Es posible agrupar por campos de registro conectados o campos de búsqueda.
* Cuando se agrupan por campos de búsqueda con varios valores (que no se hayan resumido por un agregador), los registros se agruparán según cada combinación única de valores de campo.
* Puede hacer referencia a un campo que esté situado a una distancia de hasta 4 niveles del tipo de registro actual. Por ejemplo, si se crea una agrupación para un tipo de registro de actividad y la actividad estuviera conectada al tipo de registro de producto, que está conectado al tipo de registro de campaña, y que está conectado a un proyecto de Workfront, se podrá hacer referencia al estado del proyecto en la agrupación que esté creando para el tipo de registro de actividad.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Para añadir una agrupación en la vista de línea de tiempo:

1. Cree una vista de línea de tiempo para un tipo de registro, tal y como se describe en el artículo [Administración de vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Haga clic en **Agrupación** en la esquina superior derecha de la vista de línea de tiempo.

   ![Vista de línea de tiempo de IU de agrupación con campos vinculados](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Haga clic en uno de los campos sugeridos o haga clic en **Elegir un campo diferente**, busque un campo diferente y, a continuación, haga clic en él cuando se muestre en la lista.

   La agrupación se aplica automáticamente a la línea de tiempo y los registros se muestran dentro del cuadro de agrupación.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Opcional) Repita los pasos anteriores para añadir hasta 3 agrupaciones.

   El número de campos seleccionados para la agrupación se muestra junto al icono de Agrupación.

   <!-- update screen shot with view redesign-->

   ![La agrupación se aplica en la vista de escala de tiempo](assets/grouping-applied-in-timeline-view.png)

1. (Opcional) Dentro del cuadro **Agrupar registros por**, haga clic en el icono **x** a la derecha de un campo seleccionado para la agrupación para quitar la agrupación

   O

   Haga clic en **Borrar todo** para quitar todos los campos.

1. Haga clic fuera del cuadro **Agrupar registros por** para cerrarlo.
1. (Opcional) Haga clic en **Configuración** y, a continuación, en **Color** para añadir agrupaciones con códigos de color. Para obtener más información, consulte la sección [Editar la configuración de la vista de línea de tiempo](#edit-the-timeline-view-settings) en este artículo.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Editar la configuración de la vista de línea de tiempo {#edit-the-timeline-view-settings}

Actualice la configuración de la vista de línea de tiempo para indicar qué información se muestra en la sección de línea de tiempo de la vista y cómo se muestra.

1. Cree una vista de línea de tiempo para un tipo de registro, tal y como se describe en el artículo [Administración de vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. Haga clic en **Configuración**.
1. Haga clic en **Fecha y hora** en el panel izquierdo, luego seleccione una **Fecha de inicio** y una **Fecha de finalización** para mostrar en la línea de tiempo. Puede elegir las fechas de inicio y finalización predeterminadas, o bien puede elegir cualquier campo de fecha disponible. Las barras que representan los registros comienzan en la fecha que se indica para la Fecha de inicio y finalizan en la fecha correspondiente a la Fecha de finalización.

   >[!NOTE]
   >
   >Los registros que no tienen valores para las fechas de inicio o finalización o que tienen una fecha de inicio posterior a la fecha de finalización no se muestran en la vista de línea de tiempo.

1. Haga clic en **Estilo de barra** en el panel izquierdo para indicar qué información desea mostrar en las barras de registro.

   El campo principal (o título) del registro, tal y como se define en la vista de tabla del registro, está seleccionado de forma predeterminada. <!--adjust this when the primary field is released??-->

1. (Opcional y condicional) Si ha añadido miniaturas a los registros, seleccione la opción Miniatura para mostrar la imagen asociada a los registros en la barra de registros.

   >[!NOTE]
   >
   >    Primero debe añadir miniaturas en la vista de tabla para poder mostrarlas en la vista de línea de tiempo. Para obtener más información, consulte [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Haga clic en **Agregar campo**, luego haga clic dentro del cuadro **Buscar campos** y luego haga clic en el campo que desee agregar.

   >[!TIP]
   >
   >   * Debe crear los campos antes de poder añadirlos a las barras de registro.
   > 
   >   * Debe tener al menos un campo seleccionado. **Nombre** está seleccionado de manera predeterminada.
   >
   >   * Se pueden añadir hasta cinco campos.

   A la derecha aparece una vista previa del aspecto que tendrán las barras en la línea de tiempo.

   ![Registrar configuración de escala de tiempo del panel de detalles con vista previa](assets/record-details-panel-timeline-settings-with-preview.png)

1. <span class="preview"> (opcional y condicional) Si muestra la cronología en el modo Estándar, habilite la configuración **Detalles de la barra de truncado**. Cuando está habilitada, la información de las barras de registros se trunca y sólo se muestra completamente al pasar el ratón por encima de las barras. Esta configuración está deshabilitada de forma predeterminada y la información se muestra completamente en las barras. </span>

   ![Se ha resaltado la configuración de truncado en el cuadro de configuración de la cronología](assets/truncate-setting-enabled-on-timeline-settings-highlighted.png)

   >[!TIP]
   >
   >* <span class="preview">La configuración Truncar detalles de barra no está disponible cuando se muestra la vista de escala de tiempo en el modo compacto y no está disponible en la vista Calendario.</span>
   >
   >* <span class="preview">Si desglosa la vista de escala de tiempo para mostrar los objetos conectados, la configuración Truncar bar details sólo se aplica al tipo de registro principal. No se aplica a las barras de registros conectadas.</span>


1. Haga clic en **Color** en el panel izquierdo para personalizar los colores de los registros y agrupaciones en la línea de tiempo.

   ![Vista de la cronología de la ficha de color](assets/color-tab-timeline-view.png)

1. (Condicional y opcional) Si ha añadido una agrupación a la vista de línea de tiempo, seleccione una de las siguientes opciones para establecer un color para la agrupación en la sección **Establecer color de agrupación**:

   * **Predeterminado (gris)**: el color de las agrupaciones está establecido en gris. Es la opción predeterminada.
   * **Valores de campo**: el color de las agrupaciones coincide con el color del campo por el que se agrupa.

     >[!NOTE]
     >
     >    * Puede hacer coincidir el color solo con los campos con opciones codificadas por colores. Por ejemplo, puede hacer coincidir el color con campos de Estado, o campos con opciones asociadas a colores.
     >    
     >    * No se puede hacer coincidir el color con los campos de búsqueda de tipos de objeto o registro vinculados.


   Por ejemplo, los campos de selección múltiple o de selección única pueden tener opciones codificadas por colores.

   Si agrupa por campos sin opciones codificadas por colores, el color de agrupación permanece gris.

   >[!TIP]
   >
   >Si no ha añadido agrupaciones a la vista de línea de tiempo, esta sección no aparece.

1. En la sección **Establecer color de registro**, seleccione entre las siguientes opciones para establecer un color para los registros:

   * **Tipo de registro**: el color de los registros coincide con el color del tipo de registro seleccionado. Esta es la opción predeterminada.
   * **Valores de campo**: el color de los registros coincide con el color de un campo que especifique. Continúe con el paso 10. <!--ensure this stays accurate-->
   * **Agrupación**: el color de los registros coincide con el color indicado para las agrupaciones. Esta opción aparece atenuada cuando no se han aplicado agrupaciones a la vista de línea de tiempo.
   * **Ninguno**: los registros se muestran en una barra blanca.

1. (Condicional) Si ha seleccionado **Valores de campo** para los colores de registro, seleccione un campo en el menú desplegable **Hacer coincidir el color del registro con**.

   ![Menú desplegable de selector de campo en la vista de cronología](assets/field-selector-drop-down-menu-timeline-view.png)

   En el menú desplegable solo se muestran los campos con opciones codificadas por colores.

   Por ejemplo, los campos de selección múltiple o de selección única pueden tener opciones codificadas por colores.

   Si no tiene ningún campo con opciones codificadas por colores para el tipo de registro seleccionado, esta opción aparece atenuada.

1. Haga clic en **Guardar**.

   Los registros se muestran en la vista de línea de tiempo con las especificaciones seleccionadas.

### Desglose de registros conectados en la vista de cronología

Puede mostrar los registros conectados en la vista de escala de tiempo de un registro mediante la función Desglose. El desglose de registros por sus conexiones le permite ver las escalas de tiempo de otros registros conectados y comprender cómo pueden afectar al rendimiento y a los plazos de los registros.

#### Consideraciones al utilizar la función Desglose

* Puede mostrar registros u objetos conectados debajo de los registros del tipo de registro seleccionado en la vista de escala de tiempo.
* Puede mostrar lo siguiente en la vista de cronología mediante la función Desglose:
   * Registros de Workfront Planning conectados al tipo de registro seleccionado.
   * Tipos de objetos Workfront o recursos Experience Manager conectados al tipo de registro seleccionado.
   * Registros de Workfront Planning u objetos de otra aplicación conectados a registros conectados al tipo de registro seleccionado.

     Por ejemplo, puede conectar campañas a portafolios. Además, puede conectar otro tipo de registro, productos, con proyectos, así como con campañas. Cuando genere la vista de la cronología de la campaña, puede desglosar las campañas por portafolios, productos y proyectos.

* No se pueden mostrar tipos de objetos que sólo están conectados a objetos de Workfront en Workfront, pero que no están conectados a un tipo de registro de Workfront Planning. Sólo se pueden mostrar los tipos de objetos o registros conectados en Workfront Planning.

  Por ejemplo, las tareas están conectadas a proyectos en Workfront. Con la función Desglose, puede mostrar los proyectos que están conectados a campañas en Planning, pero no las tareas conectadas a proyectos en Workfront.

  Si desea mostrar tanto los portafolios como los proyectos en la vista de escala de tiempo de un tipo de registro de Workfront Planning, tanto los portafolios como los proyectos deben estar conectados al registro de Planning o a un registro conectado al registro de Planning cuya vista de escala de tiempo esté administrando.
* Solo puede mostrar tipos de registro asociados con al menos dos campos de fecha.
* Los campos de fecha para los tipos de registro que desea mostrar en la vista de escala de tiempo deben estar visibles en la vista de tabla del tipo de registro seleccionado, como campos de búsqueda.
* Las fechas de inicio y finalización de los tipos de registro que desea mostrar en la vista de escala de tiempo deben estar en orden cronológico. Por ejemplo, si un registro tiene una fecha de inicio del 31 de enero y una fecha de finalización del 1 de enero, no se muestra en la vista de escala de tiempo. Para obtener más información, consulte la sección [Administrar una vista de escala de tiempo](#manage-a-timeline-view) en este artículo.
* Hay un límite de 5 tipos de registros que puede incluir en el desglose de un registro.

#### Desglose de registros conectados

1. Cree una vista de línea de tiempo para un tipo de registro, tal y como se describe en el artículo [Administración de vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).
1. (Condicional) Si está viendo la vista de escala de tiempo en el modo Estándar, haga clic en **Desglose**.
1. Expanda el cuadro **Seleccionar un tipo de registro vinculado** y seleccione un tipo de registro conectado. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![Selector de desglose y botón en la vista de cronología](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Si no tiene ningún registro conectado o si los registros conectados no tienen al menos dos campos de fecha, la casilla **Seleccionar un tipo de registro vinculado** no está disponible.

1. Elija **fecha de inicio** y **campo de fecha de finalización**.

   >[!TIP]
   >
   >    Las fechas de inicio y finalización deben ser secuenciales. Si la fecha de finalización es anterior a la fecha de inicio, no se mostrará ningún registro en la cronología.

   Si están conectados con otros registros, aparecerá una flecha hacia la derecha en la barra del registro seleccionado de la escala de tiempo.
1. Haga clic en la flecha que señala a la derecha para expandir un tipo de registro y mostrar sus conexiones.

   ![Campañas desglosadas por programas en la vista de escala de tiempo](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (Opcional) Repita los pasos anteriores para agregar más registros conectados.



