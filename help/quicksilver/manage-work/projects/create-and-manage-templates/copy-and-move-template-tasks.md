---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar y mover tareas de plantilla
description: Puede copiar o mover una tarea de plantilla a la misma plantilla o a otra plantilla.
author: Alina
feature: Work Management
source-git-commit: 4a33d72e234ff812a72d7d7a382226697f858df6
workflow-type: tm+mt
source-wordcount: '2101'
ht-degree: 3%

---


# Copiar y mover tareas de plantilla

<span class="preview">La copia y el desplazamiento de una tarea de plantilla están disponibles en el entorno Producción. Sin embargo, los pasos descritos en esta página hacen referencia a funcionalidades solo en el entorno de Vista previa. Esta funcionalidad estará disponible en Producción el 2 de marzo de 2023.</span>

Puede copiar una tarea de plantilla de una plantilla a otra plantilla o moverla a otra plantilla o a otro lugar de la misma plantilla.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a plantillas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para una plantilla y para la tarea de plantilla </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para copiar o mover tareas de plantilla

Tenga en cuenta lo siguiente al copiar una tarea de plantilla:

* Los hitos no se transfieren a la tarea de plantilla copiada o movida.

* Puede copiar una tarea de plantilla en las siguientes áreas de la aplicación web de Adobe Workfront:

   * En el nivel de tarea de plantilla, desde el **Más icono** ![](assets/more-icon.png) a la derecha del nombre de la tarea de plantilla.

   * En una lista de tareas de plantilla.
* Puede copiar o mover tareas de plantilla de una en una, o seleccionando varias tareas de plantilla.

## Copiar tareas de plantilla

1. Vaya a la plantilla que contiene la tarea de plantilla o las tareas de plantilla que desea copiar.
1. Haga clic en **Tareas de plantilla** en el panel izquierdo.
1. Realice una de las siguientes acciones:
   * Haga clic en el nombre de una tarea de plantilla para abrirla.
   * Seleccione una o varias tareas de plantilla en la lista.
1. (Condicional) Haga clic en el **Más** menú ![](assets/more-icon.png) en la parte superior de la lista de tareas de plantilla o a la derecha del nombre de la tarea de plantilla si ha abierto la tarea, haga clic en **Copiar en** o **Copiar**, según desde dónde acceda a la opción Copiar.
Se abre el cuadro Copiar tarea de plantilla.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Opcional) Cambie el nombre de la tarea de plantilla en la **Nombre de tarea de plantilla** campo .

   >[!TIP]
   >
   >Este campo está atenuado y no se puede editar al seleccionar para copiar varias tareas de plantilla en una lista. Puede situarse sobre el campo Nombre de tarea de plantilla y mostrar una lista de todas las tareas de plantilla seleccionadas.

1. Comience a escribir el nombre de la variable **Plantilla de destino** donde desea copiar la tarea de plantilla en el **Seleccionar plantilla de destino** y selecciónelo cuando aparezca en la lista.

   El nombre de la plantilla actual se muestra de forma predeterminada. Si desea copiar la tarea de plantilla dentro de la misma plantilla, deje este campo sin modificar.

   >[!TIP]
   >
   >También puede empezar a escribir el número de referencia o introducir el ID de la plantilla. Esto puede ayudarle a distinguir entre plantillas con nombres idénticos.

1. (Condicional) Haga clic en **acceso de solicitud** para solicitar acceso a la plantilla de destino, si no tiene acceso a la plantilla seleccionada.
1. (Condicional) Continúe copiando la tarea de plantilla en la plantilla de destino seleccionada sin solicitar acceso si tiene acceso para añadir tareas de plantilla a una de las tareas de plantilla de la plantilla de destino.

