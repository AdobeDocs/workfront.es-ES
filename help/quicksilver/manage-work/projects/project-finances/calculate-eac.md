---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular estimación al finalizar (EAC)
description: Como métrica de rendimiento, Estimar al finalizar (EAC) representa el costo total proyectado del proyecto o tarea cuando finaliza.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Calcular estimación al finalizar (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Como métrica de rendimiento, Estimar al finalizar (EAC) representa el costo total proyectado del proyecto o tarea cuando finaliza.

Como configuración, le permite definir cómo se debe calcular el valor EAC. 

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
   <td> <p>Ver acceso a proyectos y datos financieros</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores al proyecto con permisos para Ver finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Defina cómo calcular EAC

Como parte de las preferencias del sistema del proyecto, el administrador de Adobe Workfront puede definir cómo calcular el EAC. EAC se puede calcular de una de las dos maneras siguientes:

* [Calcular en el nivel de proyecto](#calculate-at-the-project-level)
* [Resumir a partir de tareas y subtareas](#roll-up-from-tasks-and-subtasks)

Para obtener más información acerca de cómo configurar las preferencias del proyecto en Workfront, incluido cómo calcular la estimación al finalizar, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Como jefe de proyecto, también puede cambiar esta preferencia en el nivel de proyecto, en la subpestaña Finance del proyecto. Para obtener más información sobre cómo editar la subpestaña Finanzas de un proyecto, consulte [Administrar información en el área Finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calcular a nivel de proyecto {#calculate-at-the-project-level}

El valor de EAC para la tarea y el proyecto principales se determina introduciendo las horas reales/el coste laboral real en las fórmulas de EAC. Este cálculo incluye las horas, los costos y los gastos reales agregados directamente a la tarea o al proyecto principal.

### Resumir a partir de tareas y subtareas {#roll-up-from-tasks-and-subtasks}

EAC para la tarea principal y el proyecto se determinan sumando el EAC para cada tarea secundaria. Este cálculo excluye las horas, los costos y los gastos reales agregados directamente a la tarea o al proyecto principal.

## Cómo calcular EAC en función del método de índice de rendimiento (PIM)

En Workfront, el cálculo de EAC depende del Método de índice de rendimiento (PIM) seleccionado del proyecto. Para obtener más información acerca de cómo establecer el PIM para el sistema o para el proyecto, vea [Establecer el método de índice de rendimiento (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcular EAC usando PIM basado en horas](#calculate-eac-using-hour-based-pim)
* [Calcular EAC utilizando PIM basado en costes](#calculate-eac-using-cost-based-pim)

### Calcular EAC mediante PIM basado en horas {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Si el índice de rendimiento de costos [Calcula el índice de rendimiento de costos (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total de horas planificadas + Horas reales. Esto ocurre cuando se han capturado horas, pero el proyecto/tarea está al 0% completado.

Para obtener más información acerca del cálculo del CPI, vea [Calcular el índice de rendimiento de costos (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcular EAC utilizando PIM basado en costes {#calculate-eac-using-cost-based-pim}

El EAC de un proyecto se calcula mediante la siguiente fórmula:

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC Labor =  <em>IF</em> IPC Mano de obra &lt;&gt; 0 ENTONCES EAC Mano de obra = Costo laboral planificado / IPC Mano de obra</pre><pre><em>ELSE</em> EAC  Mano de Obra = Coste Laboral Planificado + Coste Laboral Real</pre><pre>IRC Mano de Obra = SI Coste Laboral Real &lt;&gt; 0 ENTONCES IRC Mano de Obra = TotalBudgetedCostWorkPerformed / Coste Laboral Real</pre><pre>IRC = Trabajo = 1 </pre>Los campos siguientes se tienen en cuenta al calcular el EAC:

* Trabajo presupuestado total realizado (CPTR) = Resultado de multiplicar el costo presupuestado del trabajo planeado (costo presupuestado) y el porcentaje de la tarea que se ha completado hasta el momento.

  Para obtener información sobre el trabajo de costo presupuestado total realizado (CPTR), vea [Calcular el trabajo de costo presupuestado realizado (CPTR)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Para una tarea que no es principal:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Para una tarea principal:**
Trabajo presupuestado total realizado = la suma del campo Trabajo presupuestado total realizado para todas las tareas secundarias directas.

   * **Para un proyecto:**
Trabajo presupuestado total realizado = la suma del campo Trabajo presupuestado total realizado para todas las tareas de nivel superior (tareas principales y autónomas). 

* Gasto EAC = el resultado de agregar el costo de gasto real incurrido al costo de gasto planificado no incurrido. Se calcula mediante la fórmula siguiente:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Costo de gasto real incurrido = La suma del campo Importe planificado para todos los gastos donde el campo Importe real > 0. Por ejemplo, si crea un gasto para la Tarea 1 y especifica 500,00 $ en el campo Importe planificado y un importe > 0 en el campo Importe real (es decir, 600,00 $), el costo de gasto planificado incurrido para esta tarea es 500,00 $.
   * Gasto planificado no incurrido = La suma del campo Importe planificado para todos los gastos donde el campo Importe real = 0. Por ejemplo, si crea dos gastos para la Tarea 1 en los que para el primer gasto el valor del campo Importe planificado es 500,00 $ y el valor del importe real es 600,00 $ y para el segundo gasto, el valor del campo Importe planificado es 300,00 $ y el valor del campo Importe real es 0,00 $, el valor del gasto planificado no incurrido de esta tarea es 300,00 $. 

## Busque el EAC en un proyecto o una tarea

1. Vaya al proyecto o tarea donde desee ver el EAC.
1. Expanda **Detalles del proyecto** o **Detalles de tareas** en el panel izquierdo del proyecto o tarea, según el lugar donde vea el EAC.

1. Haga clic en **Finanzas**. 

   El valor EAC se muestra en el campo **Estimar al finalizar**.

   ![](assets/eac-highlighted-on-project-350x112.png)
