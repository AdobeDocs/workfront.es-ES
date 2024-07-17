---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular índice de rendimiento de costes (CPI)
description: El índice de rendimiento de costos (CPI) describe la relación en el nivel de proyecto o tarea entre el costo planificado y el costo real. Los administradores de proyectos revisan esta métrica para identificar las tareas o los proyectos cuyo seguimiento actual sea inferior o superior al costo en un momento determinado.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Calcular índice de rendimiento de costes (CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

El índice de rendimiento de costos (CPI) describe la relación en el nivel de proyecto o tarea entre el costo planificado y el costo real. Los administradores de proyectos revisan esta métrica para identificar las tareas o los proyectos cuyo seguimiento actual sea inferior o superior al costo en un momento determinado. El costo se puede medir en horas o dólares, según el método de índice de rendimiento (PIM). Para obtener más información acerca de cómo establecer el método de índice de rendimiento, vea [Establecer el método de índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Solo las organizaciones que requieren introducir tiempo pueden utilizar CPI. Además, los valores de PIM basados en costes solo son precisos en organizaciones que han definido tasas de coste para los usuarios asignados a tareas (roles de trabajo o usuarios).

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
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a proyectos y datos financieros</p> <p> Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores al proyecto con permisos para Ver finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Resumen del índice de rendimiento de costes (CPI)

* [El valor CPI](#the-cpi-value)
* [Cómo se calcula el IPC](#how-cpi-is-calculated)

### El valor del IPC {#the-cpi-value}

Los jefes de proyecto entienden que un valor de CPI de 1 significa que el proyecto se ajusta exactamente al presupuesto. Los valores mayores que 1 indican que un proyecto está por debajo del presupuesto (se han registrado menos horas o gastos de los planeados originalmente) y los valores menores que 1 significan que un proyecto está por encima del presupuesto (se han registrado más horas o gastos de los planeados originalmente). Cuanto más lejos esté 1, mayor será la desviación con respecto al plan.

| **Valor CPI** | **Indicación en el presupuesto** |
|---|---|
| 1 | Dentro del plan o presupuesto |
| > 1 (mayor que 1) | Por debajo del presupuesto |
| &lt; 1 (menos de 1) | Presupuesto excesivo |


### Cómo se calcula el IPC {#how-cpi-is-calculated}

En Adobe Workfront, el cálculo del CPI depende del método de índice de rendimiento seleccionado para el proyecto. Para obtener más información acerca de cómo establecer el método de índice de rendimiento, vea [Establecer el método de índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Cálculos de CPI al usar PIM basados en horas](#cpi-calculations-when-using-hour-based-pim)
* [Cálculos de CPI al usar PIM basado en costos](#cpi-calculations-when-using-cost-based-pim)

#### Cálculos de CPI al usar PIM basado en horas {#cpi-calculations-when-using-hour-based-pim}

Si

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Caso contrario

```
CPI = 1
```

* **Para una tarea que no es principal:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **Para una tarea principal:**
Trabajo presupuestado total realizado = la suma del campo Trabajo presupuestado total realizado para todas las tareas secundarias directas.

* **Para un proyecto:**
Trabajo presupuestado total realizado = la suma del campo Trabajo presupuestado total realizado para todas las tareas de nivel superior (tareas principales y autónomas).

Para obtener información sobre el trabajo de costo presupuestado total realizado (CPTR), vea [Calcular el trabajo de costo presupuestado realizado (CPTR)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Cálculos de CPI al usar PIM basado en costos {#cpi-calculations-when-using-cost-based-pim}

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



Caso contrario

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

Gasto incurrido es el gasto en el cual el costo real es > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* El costo planificado del trabajo realizado se calcula mediante la siguiente fórmula:

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

El Trabajo total presupuestado realizado se calcula para lo siguiente:

* **Para una tarea que no es principal:**

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



## Localizar CPI en un proyecto o tarea

Puede mostrar el CPI de un proyecto o una tarea en una lista de proyectos o tareas o en un informe. Además, puede verlo en el nivel de proyecto o tarea.

1. Vaya al proyecto o tarea donde desee ver el CPI.
1. Expanda **Detalles del proyecto** o **Detalles de la tarea** en el panel izquierdo, dependiendo de si está viendo el CPI de un proyecto o tarea.

1. Haga clic en **Finanzas**.

   El CPI se muestra en el campo **CPI/ SPI/ CSI**.

   ![](assets/cpi-on-project-nwe.png)
