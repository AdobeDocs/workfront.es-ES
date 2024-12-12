---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular estimación al finalizar (EAC)
description: Como métrica de rendimiento, Estimar al finalizar (EAC) representa el coste total proyectado del proyecto o la tarea cuando finaliza.
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 100%

---

# Calcular estimación al finalizar (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Como métrica de rendimiento, Estimar al finalizar (EAC) representa el coste total proyectado del proyecto o la tarea cuando finaliza.

Como configuración, le permite definir cómo se debe calcular el valor EAC. 

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: Light o superior</p>
   <p>o</p>
   <p>Actual: revisión o superior</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Ver el acceso a proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Permisos de visualización o superiores al proyecto con permisos para Ver finanzas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Defina cómo calcular el valor EAC

Como parte de las preferencias del sistema del proyecto, el administrador de Adobe Workfront puede definir cómo calcular el valor EAC. EAC se puede calcular de una de las dos maneras siguientes:

* [Calcular en el nivel de proyecto](#calculate-at-the-project-level)
* [Resumir a partir de tareas y subtareas](#roll-up-from-tasks-and-subtasks)

Para obtener más información sobre cómo configurar las preferencias del proyecto en Workfront, incluido cómo calcular el valor Estimar al finalizar, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Como jefe de proyecto, también puede cambiar esta preferencia en el nivel de proyecto, en la subpestaña Finanzas del proyecto. Para obtener más información sobre cómo editar la subpestaña Finanzas de un proyecto, consulte [Administrar información en el área Finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calcular en el nivel de proyecto {#calculate-at-the-project-level}

El valor de EAC para la tarea principal y el proyecto se determina introduciendo las horas reales/coste real de la mano de obra en las fórmulas de EAC. El cálculo incluye las horas/costes reales y los gastos añadidos directamente a la tarea o proyecto principal.

### Resumir a partir de tareas y subtareas {#roll-up-from-tasks-and-subtasks}

El valor EAC para la tarea principal y el proyecto se determinan sumando el valor EAC de cada tarea secundaria. El cálculo excluye las horas/costes reales y los gastos añadidos directamente a la tarea o proyecto principal.

## Cómo calcular el valor EAC en función del método de índice de rendimiento (PIM)

En Workfront, el cálculo de EAC depende del Método de índice de rendimiento (PIM) seleccionado del proyecto. Para obtener más información sobre cómo configurar el PIM para el sistema o para el proyecto, consulte [Establecer el método de índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcular EAC usando el PIM basado en horas](#calculate-eac-using-hour-based-pim)
* [Calcular EAC usando el PIM basado en costes](#calculate-eac-using-cost-based-pim)

### Calcular EAC usando el PIM basado en horas {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Si el índice de rendimiento de costos [Calcular índice de rendimiento de costos (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total de horas planificadas + horas reales. Esto ocurre cuando se han capturado horas, pero el proyecto/tarea está al 0% completado.

Para obtener más información acerca del cálculo del CPI, consulte [Calcular el índice de rendimiento de costos (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcular EAC usando el PIM basado en costes {#calculate-eac-using-cost-based-pim}

El valor EAC de un proyecto se calcula mediante la siguiente fórmula:

```
EAC = EAC Labor + EAC Expense 
```

<pre>Mano de obra de EAC =  <em>IF</em> Mano de obra de CPI &lt;&gt; 0 THEN Mano de obra de EAC = Coste planificado de mano de obra / mano de obra de CPI</pre><pre><em>ELSE</em> Mano de obra de EAC  = Coste planificado de mano de obra + Coste real de la mano de obra</pre><pre>Mano de obra de CPI = IF Coste real de la mano de obra &lt;&gt; 0 THEN Mano de obra de CPI = TotalBudgetedCostWorkPerformed / Coste real de la mano de obra</pre><pre>ELSE Mano de obra de CPI = 1 </pre>Los campos siguientes se tienen en cuenta al calcular el valor EAC:

* Coste presupuestado total de trabajo realizado (CPTR) = Resultado de multiplicar el coste presupuestado del trabajo planificado (coste presupuestado) y el porcentaje de la tarea que se ha completado hasta el momento.

  Para obtener información sobre el coste presupuestado total de trabajo realizado (CPTR), consulte [Calcular el coste presupuestado total de trabajo realizado (CPTR)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Para una tarea que no es principal:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Para una tarea principal:**
Coste presupuestado total de trabajo realizado = la suma del campo Coste presupuestado total de trabajo realizado para todas las tareas secundarias directas.

   * **Para un proyecto:**
Coste presupuestado total de trabajo realizado = la suma del campo Coste presupuestado total de trabajo realizado para todas las tareas de nivel superior (tareas principales y autónomas). 

* Gasto EAC = el resultado de añadir el coste real de gastos incurridos al coste planificado de gastos no incurridos. Se calcula mediante la fórmula siguiente:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Coste real de gastos incurridos = la suma del campo Importe planificado para todos los gastos donde el campo Importe real es > 0. Por ejemplo, si crea un gasto para la Tarea 1 y especifica 500,00 USD en el campo Importe planificado y un importe > 0 en el campo Importe real (es decir, 600,00 USD), el coste planificado de gastos incurridos para esta tarea es de 500,00 USD.
   * Gasto planificado no incurrido = la suma del campo Importe planificado para todos los gastos donde el campo Importe real es = 0. Por ejemplo, si crea dos gastos para la Tarea 1 en los que para el primer gasto el valor del campo Importe planificado es de 500,00 USD y el valor del Importe real es de 600,00 USD, y para el segundo gasto el valor del campo Importe planificado es de 300,00 USD y el valor del campo Importe real es de 0,00 USD, el valor del gasto planificado no incurrido para esta tarea es de 300,00 USD. 

## Localizar el EAC en un proyecto o una tarea

1. Vaya al proyecto o tarea donde desee ver el EAC.
1. Expanda **Detalles del proyecto** o **Detalles de tareas** en el panel izquierdo del proyecto o la tarea, según el lugar donde vea el EAC.

1. Haga clic en **Finanzas**. 

   El valor EAC se muestra en el campo **Estimar al finalizar**.

   ![](assets/eac-highlighted-on-project-350x112.png)
