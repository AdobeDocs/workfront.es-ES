---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Ejemplo de cálculo: Calcular EAC como resumen a partir de tareas'
description: Este artículo proporciona un ejemplo de cálculo de la estimación al finalizar (EAC) de un proyecto como resumen de todas las tareas del proyecto en Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 88%

---

# Ejemplo de cálculo: calcular EAC como resumen a partir de tareas

## Método EAC: resumen a partir de tareas o subtareas

* [PIM= basado en horas](#pim-hour-based)
* [PIM = basado en costes](#pim-cost-based)

### PIM= basado en horas {#pim-hour-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)
* [Ejemplo complicado: un proyecto tiene tareas secundarias](#complicated-example-project-has-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks}

PIM = Basado en horas

Método EAC: resumen a partir de tareas/subtareas

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo coste/hora sea de 100,00 USD.
1. Añadir horas planificadas/horas reales a cada tarea y el % completado según la tabla siguiente:

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
   <td> <p>5 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>20 %</p> </td> 
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
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalcular finanzas
1. **IRC de la tarea 1** = 0,04 calculado de la siguiente manera:\
   **IRC de la tarea 1** = *IF* Horas reales > 0 *THEN* IRC = CosteTotalPresupuestadoTrabajoRealizado/Horas reales\
   *ELSE* IRC = 1\
   **IRC de la tarea 1** = 1 / 25\
   **IRC de la tarea 1** = 0,04

1. **EAC de la tarea 1** = 125 horas calculadas de la siguiente manera:\
   **EAC de la tarea 1** = *IF* IRC &lt;> 0 *THEN* EAC = Horas planificadas/IRC\
   *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC para la tarea 1** = 5 / 0,04\
   **EAC para la tarea 1** = 125 horas

1. Los IRC y EAC de las tareas 2 y 3 son los siguientes:\
   Tarea 2 = 0,12 / 83,33 horas\
   Tarea 3 = 0,24 / 62,5 horas

1. **IRC del proyecto** = 0,13 calculado de la siguiente manera:\
   **IRC del proyecto** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* IRC = 1\
   **IRC del proyecto** = 10 / 75\
   **IRC del proyecto** = 0,13

1. **EAC del proyecto** = 270,83 horas calculadas de la siguiente manera:\
   **EAC para el proyecto** = EAC Tarea 1 + EAC Tarea 2 + EAC Tarea 3\
   **EAC para el proyecto** = 125 + 83,33 + 62,5\
   **EAC para el proyecto** = 270,83 horas

#### Ejemplo complicado: un proyecto tiene tareas secundarias {#complicated-example-project-has-children-tasks}

PIM = Basado en horas

Método EAC: resumen a partir de tareas/subtareas

1. Cree el proyecto A con seis tareas en las que la Tarea 3 sea la principal de las Tareas 4 y 5 y la Tarea 1 sea la principal de las Tareas 2 y 3, como se muestra a continuación:

   ```
   Task 1  
      Task 2  
      Task 3  
         Task 4  
         Task 5  
   Task 6
   ```

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
      <td> </td> 
      <td> <p>10 horas</p> </td> 
      <td> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarea 2</p> </td> 
      <td> <p>5 horas</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>20 %</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarea 3</p> </td> 
      <td> </td> 
      <td> <p>10 horas</p> </td> 
      <td> </td> 
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

1. Añada 50 horas directamente al proyecto (Más>Horas>Registrar horas) para que haya 5000.00 $ de coste real de la mano de obra registrada directamente en el proyecto.
1. Ejecute Recalcular finanzas.
1. **CPI para la tarea 2** = 0,1, calculado de la siguiente manera:\
   **CPI para la tarea 2** = *SI* Horas reales > 0 *ENTONCES*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* IRC = 1\
   **CPI para Tarea 2** = 1 / 10\
   **IRC para la tarea 2** = 0,1

1. **CAE para la tarea 2** = 50 horas calculadas de la siguiente manera:\
   **EAC para la tarea 2** = *IF* IRC &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

   *ELSE* EAC = Horas planificadas + Horas reales\
   **IRC para la tarea 2** = 5 / 0,1\
   **IRC para la tarea 2** = 50 horas

1. IRC/EAC para la tarea 4, tarea 5 y tarea 6:\
   Tarea 4 = 0,4 / 25 horas\
   Tarea 5 = 0,75 / 20 horas\
   Tarea 6 = 1,2 / 16,67 horas

1. **IRC para la tarea 3** = 0,38\
   **IRC para la tarea 3** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* IRC = 1\
   **IRC para la tarea 3** = 11,5 / 30\
   **IRC para la tarea 3** = 0,38

1. **EAC para la tarea 3** = EAC 4 tarea + EAC tarea 5\
   **EAC para la tarea 3** = 25 + 20\
   **EAC para la tarea 3** = 45 horas

1. **IRC para la tarea 1** = 0,25 calculado de la siguiente manera:\
   **IRC para la tarea 1** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* IRC = 1\
   **IRC para la tarea 1** = 12,5 / 50\
   **IRC para la tarea 1** = 0,25

1. **EAC para la tarea 1** = EAC tarea 2 + EAC tarea 3\
   **EAC para la tarea 1** = 50 + 45\
   **EAC para la tarea 1** = 95 horas

1. IRC para el proyecto = 0,22 calculado de la siguiente manera:\
   **IRC para el proyecto** = *IF* Horas reales > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* IRC = 1\
   **IRC para el proyecto** = 24,5 / 110\
   **IRC para el proyecto** = 0,22272\
   **IRC para el proyecto** = 0,22

1. **EAC para el proyecto** = EAC tarea 1 + EAC tarea 6\
   **EAC para el proyecto** = 95 + 16,67\
   **EAC para el proyecto** = 111,67 horas

### PIM = basado en costes {#pim-cost-based}

* [Ejemplo sencillo: el proyecto no tiene tareas secundarias](#simple-example-project-has-no-children-tasks)

#### Ejemplo sencillo: el proyecto no tiene tareas secundarias {#simple-example-project-has-no-children-tasks-1}

PIM = basado en costes

Método EAC: resumen a partir de tareas/subtareas

1. Cree el proyecto A con tres tareas (sin tareas secundarias) asignadas al usuario 1 cuyo coste/ hora es de 100 00 USD.
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
      <td> <p>2700,00 $</p> </td> 
   </tr> 
   </tbody> 
   </table>

1. En Acciones de proyecto, ejecute Recalcular finanzas
1. **IRC**** de la tarea 1** = 0,14 calculado de la siguiente manera:\
   **CPI****para la tarea 1** = *IF* Costo de mano de obra real + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* IPC = CPI_Labor\
     **IRC****para Tarea 1** = (100+300) / (2500+400)\
     **IRC****para Tarea 1** = 400 / 2900\
     **IRC****para la tarea 1** = 0,14

1. **EAC****de la tarea 1** = 13 400,00 $\
   **Mano de obra de IRC***de la tarea 1** = IF Coste real de la mano de obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mano de obra de IRC***de la tarea 1** = 100/2500\
   **Mano de obra de IRC***de la tarea 1** = 0,04

   **Mano de obra de EAC****de la tarea 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* EAC Mano de Obra = Coste Laboral Planificado + Coste Laboral Real\
     **Mano de obra EAC**** de la tarea 1** = 500,00/0,04\
     **Mano de obra EAC**** de la tarea 1** = 12 500,00 $

   **Gasto EAC****de la tarea 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Gasto EAC****de la tarea 1** = 400,00 $ + 500,00 $\
   **Gasto EAC****de la tarea 1** = 900,00 $

   **EAC****de la tarea 1** = mano de obra EAC + gasto EAC\
   **EAC****para la tarea 1** = 12.500,00 $ + 900,00 $\
   **EAC****para la tarea 1** = 13.400,00 $

1. Estos son los valores CPI / EAC para la tarea 2 y la tarea 3:\
   Tarea 2 = 0,19 / 8.433,33 $\
   Tarea 3 = 0,44 / 6 950,00 $****

1. IRC del proyecto = 0,32\
   **CPI****para el proyecto** = *IF* Costo de mano de obra real + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* IPC = CPI_Labor\
     **IRC****del proyecto** = (1000 + 2300) / (7500 + 2700)\
     **IRC****del proyecto** = 3300 / 10200\
     **IRC****del proyecto** = 0,32

1. El EAC del proyecto es 28 783.33 $\
   **EAC****del proyecto** = EAC Tarea 1 + EAC Tarea 2 + EAC Tarea 3\
   **EAC****del proyecto** = 13 400,00 $ + 8 433,33 $ + 6 950,00 $\
   **EAC****del proyecto** = 28 783,33 $
