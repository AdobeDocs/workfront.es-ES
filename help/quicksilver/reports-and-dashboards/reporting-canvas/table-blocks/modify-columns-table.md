---
title: Configuración de una columna de tabla en el lienzo de informes
description: Configuración de una columna de tabla en el lienzo de informes
author: Nolan
feature: Reports and Dashboards
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 2%

---


# Configuración de una columna de tabla en el lienzo de informes

Las columnas de una tabla se pueden configurar para su visualización. Puede modificar los siguientes aspectos de una columna:

* Nombre
* Ordenar
* Editar permiso
* Texto al pasar el cursor
* Agregación
* Formato condicional

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Resumen de Lienzo de informes beta](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Modificación de columnas de una tabla

1. Vaya a un informe existente y haga clic en **Menú Más** icono ![](assets/more-icon.png) en el encabezado del informe, seleccione **Editar**.
1. En el encabezado de tabla del informe, haga clic en **Editar** icono ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si acaba de crear la tabla y aún no ha agregado ningún campo, haga clic en el botón Editar en el centro de la tabla.

1. (Opcional) Agregue, cambie de posición o elimine columnas de la tabla. Para obtener más información sobre cómo editar los campos de una tabla, consulte [Adición o edición de un bloque de tabla en el lienzo de informes](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Añadir una columna nueva | Para agregar una columna a una tabla, haga clic en un campo y arrástrelo desde el **Campos** panel situado a la derecha de la página en la tabla donde desea colocarla, o haga doble clic en un campo para agregarlo como la columna situada más a la derecha. |
   |---|---|
   | Mover una columna | Para reorganizar el orden de las columnas de una tabla, haga clic en el nombre de una columna y arrástrela a una nueva ubicación. |
   | Eliminación de una columna | Para eliminar una columna de una tabla, haga clic en la columna que desee eliminar y, a continuación, haga clic en la x situada en la parte derecha del nombre de la columna. |

   {style="table-layout:auto"}

1. Para configurar una columna, haga clic en el nombre de la columna que desea modificar en la fila de encabezado de la tabla y, a continuación, en una de las siguientes pestañas del panel derecho:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-step-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Pestaña Datos</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Acumulado basado en</td>
      <td><p> Para agregar (resumir en el encabezado) la información de una columna, seleccione el tipo de agregación que desee en la <strong>Acumulado basado en</strong> menú desplegable. Las opciones disponibles dependen del tipo de datos contenidos en la columna.</p><p>Si utiliza grupos en la tabla, el valor agregado se muestra en la fila del grupo encima del nombre de la columna en lugar de junto al nombre de la columna.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Formato de campo</td>
      <td><p>(Disponible únicamente cuando la columna contiene datos de fecha, porcentaje, moneda u hora, no texto). Seleccione el formato que desee para los datos en la <b>Formato de campo</b> menú desplegable. Por ejemplo, puede mostrar símbolos de porcentaje después de los números de una columna o cambiar la forma en que se muestran las fechas.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">El campo es editable</td>
      <td><span>Habilite la <strong>El campo es editable</strong> si desea permitir que los usuarios que ven la tabla editen el nombre de la columna.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Ordenar</strong></td>
      <td><p>De forma predeterminada, la tabla se ordena en orden ascendente según los datos de la columna situada más a la izquierda. Para ordenar por la columna seleccionada, haga clic en la flecha hacia abajo situada junto a <strong>Ordenar</strong>, luego haga clic en la casilla de verificación <b>Ordenar por esta columna</b>. A continuación, puede seleccionar una <strong>Ordenando</strong> dirección (valores ascendentes o descendentes) y un <strong>Orden de clasificación</strong> (la prioridad relativa de ordenación de esta columna comparada con otras columnas de ordenación de la tabla).</p><p>Puede repetir este proceso para ordenar la tabla por hasta 5 columnas diferentes. Asegúrese de que cada columna tiene el <strong>Orden de clasificación</strong> en relación con cualquier columna nueva que seleccione para ordenar.</p><p>Nota: Si elimina una columna seleccionada para ordenar una tabla y también se selecciona otra columna para ordenar, esa columna se utiliza para ordenar la tabla en lugar de en orden descendente. Si no hay otras columnas seleccionadas para ordenar, la tabla vuelve al valor predeterminado: ordenar por su primera columna.</p><p>Cuando se designa una columna para ordenar la tabla, aparece un pequeño cuadro junto al nombre de la columna con un número que indica la prioridad relativa de la columna al ordenar la tabla (la tabla se ordena primero por 1, luego 2, etc.) y una flecha para indicar si la dirección de ordenación es ascendente o descendente. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Pestaña Estilo</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Etiqueta de columna personalizada</strong> </td> 
      <td>Introduzca un nuevo nombre para mostrar para la columna (límite de 100 caracteres).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar la activación del texto</td> 
      <td> <p>Determine si desea que se muestre texto explicativo cuando alguien pasa el ratón sobre un nombre de columna.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto al pasar el cursor</td> 
      <td>(Disponible solo cuando <strong>Mostrar texto de desplazamiento</strong> está activada). Personalice el texto explicativo que se muestra cuando alguien pasa el ratón sobre un nombre de columna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato condicional</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Añadir <img src="assets/add-rule.png">, editar <img src="assets/edit-icon.png">, o eliminar <img src="assets/delete.png"> regla que da formato a las celdas de la columna cuando sus valores cumplen los criterios especificados.</p> <p>Por ejemplo, puede crear una regla que cambie la fuente del campo "Estado del proyecto" a negrita morada cuando el valor de ese campo sea igual a "Generando".</p> <p>O puede usar <b>Mostrar un icono</b> para añadir un icono de indicador verde a cada elemento de la columna que tenga el estado "Actual".</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Nota: Si utiliza <strong>Mostrar un icono</strong>Sin embargo, las demás opciones de formato no están disponibles.</p> <p>Puede seleccionar <strong>Aplicar a toda la fila</strong> si desea que el formato afecte a toda la fila de una celda que cumpla la condición de la regla. Por ejemplo, puede resaltar proyectos que vencen después de una fecha determinada aplicando un color de fondo amarillo no solo a las celdas de fecha de la columna "Vence el", sino a toda la fila en la que se producen esas fechas.</p> <p>Sugerencia: A medida que se añaden opciones de formato a una regla, el formato de celda resultante se muestra en <strong>Previsualizar</strong> en la parte inferior del panel.</p> </li> 
        <li value="2">Cuando termine de agregar una regla, haga clic en <strong>Guardar</strong>.</li> 
        <li value="3"> <p>(Opcional) Haga clic en <b>+ Agregar regla</b> para agregar reglas adicionales a la misma columna.</p> <p>Varias reglas de formato condicional en una tabla se aplican en el siguiente orden:</p> 
         <ul> 
          <li> <p>Las reglas que se aplican a filas completas se evalúan primero, de izquierda a derecha para cada columna y, a continuación, de arriba abajo dentro de una columna.</p> <p>Nota: El formato de fila anula cualquier otro formato condicional de las celdas de esa fila, incluso si cumplen la condición de la regla de otra columna.</p> </li> 
          <li> <p>A continuación, se evalúan otras reglas, de arriba a abajo, tal como se enumeran en el panel derecho de una columna. Puede arrastrar <img src="assets/drag-object-icon.png"> guardó las reglas en ese panel para modificar su orden.</p> <p>Nota: El formato de las celdas se establece en función de la primera condición que cumplan y no se aplicará formato adicional aunque cumplan otras condiciones.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Volver atrás** en la esquina superior izquierda de la pantalla para volver al informe.
