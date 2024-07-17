---
product-previous: workfront-goals
navigation-topic: goal-management
title: Información general sobre el progreso y la condición de los objetivos en Adobe Workfront Goals
description: El progreso de los objetivos está impulsado por indicadores de progreso como actividades, resultados o metas para niños. La condición de objetivo está determinada por el progreso de la meta en el momento actual.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Información general sobre el progreso y la condición de los objetivos en Adobe Workfront Goals

Su organización debe tener lo siguiente para utilizar la funcionalidad descrita en este artículo:

* Para el nuevo plan y la estructura de licencias:

   * Un plan definitivo

     O

     Licencia adicional para objetivos de Adobe Workfront para los planes Prime o Select Adobe Workfront. Para obtener más información, consulte [plan de Adobe Workfront](https://www.workfront.com/plans).

* Para el plan y la estructura de licencias actuales:

   * A Pro o superior
   * Una licencia de Adobe Workfront Goals además de una licencia de Workfront.

Póngase en contacto con el administrador de cuentas de Workfront para obtener más información sobre una licencia de Workfront Goals.

Para obtener información adicional sobre el acceso a las metas de Workfront, consulte [Requisitos para usar las metas de Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront calcula automáticamente el progreso de la meta en función del progreso de sus indicadores de progreso.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área de Objetivos en el menú principal.

## Información general sobre el progreso y el umbral del objetivo

Después de activar una meta, Workfront Goals empieza a calcular su progreso y condición y muestra los siguientes indicadores al pasar el ratón por encima del campo Progress:

| Indicador | Descripción del indicador |
|---|---|
| Porcentaje real completado | La parte de la meta que se ha completado hasta ahora. Workfront Goals calcula este valor promediando el porcentaje completado de todos los indicadores de progreso asociados con la meta. |
| Porcentaje completado esperado | La cantidad de la meta debe completarse hasta el momento para que la meta se complete a tiempo. Workfront Goals calcula este valor mirando la Duración de la meta y el momento actual en el tiempo. La meta debería mostrar este valor en el momento actual, si se completara a tiempo. |
| Progreso | Una etiqueta que indica si la meta está en el objetivo de completarse a tiempo o si está en riesgo o en problemas de no completarse. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Porcentaje real completado](#actual-percent-complete)
* [Porcentaje completado esperado](#expected-percent-complete)
* [Progreso y condición](#progress)

### Porcentaje real completado {#actual-percent-complete}

Workfront Goals calcula automáticamente el porcentaje completado real de una meta basándose en el porcentaje completado promedio de los indicadores de progreso de la meta.

Los siguientes puntos se consideran indicadores de progreso para los objetivos:

* Resultados

  Para obtener información acerca de cómo agregar resultados a las metas, vea [Agregar resultados a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Actividades

  Para obtener información acerca de cómo agregar actividades, incluidos proyectos, a las metas, vea [Agregar actividades a las metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Metas secundarias alineadas

  Para obtener información acerca de las metas principales y secundarias, vea [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  Workfront Goals calcula el porcentaje real completado con la fórmula siguiente:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Por ejemplo, si un objetivo tiene un resultado al 20 % completado, una barra de progreso manual al 30 % completado, un proyecto al 10 % completado y un objetivo secundario al 40 % completado, el porcentaje de objetivo completado es el 25 %.

### Porcentaje completado esperado {#expected-percent-complete}

Workfront Goals calcula automáticamente el porcentaje completado esperado de un objetivo en función del número total de días que dura el objetivo, así como del número de días que han pasado desde la fecha de inicio del objetivo.

Workfront Goals calcula el porcentaje completado esperado utilizando la fórmula siguiente:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Por ejemplo, si un objetivo se debe completar en 90 días y hoy es el día 45 de esa duración, el porcentaje completado esperado es del 50 %.

### Progreso y condición {#progress}

Workfront Goals calcula un porcentaje de progreso y asigna una etiqueta de progreso a los objetivos, en función del porcentaje de progreso alcanzado con respecto al porcentaje esperado completado en el momento actual. El color de la barra de porcentaje completado de la meta cambia para indicar el progreso de la meta.

La Condición de la meta también se actualiza, en consecuencia, para indicar si la meta está en el objetivo para completarse a tiempo o si se está quedando atrás.

Workfront Goals calcula el porcentaje de progreso de una meta utilizando la fórmula siguiente:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Por ejemplo, si el porcentaje completado esperado es del 53 % en el momento actual y el porcentaje completado real es del 30 %, el porcentaje de progreso completado del objetivo es del 56 %. Workfront Goals etiqueta esta meta con la condición &quot;en problemas&quot;.

El siguiente gráfico ilustra la relación entre las etiquetas de condición y el porcentaje de progreso:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

En la tabla siguiente se enumeran las etiquetas de condición de objetivo y los porcentajes de progreso de objetivo asociados a cada etiqueta.

>[!TIP]
>
>Las etiquetas de condición de objetivo coinciden con el nombre y el color de la condición del proyecto de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Nombre del progreso del objetivo</b></td> 
   <td><b>Definición del progreso del objetivo</b></td> 
   <td><b>Porcentaje de progreso del objetivo</b></td> 
   <td><b>Color de la barra de porcentaje completado</b></td> 
   <td><b>Icono de indicador de condición</b></td> 
  </tr> 
  <tr> 
   <td>Nuevo</td> 
   <td> <p>La meta es de nueva creación y aún no está registrando el progreso. El progreso de una meta se muestra como Nuevo hasta que alguien actualice su progreso por primera vez. </p> <p>Para obtener información sobre cómo actualizar el progreso de la meta, consulte <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Actualizar progreso de la meta en Adobe Workfront Goals</a>.</p> </td> 
   <td>Sin porcentaje</td> 
   <td>Sin barra</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>En destino</span> </p> </td> 
   <td>El objetivo está funcionando según lo esperado y hay una gran probabilidad de que se complete a tiempo. </td> 
   <td>90-100 %</td> 
   <td>Verde</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>En riesgo</span> </p> </td> 
   <td>El objetivo está rezagado, pero es posible que aún sea posible completarlo a tiempo. </td> 
   <td>70-89,99 %</td> 
   <td>Amarillo</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>Con Problemas</span> </p> </td> 
   <td> <p>Es muy probable que el objetivo no se complete a tiempo. </p> </td> 
   <td>0-69,99 %</td> 
   <td>Rojo</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouge_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>