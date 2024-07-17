---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Ejemplo de cálculo: calcule el EAC en el nivel de proyecto'
description: PIM = Basado en horas
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Ejemplo de cálculo: calcule el EAC en el nivel de proyecto

## Método EAC: calcular en el nivel de proyecto

* [PIM = Basado en horas](#pim-hour-based)
* [PIM= Basado en costes](#pim-cost-based)

### PIM = Basado en horas {#pim-hour-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: un proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks}

PIM = Basado en horas

Método EAC = Calcular a nivel de proyecto ****

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo costo/hora sea de 100,00 $.
1. Agregar horas planificadas y reales a cada tarea y % completado según la tabla siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Tarea</strong></p></th>
      <th><br><p><strong>Hrs pln</strong></p></th>
      <th><br><p><strong>Hs reales</strong></p></th>
      <th><p><strong>% Finalizado</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Tarea 1</p></td>
      <td><p>5 horas</p></td>
      <td><p>25 horas</p></td>
      <td><p>20 %</p></td>
     </tr>
     <tr>
      <td><p>Tarea 2</p></td>
      <td><p>10 horas</p></td>
      <td><p>25 horas</p></td>
      <td><p>30 %</p></td>
     </tr>
     <tr>
      <td><p>Tarea 3</p></td>
      <td><p>15 horas</p></td>
      <td><p>25 horas</p></td>
      <td><p>40 %</p></td>
     </tr>
    </tbody>
   </table>

1. Volver a calcular finanzas en el proyecto.
1. **IRC para la tarea 1** = 0,04 calculado de la siguiente manera:\
   **IRC para la tarea 1** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
      *ELSE* IRC = 1\
   **IRC para Tarea 1** = 1 / 25\
   **IRC para la tarea 1** = 0,04

1. **EAC para la tarea 1** = 125 horas calculado de la siguiente manera:\
   **EAC para la tarea 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas/CPI planificadas\
       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para la tarea 1** = 5 / .04\
   **EAC para la tarea 1** = 125 horas****

1. IRC/EAC para las Tareas 2 y 3 son:\
   Tarea  2 = 0,12 / 83,33  h\
   Tarea 3 = 0,24 / 62,5 horas

1. **IRC del proyecto** = 0,13 calculado de la siguiente manera:\
   **IRC para el proyecto** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
       *ELSE* IRC = 1\
   **IRC del proyecto** = 10 / 75\
   **IRC del proyecto** = 0,13

1. **EAC para el proyecto** = 225 horas calculado de la siguiente manera:\
   **EAC para el proyecto** = *IF* CPI &lt;> 0 *THEN* EAC = Horas/CPI planificadas\
       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para el proyecto** = 30 / .13333\
   **EAC para el proyecto** = 225 horas

#### Ejemplo complicado: un proyecto tiene tareas secundarias {#complicated-example-project-has-children-tasks}

PIM = Basado en horas

Método EAC = Calcular a nivel de proyecto

1. Cree el proyecto A con seis tareas en las que la Tarea 3 sea la principal de las Tareas 4 y 5 y la Tarea 1 sea la principal de las Tareas 2 y 3, como se muestra a continuación:\
   Tarea 1\
      Tarea 2\
      Tarea 3\
         Tarea 4\
         Tarea 5\
   Tarea 6

1. Asigne las Tareas 2, 4, 5 y 6 al Usuario 1 cuya tarifa de costo/hora sea de $100.00.
1. Agregar horas planificadas/ reales a cada tarea y % completado según la tabla siguiente.

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

1. Agregue 50 horas directamente al proyecto (Más>Horas>Registrar horas).
1. **IRC para la tarea 2** = .1 calculado de la siguiente manera:\
   **IRC para la tarea 2** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
       *ELSE* IRC = 1\
   **IRC para Tarea 2** = 1 / 10\
   **IRC para la tarea 2** = .1

1. **EAC para la tarea 2** = 50 horas calculado de la siguiente manera:\
   **EAC para la tarea 2** = *IF* CPI &lt;> 0 *THEN* EAC = Horas/CPI planificadas\
       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para la tarea 2** = 5 / .1\
   **EAC para la tarea 2** = 50 horas

1. El IRC/EAC para las Tareas 4, 5 y 6 es el siguiente:\
   Tarea 4: 0,4 / 25 horas\
   Tarea 5: 0,75/20 h\
   Tarea 6: 1,2 / 16,67 horas

1. **IRC para la tarea 3** = 0,38  se calcula de la siguiente manera:\
   **IRC para la tarea 3** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
       *ELSE* IRC = 1\
   **IRC para la tarea 3** = 11.5 / 30\
   **IRC para la tarea 3** = 0,38

1. **EAC para la tarea 3** = 65,22 horas calculado de la siguiente manera:\
   **EAC para la tarea 3** = *IF* CPI &lt;> 0 *THEN* EAC = Horas/CPI planificadas\
       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para la tarea 3** =  25 / .383333\
   **EAC para la tarea 3** = 65,22 horas

1. **IRC para la tarea 1** = 0,25 calculado de la siguiente manera:\
   **IRC para la tarea 1** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
       *ELSE* IRC = 1\
   **IRC de la tarea 1** = 12,5 / 50\
   **IRC para la tarea 1** = 0,25

1. **EAC para la tarea 1** = 120 horas calculado de la siguiente manera:\
   **EAC para la tarea 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas planificadas / CPI\
       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para la tarea 1** =  30/,25\
   **EAC para la tarea 1** = 120 horas

1. **IRC del proyecto** = 0,22 calculado de la siguiente manera:\
   **IRC para el proyecto** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
       *ELSE* IRC = 1\
   **IRC del proyecto** = 24,5 / 110\
   **IRC del proyecto** = .22272\
   **IRC del proyecto** = .22

1. **EAC para el proyecto** = 224.49  h calculadas como se indica a continuación:\
   **EAC para el proyecto** = *IF* CPI &lt;> 0 *THEN* EAC = Horas/CPI planificadas\
       *ELSE* EAC = Planificado  Horas + Real  Horas\
   **EAC para el proyecto** =  50 / .22272\
   **EAC para el proyecto** = 224,49 horas

### PIM= Basado en costes {#pim-cost-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: un proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks-1}

PIM = Basado en Costes

Método EAC = Calcular a nivel de proyecto

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo costo/hora sea de 100,00 $.
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
   <td> <p> 2.700,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. En Acciones de proyecto, ejecute Recalcular finanzas
1. **IRC para la tarea 1** = 0,14
1. **IRC****para la tarea 1** = 0,14 calculado de la siguiente manera:\
   **IRC**  **para la tarea 1** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **IRC****para Tarea 1** = (100+300) / (2500+400)\
   **IRC**  **para la tarea 1** = 400 / 2900\
   **IRC**  **para la tarea 1**  = 0,14****

1. **EAC****para la tarea 1** = 13.400,00 $\
   **Trabajo CPI**  **para Tarea 1** = IF Costo de mano de obra real &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Trabajo CPI**  **para Tarea 1** = 100/2500\
   **Trabajo CPI**  **para la tarea 1** = .04 ****** Mano de obra EAC ****para la tarea 1 **=*IF *CPI_Labor &lt;> 0*THEN *Mano de obra EAC = Costo de mano de obra planificado/CPI_Labor\
   *    ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC ****para la tarea 1** = 500.00/.04\
   **Trabajo EAC****para la tarea 1** = 12.500,00 $\
   **EAC Expense****for Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto EAC****para la tarea 1** = 400,00 $ + 500,00 $\
   **Gasto EAC****para la tarea 1** = 900,00 $\
   **EAC****para Tarea 1** = Mano de obra EAC + Gasto EAC\
   **EAC****para la tarea 1**  = 12.500,00 $ + 900,00 $\
   **EAC****para la tarea 1**  = 13.400,00 $

1. Estos son los valores CPI / EAC para la Tarea 2 y la Tarea 3:\
   Tarea 2 = 0,19 / 8.433,33 $\
   Tarea 3 = 0,44 / 6.950,00 $

1. **IRC del proyecto** = 0,32 calculado de la siguiente manera:\
   **CPI****para el proyecto** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **IRC****para el proyecto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****para el proyecto** = 3300 / 10200\
   **IRC****para el proyecto** = 0,32

1. **EAC para el proyecto** = 28.200,00 $ calculado de la siguiente manera:\
   **Trabajo del IRC****para el proyecto** = SI Costo de mano de obra real &lt;> 0 ENTONCES

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Trabajo de CPI****para el proyecto** = 1000 / 7500\
   **Trabajo de CPI****para el proyecto** = .13333\
   **Trabajo de CPI****para el proyecto** = .13

   **Trabajo EAC****para el proyecto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC****para el proyecto** = 3000/.13333\
   **Trabajo EAC****para el proyecto** = 22.500,00 $

   **Proyecto****Gasto EAC** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Proyecto****Gasto EAC** = 3000,00 $ + 2.700,00 $\
   **Proyecto****Gasto EAC** = 5.700,00 $

   **EAC****Proyecto** = Mano de obra EAC + Gasto EAC\
   **EAC****Project**  = 22.500,00 $ + 5.700,00 $\
   **EAC****Project**  = 28.200,00 $

#### Ejemplo complicado: un proyecto tiene tareas secundarias {#complicated-example-project-has-children-tasks-1}

PIM = Basado en Costes

Método EAC = Calcular a nivel de proyecto

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
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>$2.000,00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Agregue 50 horas directamente al proyecto (Más>Horas>Registrar horas) de modo que haya $5,000.00 de costo laboral real registrado directamente en el proyecto. ****
1. Agregar gastos a cada tarea según la tabla siguiente (he agregado una fila en blanco entre cada tarea para facilitar la lectura):

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
   <td> <p>- 400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>Tarea 1 Cad 2</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>Tarea 1 Cad 3</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>0,00 USD</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Tarea 2 Cad 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Tarea 2 Cad 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>0,00 USD</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Tarea 2 Cad 3</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Tarea 2 Cad 4</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>Tarea 3 Cad</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>$1.000,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>Tarea 4 Cad 1</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>0,00 USD</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>Tarea 4 Cad 2</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4 </p> </td> 
   <td> <p>Tarea 4 Cad 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>0,00 USD</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>Tarea 5 Exp 1</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>Tarea 5 Cad 2</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>Tarea 5 Cad 3</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>Tarea 6 Exp 1</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>Tarea 6 Exp 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>- 300,0 $</p> </td> 
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
   <td> <p> 0,00 USD <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. En función de los valores anteriores, los costes incurridos/no incurridos se determinan de la siguiente manera:

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
   <td> <p>400,00 $</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>1.300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>$1.000,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1.100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>0,00 USD</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>$1.000,00</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. En Acciones de proyecto, ejecute Recalcular finanzas
1. **IRC** para la Tarea 2 = 0,17 calculado de la siguiente manera:\
   **Tarea CPI 2** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **IRC****Tarea 2** = (100+300) / (1000+1300)\
   **IRC****Tarea 2**  = 400 / 2300\
   **IRC****Tarea 2**  = 0,17

1. **EAC** para la Tarea 2 = $5,900.00\
   **CPI Trabajo****Tarea 2** = SI Costo de mano de obra real &lt;> 0 ENTONCES CPI_Trabajo = TotalBudgetedCostWorkPerformed / Costo de mano de obra real\
      ELSE CPI_Labor = 1\
   **Trabajo **** IRC 2** = 100/1000\
   **Trabajo de IRC****tarea 2** = .1

   **EAC Labor****Task 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC****Tarea 2** = 500.00/.1\
   **Trabajo EAC****Tarea 2** = 5.000,00 $****** Gasto EAC ****Tarea 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto EAC ****Tarea 2** = $1,300.00 + -$400.00\
   **Gasto EAC****Tarea 2** = 900,00 $

   **EAC****Tarea 2** = Mano de obra EAC + Gasto EAC\
   **EAC****Tarea 2**  = 5.000,00 $ + 900,00 $\
   **EAC****Tarea 2**  = 5.900,00 $

1. El IRC/EAC para las tareas 4, 5 y 6 se determina de la misma manera, así que proporcionaré los siguientes valores:\
   Tarea 4: 0,23 / 3.400,00 $\
   Tarea 5: 0,64 / 3.100,00 $\
   Tarea 6: 1,06 / 2.366,67 dólares

1. IRC para la Tarea 3 = 0,31 calculado de la siguiente manera:\
   **CPI****Tarea 3** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **IRC****Tarea 3**  = (1 150 + 500) / (3 000 + 2 400)\
   **IRC****Tarea 3**  =  5400 / 1650\
   **IRC****Tarea 3**  = 0,31 ****** EAC para la tarea 3 **= 9.521,74 $ calculado de la siguiente manera:\
   **Trabajo IRC ****Tarea 3** = SI Costo de mano de obra real &lt;> 0 ENTONCES

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Trabajo **** CPI 3** = 1150/3000\
   **Trabajo de IRC****tarea 3** = .383333\
   **Trabajo de CPI****Tarea 3** = 0,38

   **EAC Labor****Task 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC****Tarea 3** = $2,500.00 /.383333\
   **Tarea **** mano de obra EAC 3** = 6.521,74 $

   **EAC Expense****Task 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto****Tarea EAC 3** = 2.400,00 $ + 600,00 $\
   **Gasto EAC****Tarea 3** = 3.000,00 $

   **EAC****Tarea 3** = Mano de obra EAC + Gasto EAC\
   **EAC****Tarea 3**  = 6.521,74 $ + 3.000,00 $\
   **EAC****Tarea 3**  = 9.521,74 $

1. IRC para la Tarea 1 = 0,16 calculado de la siguiente manera:\
   **CPI****Tarea 1** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **IRC****Tarea 1**  = (1250 + 300) / (5000 + 4500)\
   **IRC****Tarea 1**  =  1550 / 9500=\
   **IRC****Tarea 1**  = 0,16

1. El valor de EAC para la Tarea 1 es de 17.100,00 $, calculado de la siguiente manera:\
   **CPI Trabajo****Tarea 1** = IF Costo de mano de obra real &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Trabajo****Tarea 1** = 1250 / 5000\
   **Trabajo de IRC****tarea 1** = 0,25

   **Trabajo EAC****Tarea 1** = *IF* CPI_Labor &lt;> 0 *ENTONCES* Trabajo EAC = Costo de mano de obra planificado / CPI_Labor\
   *   ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC****Tarea 1** = $3,000.00 /.25\
   **Trabajo EAC****Tarea 1** = 12.000,00 $

   **EAC Expense****Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto****Tarea 1 de EAC** = $4500 + 600\
   **Gasto EAC****Tarea 1** = 5.100,00 $

   **EAC****Tarea 1** = Mano de obra EAC + Gasto EAC\
   **EAC****Tarea 1**  = 12 000,00 $ + 5 100,00\
   **EAC****Tarea 1**  = 17.100,00 $

1. El IRC del proyecto es de 0,25\
   **CPI****para el proyecto** = *IF* Costo de mano de obra real + IncurredActualExpenseCost  &lt;> 0 *ENTONCES*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **IRC****para el proyecto** = (2450 + 1900) / (11000 + 6700)\
   **IRC****para el proyecto** =   4350 / 17700\
   **IRC****para el proyecto** = 0,25

1. **EAC para el proyecto** = 32.248,98 $ calculado de la siguiente manera:\
   **Trabajo del IRC****para el proyecto** = SI Costo de mano de obra real &lt;> 0 ENTONCES

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Trabajo de CPI****para el proyecto** = 2450 / 11000\
   **Trabajo de CPI****para el proyecto** = .22272\
   **Trabajo de CPI****para el proyecto** = .22

   **Trabajo EAC****para el proyecto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
   **Trabajo EAC****para el proyecto** = 5.000,00 $ / .22272\
   **Trabajo EAC****para el proyecto** = 22.448,97959 $\
   **Trabajo EAC****para el proyecto** = 22.448,98 $

   **EAC Expense****Project** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Proyecto****Gasto EAC** = 3.100,00 $ + 6.700,00 $\
   **Proyecto****Gasto EAC** = 9.800,00 $

   **EAC****Proyecto** = Mano de obra EAC + Gasto EAC\
   **EAC****Project**  = 22.448,98 $ + 9.800,00 $\
   **EAC****Project**  = 32.248,98 $
