---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Ejemplo de cálculo: calcule EAC en el nivel de proyecto'
description: Este artículo proporciona un ejemplo de cálculo de la estimación al finalizar (EAC) de un proyecto a nivel de proyecto en Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '2214'
ht-degree: 98%

---

# Ejemplo de cálculo: calcular el EAC en el nivel de proyecto

## Método EAC: calcular en el nivel de proyecto

* [PIM = basado en horas](#pim-hour-based)
* [PIM = basado en costes](#pim-cost-based)

### PIM = Basado en horas {#pim-hour-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: un proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks}

PIM = Basado en horas

Método EAC = calcular en el nivel de proyecto ****

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo coste/hora sea de 100,00 USD.
1. Añadir horas planificadas y reales a cada tarea y el % completado según la tabla siguiente:

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
      <td><p>20 %</p></td>
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
      <td><p>40 %</p></td>
     </tr>
    </tbody>
   </table>

1. Volver a calcular las finanzas en el proyecto.
1. **IRC de la tarea 1** = 0,04 calculado de la siguiente manera:\
   **IRC de la tarea 1** = *IF* Horas reales > 0 *THEN* IRC = TotalBudgetedCostWorkPerformed/Horas reales\
      *ELSE* IRC = 1\
   **IRC de la tarea 1** = 1 / 25\
   **IRC de la tarea 1** = 0,04

1. **EAC para la tarea 1** = 125 horas calculado de la siguiente manera:\
   **EAC de la tarea 1** = *IF* IRC &lt;> 0 *THEN* EAC = Horas planificadas/IRC\
       *ELSE* EAC = Horas planificadas + Horas reales\
   **EAC para la tarea 1** = 5 / 0,04\
   **EAC para la tarea 1** = 125 horas****

1. Los IRC y EAC de las tareas 2 y 3 son los siguientes:\
   Tarea  2 = 0,12 / 83,33  h\
   Tarea 3 = 0,24 / 62,5 horas

1. **IRC del proyecto** = 0,13 calculado de la siguiente manera:\
   **IRC del proyecto** = *IF* Horas reales > 0 *THEN* IRC = CosteTotalPresupuestadoTrabajoRealizado/Horas reales\
       *ELSE* IRC = 1\
   **IRC del proyecto** = 10 / 75\
   **IRC del proyecto** = 0,13

1. **EAC del proyecto** = 225 horas calculado de la siguiente manera:\
   **EAC para el proyecto** = *IF* CPI &lt;> 0 *THEN* EAC = CPI/Horas planificadas\
       *ELSE* EAC = Horas planificadas + Horas reales\
   **EAC para el proyecto** = 30/0,13333\
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

1. Asigne las Tareas 2, 4, 5 y 6 al Usuario 1, cuya tarifa de coste/hora es de 100,00 $.
1. Añada horas planificadas/reales a cada tarea y % completado según la tabla siguiente.

   >[!NOTE]
   >
   >Para las Tareas 1 y 3, solo añade horas reales.

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
   <td> <p>20 %</p> </td> 
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
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Añada 50 horas directamente al proyecto (Más>Horas>Registrar horas).
1. **CPI para la Tarea 2** = 0,1 calculado de la siguiente manera:\
   **CPI para la Tarea 2** = *IF* Horas reales > 0 *THEN* CPI = CosteTotalPresupuestadoTrabajoRealizado/Horas reales\
   *ELSE* IRC = 1\
   **CPI para Tarea 2** = 1 / 10\
   **IRC para la tarea 2** = 0,1

1. **EAC para la Tarea 2** = 50 horas calculadas de la siguiente manera:\
   **EAC para la Tarea 2** = *IF* CPI &lt;> 0 *THEN* EAC = CPI/Horas planificadas\
       *ELSE* EAC = Horas planificadas + Horas reales\
   **IRC para la tarea 2** = 5 / 0,1\
   **EAC para la Tarea 2** = 50 horas

1. El CPI/EAC para las Tareas 4, 5 y 6 es el siguiente:\
   Tarea 4: 0,4/25 horas\
   Tarea 5: 0,75/20 horas\
   Tarea 6: 1,2/16,67 horas

1. **CPI para la Tarea 3** = 0,38 calculado de la siguiente manera:\
   **CPI para la Tarea 3** = *IF* Horas reales > 0 *THEN* CPI = CosteTotalPresupuestadoTrabajoRealizado/Horas reales\
       *ELSE* CPI = 1\
   **IRC para la tarea 3** = 11,5 / 30\
   **CPI para la Tarea 3** = 0,38

1. **EAC para la Tarea 3** = 65,22 horas calculadas de la siguiente manera:\
   **EAC para la Tarea 3** = *IF* CPI &lt;> 0 *THEN* EAC = Horas planificadas/CPI\
       *ELSE* EAC = Horas planificadas + Horas reales\
   **EAC para la Tarea 3** =  25/0,383333\
   **EAC para la Tarea 3** = 65,22 horas

1. **CPI para la Tarea 1** = 0,25 calculado de la siguiente manera:\
   **CPI para la Tarea 1** = *IF* Horas reales > 0 *THEN* CPI = CosteTotalPresupuestadoTrabajoRealizado/Horas reales\
       *ELSE* CPI = 1\
   **IRC para la tarea 1** = 12,5 / 50\
   **CPI para la Tarea 1** = 0,25

1. **EAC para la Tarea 1** = 120 horas calculadas de la siguiente manera:\
   **EAC para la Tarea 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas planificadas/CPI\
       *ELSE* EAC = Horas planificadas + Horas reales\
   **EAC para la Tarea 1** = 30/0,25\
   **EAC para la Tarea 1** = 120 horas

1. **CPI para el Proyecto** = 0,22 calculado de la siguiente manera:\
   **CPI para el proyecto** = *IF* Horas reales > 0 *THEN* CPI = CosteTotalPresupuestadoTrabajoRealizado/Horas reales\
       *ELSE* CPI = 1\
   **IRC para el proyecto** = 24,5 / 110\
   **IRC para el proyecto** = 0,22272\
   **CPI para el Proyecto** = 0,22

1. **EAC para el Proyecto** = 224,49 horas calculadas de la siguiente manera:\
   **EAC para el proyecto** = *IF* CPI &lt;> 0 *THEN* EAC = CPI/Horas planificadas\
       *ELSE* EAC = Horas planificadas + Horas reales\
   **EAC para el Proyecto** = 50/0,22272\
   **EAC para el Proyecto** = 224,49 horas

### PIM = basado en costes {#pim-cost-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: un proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks-1}

PIM = basado en costes

Método EAC = Calcular a nivel de proyecto

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo coste/hora sea de 100,00 USD.
1. Añadir horas planificadas/horas reales a cada tarea y el % completado según la tabla siguiente:

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
   <th> <br> <p><strong>Coste plan man obr</strong> </p> </th> 
   <th> <br> <p><strong>Hs reales</strong> </p> </th> 
   <th> <br> <p><strong>Coste plan man obr real</strong> </p> </th> 
   <th> <p><strong>% finalizado</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>2500,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>2500,00 $</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>1500,00 $</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>2500,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Añada gastos a cada tarea según la tabla siguiente:

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
   <td> <p>Tarea 1 Exp 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>Tarea 2 Cad</p> </td> 
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

1. Añada dos gastos al proyecto (es decir, no vinculados a una tarea) de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>‘<strong>Gasto</strong> </p> </th> 
   <th> <p><strong>Importe planificado</strong> </p> </th> 
   <th> <p><strong>Importe real</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Proyecto Cad 1</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>1500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1 Exp 2</p> </td> 
   <td> <p>2500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>500,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>3000,00 $</p> </td> 
   <td> <p>2300,00 $</p> </td> 
   <td> <p> 2700,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. En Acciones de proyecto, ejecute Recalcular finanzas
1. **CPI de la tarea 1** = 0,14
1. **CPI**** de la tarea 1** = 0,14 calculado de la siguiente manera:\
   **CPI**  **de la tarea 1** = *IF* Coste real de la mano de obra + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI**** de la tarea 1** = (100+300) / (2500+400)\
   **CPI**  **de la tarea 1** = 400 / 2900\
   **CPI**  **de la tarea 1** = 0,14****

1. **EAC**** de la tarea 1** = 13.400,00 $\
   **Mano de obra CPI**  **de la tarea 1** = IF Coste real de la mano de obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mano de obra CPI**  **de la tarea 1** = 100/2500\
   **Mano de obra CPI**  **de la tarea 1** = 0,04 ****** Mano de obra EAC ****de la tarea 1 **=*IF *CPI_Labor &lt;> 0*THEN *Mano de obra EAC = Coste planificado de mano de obra/CPI_Labor\
   *    ELSE* EAC  Mano de obra = coste planificado de mano de obra + coste real de la mano de obra\
   **Mano de obra EAC ****de la tarea 1** = 500,00/0,04\
   **Mano de obra EAC**** de la tarea 1** = 12.500,00 $\
   **Gasto EAC****de la tarea 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto EAC****de la tarea 1** = 400,00 $ + 500,00 $\
   **Gasto EAC****de la tarea 1** = 900,00 $\
   **EAC****de la tarea 1** = mano de obra EAC + gasto EAC\
   **EAC****de la tarea 1**  = 12 500,00 $ + 900,00 $\
   **EAC****de la tarea 1**  = 13 400,00 $

1. Estos son los valores CPI / EAC para la tarea 2 y la tarea 3:\
   Tarea 2 = 0,19 / 8.433,33 $\
   Tarea 3 = 0,44 / 6.950,00 $

1. **CPI del proyecto** = 0,32 calculado de la siguiente manera:\
   **CPI****para el proyecto** = *IF* Coste real de la mano de obra + CosteGastoRealIncurrido &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IRC = CPI_Labor\
   **IRC****del proyecto** = (1000 + 2300) / (7500 + 2700)\
   **IRC****del proyecto** = 3300 / 10200\
   **CPI****para el proyecto** = .32

1. **EAC para el proyecto** = 28 200 00 USD calculado de la siguiente manera:\
   **Trabajo de CPI****para el proyecto** = IF Coste real de la mano de obra &lt;> 0 THEN

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

   *   ELSE* Trabajo EAC = Coste planificado de mano de obra + Coste real de mano de obra\
   **Trabajo EAC****para el proyecto** = 3000/.13333\
   **Trabajo EAC****para el proyecto** = 22 500 00 USD

   **EAC gasto****Proyecto** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Proyecto****Gasto EAC** = 3000 00 USD + 2 700 USD\
   **Proyecto****Gasto EAC** = 5 700 00 USD

   **EAC****Proyecto** = Mano de obra EAC + Gasto EAC\
   **EAC****Proyecto**  = 22 500 00 $ + 5 700 00 USD\
   **EAC****Proyecto**  = 28 200 00 USD

#### Ejemplo complicado: un proyecto tiene tareas secundarias {#complicated-example-project-has-children-tasks-1}

PIM = basado en costes

Método EAC = Calcular a nivel de proyecto

1. Cree el proyecto A con seis tareas en las que la Tarea 3 sea la principal de las Tareas 4 y 5 y la Tarea 1 sea la principal de las Tareas 2 y 3, como se muestra a continuación:\
   Tarea 1\
      Tarea 2\
      Tarea 3\
         Tarea 4\
         Tarea 5\
   Tarea 6

1. Asigne las Tareas 2, 4, 5 y 6 al Usuario 1, cuya tarifa de coste/hora es de 100,00 $.
1. Añada horas planificadas/reales a cada tarea y % completado según la tabla siguiente.

   >[!NOTE]
   >
   >Para las Tareas 1 y 3, solo añade horas reales.

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
   <th> <br> <p><strong>Coste plan man obr</strong> </p> </th> 
   <th> <br> <p><strong>Hs reales</strong> </p> </th> 
   <th> <br> <p><strong>Coste plan man obr real</strong> </p> </th> 
   <th> <p><strong>% finalizado</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 2</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>1500,00 $</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>2.000,00 $</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Añada 50 horas directamente al proyecto (Más>Horas>Registrar horas) para que haya 5000.00 $ de coste real de la mano de obra registrada directamente en el proyecto. ****
1. Añada gastos a cada tarea según la tabla siguiente (he añadido una fila en blanco entre cada tarea para facilitar la lectura):

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
   <td> <p>Tarea 1 Exp 2</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1</p> </td> 
   <td> <p>Tarea 1 Cad 3</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>0,00 $</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
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
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>Tarea 6 Cad 1</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>Tarea 6 Cad 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>- 300,0 $</p> </td> 
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
   <th> <p>‘<strong>Gasto</strong> </p> </th> 
   <th> <p><strong>Importe planificado</strong> </p> </th> 
   <th> <p><strong>Importe real</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Proyecto Cad 1</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>1500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 1 Exp 2</p> </td> 
   <td> <p>2500,00 $</p> </td> 
   <td> <p> 0,00 $ <strong></strong></p> </td> 
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
   <td> <p>0,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 5</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarea 6</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Proyecto</p> </td> 
   <td> <p>2500,00 $</p> </td> 
   <td> <p>1000,00 $</p> </td> 
   <td> <p>1500,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. En Acciones de proyecto, ejecute Recalcular finanzas
1. **IRC** para la tarea 2 = 0,17 calculado de la siguiente manera:\
   **Tarea IRC 2** = *IF* Coste real de la mano de obra + IncurredActualExpenseCost  &lt;> 0 *THEN* IRC = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)\
   *   ELSE* IRC = CPI_Labor\
   **IRC****Tarea 2** = (100+300) / (1000+1300)\
   **IRC****Tarea 2**  = 400 / 2300\
   **IRC****Tarea 2**  = 0,17

1. **EAC** para la tarea 2 = 5900,00 $\
   **Trabajo IRC****Tarea 2** = IF Coste real de la mano de obra &lt;> 0 THEN CPI_Labor = CostePresupuestadoTotalTrabajoRealizado / Coste real de la mano de obra\
      ELSE CPI_Labor = 1\
   **Trabajo IRC****Tarea 2** = 100/1000\
   **Trabajo IRC****Tarea 2** = 0,1

   **Trabajo EAC****Tarea 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Trabajo = Coste planificado de mano de obra + Coste real de la mano de obra\
   **Trabajo EAC****Tarea 2** = 500,00/0,1\
   **Trabajo EAC****Tarea 2** = 5000,00 $****** Gasto EAC ****Tarea 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto EAC ****Tarea 2** = 1300,00 $ + -400,00 $\
   **Gasto EAC****Tarea 2** = 900,00 $

   **EAC****Tarea 2** = Trabajo EAC + Gasto EAC\
   **EAC****Tarea 2**  = 5000,00 $ + 900,00 $\
   **EAC****Tarea 2**  = 5900,00 $

1. El IRC/EAC de las tareas 4, 5 y 6 se determina de la misma manera, así que proporcionaré los siguientes valores:\
   Tarea 4: 0,23 / 3400,00 $\
   Tarea 5: 0,64 / 3100,00 $\
   Tarea 6: 1,06 / 2366,67 $

1. IRC para la tarea 3 = 0,31 calculado de la siguiente manera:\
   **IRC****Tarea 3** = *IF* Coste real de la mano de obra + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IRC = CPI_Labor\
   **IRC****Tarea 3**  = (1150 + 500) / (3000 + 2400)\
   **IRC****Tarea 3**  =  1650 / 5400\
   **IRC****Tarea 3**  = 0,31 ****** EAC para la tarea 3 **= 9521,74 $ calculado de la siguiente manera:\
   **Trabajo IRC ****Tarea 3** = IF Coste real de la mano de obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Trabajo IRC****Tarea 3** = 1150/3000\
   **Trabajo IRC****Tarea 3** = 0,383333\
   **Trabajo IRC****Tarea 3** = 0,38

   **Trabajo EAC****Tarea 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Trabajo EAC = Coste planificado de mano de obra + Coste real de mano de obra\
   **Trabajo EAC****Tarea 3** = 2500,00 $ / 0,383333\
   **Mano de obra de EAC****Tarea 3** = 6521,74 $

   **Gasto de EAC****Tarea 3** = CosteGastoRealIncurrido + GastoPrevistoNoIncurrido\
   **Gasto de EAC****Tarea 3** = 2400,00 $ + 600,00 $\
   **Gasto de EAC****Tarea 3** = 3000,00 $

   **EAC****Tarea 3** = Mano de obra de EAC + Gasto de EAC\
   **EAC****Tarea 3**  = 6521,74 $ + 3000,00 $\
   **EAC****Tarea 3**  = 9521,74 $

1. CPI para la Tarea 1 = 0,16 calculado de la siguiente manera:\
   **CPI****Tarea 1** = *IF* Coste real de la mano de obra + CosteGastoRealIncurrido &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Mano de obra\
   **IRC****Tarea 1**  = (1250 + 300) / (5000 + 4500)\
   **IRC****Tarea 1**  =  1550/9500=\
   **IRC****Tarea 1** = 0,16

1. El valor de EAC para la Tarea 1 es de 17 100,00 $, calculado de la siguiente manera:\
   **Mano de obra de CPI***Tarea 1** = IF Coste real de la mano de obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mano de obra de CPI****Tarea 1** = 1250/5000\
   **Mano de obra de CPI****Tarea 1** = 0,25

   **Mano de obra de EAC****Tarea 1** = *IF* CPI_Mano de obra &lt;> 0 *THEN* Mano de obra de EAC = Coste planificado de mano de obra / CPI_Mano de obra\
   *   ELSE* Mano de obra de EAC = Coste planificado de mano de obra + Coste real de la mano de obra\
   **Mano de obra de EAC****Tarea 1** = 3000,00/0,25\
   **Mano de obra de EAC****Tarea 1** = 12 000,00 $

   **Gasto de EAC****Tarea 1** = CosteGastoRealIncurrido + GastoPrevistoNoIncurrido\
   **Gasto de EAC****Tarea 1** = 4500 $ + 600\
   **Gasto de EAC****Tarea 1** = 5100,00 $

   **EAC****Tarea 1** = Mano de obra de EAC + Gasto de EAC\
   **EAC****Tarea 1** = 12 000,00 $ + 5100,00\
   **EAC****Tarea 1** = 17 100,00 $

1. El CPI para el proyecto es de 0,25\
   **CPI****para el proyecto** = *IF* Coste real de la mano de obra + CosteGastoRealIncurrido &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Mano de obra

   **CPI****para el proyecto** = (2450 + 1900) / (11 000 + 6700)\
   **CPI****para el proyecto** =   4350/17 700\
   **CPI****para el proyecto** = 0,25

1. **EAC para el proyecto** = 32 248,98 $ calculado de la siguiente manera:\
   **Mano de obra de CPI****para el proyecto** = IF Coste real de la mano de obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mano de obra de CPI****para el proyecto** = 2450/11 000\
   **Mano de obra de CPI****para el proyecto** = 0,22272\
   **Mano de obra de CPI****para el proyecto** = 0,22

   **Mano de obra de EAC****para el proyecto** = *IF* CPI_Mano de obra &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Mano de obra de EAC = Coste planificado de mano de obra + Coste real de la mano de obra\
   **Mano de obra de EAC****para el proyecto** = 5000,00 $ / 0,22272\
   **Mano de obra de EAC****para el proyecto** = 22 448,97959 $\
   **Mano de obra de EAC****para el proyecto** = 22 448,98 $

   **Gasto de EAC****Proyecto** = CosteGastoRealIncurrido + GastoPrevistoNoIncurrido\
   **Gasto de EAC****Proyecto** = 3100,00 $ + 6700,00 $\
   **Gasto de EAC****Proyecto** = 9800,00 $

   **EAC****Proyecto** = Mano de obra de EAC + Gasto de EAC\
   **EAC****Proyecto**  = 22 448,98 $ + 9800,00\
   **EAC****Proyecto** = 32.248,98$
