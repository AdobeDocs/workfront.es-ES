---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar y mover tareas de plantilla
description: Puede copiar o mover una tarea de plantilla a la misma plantilla o a otra plantilla.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '2127'
ht-degree: 3%

---

# Copiar y mover tareas de plantilla

Puede copiar una tarea de plantilla de una plantilla a otra o moverla a otra plantilla o a otro lugar de la misma plantilla.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a las plantillas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para una plantilla y para la tarea de plantilla </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones para copiar o mover tareas de plantilla

Tenga en cuenta lo siguiente al copiar tareas de plantilla:

* La siguiente información no se transfiere a la tarea copiada:

   * Hitos

* Puede seleccionar copiar algunos elementos asociados con la tarea de plantilla en la tarea copiada durante el proceso de copia. Sin embargo, de forma predeterminada, los siguientes objetos no se transfieren a la tarea copiada:

   * Comentarios del usuario

* Los formularios personalizados se copian con la tarea de plantilla al copiar una tarea de plantilla. La información de los campos personalizados se transfiere a la nueva tarea de plantilla solo cuando selecciona copiar Datos personalizados.

* Los siguientes elementos se transfieren a la tarea de plantilla copiada de forma predeterminada:

   * Subtareas

Tenga en cuenta lo siguiente al mover tareas de plantilla:

* La siguiente información se transfiere a la tarea desplazada de forma predeterminada:

   * Formularios personalizados e información de campos personalizados.
   * Subtareas.
   * Comentarios del usuario.

* La siguiente información no se transfiere a la tarea desplazada:

   * Hitos.

## Copiar tareas de plantilla

Puede copiar una sola tarea de plantilla o copiar varias tareas de plantilla de forma masiva.

1. Vaya a la plantilla que contiene la tarea de plantilla o las tareas de plantilla que desea copiar.
1. Clic **Tareas de plantilla** en el panel izquierdo.
1. Realice una de las siguientes acciones:
   * Haga clic en el nombre de una tarea de plantilla para abrirla.
   * Seleccione una o varias tareas de plantilla en la lista.
1. (Condicional) Haga clic en **Más** menú ![](assets/more-icon.png) en la parte superior de la lista de tareas de plantilla o a la derecha del nombre de la tarea de plantilla si ha abierto la tarea, haga clic en **Copiar a** o **Copiar**, según desde dónde acceda a la opción Copiar.
Se abrirá el cuadro Copiar tarea de plantilla.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Opcional) Cambie el nombre de la tarea de plantilla en la **Nombre de tarea de plantilla** field.

   >[!TIP]
   >
   >Este campo aparece atenuado y no se puede editar al seleccionar copiar varias tareas de plantilla en una lista. Puede pasar el ratón sobre el campo Nombre de tarea de plantilla y se mostrará una lista de todas las tareas de plantilla seleccionadas.

1. Empiece a escribir el nombre del **Plantilla de destino** donde desee copiar la tarea de plantilla en el **Seleccionar plantilla de destino** y, a continuación, selecciónelo cuando se muestre en la lista.

   El nombre de la plantilla actual se muestra de forma predeterminada. Si desea copiar la tarea de plantilla dentro de la misma plantilla, deje este campo sin cambiar.

   >[!TIP]
   >
   >También puede empezar a escribir el número de referencia o introducir el ID de la plantilla. Esto puede ayudarle a distinguir entre plantillas con nombres idénticos.

1. (Condicional) Haga clic en **solicitar acceso** para solicitar acceso a la plantilla de destino, si no tiene acceso a la plantilla seleccionada.
1. (Condicional) Continúe copiando la tarea de plantilla en la plantilla de destino seleccionada sin solicitar acceso si tiene acceso para agregar tareas de plantilla a una de las tareas de plantilla de la plantilla de destino.

