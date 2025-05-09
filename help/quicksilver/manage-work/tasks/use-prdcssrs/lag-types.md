---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Información general sobre los tipos de retardo
description: El retardo es la cantidad de tiempo que debe transcurrir tras la finalización de una predecesora forzada hasta que la tarea dependiente pueda iniciarse (Retardo positivo) o la cantidad de tiempo que una tarea dependiente podría iniciarse antes de que lo haga la predecesora (Retardo negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 100%

---

# Información general sobre los tipos de retardo

<!-- Audited: 01/2024 -->

El retardo es la cantidad de tiempo que debe transcurrir tras la finalización planificada de una predecesora hasta que la tarea dependiente pueda iniciarse (Retardo positivo) o la cantidad de tiempo que una tarea dependiente podría iniciarse antes de que lo haga la predecesora (Retardo negativo).

Las fechas planificadas, proyectadas y estimadas de las tareas sucesoras se calculan teniendo en cuenta las fechas de retardo y planificadas, proyectadas y estimadas de inicio (finalización) de las tareas predecesoras.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de retardo {#lag-types}

Un ejemplo de una tarea que requeriría un tiempo de retardo podría ser el aserrado de árboles para convertirlos en madera. Si la madera recién talada debe secarse durante un tiempo antes de poder cortarse, habría un tiempo de retardo entre la tala de los árboles y el aserrado para convertirlos en madera.

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
   <td> <p>El retraso entre dos tareas vinculadas por dependencia se mide en días laborables. Este es el tipo de retardo predeterminado. </p> <p>Por ejemplo, si hay una dependencia finalización-inicio con un retardo de 2 días laborables y la tarea predecesora finaliza el viernes, la tarea dependiente se iniciará el miércoles. Los días de fin de semana no cuentan como parte del retardo. </p> <p>Nota: El límite máximo de retardo para los días es de 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Días naturales (c o ce)</p> </td> 
   <td> <p>El retraso entre dos tareas se mide en días naturales, incluidos festivos y fines de semana. </p> <p>Nota: Aunque este tipo de retardo cuenta los días no laborables como parte del retardo, una tarea dependiente nunca puede iniciarse en un día no laborable. Si este tipo de retardo hace que la tarea dependiente se inicie en un día no laborable, la fecha planificada de inicio de la tarea dependiente se programará para el siguiente día laborable. </p> <p>Por ejemplo, si hay una dependencia finalización-inicio con un retardo de 2 días naturales y la tarea predecesora finaliza el jueves, la tarea dependiente se iniciará el lunes en lugar del domingo. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Porcentaje (p o pe)</p> </td> 
   <td> <p>El retraso se expresa como un porcentaje del tiempo estimado para completar la tarea predecesora. </p> <p>Por ejemplo, si hay una dependencia finalización-inicio con un retardo del 20 % en una tarea predecesora de 10 días, el sistema calculará cuántos días representan el 20 % de la duración de la tarea predecesora y los usará como retardo. En este caso, serían 2 días tras la finalización de la tarea. </p>

<p><b>NOTA</b></p> El límite de retardo máximo para el porcentaje es de 2000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Día de la semana (w o we) </p> </td> 
   <td> <p>El retraso entre dos tareas se mide indicando los días de la semana correspondientes a la semana que contiene la fecha planificada de finalización de la predecesora.</p> <p>Para este tipo de retardo, cada día de la semana está asociado a un número:</p> 
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

Si se calcula que la fecha de inicio de la tarea sucesora es un martes determinado y que ese día ha transcurrido durante la semana actual, la fecha de inicio planificada de la tarea sucesora es el mismo día (martes) de la semana siguiente, si está disponible. </p> <p>Si desea indicar que el retraso debe caer en un sábado de la semana actual, y el sábado es después de la fecha planificada de finalización de la tarea predecesora, debe codificar la tarea sucesora con la siguiente fórmula:</p> <p><code>4fs+7w</code> </p> <p>Si sábado es un día no laborable, se selecciona el siguiente día disponible después del sábado (para indicar un retraso positivo) como la fecha planificada de inicio de la tarea sucesora. </p>

<p>Esto no se aplica a las excepciones de programación. En caso de que una fecha también sea una excepción de programación y la fecha de inicio de la tarea sucesora se calcule en ese día, el sistema intenta encontrar la fecha disponible más cercana, que es el día de la semana especificado en la expresión predecesora.</p>

<p>Por ejemplo, si se calcula que la fecha de inicio es un martes determinado y ese día es una excepción de programación y el retraso de la tarea predecesora es positivo, elegirá el martes siguiente (si también es un día laborable) como fecha de inicio de la tarea sucesora. Si el retraso es negativo, el sistema elige el martes anterior como fecha de inicio.</p>

<p>Para indicar semanas pasadas o futuras, puede añadir un número delante del número de día para el tipo de retraso. </p> <p>Por ejemplo, para indicar el lunes de hace 10 semanas, puede utilizar este código para indicar la tarea predecesora de la tarea sucesora:</p> <p><code>4fs-102w</code> </p> <p>10 indica que fue hace 10 semanas y 2 es el número asignado al lunes. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Día de la semana distinto de cero (k o ke)</p> </td> 
   <td> <p>El retraso entre dos tareas se mide de forma idéntica al tipo de retraso Día de la semana, excepto si la hora de la tarea predecesora termina el mismo día de la semana especificada. El tiempo de retraso se calcula entonces en la semana adyacente (+/-). </p> <p>En este caso, el tiempo de retraso nunca puede ser 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Retraso negativo

Puede utilizar un retraso negativo para indicar la necesidad o la capacidad de que la tarea comience antes de que finalice la tarea predecesora.

Tenga en cuenta las siguientes reglas cuando utilice retrasos negativos:

* Un retraso negativo no puede forzar que las fechas de inicio o fin de una tarea sean anteriores o posteriores a las fechas de inicio o finalización planeadas del proyecto. Estas fechas se especifican en el campo Programar desde del proyecto.

  En este caso, tenga en cuenta lo siguiente:

   * Programe el proyecto desde la fecha de finalización.
   * La última tarea del proyecto debe utilizar la restricción de tarea Debe finalizar el. Se recomienda dar a la tarea una duración lo suficientemente larga para tener en cuenta todas las tareas del proyecto. Las tareas restantes funcionan bien con la restricción Lo antes posible.

* El uso de una relación de tarea predecesora Fin-Inicio con tareas puede producir un mensaje de error.

  En este caso, tenga en cuenta lo siguiente:

   * Establezca una relación predecesora Fin-Fin entre las tareas.
   * La duración de la tarea sucesora debe ser igual o superior al número deseado de días de retraso entre las tareas.

## Indicar tipos de retraso y retraso en las tareas

Puede indicar tipos de retraso en las tareas cuando defina sus relaciones de tareas predecesoras.

### Indicar tipos de retraso en la sección Tareas predecesoras de una tarea {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Vaya a una tarea para la que desee definir la tarea predecesora y el Tipo de retraso.
1. Haga clic en **Predecesoras** en el panel izquierdo.
1. Haga clic en **Añadir tarea predecesora**.
1. (Opcional) Si desea añadir una tarea predecesora entre proyectos, reemplace el nombre de **Proyecto principal** por otro proyecto.
1. Comience a escribir el nombre de la tarea predecesora y, a continuación, selecciónela cuando aparezca en la lista.
1. Seleccione el **Tipo de dependencia**.

   Para obtener más información acerca de los tipos de dependencias predecesoras, consulte [Información general sobre los tipos de dependencias entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique una cantidad de **Retraso** con un valor numérico. Puede especificar números negativos para indicar un retraso negativo.
1. Seleccione entre las siguientes opciones para identificar el tipo de retraso que desea indicar para su tarea predecesora:

   * **Días**
   * **Días del calendario**
   * **Porcentaje**
   * **Día de la semana**
   * **Día de la semana (diferente de cero)**

     Para obtener más información acerca de estos tipos de retardo y cómo se calculan, consulte la sección [Tipos de retardo](#lag-types) de este artículo.

1. Haga clic en **Guardar**.

### Indicar tipos de retardo en una lista de tareas  {#indicate-lag-types-in-a-task-list}

1. Vaya a una lista de tareas y seleccione la vista **Estándar**.

1. Haga clic dentro de la columna **Predecesoras** correspondiente a la tarea para la que quiera especificar un predecesor y una cantidad de retardo.
1. Introduzca lo siguiente sin espacios:

   * el número de la tarea que quiera indicar como predecesora de la tarea seleccionada
   * la abreviatura del tipo de dependencia que quiera indicar entre las tareas

     Para obtener más información acerca de las abreviaciones para tipos de dependencia, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * un signo **+** para un retardo positivo o un signo **-** para un retardo negativo

   * la cantidad de retardo
   * la abreviatura del tipo de retardo que quiera utilizar

     Para obtener más información acerca de las abreviaturas de tipos de retardo, consulte la sección [Tipos de retardo](#lag-types) de este artículo.

   Por ejemplo, para indicar que una tarea tiene una predecesora y un retardo positivo de 2 días, se debería escribir `1fs+2d` en la columna Predecesoras.

1. Pulse Entrar en el teclado para guardar los cambios de la tarea.
