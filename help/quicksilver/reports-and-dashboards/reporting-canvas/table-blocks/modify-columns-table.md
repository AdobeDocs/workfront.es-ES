---
title: Configuración de una columna de tabla en el Lienzo de informes
description: Configuración de una columna de tabla en el Lienzo de informes
author: Nolan
feature: Reports and Dashboards
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 2%

---


# Configuración de una columna de tabla en el Lienzo de informes

Las columnas de una tabla se pueden configurar para su visualización. Puede modificar los siguientes aspectos de una columna:

* Nombre
* Ordenar
* Editar permiso
* Texto al pasar el cursor
* Agregación
* Formato condicional

## Requisitos previos

Antes de comenzar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Reporting Canvas beta: información general](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Modificar columnas en una tabla

1. Vaya a un informe existente y haga clic en el botón **Más menú** icono ![](assets/more-icon.png) en el encabezado del informe, seleccione **Editar**.
1. En el encabezado de tabla del informe, haga clic en el botón **Editar** icono ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si acaba de crear la tabla y aún no ha añadido ningún campo, haga clic en el botón Editar en el centro de la tabla.

1. (Opcional) Añada, vuelva a colocar o elimine columnas de la tabla. Para obtener más información sobre la edición de campos en una tabla, consulte [Agregar o editar un bloque de tabla en el Lienzo de informes](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Añadir una columna nueva | Para agregar una columna a una tabla, haga clic y arrastre un campo desde el **Campos** a la derecha de la página en la tabla donde desee colocarla, o haga doble clic en un campo para agregarlo como la columna más a la derecha. |
   |---|---|
   | Mover una columna | Para reorganizar el orden de las columnas de una tabla, haga clic en el nombre de una columna y arrástrela a una nueva ubicación. |
   | Eliminar una columna | Para eliminar una columna de una tabla, haga clic en la columna que desee eliminar y luego haga clic en la x a la derecha del nombre de la columna. |

   {style=&quot;table-layout:auto&quot;}

1. Para configurar una columna, haga clic en el nombre de la columna que desee modificar en la fila de encabezado de la tabla y, a continuación, en una de las fichas siguientes del panel derecho:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-step-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Ficha Datos</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Acumulado basado en</td>
      <td><p> Para acumular (resumir en el encabezado) la información de una columna, seleccione el tipo de agregación que desee en el <strong>Agregado basado en</strong> menú desplegable. Las opciones disponibles dependen del tipo de datos contenido en la columna .</p><p>Si utiliza grupos en la tabla, el valor agregado aparece en la fila del grupo por encima del nombre de la columna en lugar de junto al nombre de la columna.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Formato de campo</td>
      <td><p>(Disponible solo cuando la columna contiene datos de fecha, porcentaje, moneda o hora, no texto). Seleccione el formato que desee para los datos en la <b>Formato de campo</b> lista desplegable. Por ejemplo, puede mostrar signos de porcentaje después de los números de una columna o cambiar la forma en que se muestran las fechas.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">El campo es editable</td>
      <td><span>Active la variable <strong>El campo es editable</strong> si desea permitir que los usuarios que ven la tabla editen el nombre de la columna.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Ordenar</strong></td>
      <td><p>De forma predeterminada, la tabla se ordena según los datos de la columna situada más a la izquierda, en orden ascendente. Para ordenar por la columna seleccionada en su lugar, haga clic en la flecha hacia abajo situada junto a <strong>Ordenar</strong>y, a continuación, haga clic en la casilla de verificación <b>Ordenar por esta columna</b>. A continuación, puede seleccionar un <strong>Ordenar</strong> dirección (valores ascendentes o descendentes) y <strong>Orden</strong> (la prioridad de clasificación relativa de esta columna comparada con otras columnas de clasificación de la tabla).</p><p>Puede repetir este proceso para ordenar la tabla por un máximo de 5 columnas diferentes. Asegúrese de que cada columna tiene la correcta <strong>Orden</strong> en relación con las columnas nuevas que seleccione para ordenar.</p><p>Nota: Si elimina una columna que está seleccionada para ordenar una tabla y otra columna también está seleccionada para ordenarla, esa columna se utiliza para ordenar la tabla en su lugar en orden descendente. Si no hay otras columnas seleccionadas para ordenar, la tabla vuelve al valor predeterminado: ordenar por su primera columna.</p><p>Cuando se designa una columna para ordenar la tabla, aparece un pequeño cuadro junto al nombre de la columna con un número que indica la prioridad relativa de esa columna al ordenar la tabla (la tabla se ordena primero por 1, después por 2, etc.) y una flecha para indicar si la dirección de clasificación es ascendente o descendente. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Ficha Estilo</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Etiqueta de columna personalizada</strong> </td> 
      <td>Introduzca un nuevo nombre para mostrar para la columna (límite de 100 caracteres).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar la activación del texto</td> 
      <td> <p>Determine si desea que se muestre texto explicativo cuando alguien pase el ratón por encima del nombre de una columna.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto al pasar el cursor</td> 
      <td>(Disponible solo cuando <strong>Mostrar texto al pasar el ratón por encima</strong> está activada). Personalice el texto explicativo que aparece cuando alguien pasa el ratón por encima del nombre de una columna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato condicional</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Agregar <img src="assets/add-rule.png">, editar <img src="assets/edit-icon.png">o eliminar <img src="assets/delete.png"> regla que da formato a las celdas de la columna cuando sus valores cumplen los criterios especificados.</p> <p>Por ejemplo, puede crear una regla que cambie la fuente del campo "Estado del proyecto" a negrita morada cuando el valor de ese campo sea igual a "Generación".</p> <p>O puede usar <b>Mostrar un icono</b> para agregar un icono de indicador verde a todos los elementos de la columna que tengan el estado "Actual".</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Nota: Si usa <strong>Mostrar un icono</strong>, las demás opciones de formato no están disponibles.</p> <p>Puede seleccionar <strong>Se aplican a toda la fila</strong> si desea que el formato afecte a toda la fila de una celda que cumpla la condición de la regla. Por ejemplo, puede resaltar los proyectos que vencen después de una fecha determinada aplicando un color de fondo amarillo no solo a las celdas de fecha de la columna "Vencimiento", sino a toda la fila donde se producen esas fechas.</p> <p>Sugerencia: A medida que agrega opciones de formato a una regla, el formato de celda resultante se muestra en <strong>Vista previa</strong> en la parte inferior del panel.</p> </li> 
        <li value="2">Cuando haya terminado de agregar una regla, haga clic en <strong>Guardar</strong>.</li> 
        <li value="3"> <p>(Opcional) Haga clic en <b>+ Agregar regla</b> para agregar reglas adicionales a la misma columna.</p> <p>Se aplican varias reglas de formato condicional en una tabla en el siguiente orden:</p> 
         <ul> 
          <li> <p>Las reglas que se aplican a filas enteras se evalúan primero, de izquierda a derecha para cada columna y después de arriba a abajo en una columna.</p> <p>Nota: El formato de fila anulará otros formatos condicionales para las celdas de esa fila, incluso si cumplirían la condición de la regla de otra columna.</p> </li> 
          <li> <p>A continuación, se evalúan otras reglas, de arriba a abajo, ya que aparecen enumeradas en el panel derecho de una columna. Puede arrastrar <img src="assets/drag-object-icon.png"> las reglas guardadas en ese panel para modificar su orden.</p> <p>Nota: Las celdas tienen un formato basado en la primera condición que cumplen y no se les aplicará ningún formato aunque cumplan otras condiciones.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en el **Volver** en la esquina superior izquierda de la pantalla para volver al informe.