1. Clic **Opciones** en el panel izquierdo, anule la selección de los atributos de tarea de plantilla que no desee copiar con la tarea de plantilla. Todas las opciones están seleccionadas de forma predeterminada.

   >[!TIP]
   >
   >Anulando selección **Seleccionar todo** anula la selección de todas las opciones.

   Anule la selección de las siguientes opciones para no transferirlas a la tarea de plantilla copiada. En la tabla siguiente se describe lo que sucede cuando no se seleccionan las opciones:

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
      <td> <p>La restricción de tarea de plantilla se establece en Lo antes posible o Lo más tarde posible según la configuración del modo de programación de la plantilla.</p> <p> Si se selecciona, la restricción actual de la tarea de plantilla se transfiere a la tarea de plantilla copiada. </p> 
      <p><b>NOTA</b>

   Cuando se copia una tarea de plantilla con delimitaciones específicas de fecha en otra plantilla y las fechas de delimitación de la tarea de plantilla están fuera de las fechas de la nueva plantilla, la delimitación de la tarea de plantilla cambia a Lo antes posible o Lo más tarde posible o se ajustan las fechas planificadas de inicio o finalización de las plantillas.

   Los siguientes son ejemplos de restricciones específicas de la fecha:
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
      <td> <p>Todas las asignaciones se quitan de la tarea de plantilla. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Todos los procesos de aprobación se eliminan de la tarea de plantilla.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Todas las predecesoras</td> 
      <td> <p>Esto significa que las dependencias no se transferirán a las tareas de plantilla copiadas. </p> <p>Si se selecciona, se conservan las tareas predecesoras dentro del grupo de tareas de plantilla copiadas y se eliminan otras.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Los valores de los campos personalizados se borran y los formularios personalizados se transfieren a la tarea de plantilla copiada. </p> <p>Cuando se seleccionan, tanto los formularios como los valores de los campos personalizados se transfieren a la tarea de plantilla copiada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>La información financiera de la tarea de plantilla copiada se elimina y Workfront actualiza el tipo de coste de la tarea de plantilla a Sin coste y el tipo de ingresos de la tarea de plantilla a No facturable.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea de plantilla no se transfieren a la tarea de plantilla copiada. Esto incluye versiones, pruebas y documentos vinculados.</p> <p><b>NOTA</b></p>

   <p>Esto no incluye las aprobaciones de documentos. Las aprobaciones de documentos nunca se pueden copiar cuando se copia una tarea de plantilla.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de la tarea de plantilla no se transfieren a la tarea de plantilla copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea de plantilla no se transfieren a la tarea de plantilla copiada. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo, seleccione la tarea de plantilla en la plantilla de destino que desea que sea la principal de la tarea de plantilla copiada.

   >[!TIP]
   >
   >Al seleccionar copiar varias tareas de plantilla en una lista, todas las tareas de plantilla seleccionadas se convierten en los hijos del padre seleccionado y se añaden después de las tareas hijas existentes.

   Seleccione un padre mediante una de las siguientes acciones:

   * En la lista de tareas de plantilla, seleccione uno de los elementos primarios del plan de plantilla.
   * Haga clic en el icono de búsqueda ![Icono de búsqueda](assets/search-icon.png) y busque una tarea de plantilla principal por su nombre.

   La tarea de plantilla debe aparecer en la lista.

1. Seleccione el botón de opción del elemento principal, una vez encontrado.

   Si no selecciona una tarea de plantilla principal, las tareas de plantilla se copian como tareas de plantilla principales en lugar de subtareas y se colocan al final de la lista de tareas de plantilla en la plantilla de destino.

1. Clic **Copiar tarea de plantilla**.

   Las tareas de plantilla copiadas ahora están en la plantilla especificada y son subtareas de la tarea de plantilla principal seleccionada o las últimas tareas de plantilla de la plantilla.


## Mover tareas de plantilla

Puede mover una tarea de plantilla a otra tarea de plantilla de la misma plantilla o a otra plantilla. Puede mover una o varias tareas de plantilla de forma masiva.

1. Vaya a la plantilla que contiene la tarea de plantilla o las tareas de plantilla que desea mover.
1. Clic **Tareas de plantilla** en el panel izquierdo.
1. Realice una de las siguientes acciones:
   * Haga clic en el nombre de una tarea de plantilla para abrirla.
   * Seleccione una o varias tareas de plantilla en la lista.
1. (Condicional) Haga clic en **Más** menú ![](assets/more-icon.png) en la parte superior de la lista de tareas de plantilla o a la derecha del nombre de la tarea de plantilla si ha abierto la tarea, haga clic en **Mover a** o **Mover**, según desde dónde acceda a la opción Mover.
Se abrirá el cuadro Mover tarea de plantilla.
   ![](assets/move-template-task-box-unshimmed.png)

1. (Opcional) Cambie el nombre de la tarea de plantilla en la **Nombre de tarea de plantilla** field.

   >[!TIP]
   >
   >Este campo aparece atenuado y no se puede editar al seleccionar mover varias tareas de plantilla en una lista. Puede pasar el ratón sobre el campo Nombre de la tarea de plantilla y se mostrará una lista de todas las tareas de plantilla seleccionadas.

1. Empiece a escribir el nombre del **Plantilla de destino** donde desee mover la tarea de plantilla en el **Seleccionar plantilla de destino** y, a continuación, selecciónelo cuando se muestre en la lista.

   >[!TIP]
   >
   >También puede empezar a escribir el número de referencia o introducir el ID de la plantilla. Esto puede ayudarle a distinguir entre plantillas con nombres idénticos.

