---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcular el coste presupuestado
description: Cálculo del Progreso del Proyecto de Seguimiento de Costes Presupuestados con un Informe de Utilización
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: 13621c29f32a514af46489fb58397f3e96f640ce
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 97%

---

# Calcular el coste presupuestado

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

El coste presupuestado de un proyecto es el coste total asociado con el proyecto según lo estimado al planificar el proyecto.

## Información general sobre el coste presupuestado de un proyecto

No puede modificar manualmente el coste presupuestado de un proyecto. Adobe Workfront calcula el coste presupuestado mediante la siguiente fórmula:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* El **coste de mano de obra presupuestado del planificador de recursos** en el cálculo anterior es el coste asociado con las funciones en el proyecto.

  Puede realizar un seguimiento del coste de mano de obra presupuestado de un proyecto en el área de presupuesto de recursos del caso comercial o del planificador de recursos.

  >[!TIP]
  >
  >  El coste de mano de obra presupuestado de un proyecto en el caso empresarial se muestra como coste de mano de obra presupuestado del Planificador de recursos en informes y listas.

  Para obtener información acerca de los costes de mano de obra presupuestados, consulte el artículo [Explicación del coste de mano de obra presupuestado y las horas presupuestadas de los proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* El **coste de gastos presupuestado** en el cálculo anterior es el coste planificado asociado con los gastos del proyecto, ya que se calculan en el área de gastos del caso empresarial o en la ficha Gastos del proyecto.\
  Para obtener más información sobre los gastos de un proyecto, consulte el artículo [Administrar gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* El **coste fijo** del cálculo anterior es la cantidad fija asociada con el coste del proyecto, tal como se define en el área de finanzas de la sección Detalles del proyecto.\
  Para obtener más información acerca de la subpestaña Finanzas de un proyecto, consulte el artículo [Administrar información en el área Finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcula toda la información sobre los costes utilizando la divisa del proyecto. Si especifica Horas presupuestadas para los recursos en el Planificador de recursos, se deshabilita la opción para cambiar la divisa del proyecto.
>
>Para obtener más información acerca de cómo cambiar la divisa de un proyecto, consulte el artículo [Cambiar la divisa del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Localizar el coste presupuestado de un proyecto

El coste presupuestado tal como se refleja en el área de presupuesto de recursos del caso empresarial o del planificador de recursos, se muestra en las siguientes áreas de Workfront con los siguientes nombres:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nombre para mostrar del coste presupuestado</strong></td> 
     <td><strong>Área de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado</td> 
     <td> <p>Resumen de caso comercial</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Coste</td> 
     <td> <p>Optimizador de portafolios</p> <p>Sugerencia: el total de todos los valores del coste presupuestado del proyecto es el coste presupuestado del portafolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado de proyecto</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Informe de proyecto</p> <p>Informe de proyecto (datos financieros)</p> <p>Informe de tarea</p> <p>Informe de problema</p> <p>Informe de horas presupuestadas</p> <p>Para obtener más información acerca de cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creación de un informe personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
