---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Resumen de tipos de retardo
description: Retardo es la cantidad de tiempo que debe transcurrir después de la finalización de un predecesor forzado hasta que puede comenzar la tarea dependiente (Retardo positivo) o la cantidad de tiempo que una tarea dependiente puede comenzar antes de que se inicie el predecesor (Retardo negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# Resumen de tipos de retardo

<!-- Audited: 01/2024 -->

Retardo es la cantidad de tiempo que debe transcurrir después de la finalización planificada de un predecesor hasta que puede comenzar la tarea dependiente (Retardo positivo) o la cantidad de tiempo que una tarea dependiente puede iniciarse antes de que se inicie el predecesor (Retardo negativo).

Las fechas planificadas, proyectadas y estimadas de las tareas sucesoras se calculan teniendo en cuenta las fechas de retardo y planificadas, proyectadas y estimadas de inicio (finalización) de las tareas predecesoras.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Indicar tipos de retardo y retardo en las tareas

Puede indicar tipos de retardo en las tareas cuando defina sus relaciones de predecesoras.

### Indicar tipos de retardo en la sección Predecesoras de una tarea {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Vaya a una tarea para la que desee definir el predecesor y el Tipo de retardo.
1. Haga clic en **Predecesoras** en el panel izquierdo. Es posible que tengas que hacer clic en **Mostrar más** y luego en **Predecesoras**.
1. Haga clic en **Agregar predecesora**.
1. (Opcional) Si desea agregar una tarea predecesora entre proyectos, reemplace el nombre de **Proyecto principal** por otro proyecto.
1. Comience a escribir el nombre de la tarea predecesora y, a continuación, selecciónela cuando aparezca en la lista.
1. Seleccione el **tipo de dependencia**.

   Para obtener más información acerca de los tipos de dependencias predecesoras, vea [Información general sobre los tipos de dependencias entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique una cantidad de **Lag** con un valor numérico. Puede especificar números negativos para indicar un retardo negativo.
1. Seleccione entre las siguientes opciones para identificar el tipo de retardo que desea indicar para su predecesor:

   * **Días**
   * **Días del calendario**
   * **Porcentaje**
   * **Día de la semana**
   * **Día de la semana (distinto de cero)**

     Para obtener más información acerca de estos tipos de retardo y cómo se calculan, vea la sección [Tipos de retardo](#lag-types) en este artículo.

1. Haga clic en **Guardar**.

### Indicar tipos de retardo en una lista de tareas  {#indicate-lag-types-in-a-task-list}

1. Vaya a una lista de tareas y seleccione la vista **Estándar**.

1. Haga clic dentro de la columna **Predecesoras** correspondiente a la tarea para la que desea especificar un predecesor y una cantidad de posposición.
1. Introduzca lo siguiente sin espacios:

   * el número de la tarea que desea indicar como predecesora de la tarea seleccionada
   * la abreviatura del tipo de dependencia que desea indicar entre las tareas

     Para obtener más información acerca de las abreviaciones para los tipos de dependencia, vea [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * un **+** para un retardo positivo o un **-** para un retardo negativo

   * el importe del retardo
   * la abreviatura del tipo de retardo que desee utilizar

     Para obtener más información acerca de las abreviaturas para los tipos de retardo, vea la sección [Tipos de retardo](#lag-types) en este artículo.

   Por ejemplo, para indicar que una tarea tiene un predecesor y un retardo positivo de 2 días, debe escribir `1fs+2d` en la columna Predecesores.

1. Pulse Enter en el teclado para guardar los cambios en la tarea.

## Tipos de retardo {#lag-types}

Un ejemplo de una tarea que requeriría un tiempo de retardo podría ser la sierra de árboles en la madera. Si la madera recién cortada debe secarse durante un tiempo antes de poder cortarla, entonces habría un tiempo de retardo entre cortar los árboles y serrarlos en madera.

La siguiente tabla ilustra los tipos de retardo y cómo indicar la cantidad de tiempo para cada uno:

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
   <td> <p>Días (d o de)</p> </td> 
   <td> <p>El retraso entre dos tareas vinculadas por dependencia se mide en días laborables. Este es el tipo de retardo predeterminado. </p> <p>Por ejemplo, si hay una dependencia fin-comienzo con un retraso de 2 días laborables y la tarea predecesora finaliza el viernes, la tarea dependiente comienza el miércoles. Los días de fin de semana no se cuentan como parte del retraso. </p> <p>Nota: El límite máximo de retardo para los días es de 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Días del calendario (c o ce)</p> </td> 
   <td> <p>El retraso entre dos tareas se mide en días naturales, incluidos festivos y fines de semana. </p> <p>Nota: Aunque este tipo de retardo cuenta los días no laborables como parte del retardo, una tarea dependiente nunca puede comenzar en un día no laborable. Si este tipo de retardo hace que la tarea dependiente comience en un día no laborable, la fecha planificada de inicio de la tarea dependiente se programa para el siguiente día laborable. </p> <p>Por ejemplo, si hay una dependencia fin-comienzo con un retraso de dos días de calendario y la tarea predecesora finaliza el jueves, la tarea dependiente comienza el lunes en lugar de un domingo. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Porcentaje (p o pe)</p> </td> 
   <td> <p>El retraso se expresa como un porcentaje del tiempo estimado para completar la tarea predecesora. </p> <p>Por ejemplo, si hay una dependencia de fin a comienzo con un retraso del 20% en una tarea predecesora de 10 días, el sistema calculará cuántos días representan el 20% de la duración de la tarea del predecesor y los usará como posposición. En este caso, serían 2 días después de la finalización de la tarea. </p>

<p><b>NOTA</b></p> El límite de retardo máximo para el porcentaje es de 2000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Día de la semana (w o we) </p> </td> 
   <td> <p>El retraso entre dos tareas se mide indicando los días de la semana de la semana que contiene la fecha planificada de finalización de la tarea predecesora.</p> <p>Para este tipo de retardo, cada día de la semana está asociado con un número:</p> 
    <ul> 
     <li>Domingo=1</li> 
     <li>Lunes=2</li> 
     <li>Martes=3</li> 
     <li>Miércoles=4</li> 
     <li>Jueves=5</li> 
     <li>Viernes=6</li> 
     <li>Sábado=7</li> 
    </ul> <p>Si desea indicar que la fecha planificada de inicio de la tarea sucesora debe ser un martes de la semana actual y que el martes es anterior a la fecha planificada de finalización de la tarea predecesora, debe codificar la tarea sucesora con la fórmula siguiente: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTA</b></p>

Si se calcula que la fecha de inicio de la tarea sucesora es un martes determinado y que ese día ha transcurrido durante la semana actual, la fecha de inicio planificada de la tarea sucesora es el mismo día (martes) de la semana siguiente, si está disponible. </p> <p>Si desea indicar que el retraso debe caer en un sábado de la semana actual, y el sábado es después de la fecha planificada de finalización del predecesor, debe codificar el sucesor con la siguiente fórmula:</p> <p><code>4fs+7w</code> </p> <p>Si sábado es un día no laborable, se selecciona el siguiente día disponible después del sábado (para indicar un retraso positivo) como la fecha planificada de inicio de la tarea sucesora. </p>

<p>Esto no se aplica a las excepciones de programación. En caso de que una fecha también sea una excepción de programación y la fecha de inicio de la tarea sucesora se calcule en ese día, el sistema intenta encontrar la fecha disponible más cercana, que es el día de la semana especificado en la expresión predecesora.</p>

<p>Por ejemplo, si se calcula que la fecha de inicio es un martes determinado y ese día es una excepción de programación y el retardo del predecesor es positivo, elegirá el martes siguiente (si también es un día laborable) como fecha de inicio del sucesor. Si el retardo es negativo, el sistema elige el martes anterior como fecha de inicio.</p>

<p>Para indicar semanas pasadas o futuras, puede agregar un número delante del número de día para el tipo de retardo. </p> <p>Por ejemplo, para indicar el lunes de hace 10 semanas, puede utilizar este código para indicar el predecesor del sucesor:</p> <p><code>4fs-102w</code> </p> <p>10 indica que fue hace 10 semanas y 2 es el número asignado al lunes. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Día de la semana distinto de cero (k o ke)</p> </td> 
   <td> <p>El retraso entre dos tareas se mide de forma idéntica al tipo de retraso Día de la semana, excepto si la hora del predecesor termina el mismo día de la semana especificada. El tiempo de retardo se calcula entonces a la semana adyacente (+/-). </p> <p>En este caso, el tiempo de retardo nunca puede ser 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Retardo negativo

Puede utilizar un retardo negativo para indicar la necesidad o la capacidad de que la tarea comience antes de que finalice la tarea predecesora.

Tenga en cuenta las siguientes reglas cuando utilice retardos negativos:

* Un retardo negativo no puede forzar que las fechas de comienzo o fin de una tarea sean anteriores o posteriores a las fechas de comienzo o fin planeadas del proyecto. Estas fechas se especifican en el campo Programar desde del proyecto.

  En este caso, tenga en cuenta lo siguiente:

   * Programe el proyecto desde la fecha de finalización.
   * La última tarea del proyecto debe utilizar la restricción Debe finalizar con la tarea. Se recomienda dar a la tarea una duración lo suficientemente larga para tener en cuenta todas las tareas del proyecto. Las tareas restantes funcionan bien con la delimitación Lo antes posible.

* El uso de una relación de predecesora Fin-Comienzo con tareas puede producir un mensaje de error.

  En este caso, tenga en cuenta lo siguiente:

   * Establezca una relación predecesora Fin-Fin entre las tareas.
   * La duración de la tarea sucesora debe ser igual o superior al número deseado de días de posposición entre las tareas.
