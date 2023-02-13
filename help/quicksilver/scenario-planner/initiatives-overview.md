---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Información general sobre las iniciativas en el planificador de escenarios
description: El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte Información general sobre el planificador de escenarios.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Información general sobre las iniciativas de [!DNL Scenario Planner]

La variable [!DNL Scenario Planner] solo está disponible en el nuevo [!DNL Adobe Workfront] experiencia y requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte [La variable [!DNL Scenario Planner] información general](../scenario-planner/scenario-planner-overview.md).
Como administrador empresarial, puede crear iniciativas para planes en la [!DNL Adobe Workfront Scenario Planner]. Para obtener información sobre la creación de planes, consulte el artículo [Cree y edite planes en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Información general sobre las iniciativas

Al usar la variable [!DNL Workfront Scenario Planner], puede estimar y revisar la siguiente información para cada iniciativa:

* Calcular el tipo y el número de funciones que se necesitarían para completar la iniciativa. Esto agrega al recuento de la función de trabajo requerida para el plan, así como calcula los costes de personal que puede revisar para una iniciativa.
* Calcule los costos fijos asociados con el trabajo necesario para completar la iniciativa.
* Calcule los beneficios planificados que su empresa podría obtener cuando se complete la iniciativa.

Para ver información sobre sus iniciativas, puede acceder a iniciativas individuales dentro de un plan. Para obtener información sobre la creación y el acceso a iniciativas, consulte el artículo [Cree y edite iniciativas en la [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Consideraciones sobre iniciativas

Tenga en cuenta lo siguiente al crear iniciativas:

* Debe crear un plan para poder crear una iniciativa.
* Puede crear iniciativas desde cero o importar proyectos en un plan. Los proyectos se convierten en iniciativas dentro del plan.

   Para obtener información sobre la creación de iniciativas desde cero, consulte [Cree y edite iniciativas en la [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   Para obtener información sobre la importación de proyectos en un plan para crear iniciativas a partir de proyectos, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Las iniciativas son unidades de planificación más pequeñas que los planes y se crean sólo como parte de un plan.
* La iniciativa más corta puede tener una duración de 1 mes. La iniciativa más larga puede tener una duración de 5 años.
* No se puede realizar un trabajo real en una iniciativa. A nivel de iniciativa, puede definir qué recursos se necesitan y en qué se incurrirán para que pueda empezar a ejecutar una de las demandas del plan. Por ejemplo, si su empresa tiene un plan para expandir y adquirir una nueva oficina en una nueva ubicación, su departamento podría tener una iniciativa para instalar la infraestructura de red para esa nueva ubicación.
* Puede crear varias iniciativas en un plan. Con cada iniciativa, puede esbozar una estrategia de alto nivel para llevar a cabo el trabajo en su departamento.
* Puede priorizar las iniciativas dentro de un plan para asegurarse de que la iniciativa más importante reciba la mayor cantidad de presupuesto y recursos.
* Cuando crea iniciativas dentro de un plan, todos los que vean ese plan también podrán ver todas las iniciativas dentro del plan.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Puede publicar iniciativas para crear proyectos o actualizar los proyectos vinculados a ellos. Para obtener información sobre las iniciativas de publicación, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Información financiera sobre iniciativas

Puede revisar la información financiera sobre iniciativas individuales para comprender cómo encajan las iniciativas dentro del plan. Para obtener información sobre el acceso a una iniciativa, consulte el artículo [Cree y edite iniciativas en la [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Puede ver los siguientes indicadores financieros sobre una iniciativa accediendo a ella dentro de un plan:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costes totales]</td> 
   <td> <p style="font-weight: normal;">Se trata de un cálculo del coste total de una iniciativa. </p> <p style="font-weight: normal;">[!DNL Workfront] calcula el valor total de Costes de una iniciativa mediante esta fórmula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costes fijos]</td> 
   <td> <p><span style="font-weight: normal;">Esta es una entrada manual en la que puede estimar <span>una cantidad mensual de Costes fijos para cada mes de la iniciativa.</span> Esto no incluye los costes asociados con las funciones agregadas a la iniciativa que se capturan en el campo [!UICONTROL People Cost].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costes]</td> 
   <td> <p style="font-weight: normal;">Se trata de un cálculo total de los costes asociados a las funciones de la iniciativa durante su duración. Este número depende de cuántos FTE u horas estime para una función de trabajo para cada mes de la iniciativa. </p> 
     <p><b>SUGERENCIAS</b>  
     <ul> 
      <li> <p>El número de ETC mensuales para el mismo puesto de trabajo puede ser diferente de un mes a otro.</p> </li> 
      <li> <p>[!DNL Workfront] considera que hay 160 horas de trabajo en un mes. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcula los [!UICONTROL People Costs] de una iniciativa mediante la fórmula siguiente:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcula los costes de persona mensuales de cada mes durante la duración de la Iniciativa utilizando la fórmula siguiente:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EJEMPLO</b></p>
      <p>Si tiene una iniciativa con una duración de 6 meses que requiere 1 Diseñador con una tasa de 50 dólares por hora para 1 FTE cada mes y un Diseñador Web con una tasa por hora de 100 dólares para 2 meses de la iniciativa, los Costes Personas de la iniciativa se calculan de la siguiente manera:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beneficio planificado]</td> 
   <td>Esta es una entrada manual en la que puede estimar el beneficio general que su departamento obtendría completando esta iniciativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cantidad del valor neto]</td> 
   <td> <p style="font-weight: normal;">Esto representa el valor de su iniciativa al tener en cuenta los costes generales y el beneficio planeado estimado en la iniciativa. [!DNL Workfront] calcula el valor neto de una iniciativa mediante la fórmula siguiente:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

## Información sobre la iniciativa en los informes

Puede mostrar la información de la iniciativa en los informes, tal como se describe en la tabla siguiente. Esta información está disponible en la instancia de Workfront solo cuando su empresa ha adquirido una licencia de Workfront Scenario Planner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo de informe</b></td> 
   <td><b>Información sobre la iniciativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Nombre, Duración, Fechas de inicio y finalización, Introducido por, ID, Última fecha de publicación*, Todos los campos del proyecto, incluidos los campos personalizados*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Toda la información de la iniciativa como se indica anteriormente, ID (función de trabajo), Proyecto*, Horas planificadas de asignación de proyectos*, Horario de funciones de la iniciativa, Recuento de funciones de trabajo, Todos los campos del proyecto, incluidos los campos personalizados*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>Toda la información de la Iniciativa enumerada anteriormente*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Estos campos se rellenan con información del proyecto vinculado a la iniciativa, solo cuando la iniciativa se creó a partir de un proyecto o se publicó en un proyecto al menos una vez. Para obtener información sobre las iniciativas de publicación, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
