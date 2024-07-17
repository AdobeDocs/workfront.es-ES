---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcular costo presupuestado
description: "Calcular progreso de proyecto de seguimiento de costes presupuestado con un informe de utilización"
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# Calcular costo presupuestado

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

El costo presupuestado de un proyecto es el costo total asociado con el proyecto según lo estimado al planificar el proyecto.

## Visión General de Costes Presupuestados en un Proyecto

No puede cambiar manualmente el costo presupuestado de un proyecto. Adobe Workfront calcula el coste presupuestado mediante la siguiente fórmula:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* **Costo de mano de obra presupuestado del planificador de recursos** en el cálculo anterior es el costo asociado con los roles en el proyecto.

  Puede realizar un seguimiento del costo de mano de obra presupuestado de un proyecto en el área de presupuesto de recursos del caso comercial o del planificador de recursos.

  >[!TIP]
  >
  >  El costo de mano de obra presupuestado de un proyecto en el caso empresarial se muestra como Costo de mano de obra presupuestado del Planificador de recursos en informes y listas.

  Para obtener información acerca de los costos laborales presupuestados, vea el artículo [Comprender el costo laboral presupuestado y las horas presupuestadas de los proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* El **costo de gastos presupuestado** en el cálculo anterior es el costo planificado asociado con los gastos del proyecto, ya que se calculan en el área Gastos del caso comercial o en la pestaña Gastos del proyecto.\
  Para obtener más información sobre los gastos de un proyecto, consulte el artículo [Administrar gastos de proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* El **Costo fijo** del cálculo anterior es la cantidad fija asociada con el Costo del proyecto, tal como se define en el área Finanzas de la sección Detalles del proyecto.\
  Para obtener más información acerca de la subficha Finanzas de un proyecto, vea el artículo [Administrar información en el área Finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcula toda la información de costes utilizando la divisa del proyecto. Si especifica Horas presupuestadas para los recursos en el Planificador de recursos, se deshabilita la opción para cambiar la divisa del proyecto.
>
>Para obtener más información acerca de cómo cambiar la moneda de un proyecto, vea el artículo [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Buscar el costo presupuestado de un proyecto

El costo presupuestado tal como se refleja en el área de presupuesto de recursos del caso comercial o del planificador de recursos se muestra en las siguientes áreas de Workfront con los siguientes nombres:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nombre para mostrar Costo presupuestado</strong></td> 
     <td><strong>Área de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado</td> 
     <td> <p>Resumen de caso comercial</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Costo</td> 
     <td> <p>Portfolio Optimizer</p> <p>Sugerencia: El total de todos los valores de Coste presupuestado de proyecto es el Coste presupuestado del portafolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado de proyecto</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Informe de proyecto</p> <p>Informe de proyecto (datos financieros)</p> <p>Informe de tareas</p> <p>Informe de problema</p> <p>Informe de horas presupuestadas</p> <p>Para obtener más información acerca de cómo crear un informe, vea el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
