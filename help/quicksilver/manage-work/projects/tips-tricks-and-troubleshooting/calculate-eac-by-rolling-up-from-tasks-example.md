---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Ejemplo de cálculo: Calcular EAC como un resumen de tareas'
description: PIM = basado en horas
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# Ejemplo de cálculo: Calcular EAC como un resumen de tareas

## Método EAC: resumir desde tareas o subtareas

* [PIM= Basado en horas](#pim-hour-based)
* [PIM= Basado en Costes](#pim-cost-based)

### PIM= Basado en horas {#pim-hour-based}

* [Ejemplo sencillo: proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks}

PIM = basado en horas

Método EAC = Resumen de tareas/subtareas

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas todas al usuario 1 cuyo coste/hora sea de 100,00 $.
1. Agregue horas planificadas/reales a cada tarea y % completado según la siguiente tabla:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tarea</strong> </p> </th> 
   <th> <br> <p><strong>Hrs pln</strong> </p> </th> 
   <th> <br> <p><strong>Hs reales</strong> </p> </th> 
   <th> <p><strong>% Finalizadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalcular finanzas
1. **CPI para la tarea 1** = 0,04 calculado de la siguiente manera:\
   **CPI para la tarea 1** = *IF* Horas reales > 0 *ENTONCES* CPI = TotalBudgetedCostWorkPerformance/horas reales\
       *ELSE* CPI = 1\
   **CPI para la tarea 1** = 1 / 25\
   **CPI para la tarea 1** = 0,04

1. **EAC para la tarea 1** = 125 horas calculadas de la siguiente manera:\
   **EAC para la tarea 1** = *IF* CPI &lt;> 0 *ENTONCES* EAC = Horas planificadas/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC para la tarea 1** = 5 / .04\
   **EAC para la tarea 1** = 125 horas

1. CPI/EAC para las tareas 2 y 3 son:\
   Tarea 2 = 0,12 / 83,33 horas\
   Tarea 3 = 0,24 / 62,5 horas

1. **CPI para proyecto** = 0,13 calculado de la siguiente manera:\
   **CPI para proyecto** = *IF* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI para proyecto** = 10 / 75\
   **CPI para proyecto** = 0,13

1. **EAC para proyecto** = 270,83 horas calculadas de la siguiente manera\
   **EAC para proyecto** = Tarea EAC 1 + Tarea EAC 2 + Tarea EAC 3\
   **EAC para proyecto** = 125 + 83,33 + 62,5\
   **EAC para proyecto** = 270,83 horas

#### Ejemplo complicado: proyecto tiene tareas secundarias {#complicated-example-project-has-children-tasks}

PIM = basado en horas

Método EAC = Resumen de tareas/subtareas

1. Crear el proyecto A con seis tareas en las que la tarea 3 es la principal de las tareas 4 y 5 y la tarea 1 es la principal de las tareas 2 y 3, como se muestra a continuación:\
   Tarea 1\
      Tarea 2\
      Tarea 3\
         Tarea 4\
         Tarea 5\
   Tarea 6

1. Asigne las tareas 2, 4, 5 y 6 al usuario 1 cuya tasa de coste/hora sea de 100,00 $.
1. Agregue horas planificadas/reales a cada tarea y % completado según la siguiente tabla.

   >[!NOTE]
   >
   >Para las tareas 1 y 3, solo está agregando horas reales.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tarea</strong> </p> </th> 
   <th> <br> <p><strong>Hrs pln</strong> </p> </th> 
   <th> <br> <p><strong>Hs reales</strong> </p> </th> 
   <th> <p><strong>% Finalizadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> </td> 
   <td> <p>10 Hrs</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Agregue 50 horas directamente al proyecto (Más>Horas>Horario de registro) para que haya 5.000,00 dólares de costo real de mano de obra registrados directamente en el proyecto.
1. Ejecutar nuevo cálculo de finanzas
1. **CPI para la tarea 2** = 0,1 calculado de la siguiente manera:\
   **CPI para la tarea 2** = *IF* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI para la tarea 2** = 1 / 10\
   **CPI para la tarea 2** = 0,1

1. **EAC para la tarea 2** = 50 horas calculadas de la siguiente manera:\
   **EAC para la tarea 2** = *IF* CPI &lt;> 0 *ENTONCES*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Horas planificadas + Horas reales\
   **EAC para la tarea 2** = 5 / 0,1\
   **EAC para la tarea 2** = 50 horas

1. CPI/EAC para la tarea 4, la tarea 5 y la tarea 6:\
   Tarea 4 = 0,4 / 25 horas\
   Tarea 5 = 0,75 / 20 horas\
   Tarea 6 = 1,2 / 16,67 horas

1. **CPI para la tarea 3** = 0,38\
   **CPI para la tarea 3** = *IF* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI para la tarea 3** = 11,5 / 30\
   **CPI para la tarea 3** = 0,38

1. **EAC para la tarea 3** = Tarea EAC 4 + Tarea EAC 5\
   **EAC para la tarea 3** = 25 + 20\
   **EAC para la tarea 3** = 45 horas

1. **CPI para la tarea 1** = 0,25 calculado de la siguiente manera:\
   **CPI para la tarea 1** = *IF* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI para la tarea 1** = 12,5 / 50\
   **CPI para la tarea 1** = 0,25

1. **EAC para la tarea 1** = Tarea EAC 2 + Tarea EAC 3\
   **EAC para la tarea 1** = 50 + 45\
   **EAC para la tarea 1** = 95 horas

1. CPI para Project = 0,22 calculado de la siguiente manera:\
   **CPI para proyecto** = *IF* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI para proyecto** = 24,5 / 110\
   **CPI para proyecto** = .22272\
   **CPI para proyecto** = 0,22

1. **EAC para proyecto** = Tarea EAC 1 + Tarea EAC 6\
   **EAC para proyecto** = 95 + 16,67\
   **EAC para proyecto** = 111,67 horas

### PIM= Basado en Costes {#pim-cost-based}

* [Ejemplo sencillo: proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)

#### Ejemplo sencillo: proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks-1}

PIM = Basado en Costes

Método EAC = Resumen de tareas/subtareas

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas todas al usuario 1 cuyo coste/ hora es de 100,00 $.
1. Agregue horas planificadas/reales a cada tarea y % completado según la siguiente tabla:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tarea</strong> </p> </th> 
   <th> <br> <p><strong>Hrs pln</strong> </p> </th> 
   <th> <br> <p><strong>Coste de libra</strong> </p> </th> 
   <th> <br> <p><strong>Hs reales</strong> </p> </th> 
   <th> <br> <p><strong>Coste de la biblioteca de leyes</strong> </p> </th> 
   <th> <p><strong>% Finalizadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Agregue gastos a cada tarea según la siguiente tabla:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tarea</strong> </p> </th> 
   <th> <p><strong>Gasto</strong> </p> </th> 
   <th> <p><strong>Importe planificado</strong> </p> </th> 
   <th> <p><strong>Importe real</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>Tarea 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>Tarea 1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Tarea 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>Tarea 3 Exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Añada dos gastos al proyecto (es decir, no vinculados a una tarea) de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Gasto</strong> </p> </th> 
   <th> <p><strong>Importe planificado</strong> </p> </th> 
   <th> <p><strong>Importe real</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Proyecto Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. En función de los valores anteriores, los costes incurridos/ no incurridos se determinan de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tarea</strong> </p> </th> 
   <th> <p><strong>Gastos planificados no incurridos</strong> </p> </th> 
   <th> <p><strong>Gastos planificados incurridos</strong> </p> </th> 
   <th> <p><strong>Gastos reales incurridos</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Desde Acciones de proyecto, ejecute Recalcular finanzas
1. **CPI****para la tarea 1** = 0,14 calculado de la siguiente manera:\
   **CPI****para la tarea 1**  = *IF* Coste real de mano de obra + Coste real de gastos &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****para la tarea 1**  = (100+300) / (2500+400)\
   **CPI****para la tarea 1**  = 400 / 2900\
   **CPI****para la tarea 1**  = 0,14

1. **EAC****para la tarea 1** = 13 400,00 $\
   **CPI Labor****para la tarea 1** = SI costo laboral real &lt;> 0 ENTONCES

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****para la tarea 1** = 100/2500\
   **CPI Labor****para la tarea 1** = 0,04

   **EAC Labor****para la tarea 1** = *IF* CPI_Labor &lt;> 0 *ENTONCES*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Trabajo de la CAO = costo laboral previsto + costo laboral real\
   **EAC Labor****para la tarea 1** = 500,00/,04\
   **EAC Labor****para la tarea 1** = 12.500,00 $

   **Gastos de EAC****para la tarea 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gastos de EAC****para la tarea 1** = 400,00 $ + 500,00 $\
   **Gastos de EAC****para la tarea 1** = 900,00 $

   **EAC****para la tarea 1** = Trabajo EAC + Gastos EAC\
   **EAC****para la tarea 1**  = 12.500,00 $ + 900,00 $\
   **EAC****para la tarea 1**  = 13 400,00 $

1. Estos son los valores de CPI/EAC para la tarea 2 y la tarea 3:\
   Tarea 2 = 0,19 / 8,433,33\
   Tarea 3 = 0,44 / 6.950,00 $***

1. El IPC para el proyecto = 0,32\
   **CPI****para proyecto** = *IF* Coste real de mano de obra + Coste real de gastos &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****para proyecto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****para proyecto** = 3300 / 10200\
   **CPI****para proyecto** = 0,32

1. La CAO para el proyecto es de 28.783,33 dólares\
   **EAC****para proyecto** = Tarea EAC 1 + Tarea EAC 2 + Tarea EAC 3\
   **EAC****para proyecto** = 13.400,00 $ + 8.433,33 $ + 6.950,00 $\
   **EAC****para proyecto** = 28.783,33 $
