---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Ejemplo de cálculo: Calcule EAC como resumen a partir de tareas'
description: PIM = Basado en horas
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# Ejemplo de cálculo: Calcule EAC como resumen a partir de tareas

## Método EAC: resumen de tareas o subtareas

* [PIM= basado en horas](#pim-hour-based)
* [PIM= Basado en costes](#pim-cost-based)

### PIM= Basado en horas {#pim-hour-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: un proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks}

PIM = Basado en horas

Método EAC = Resumir a partir de tareas/ subtareas

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo costo/hora sea de 100,00 $.
1. Agregar horas planificadas/ reales a cada tarea y % completado según la tabla siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tarea</strong> </p> </th> 
   <th> <br> <p><strong>Hrs pln</strong> </p> </th> 
   <th> <br> <p><strong>Horas reales</strong> </p> </th> 
   <th> <p><strong>% completado</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalcular finanzas
1. **IRC para la tarea 1** = 0,04 calculado de la siguiente manera:\
   **IRC para la tarea 1** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
       *ELSE* IRC = 1\
   **IRC para Tarea 1** = 1 / 25\
   **IRC para la tarea 1** = 0,04

1. **EAC para la tarea 1** = 125 horas calculado de la siguiente manera:\
   **EAC para la tarea 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas/ CPI planificadas\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC para la tarea 1** = 5 / .04\
   **EAC para la tarea 1** = 125 horas

1. IRC/EAC para las Tareas 2 y 3 son:\
   Tarea  2 = 0,12 / 83,33  h\
   Tarea 3 = 0,24 / 62,5 horas

1. **IRC del proyecto** = 0,13 calculado de la siguiente manera:\
   **IRC para el proyecto** = *SI* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IRC = 1\
   **IRC del proyecto** = 10 / 75\
   **IRC del proyecto** = 0,13

1. **EAC para el proyecto** = 270,83 horas calculado de la siguiente manera\
   **EAC para el proyecto** = Tarea EAC 1 + Tarea EAC 2 + Tarea EAC 3\
   **EAC para el proyecto** = 125 + 83,33 + 62,5\
   **EAC para el proyecto** = 270,83 horas

#### Ejemplo complicado: un proyecto tiene tareas secundarias {#complicated-example-project-has-children-tasks}

PIM = Basado en horas

Método EAC = Resumir a partir de tareas/ subtareas

1. Cree el proyecto A con seis tareas en las que la Tarea 3 sea la principal de las Tareas 4 y 5 y la Tarea 1 sea la principal de las Tareas 2 y 3, como se muestra a continuación:\
   Tarea 1\
      Tarea 2\
      Tarea 3\
         Tarea 4\
         Tarea 5\
   Tarea 6

1. Asigne las Tareas 2, 4, 5 y 6 al Usuario 1 cuya tarifa de costo/hora sea de $100.00.
1. Agregar horas planificadas/reales a cada tarea y % completado según la tabla siguiente.

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
   <th> <br> <p><strong>Horas reales</strong> </p> </th> 
   <th> <p><strong>% completado</strong> </p> </th> 
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
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Agregue 50 horas directamente al proyecto (Más>Horas>Registrar horas) de modo que haya $5,000.00 de costo laboral real registrado directamente en el proyecto.
1. Ejecutar recalcular finanzas
1. **IRC para la tarea 2** = .1 calculado de la siguiente manera:\
   **IRC para la tarea 2** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IRC = 1\
   **IRC para Tarea 2** = 1 / 10\
   **IRC para la tarea 2** = .1

1. **EAC para la tarea 2** = 50 horas calculado de la siguiente manera:\
   **EAC para la tarea 2** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para la tarea 2** = 5 / .1\
   **EAC para la tarea 2** = 50 horas

1. IRC/EAC para Tarea 4, Tarea 5 y Tarea 6:\
   Tarea 4 = 0,4 / 25 horas\
   Tarea 5 = 0,75 / 20 horas\
   Tarea 6 = 1,2 / 16,67 horas

1. **IRC para la tarea 3** = 0,38\
   **IRC para la tarea 3** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IRC = 1\
   **IRC para la tarea 3** = 11.5 / 30\
   **IRC para la tarea 3** = 0,38

1. **EAC para la Tarea 3** = Tarea EAC 4 + Tarea EAC 5\
   **EAC para la tarea 3** = 25 + 20\
   **EAC para la tarea 3** = 45 horas

1. **IRC para la tarea 1** = 0,25 calculado de la siguiente manera:\
   **IRC para la tarea 1** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IRC = 1\
   **IRC de la tarea 1** = 12,5 / 50\
   **IRC para la tarea 1** = 0,25

1. **EAC para la Tarea 1** = EAC Tarea 2 + EAC Tarea 3\
   **EAC para la tarea 1** = 50 + 45\
   **EAC para la tarea 1** = 95 horas

1. IRC del proyecto = 0,22, calculado de la siguiente manera:\
   **IRC para el proyecto** = *SI* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IRC = 1\
   **IRC del proyecto** = 24,5 / 110\
   **IRC del proyecto** = .22272\
   **IRC del proyecto** = .22

1. **EAC para el proyecto** = Tarea EAC 1 + Tarea EAC 6\
   **EAC para el proyecto** = 95 + 16,67\
   **EAC para el proyecto** = 111,67 horas

### PIM= Basado en costes {#pim-cost-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks-1}

PIM = Basado en Costes

Método EAC = Resumir a partir de tareas/ subtareas

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo costo/ hora es de 100,00 $.
1. Agregar horas planificadas/ reales a cada tarea y % completado según la tabla siguiente:

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
   <th> <br> <p><strong>Costo Lbr Pln</strong> </p> </th> 
   <th> <br> <p><strong>Horas reales</strong> </p> </th> 
   <th> <br> <p><strong>Costo real Lbr</strong> </p> </th> 
   <th> <p><strong>% completado</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Agregue gastos a cada tarea según la tabla siguiente:

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
   <td> <p>Tarea 1 Cad 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>Tarea 1 Cad 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>0,00 USD</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Cad de tarea 2</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>Tarea 3 Cad</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Agregue dos gastos al proyecto (es decir, no vinculados a una tarea) de la siguiente manera:

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
   <td> <p>$1.000,00</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1 Cad 2</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>0,00 USD</p> </td> 
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
   <th> <p><strong>Gasto planificado no incurrido</strong> </p> </th> 
   <th> <p><strong>Gasto planificado incurrido</strong> </p> </th> 
   <th> <p><strong>Gasto real incurrido</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>3.000,00 $</p> </td> 
   <td> <p>2.300,00 $</p> </td> 
   <td> <p>2.700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. En Acciones de proyecto, ejecute Recalcular finanzas
1. **IRC****para la tarea 1** = 0,14 calculado de la siguiente manera:\
   **IRC****para la tarea 1**  = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **IRC****para la tarea 1**  = (100+300) / (2500+400)\
   **IRC****para la tarea 1**  = 400 / 2900\
   **IRC****para la tarea 1**  = 0,14

1. **EAC****para la tarea 1** = 13.400,00 $\
   **Trabajo del IRC****para la Tarea 1** = IF Costo de mano de obra real &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Trabajo de CPI****para la tarea 1** = 100/2500\
   **Trabajo de IRC****para la tarea 1** = 0,04

   **Trabajo EAC****para la tarea 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC****para la tarea 1** = 500.00/.04\
   **Trabajo EAC****para la tarea 1** = 12.500,00 $

   **EAC Expense****for Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto EAC****para la tarea 1** = 400,00 $ + 500,00 $\
   **Gasto EAC****para la tarea 1** = 900,00 $

   **EAC****para Tarea 1** = Mano de obra EAC + Gasto EAC\
   **EAC****para la tarea 1**  = 12.500,00 $ + 900,00 $\
   **EAC****para la tarea 1**  = 13.400,00 $

1. Estos son los valores CPI / EAC para la Tarea 2 y la Tarea 3:\
   Tarea 2 = 0,19 / 8.433,33 $\
   Tarea 3 = 0,44 / 6.950,00 $****

1. IPC del proyecto = 0,32\
   **CPI****para el proyecto** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **IRC****para el proyecto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****para el proyecto** = 3300 / 10200\
   **IRC****para el proyecto** = 0,32

1. El EAC para el proyecto es de $28,783.33\
   **EAC****para el proyecto** = Tarea EAC 1 + Tarea EAC 2 + Tarea EAC 3\
   **EAC****para el proyecto** = 13.400,00 $ + 8.433,33 $ + 6.950,00 $\
   **EAC****para el proyecto** = 28.783,33 $
