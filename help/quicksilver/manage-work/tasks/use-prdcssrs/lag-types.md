---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Descripción general de los tipos de retraso
description: El retraso es la cantidad de tiempo que debe transcurrir después de la finalización de un predecesor forzado hasta que puede comenzar la tarea dependiente (retraso positivo) o la cantidad de tiempo que una tarea dependiente podría comenzar antes de que se inicie el predecesor (retraso negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# Descripción general de los tipos de retraso

El retraso es la cantidad de tiempo que debe transcurrir después de la finalización de un predecesor forzado hasta que puede comenzar la tarea dependiente (retraso positivo) o la cantidad de tiempo que una tarea dependiente podría comenzar antes de que se inicie el predecesor (retraso negativo).

Las fechas Planificadas, Proyectadas y Estimadas de las tareas sucesoras se calculan teniendo en cuenta el retraso y las fechas de inicio (finalización) planeadas, previstas y estimadas de las tareas predecesoras.

## Requisitos de acceso

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Indicar tipos de retraso y de retraso en las tareas

Puede indicar tipos de retraso en las tareas cuando defina sus relaciones predecesoras.

* [Indicar tipos de registro en la sección Predecesores de una tarea](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [Indicar tipos de registro en una lista de tareas](#indicate-lag-types-in-a-task-list)

### Indicar tipos de registro en la sección Predecesores de una tarea {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Vaya a la tarea para la que desea definir el predecesor y el Tipo de registro.
1. Haga clic en **Predecesores** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más** y luego **Predecesores**.
1. Haga clic en **Agregar predecesor**.
1. (Opcional) Si desea agregar un predecesor de varios proyectos, reemplace el **Proyecto principal** nombre con otro proyecto.
1. Empiece a escribir el nombre de la tarea predecesora y selecciónela cuando aparezca en la lista.
1. Seleccione el **Tipo de dependencia**.

   Para obtener más información sobre los tipos de dependencias predecesores, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique un **Lag** usando un valor numérico. Puede especificar números negativos para indicar un retraso negativo.
1. Seleccione entre las siguientes opciones para identificar el tipo de retraso que desea indicar para su predecesor:

   * **Días**
   * **Días del calendario**
   * **Porcentaje**
   * **Día de la semana**
   * **Día de la semana (distinto de cero)**

      Para obtener más información sobre estos tipos de registro y cómo se calculan, consulte la sección [Información general sobre los tipos de registro](#lag-types-overview) en este artículo.

1. Haga clic en **Guardar**.

### Indicar tipos de registro en una lista de tareas  {#indicate-lag-types-in-a-task-list}

1. Vaya a la lista de tareas y seleccione la **Estándar** Ver desde el **Ver** menú desplegable.

1. Haga clic dentro del **Predecesores** correspondiente a la tarea para la que desea especificar un predecesor y una cantidad de retraso.
1. Escriba lo siguiente sin espacios:

   * el número de la tarea que desea indicar como predecesora de la tarea seleccionada
   * la abreviatura del tipo de dependencia que desea indicar entre las tareas

      Para obtener más información sobre las abreviaturas de los tipos de dependencia, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * o bien **+** para un desfase positivo o un **-** para un desfase negativo

   * el importe del retraso
   * la abreviatura del tipo de registro que desea utilizar.

      Para obtener más información sobre las abreviaciones de Tipos de registro, consulte la sección [Información general sobre los tipos de registro](#lag-types-overview) en este artículo.
   Por ejemplo, para indicar que una tarea tiene un predecesor y un retraso positivo de 2 días, debe introducir

   ```
   1fs+2d
   ```

   en la columna Predecesores .

1. Haga clic en Enter en el teclado para guardar los cambios en la tarea.

## Información general sobre los tipos de registro {#lag-types-overview}

Un ejemplo de una tarea que requeriría un tiempo de retardo podría ser la tala de árboles en madera. Si la madera recién cortada debe secarse durante un tiempo antes de cortarla, entonces habrá un tiempo de retardo entre cortar los árboles y aserrarlos en madera.

La siguiente tabla ilustra los tipos de retraso y cómo indicar la cantidad de tiempo para cada uno:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Valor</strong> </p> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Días (d)</p> </td> 
   <td> <p>El retraso entre dos tareas vinculadas por la dependencia se mide en días laborables. Este es el tipo de registro predeterminado. </p> <p>Por ejemplo, si hay una dependencia de finalización-inicio con un retraso de 2 días hábiles y la tarea predecesora finaliza el viernes, la tarea dependiente comienza el miércoles. Los días del fin de semana no cuentan como parte del retraso. </p> <p>Nota: El límite máximo de retraso para días es de 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Días naturales (c)</p> </td> 
   <td> <p>El retraso entre dos tareas se mide en días del calendario, incluidos los festivos y los fines de semana. </p> <p>Nota: Aunque este tipo de retraso cuenta los días no laborables como parte del retraso, una tarea dependiente nunca puede comenzar en un día que no sea laborable. Si este tipo de retraso hace que la tarea dependiente comience en un día no laborable, la Fecha de inicio planificada de la tarea dependiente se programa para el siguiente día laborable. </p> <p>Por ejemplo, si hay una dependencia de fin-inicio con un retraso de 2 días del calendario y la tarea predecesora finaliza el jueves, la tarea dependiente comienza el lunes en lugar de un domingo. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Porcentaje (p o pe)</p> </td> 
   <td> <p>El retraso se expresa como un porcentaje del tiempo estimado para completar la tarea predecesora. </p> <p>Por ejemplo, si hay una dependencia de finalización-inicio con un retraso del 20 % entre una tarea predecesora de 10 días, el sistema calculará cuántos días es el 20 % de la duración de la tarea predecesores y la utilizará como retraso. En este caso, tardarían 2 días desde la finalización de la tarea. </p> <p>Nota: El límite máximo de retraso para el porcentaje es del 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Día de la semana (w) </p> </td> 
   <td> <p>El retraso entre dos tareas se mide indicando los días de la semana para la semana que contiene la fecha de finalización planeada del predecesor.</p> <p>Para este tipo de registro, cada día de la semana está asociado a un número:</p> 
    <ul> 
     <li>Domingo=1</li> 
     <li>Lunes=2</li> 
     <li>Martes=3</li> 
     <li>Miércoles=4</li> 
     <li>Jueves=5</li> 
     <li>Viernes=6</li> 
     <li>Sábado=7</li> 
    </ul> <p>Si desea indicar que la Fecha de inicio planeada del sucesor debe corresponder a un martes de la semana actual y que el martes es anterior a la Fecha de finalización planeada del predecesor, debe codificar el sucesor con la siguiente fórmula: </p> <p><code style="font-style: normal;">4fs-3w</code> </p> <p>Nota: Si el martes se pasa para la semana de la fecha de finalización prevista del predecesor, la fecha de inicio prevista de la tarea sucesora es el primer día laborable disponible de esa semana. </p> <p>Si desea indicar que el retraso debe corresponder a un sábado de la semana en curso y que el sábado es posterior a la fecha de finalización prevista del predecesor, codificaría el sucesor con la fórmula siguiente:</p> <p><code style="font-style: normal;">4fs+7w</code> </p> <p>Si sábado es un día no laborable, el siguiente día disponible después del sábado (para indicar un retraso positivo) se selecciona como Fecha de inicio planeada del sucesor. </p> <p>Para indicar semanas pasadas o futuras, puede agregar un número delante del número de día para el tipo de retraso. </p> <p>Por ejemplo, para indicar el lunes de hace 10 semanas, puede utilizar este código para indicar el predecesor de su sucesor:</p> <p><code>4fs-102w</code> </p> <p>10 indica hace 10 semanas y 2 es el número asignado a lunes. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Día de la semana distinto de cero (k)</p> </td> 
   <td> <p>El retraso entre dos tareas se mide de forma idéntica al tipo de retraso Día de la semana , excepto si el tiempo del predecesor termina el mismo día de la semana especificada. A continuación, el tiempo de retraso se calcula en la semana adyacente (+/-). </p> <p>En este caso, el tiempo de retardo nunca puede ser 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información general sobre el retraso negativo

Puede utilizar un retraso negativo para indicar la necesidad o capacidad de que la tarea comience antes de que finalice la tarea predecesora.

Tenga en cuenta las siguientes reglas cuando utilice etiquetas negativas:

* El retraso negativo no puede obligar a que las fechas de inicio/fin de una tarea sean anteriores o posteriores a las fechas de inicio/fin planeadas del proyecto. Estas fechas se especifican en el campo Programar desde del proyecto.

   En este caso, tenga en cuenta lo siguiente:

   * Programar el proyecto desde la fecha de finalización.
   * La última tarea del proyecto debe utilizar la restricción Must Finish on Task Constraint. Se recomienda dar a la tarea una duración suficiente para tener en cuenta todas las tareas del proyecto. Las tareas restantes funcionan bien con la restricción Lo antes posible .

* El uso de una relación predecesora de Finish-Start con tareas puede producir un mensaje de error.

   En este caso, tenga en cuenta lo siguiente:

   * Establezca una relación predecesora Fin-Fin entre tareas.
   * La duración de la tarea sucesora debe ser igual o superior al número previsto de días de retraso entre tareas.
