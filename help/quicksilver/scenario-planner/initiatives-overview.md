---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Información general sobre iniciativas en el Scenario Planner
description: El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte Información general del Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Resumen de iniciativas en [!DNL Scenario Planner]

Como administrador de empresa, puede crear iniciativas para planes en [!DNL Adobe Workfront Scenario Planner]. Para obtener información acerca de cómo crear planes, vea el artículo [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Resumen de iniciativas

Con [!DNL Workfront Scenario Planner], puede estimar y revisar la siguiente información para cada iniciativa:

* Estime el tipo y el número de funciones del puesto que podrían ser necesarias para completar la iniciativa. Esto se añade al recuento de funciones requeridas del plan, así como calcula los costes de personas que puede revisar para una iniciativa.
* Calcular los costos fijos asociados con el trabajo necesario para completar la iniciativa.
* Calcule el beneficio planificado que su empresa podría obtener cuando se complete la iniciativa.

Para ver información sobre sus iniciativas, puede acceder a iniciativas individuales dentro de un plan. Para obtener información acerca de cómo crear y tener acceso a iniciativas, vea el artículo [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Consideraciones sobre las iniciativas

Tenga en cuenta lo siguiente al crear iniciativas:

* Debe crear un plan para poder crear una iniciativa.
* Puede crear iniciativas desde cero o importar proyectos en un plan. Los proyectos se convierten en iniciativas dentro del plan.

  Para obtener información sobre cómo crear iniciativas desde cero, consulte [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Para obtener información acerca de cómo importar proyectos a un plan para crear iniciativas a partir de proyectos, vea [Importar proyectos a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Las iniciativas son unidades de planificación más pequeñas que los planes y se crean únicamente como parte de un plan.
* La iniciativa más corta puede tener una duración de 1 mes. La iniciativa más larga puede tener una duración de 5 años.
* No se puede realizar un trabajo real en una iniciativa. A nivel de iniciativa, puede definir qué recursos se necesitan y en qué coste incurrirán esos recursos para que pueda comenzar a ejecutar una de las demandas del plan. Por ejemplo, si su empresa tiene previsto ampliar y adquirir una nueva oficina en una nueva ubicación, su departamento podría tener la iniciativa de instalar la infraestructura de red para esa nueva ubicación.
* Puede crear varias iniciativas en un plan. Con cada iniciativa, puede esbozar una estrategia de alto nivel para realizar el trabajo en su departamento.
* Puede priorizar las iniciativas dentro de un plan para asegurarse de que la iniciativa más importante reciba la mayor cantidad de presupuesto y de recursos.
* Cuando crea iniciativas dentro de un plan, todos los que vean ese plan también podrán ver todas las iniciativas dentro del plan.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Puede publicar iniciativas para crear proyectos o actualizar los proyectos vinculados a ellos. Para obtener información acerca de las iniciativas de publicación, vea [Actualizar o crear proyectos mediante iniciativas de publicación en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Información financiera sobre iniciativas

Puede revisar la información financiera sobre las iniciativas individuales para comprender cómo encajan las iniciativas dentro del plan. Para obtener información acerca de cómo tener acceso a una iniciativa, vea el artículo [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Puede ver los siguientes indicadores financieros sobre una iniciativa accediendo a ella dentro de un plan:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cantidad total de costos]</td> 
   <td> <p style="font-weight: normal;">Se trata de un cálculo del coste total de una iniciativa. </p> <p style="font-weight: normal;">[!DNL Workfront] calcula el valor de costes totales de una iniciativa mediante esta fórmula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costos fijos]</td> 
   <td> <p><span style="font-weight: normal;">Esta es una entrada manual en la que puede estimar <span>una cantidad mensual de costos fijos por cada mes de la iniciativa.</span> Esto no incluye los costos asociados con los roles agregados a la iniciativa que se capturan en el campo [!UICONTROL People Cost].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costos de personas]</td> 
   <td> <p style="font-weight: normal;">Se trata de un cálculo total de los costes asociados con las funciones de la iniciativa durante su duración. Este número depende de cuántos jornadas completas u horas calcule para un rol para cada mes de la iniciativa. </p> 
     <p><b>SUGERENCIAS</b>  
     <ul> 
      <li> <p>El número de jornadas completas mensuales para el mismo rol puede ser diferente de un mes a otro.</p> </li> 
      <li> <p>[!DNL Workfront] considera que hay 160 horas de trabajo en un mes. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcula los [!UICONTROL Costes de personas] de una iniciativa mediante la fórmula siguiente:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcula los costos mensuales de personas para cada mes durante la duración de la iniciativa mediante la siguiente fórmula:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EJEMPLO</b></p>
      <p>Si tiene una iniciativa con una duración de 6 meses que requiere 1 Designer con una tarifa por hora de 50 $ por 1 FTE cada mes y un Designer web con una tarifa por hora de 100 $ por 2 meses de la iniciativa, los costes de personas de la iniciativa se calculan de la siguiente manera:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Beneficio planificado de [!UICONTROL]</td> 
   <td>Se trata de una entrada manual en la que puede estimar el beneficio general que obtendría su departamento al completar esta iniciativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cantidad de valor neto]</td> 
   <td> <p style="font-weight: normal;">Representa el valor de su iniciativa si tiene en cuenta los costes generales y el beneficio planificado estimado de la iniciativa. [!DNL Workfront] calcula el valor neto de una iniciativa mediante la fórmula siguiente:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Información de la iniciativa en los informes

Puede mostrar la información de la iniciativa en los informes, tal como se describe en la tabla siguiente. Esta información solo está disponible en la instancia de Workfront cuando la empresa ha adquirido una licencia de Workfront Scenario Planner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo de informe</b></td> 
   <td><b>Información de iniciativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Iniciativa] </td> 
   <td>Nombre, Duración, Fechas de inicio y finalización, Ingresado por, ID, Última fecha de publicación*, Todos los campos de proyecto, incluidos los campos personalizados*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Función del puesto de la iniciativa]</td> 
   <td>Toda la información de la iniciativa como se ha indicado anteriormente, ID (función del puesto), proyecto*, horas planificadas de asignación del proyecto*, horas de función del proyecto, recuento (función del puesto), todos los campos del proyecto incluidos los campos personalizados*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Proyecto]*</p></td> 
   <td> <p>Toda la información de la iniciativa como se indica arriba*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Estos campos se rellenan con información del proyecto vinculado a la iniciativa, solo cuando la iniciativa se ha creado a partir de un proyecto o se ha publicado en un proyecto al menos una vez. Para obtener información acerca de las iniciativas de publicación, vea [Actualizar o crear proyectos mediante iniciativas de publicación en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
