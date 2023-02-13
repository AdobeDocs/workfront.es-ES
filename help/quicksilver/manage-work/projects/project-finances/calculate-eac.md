---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular estimación al finalizar (CAO)
description: Como métrica de rendimiento, la estimación al finalizar (EAC) representa el coste total proyectado de su proyecto o tarea cuando se completa.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Calcular estimación al finalizar (CAO)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Como métrica de rendimiento, la estimación al finalizar (EAC) representa el coste total proyectado de su proyecto o tarea cuando se completa.

Como ajuste, le permite definir cómo se debe calcular el valor de EAC. 

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
   <td> <p>Ver acceso a Proyectos y Datos Financieros</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores del proyecto con permisos para Ver finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Defina cómo calcular EAC

Como parte de las preferencias del sistema del proyecto, el administrador de Adobe Workfront puede definir cómo calcular la CAO. EAC se puede calcular de una de las dos maneras siguientes:

* [Calcular en el nivel de proyecto](#calculate-at-the-project-level)
* [Resumen de tareas y subtareas](#roll-up-from-tasks-and-subtasks)

Para obtener más información sobre la configuración de preferencias de proyecto en Workfront, incluido cómo calcular la estimación al completarse, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Como administrador de proyectos, también puede cambiar esta preferencia en el nivel de proyecto, en la subpestaña Finanzas del proyecto. Para obtener más información sobre la edición de la subpestaña Finanzas de un proyecto, consulte [Administrar información en el área de finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calcular en el nivel de proyecto {#calculate-at-the-project-level}

Las CAO para la tarea principal y el proyecto se determinan introduciendo las horas/coste laboral real en las Fórmulas de CAO. Este cálculo incluye horas/costes reales y gastos añadidos directamente a la tarea o proyecto principal.

### Resumen de tareas y subtareas {#roll-up-from-tasks-and-subtasks}

Las CAO para la tarea principal y el proyecto se determinan sumando la CAO para cada tarea secundaria. Este cálculo excluye las horas/costes reales y los gastos añadidos directamente a la tarea o proyecto principal.

## Cálculo de EAC en función del método de índice de rendimiento (PIM)

En Workfront, el cálculo de EAC depende del método de índice de rendimiento (PIM) seleccionado en el proyecto. Para obtener más información sobre cómo configurar el PIM para su sistema o para su proyecto, consulte [Definir el método del índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcular EAC mediante PIM basado en horas](#calculate-eac-using-hour-based-pim)
* [Calcular EAC mediante PIM basado en costes](#calculate-eac-using-cost-based-pim)

### Calcular EAC mediante PIM basado en horas {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Si el índice de rendimiento de los costes [Calcular el índice de rendimiento de costes (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total de horas planificadas + Hora real. Esto ocurre cuando se han capturado horas, pero el proyecto/tarea se ha completado al 0%.

Para obtener más información sobre el cálculo de CPI, consulte [Calcular el índice de rendimiento de costes (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcular EAC mediante PIM basado en costes {#calculate-eac-using-cost-based-pim}

La CAO de un proyecto se calcula mediante la fórmula siguiente:

```
EAC = EAC Labor + EAC Expense 
```

<pre>Trabajo EAC =  <em>IF</em> CPI Labor &lt;&gt; 0 ENTONCES Trabajo EAC = Costo laboral planificado / Trabajo CPI</pre><pre><em>ELSE</em> Trabajo de la CAO = costo laboral previsto + costo laboral real</pre><pre>CPI Labor = SI Costo real de la mano de obra &lt;&gt; 0 ENTONCES Trabajo CPI = TotalBudgetedCostWorkPerformance / Coste real de la mano de obra</pre><pre>ELSE CPI Labor = 1 </pre>Los campos siguientes se tienen en cuenta al calcular la CAO:

* Total Budgeted Cost Work Performance (BCWP) = El resultado de multiplicar el coste presupuestado del trabajo planificado (costo presupuestado) y el porcentaje de la tarea que se ha completado hasta ahora.

   Para obtener información sobre el trabajo de costo presupuestado total realizado (CPTR), consulte [Calcular el trabajo de coste presupuestado realizado (CPTR)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Para una tarea no principal:**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **Para una tarea principal:**
Total de trabajo de coste presupuestado realizado = la suma del campo Total de trabajo de coste presupuestado realizado para todas las tareas secundarias directas.

   * **Para un proyecto:**
Total de trabajo de coste presupuestado realizado = la suma del campo Total de trabajo de coste presupuestado realizado para todas las tareas de nivel superior (principales y tareas independientes). 

* Gastos EAC = el resultado de agregar el Coste Real Incurrido al Coste de Gastos Planeado No Incurrido. Se calcula mediante la fórmula siguiente:

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * Coste real incurrido = La suma del campo Importe planeado para todos los gastos donde el campo Importe real > 0. Por ejemplo, si crea un gasto para la Tarea 1 e introduce 500,00 $ en el campo Importe planificado y un importe > 0 en el campo Importe real (es decir, 600,00 $), el costo planeado incurrido para esta tarea es de 500,00 $.
   * Gastos planificados no incurridos = La suma del campo Importe planeado para todos los gastos donde el campo Importe real = 0. Por ejemplo, si crea dos gastos para la Tarea 1 donde, para el primer gasto, el valor en el campo Importe planificado es de 500,00 $ y el valor en el Importe real es de 600,00 $ y para el segundo gasto, el valor en el campo Importe planificado es de 300,00 $ y el valor del campo Importe real es de 0,00 $, el valor del valor del campo No Importe el gasto planificado currido para esta tarea es de 300,00 $. 

## Localización de la CAO en un proyecto o una tarea

1. Vaya al proyecto o la tarea donde desea ver el EAC.
1. Expandir **Detalles del proyecto** o **Detalles de tareas** en el panel izquierdo del proyecto o la tarea, en función de dónde vea la EAC.

1. Haga clic en **Finanzas**. 

   El valor de EAC se muestra en la variable **Estimación al finalizar** campo .

   ![](assets/eac-highlighted-on-project-350x112.png)