1. Haga clic en **Opciones** en el panel izquierdo, anule la selección de los atributos de tarea de plantilla que no desea copiar con la tarea de plantilla. Todas las opciones están seleccionadas de forma predeterminada.

   >[!TIP]
   >
   >Anulación de selección **Seleccionar todo** anula la selección de todas las opciones.

   Anule la selección de las siguientes opciones para no transferirlas a la tarea de plantilla copiada. La tabla siguiente describe lo que sucede cuando se anula la selección de las opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td>Anule la selección de esta opción para eliminar toda la información de la tarea de plantilla al copiarla en su nueva ubicación. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Restricción</td> 
      <td> <p>La restricción de tarea de plantilla se establece en Tan pronto como sea posible o Lo más tarde posible, en función de la configuración del Modo de programación de la plantilla.</p> <p> Cuando se selecciona, la restricción actual de la tarea de plantilla se transfiere a la tarea de plantilla copiada. </p> 
      <p><b>NOTA</b>

   Al copiar una tarea de plantilla con restricciones específicas de fechas en otra plantilla y las fechas de restricción de la tarea de plantilla están fuera de las fechas de la nueva plantilla, la tarea de plantilla Restricción cambia a Tan pronto como sea posible o Tan tarde como sea posible o se ajustan las fechas de Inicio planificado o Finalización planificada de las plantillas.

   Los siguientes son ejemplos de restricciones de fechas específicas:
   <ul>
      <li> Debe iniciarse el</li>
      <li> Debe finalizarse el</li>
      <li> No iniciar antes del</li>
      <li> No iniciar después del</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td> <p>Todas las asignaciones se eliminan de la tarea de plantilla. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Todos los procesos de aprobación se eliminan de la tarea de plantilla.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Todos los predecesores</td> 
      <td> <p>Esto significa que las dependencias no se trasladarán a las tareas de plantilla copiadas. </p> <p>Cuando se selecciona, se conservan los predecesores dentro del grupo de tareas de plantilla copiadas, mientras que otros se eliminan.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Los valores de los campos personalizados se borran y los formularios personalizados se transfieren a la tarea de plantilla copiada. </p> <p>Cuando se selecciona, tanto los formularios como los valores de los campos personalizados se transfieren a la tarea de plantilla copiada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>La información financiera de la tarea de plantilla copiada se elimina y Workfront actualiza la tarea de plantilla Tipo de coste a Sin coste y la tarea de plantilla Tipo de ingresos como No facturable.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea de plantilla no se transfieren a la tarea de plantilla copiada. Esto incluye versiones, pruebas y documentos vinculados.</p> <p><b>NOTA</b></p>

   <p>Esto no incluye aprobaciones de documentos. Las aprobaciones de documento nunca se pueden copiar cuando se copia una tarea de plantilla.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de tarea de plantilla no se transfieren a la tarea de plantilla copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea de plantilla no se transfieren a la tarea de plantilla copiada. </td> 
     </tr>  
    </tbody> 
   </table>

(PREGUNTANDO SOBRE LA ÚLTIMA FILA: LA TAREA DE PLANTILLA NO PARECE TENER &quot;COMPARTIR&quot;)