1. (Condicional) Haga clic en **solicitar acceso** para solicitar acceso a la plantilla, si no tiene acceso a la plantilla de destino.
1. (Condicional) Continúe moviendo la tarea de plantilla a la plantilla de destino seleccionada sin solicitar acceso si tiene acceso para agregar tareas de plantilla a una de las tareas de plantilla de la plantilla de destino.

1. Clic **Opciones** en el panel izquierdo, anule la selección de los atributos de tarea de plantilla que no desee copiar con la tarea de plantilla. Todas las opciones están seleccionadas de forma predeterminada.

   >[!TIP]
   >
   >* La sección Opciones solo está disponible después de seleccionar una plantilla de destino.
   >* Anulando selección **Seleccionar todo** anula la selección de todas las opciones.

   Anule la selección de las siguientes opciones para no transferir la información a la tarea de plantilla desplazada. En la tabla siguiente se describe lo que sucede cuando no se seleccionan las opciones:

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
      <td> <p>La restricción de tarea de plantilla se establece en Lo antes posible o Lo más tarde posible según la configuración del modo de programación de la plantilla.</p> <p> Cuando se selecciona, la restricción actual de la tarea de plantilla se transfiere a la tarea de plantilla desplazada. </p>

   <p><b>NOTA</b>

   Cuando se mueve una tarea de plantilla con delimitaciones específicas de fecha a otra plantilla y las fechas de delimitación de la tarea de plantilla están fuera de las fechas de la nueva plantilla, o bien la delimitación de la tarea de plantilla cambia a Lo antes posible o Lo más tarde posible, o bien se ajustan las fechas de inicio planificadas o de finalización planificada de las plantillas.

   Los siguientes son ejemplos de restricciones específicas de la fecha:
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
      <td> <p>Todas las asignaciones se quitan de la tarea de plantilla. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Todos los procesos de aprobación se eliminan de la tarea de plantilla.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Todas las predecesoras</td> 
      <td> <p>Esto significa que las dependencias no se arrastrarán con las tareas de plantilla que se hayan movido. </p> <p>Si se selecciona, se conservan las tareas predecesoras dentro del grupo de tareas de plantilla que se han movido y se eliminan otras.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Los valores de los campos personalizados se borran y los formularios personalizados se transfieren con la tarea de plantilla desplazada. </p> <p>Cuando se seleccionan, tanto los formularios como los valores de los campos personalizados se transfieren con la tarea de plantilla desplazada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>La información financiera de la tarea de plantilla desplazada se elimina y Workfront actualiza el tipo de coste de la tarea de plantilla a Sin coste y el tipo de ingresos de la tarea de plantilla a No facturable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea de plantilla no se transfieren con la tarea de plantilla desplazada. Esto incluye versiones, pruebas y documentos vinculados.</p>

   <p><b>NOTA</b></p>

   <ul><li>
      <p>Esto no incluye las aprobaciones de documentos. Las aprobaciones de documentos nunca se pueden mover cuando se mueve una tarea de plantilla.</p> </li>
      <li>Si opta por no mover los documentos con la tarea de plantilla, los documentos se eliminan y se colocan en la papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y se restaurarán en la tarea de plantilla desplazada.

   Si la tarea de plantilla se elimina después de moverla, los documentos restaurados se colocarán en el área Documentos de la página del usuario del administrador que los restaura. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de la tarea de plantilla no se transfieren a la tarea de plantilla desplazada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea de plantilla no se transfieren con la tarea de plantilla desplazada. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo, seleccione la tarea de plantilla en la plantilla de destino que desea que sea la principal de la tarea de plantilla desplazada.

   >[!TIP]
   >
   >Al seleccionar mover varias tareas de plantilla en una lista, todas las tareas de plantilla seleccionadas se convierten en los hijos del padre seleccionado y se añaden después de las tareas hijas existentes.

   Seleccione un padre mediante una de las siguientes acciones:

   * En la lista de tareas de plantilla, seleccione uno de los elementos primarios del plan de plantilla.
   * Haga clic en el icono de búsqueda ![Icono de búsqueda](assets/search-icon.png) y busque una tarea de plantilla principal por su nombre.

   La tarea de plantilla debe aparecer en la lista.

1. Seleccione el botón de opción del elemento principal, una vez encontrado.

   Si no selecciona una tarea de plantilla principal, las tareas de plantilla se mueven como tareas de plantilla principales en lugar de subtareas y se colocan al final de la lista de tareas de plantilla en la plantilla de destino.

1. Clic **Mover tarea de plantilla**.

   Las tareas de plantilla movidas ahora se encuentran en la plantilla especificada y son subtareas de la tarea de plantilla principal seleccionada o las últimas tareas de plantilla de la plantilla.
