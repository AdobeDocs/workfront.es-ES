---
product-previous: workfront-goals
navigation-topic: goal-management
title: Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront
description: El progreso de los objetivos está impulsado por indicadores de progreso como actividades, resultados o metas para niños. La condición de objetivo está determinada por el progreso del objetivo en el momento actual.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>Su organización debe tener lo siguiente para utilizar la funcionalidad descrita en este artículo:
>
>* Un Pro o superior [plan de Adobe Workfront](https://www.workfront.com/plans).
>* Licencia de Adobe Workfront para objetivos además de una licencia de Workfront.
>
>Póngase en contacto con el administrador de cuentas de Workfront para obtener más información sobre una licencia de Workfront para objetivos.
>Para obtener información adicional sobre el acceso a los objetivos de Workfront, consulte [Requisitos para utilizar los objetivos de Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront calcula el progreso del objetivo automáticamente en función del progreso de sus indicadores de progreso.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área Objetivos del menú principal.

## Resumen del progreso y el umbral del objetivo

Después de activar un objetivo, los objetivos de Workfront empiezan a calcular su progreso y condición y muestran los siguientes indicadores al pasar el ratón por encima del campo Progreso :

| Indicador | Descripción del indicador |
|---|---|
| Porcentaje real completado | ¿Cuánto de la meta se ha completado realmente hasta ahora? Workfront Goal calcula este valor promediando el porcentaje completado de todos los indicadores de progreso asociados con el objetivo. |
| Porcentaje completado esperado | ¿Cuánto de la meta debe cumplirse hasta ahora para que la meta se complete a tiempo? Los objetivos de Workfront calculan este valor mirando la Duración del objetivo y el momento actual en el tiempo. El objetivo debería mostrar este valor en el momento actual, si fuera a completarse a tiempo. |
| Progreso | Etiqueta que indica si el objetivo está en la meta de completarse a tiempo, si está en riesgo o si tiene problemas para no completarse. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Porcentaje real completado](#actual-percent-complete)
* [Porcentaje completado esperado](#expected-percent-complete)
* [Progreso y condición](#progress)

### Porcentaje real completado {#actual-percent-complete}

Los objetivos de Workfront calculan automáticamente el porcentaje completado real de un objetivo en función del promedio de porcentaje completado de los indicadores de progreso del objetivo.

Los siguientes temas se consideran indicadores de progreso para los objetivos:

* Resultados

   Para obtener información sobre cómo agregar resultados a objetivos, consulte [Agregar resultados a objetivos en Objetivos de Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Actividades

   Para obtener información sobre cómo agregar actividades, incluidos proyectos, a los objetivos, consulte [Agregar actividades a objetivos en Objetivos de Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Objetivos de los niños alineados

   Para obtener información sobre los objetivos principales y secundarios, consulte [Alinear objetivos conectándolos en los objetivos de Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

   Los objetivos de Workfront calculan el porcentaje real completado mediante la fórmula siguiente:

   ```
   Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
   ```

   Por ejemplo, si un objetivo tiene un resultado completado del 20 %, una barra de progreso manual completa del 30 %, un proyecto completado al 10 % y un objetivo secundario completado al 40 %, el porcentaje de objetivo completado es del 25 %.

### Porcentaje completado esperado {#expected-percent-complete}

Los objetivos de Workfront calculan automáticamente el porcentaje de finalización esperado de un objetivo en función del número total de días durante la duración del objetivo, así como el número de días que han transcurrido desde la fecha de inicio del objetivo.

Los objetivos de Workfront calculan el porcentaje de finalización esperado mediante la fórmula siguiente:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Por ejemplo, si un objetivo se debe completar en 90 días y hoy es el día 45 de esa duración, entonces el porcentaje esperado completado es del 50%.

### Progreso y condición {#progress}

Los objetivos de Workfront calculan un porcentaje de progreso y asignan una etiqueta de progreso a los objetivos, en función del porcentaje del porcentaje completado esperado que se haya alcanzado en el momento actual. El color de la barra de finalización del porcentaje de objetivo cambia para indicar el progreso del objetivo.

La condición del objetivo también se actualiza, en consecuencia, para indicar si el objetivo está en el objetivo de completarse a tiempo o si está rezagado.

Los objetivos de Workfront calculan el porcentaje de progreso de un objetivo mediante la fórmula siguiente:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Por ejemplo, si el porcentaje completado esperado es 53 % en el momento actual y el porcentaje completado real es 30 %, el porcentaje completado del progreso del objetivo es 56 %. Los objetivos de Workfront etiquetan este objetivo con la condición &quot;En problemas&quot;.

El siguiente gráfico ilustra la relación entre las etiquetas de condición y el porcentaje de progreso:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

En la tabla siguiente se enumeran las etiquetas de condición de objetivo y los porcentajes de progreso de objetivo asociados a cada etiqueta.

>[!TIP]
>
>Las etiquetas de condición de objetivo coinciden con el nombre y el color del proyecto de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Nombre del progreso del objetivo</b></td> 
   <td><b>Definición del progreso del objetivo</b></td> 
   <td><b>Porcentaje de progreso de los objetivos</b></td> 
   <td><b>Color de la barra de porcentaje completado</b></td> 
   <td><b>Icono del indicador de condición</b></td> 
  </tr> 
  <tr> 
   <td>Nuevo</td> 
   <td> <p>El objetivo se ha creado recientemente y aún no se está registrando el progreso. Un progreso de objetivo se muestra como Nuevo hasta que alguien actualice su progreso por primera vez. </p> <p>Para obtener información sobre cómo actualizar el progreso del objetivo, consulte <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Actualización del progreso del objetivo en los objetivos de Adobe Workfront</a>.</p> </td> 
   <td>Sin porcentaje</td> 
   <td>Sin barra</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_Goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Bien encaminado</span> </p> </td> 
   <td>El objetivo está teniendo el rendimiento esperado y existe una buena probabilidad de que se complete a tiempo. </td> 
   <td>90-100%</td> 
   <td>Verde</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>En riesgo</span> </p> </td> 
   <td>El objetivo está retrasado, pero podría ser posible completarlo a tiempo. </td> 
   <td>70-89.99%</td> 
   <td>Amarillo</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_Risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>Con problemas</span> </p> </td> 
   <td> <p>Es muy probable que el objetivo no se complete a tiempo. </p> </td> 
   <td>0-69.99%</td> 
   <td>Rojo</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_Problem_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>