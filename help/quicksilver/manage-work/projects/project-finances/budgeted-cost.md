---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcular costo presupuestado
description: Calcular el progreso del proyecto de seguimiento de costes presupuestados con un informe de uso""
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

El costo presupuestado de un proyecto es el costo total asociado con el proyecto, según se estima al planificar el proyecto.

## Descripción general del coste presupuestado en un proyecto

No se puede cambiar manualmente el costo presupuestado de un proyecto. Adobe Workfront calcula el coste presupuestado mediante la fórmula siguiente:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* La variable **Coste de trabajo presupuestado del planificador de recursos** en el cálculo anterior es el coste asociado a las funciones de trabajo del proyecto.

   Puede realizar un seguimiento del Coste de trabajo presupuestado de un proyecto en el área Presupuestación de recursos del Caso de negocio o del Planificador de recursos.

   >[!TIP]
   >
   >  El Coste Laboral Presupuestado de un proyecto en el Caso Empresarial aparece como Coste Laboral Presupuestado del Planificador de Recursos en los informes y listas.

   Para obtener información sobre los costes laborales presupuestados, consulte el artículo [Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* La variable **Coste de gastos presupuestados** en el cálculo anterior se encuentra el Coste planeado asociado con los gastos del proyecto, ya que se calculan en el área Gastos del Caso de negocio o en la pestaña Gastos del proyecto.\
   Para obtener más información sobre los gastos de un proyecto, consulte el artículo [Administrar los gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* La variable **Coste fijo** en el cálculo anterior se indica la cantidad fija asociada al coste del proyecto, tal como se define en el área Finanzas de la sección Detalles del proyecto.\
   Para obtener más información sobre la subpestaña Finanzas de un proyecto, consulte el artículo [Administrar información en el área de finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcula toda la información de coste utilizando la moneda del proyecto. Si especifica Horario presupuestado para los recursos en el Planificador de recursos, la opción para cambiar la moneda del proyecto estará deshabilitada.
>
>Para obtener más información sobre cómo cambiar la moneda de un proyecto, consulte el artículo [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Localizar el coste presupuestado de un proyecto

El Coste presupuestado tal como se refleja en el área de Presupuestación de Recursos del Caso de Negocio o el Planificador de Recursos se muestra en las siguientes áreas de Workfront con los nombres siguientes:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nombre para mostrar de Coste presupuestado</strong></td> 
     <td><strong>Área de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado</td> 
     <td> <p>Resumen de caso comercial</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Costo</td> 
     <td> <p>Optimizador de Portfolio</p> <p>Sugerencia: El total de todos los valores de Coste presupuestado del proyecto es el Coste presupuestado del portafolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado de proyecto</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Informe del proyecto</p> <p>Informe de proyecto (datos financieros)</p> <p>Informe de tareas</p> <p>Informe de problemas</p> <p>Informe de hora presupuestada</p> <p>Para obtener más información sobre la creación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
