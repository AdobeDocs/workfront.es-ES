---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el índice de rendimiento de costes (CPI)
description: El Índice de Rendimiento de Coste (IPC) describe la relación a nivel de proyecto o tarea entre el coste planificado y el coste real. Los administradores de proyectos revisan esta métrica para identificar las tareas o los proyectos que actualmente siguen por debajo o por encima del coste en un punto determinado.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Calcular el índice de rendimiento de costes (CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

El Índice de Rendimiento de Coste (IPC) describe la relación a nivel de proyecto o tarea entre el coste planificado y el coste real. Los administradores de proyectos revisan esta métrica para identificar las tareas o los proyectos que actualmente siguen por debajo o por encima del coste en un punto determinado. El coste se puede medir en horas o dólares, según el método de índice de rendimiento (PIM). Para obtener más información sobre la configuración del método de índice de rendimiento, consulte [Definir el método del índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Solo las organizaciones que requieren la entrada de tiempo pueden utilizar CPI. Además, los valores de PIM basados en costes solo son precisos en las organizaciones que tienen tasas de coste definidas para las personas asignadas a tareas (funciones de trabajo o usuarios).

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
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a Proyectos y Datos Financieros</p> <p> Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores del proyecto con permisos para Ver finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Resumen del Índice de Rendimiento de Costes (IPC)

* [El valor CPI](#the-cpi-value)
* [Cálculo del CPI](#how-cpi-is-calculated)

### El valor CPI {#the-cpi-value}

Los administradores de proyectos entienden que un valor de CPI de 1 significa que el proyecto está exactamente dentro del presupuesto. Los valores buenos a la 1 indican que un proyecto está por debajo del presupuesto (se han registrado menos horas o gastos que los planeados originalmente) y los valores inferiores a 1 indican que un proyecto está por encima del presupuesto (se han registrado más horas o gastos que los planeados originalmente). Además del 1, la buena desviación del plan.

| **Valor de CPI** | **Indicación presupuestaria** |
|---|---|
| 1 | En plan o presupuesto |
| > 1 (bueno que 1) | Bajo presupuesto |
| &lt; 1 (menor que 1) | Más de un presupuesto |


### Cálculo del CPI {#how-cpi-is-calculated}

En Adobe Workfront, el cálculo de CPI depende del método de índice de rendimiento seleccionado para el proyecto. Para obtener más información sobre la configuración del método de índice de rendimiento, consulte [Definir el método del índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Cálculos CPI al utilizar PIM basado en horas](#cpi-calculations-when-using-hour-based-pim)
* [Cálculos CPI al utilizar PIM basado en costes](#cpi-calculations-when-using-cost-based-pim)

#### Cálculos CPI al utilizar PIM basado en horas {#cpi-calculations-when-using-hour-based-pim}

Si

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

De otro modo

```
CPI = 1
```

* **Para una tarea no principal:**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **Para una tarea principal:**
Total de trabajo de coste presupuestado realizado = la suma del campo Total de trabajo de coste presupuestado realizado para todas las tareas secundarias directas.

* **Para un proyecto:**
Total de trabajo de coste presupuestado realizado = la suma del campo Total de trabajo de coste presupuestado realizado para todas las tareas de nivel superior (principales y tareas independientes).

Para obtener información sobre el trabajo de costo presupuestado total realizado (CPTR), consulte [Calcular el trabajo de coste presupuestado realizado (CPTR)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Cálculos CPI al utilizar PIM basado en costes {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

Si

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



De otro modo

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

Los campos de este cálculo se describen a continuación:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Gastos incurridos es el gasto en el que Coste real > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* El costo planificado del trabajo realizado se calcula mediante la fórmula siguiente:

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

El trabajo de coste presupuestado total realizado se calcula para lo siguiente:

* **Para una tarea no principal:**

   ```
   Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
   ```

* **Para una tarea principal:**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
   ```

* **Para un proyecto:**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
   ```



## Localización de CPI en un proyecto o tarea

Puede mostrar el CPI de un proyecto o una tarea en una lista o informe de proyecto o tarea. Además, puede verlo en el nivel de proyecto o tarea.

1. Vaya al proyecto o la tarea donde desee ver el CPI.
1. Expandir **Detalles del proyecto** o **Detalles de la tarea** en el panel izquierdo, en función de si está viendo CPI para un proyecto o una tarea.

1. Haga clic en **Finanzas**.

   La CPI se muestra en la **CPI/ SPI/ CSI** campo .

   ![](assets/cpi-on-project-nwe.png)