1. (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo, seleccione la tarea de plantilla en la plantilla de destino que desea que sea la principal de la tarea de plantilla copiada.

   >[!TIP]
   >
   >Al seleccionar para copiar varias tareas de plantilla en una lista, todas las tareas de plantilla seleccionadas se convierten en las secundarias del elemento principal seleccionado y se añaden después de las tareas secundarias existentes.

   Seleccione un elemento principal realizando una de las siguientes acciones:

   * En la lista de tareas de plantilla, seleccione uno de los elementos principales del plan de plantillas.
   * Haga clic en el icono de búsqueda ![Icono de búsqueda](assets/search-icon.png) y busque una tarea de plantilla principal por su nombre.

   La tarea de plantilla debe aparecer en la lista.

1. Seleccione el botón de opción para el elemento principal, una vez lo haya encontrado.

   Si no selecciona una tarea de plantilla principal, las tareas de plantilla se copian como tareas de plantilla principal en lugar de como subtareas y se colocan al final de la lista de tareas de plantilla en la plantilla de destino.

1. Haga clic en **Copiar tarea de plantilla**.

   Las tareas de plantilla copiadas ahora están en la plantilla especificada y son subtareas de la tarea de plantilla principal seleccionada o las últimas tareas de plantilla de la plantilla.


## Mover tareas de plantilla

Además de copiar tareas de plantilla, también puede mover una tarea de plantilla a otra tarea de plantilla en la misma plantilla o a otra plantilla.


1. Vaya a la plantilla que contiene la tarea de plantilla o las tareas de plantilla que desea mover.
1. Haga clic en **Tareas de plantilla** en el panel izquierdo.
1. Realice una de las siguientes acciones:
   * Haga clic en el nombre de una tarea de plantilla para abrirla.
   * Seleccione una o varias tareas de plantilla en la lista.
1. (Condicional) Haga clic en el **Más** menú ![](assets/more-icon.png) en la parte superior de la lista de tareas de plantilla o a la derecha del nombre de la tarea de plantilla si ha abierto la tarea, haga clic en **Mover a** o **Mover**, según desde dónde acceda a la opción Mover.
Se abre el cuadro Mover tarea de plantilla .
   ![](assets/move-template-task-box-unshimmed.png)

1. (Opcional) Cambie el nombre de la tarea de plantilla en la **Nombre de tarea de plantilla** campo .

   >[!TIP]
   >
   >Este campo está atenuado y no se puede editar al seleccionar mover varias tareas de plantilla en una lista. Puede situarse sobre el campo Nombre de la tarea de plantilla y se muestra una lista de todas las tareas de plantilla seleccionadas.

1. Comience a escribir el nombre de la variable **Plantilla de destino** donde desea mover la tarea de plantilla en la **Seleccionar plantilla de destino** y selecciónelo cuando aparezca en la lista.

   >[!TIP]
   >
   >También puede empezar a escribir el número de referencia o introducir el ID de la plantilla. Esto puede ayudarle a distinguir entre plantillas con nombres idénticos.

1. (Condicional) Haga clic en **acceso de solicitud** para solicitar acceso a la plantilla, si no tiene acceso a la plantilla de destino.
1. (Condicional) Continúe moviendo la tarea de plantilla a la plantilla de destino seleccionada sin solicitar acceso si tiene acceso para añadir tareas de plantilla a una de las tareas de plantilla de la plantilla de destino.

1. Haga clic en **Opciones** en el panel izquierdo, anule la selección de los atributos de tarea de plantilla que no desea copiar con la tarea de plantilla. Todas las opciones están seleccionadas de forma predeterminada.

   >[!TIP]
   >
   >* La sección Opciones solo está disponible después de seleccionar una plantilla de destino.
   >* Anulación de selección **Seleccionar todo** anula la selección de todas las opciones.


   Anule la selección de las siguientes opciones para no transferir la información a la tarea de plantilla movida. La tabla siguiente describe lo que sucede cuando se anula la selección de las opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td>Anule la selección de esta opción para eliminar toda la información de la tarea de plantilla al moverla a su nueva ubicación. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Restricción</td> 
      <td> <p>La restricción de tarea de plantilla se establece en Tan pronto como sea posible o Lo más tarde posible, en función de la configuración del Modo de programación de la plantilla.</p> <p> Cuando se selecciona, la restricción actual de la tarea de plantilla se transfiere a la tarea de plantilla movida. </p>

   <p><b>NOTA</b>

   Al mover una tarea de plantilla con restricciones específicas de fechas a otra plantilla y las fechas de restricción de la tarea de plantilla están fuera de las fechas de la nueva plantilla, la tarea de plantilla Restricción cambia a Tan pronto como sea posible o Tan tarde como sea posible o se ajustan las fechas de Inicio planificado o Finalización planificada de las plantillas.

   Los siguientes son ejemplos de restricciones de fechas específicas:
   <ul>
      <li> Comenzar el</li>
      <li> Debe finalizarse el</li>
      <li> No iniciar antes del</li>
      <li> No iniciar después del</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td> <p>Todas las asignaciones se eliminan de la tarea de plantilla. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Todos los procesos de aprobación se eliminan de la tarea de plantilla.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Todos los predecesores</td> 
      <td> <p>Esto significa que las dependencias no continuarán con las tareas de plantilla movidas. </p> <p>Cuando se selecciona, se conservan los predecesores dentro del grupo de tareas de plantilla movidas, mientras que otros se eliminan.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Los valores de los campos personalizados se borran y los formularios personalizados se transfieren con la tarea de plantilla movida. </p> <p>Cuando se selecciona, tanto los formularios como los valores de los campos personalizados se transfieren con la tarea de plantilla movida. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>La información financiera de la tarea de plantilla movida se elimina y Workfront actualiza la tarea de plantilla Tipo de coste a Sin coste y la tarea de plantilla Tipo de ingresos como No facturable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea de plantilla no se transfieren con la tarea de plantilla movida. Esto incluye versiones, pruebas y documentos vinculados.</p>

   <p><b>NOTA</b></p>

   <ul><li>
      <p>Esto no incluye aprobaciones de documentos. Las aprobaciones de documento nunca se pueden mover cuando se mueve una tarea de plantilla.</p> </li>
      <li>Si opta por no mover los documentos con la tarea de plantilla, los documentos se eliminan y se colocan en la Papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y restaurarlos en la tarea de plantilla movida.

   Si la tarea de plantilla se elimina después de que se mueva, los documentos restaurados se colocarán en el área Documentos de la página de usuario del administrador que los restaura. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de tarea de plantilla no se transfieren a la tarea de plantilla movida. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea de plantilla no se transfieren con la tarea de plantilla movida. </td> 
     </tr>  
    </tbody> 
   </table>

(PREGUNTANDO SOBRE LA ÚLTIMA FILA: LA TAREA DE PLANTILLA NO PARECE TENER &quot;COMPARTIR&quot;)

1. (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo, seleccione la tarea de plantilla en la plantilla de destino que desea que sea la principal de la tarea de plantilla movida.

   >[!TIP]
   >
   >Al seleccionar mover varias tareas de plantilla en una lista, todas las tareas de plantilla seleccionadas se convierten en las secundarias del elemento principal seleccionado y se añaden después de las tareas secundarias existentes.

   Seleccione un elemento principal realizando una de las siguientes acciones:

   * En la lista de tareas de plantilla, seleccione uno de los elementos principales del plan de plantillas.
   * Haga clic en el icono de búsqueda ![Icono de búsqueda](assets/search-icon.png) y busque una tarea de plantilla principal por su nombre.

   La tarea de plantilla debe aparecer en la lista.

1. Seleccione el botón de opción para el elemento principal, una vez lo haya encontrado.

   Si no selecciona una tarea de plantilla principal, las tareas de plantilla se mueven como tareas de plantilla principal en lugar de como subtareas y se colocan al final de la lista de tareas de plantilla en la plantilla de destino.

1. Haga clic en **Mover tarea de plantilla**.

   Las tareas de plantilla movidas se encuentran ahora en la plantilla especificada y son subtareas de la tarea de plantilla principal seleccionada o las últimas tareas de plantilla de la plantilla.


