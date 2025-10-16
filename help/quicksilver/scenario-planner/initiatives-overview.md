---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Información general sobre iniciativas en el Scenario Planner
description: El Planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener más información sobre el planificador de escenarios de Workfront, consulte Información general sobre el planificador de escenarios.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 99%

---

# Información general sobre iniciativas en el [!DNL Scenario Planner]

Como administrador de empresa, puede crear iniciativas para planes en [!DNL Adobe Workfront Scenario Planner]. Para obtener más información sobre cómo crear planes, consulte el artículo [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Información general sobre iniciativas

Con [!DNL Workfront Scenario Planner], puede estimar y revisar la siguiente información para cada iniciativa:

* Estimar el tipo y el número de funciones que podrían ser necesarias para completar la iniciativa. Esto se añade al recuento de funciones requeridas del plan y calcula los costes de las personas que se pueden revisar para una iniciativa.
* Estimar los costos fijos asociados al trabajo necesario para completar la iniciativa.
* Estimar el beneficio planificado que su compañía pueda obtener cuando se complete la iniciativa.

Para ver información sobre sus iniciativas, puede acceder a iniciativas individuales dentro de un plan. Para obtener más información sobre cómo crear y acceder a iniciativas, consulte el artículo [Crear y editar iniciativas en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Consideraciones sobre las iniciativas

Tenga en cuenta lo siguiente al crear iniciativas:

* Debe crear un plan antes de crear una iniciativa.
* Puede crear iniciativas desde cero o importar proyectos en un plan. Los proyectos se convierten en iniciativas dentro del plan.

  Para obtener más información sobre cómo crear iniciativas desde cero, consulte [Crear y editar iniciativas en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Para obtener más información acerca de cómo importar proyectos en un plan para crear iniciativas a partir de proyectos, consulte [Importar proyectos en planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Las iniciativas son unidades de planificación más pequeñas que los planes y se crean únicamente como parte de un plan.
* La iniciativa más corta puede tener una duración de un mes. La iniciativa más larga puede tener una duración de cinco años.
* No se puede realizar un trabajo real en una iniciativa. A nivel de iniciativa, puede definir qué recursos se necesitan y en qué coste incurrirán esos recursos para que pueda comenzar a ejecutar una de las demandas del plan. Por ejemplo, si su compañía tiene previsto ampliar y adquirir una nueva oficina en una nueva ubicación, su departamento podría tener la iniciativa de instalar la infraestructura de red para esa nueva ubicación.
* Puede crear varias iniciativas en un plan. Con cada iniciativa, puede esbozar una estrategia de alto nivel para realizar el trabajo en su departamento.
* Puede priorizar las iniciativas dentro de un plan para asegurarse de que la iniciativa más importante reciba la mayor cantidad de presupuesto y de recursos.
* Cuando crea iniciativas dentro de un plan, todos los que lo vean también podrán ver todas las iniciativas dentro de este.
* Puede publicar iniciativas para crear proyectos o actualizar los proyectos vinculados a ellas. Para obtener más información sobre cómo publicar iniciativas, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Información financiera sobre iniciativas

Puede revisar la información financiera sobre las iniciativas individuales para comprender cómo encajan las iniciativas dentro del plan. Para obtener más información sobre cómo acceder a una iniciativa, consulte el artículo [Crear y editar iniciativas en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Puede ver los siguientes indicadores financieros sobre una iniciativa accediendo a ella dentro de un plan:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs total amount]</td> 
   <td> <p style="font-weight: normal;">Se trata de un cálculo del coste total de una iniciativa. </p> <p style="font-weight: normal;">[!DNL Workfront] calcula el valor de costo total de una iniciativa mediante esta fórmula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixed Costs]</td> 
   <td> <p><span style="font-weight: normal;">Esta es una entrada manual en la que puede estimar <span>una cantidad mensual de costes fijos por cada mes de la iniciativa.</span> Esto no incluye los costes asociados a las funciones añadidas a la iniciativa que se capturan en el campo [!UICONTROL People Cost].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">Se trata de un cálculo total de los costes asociados a las funciones de la iniciativa durante su duración. Este número depende de cuántas jornadas completas u horas estime para una función en cada mes de la iniciativa. </p> 
     <p><b>SUGERENCIAS</b>  
     <ul> 
      <li> <p>El número de jornadas completas mensuales para la misma función puede ser diferente de un mes a otro.</p> </li> 
      <li> <p>[!DNL Workfront] considera que hay 160 horas laborables en un mes. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcula los [!UICONTROL People Costs] de una iniciativa mediante la siguiente fórmula:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcula los costes mensuales de personas correspondientes a cada mes durante el curso de la iniciativa mediante la siguiente fórmula:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>Ejemplo</b></p>
      <p>Si tiene una iniciativa cuya duración es de 6 meses que requiere 1 diseñador con una tarifa por hora de 50 USD por 1 jornada completa cada mes y un diseñador web con una tarifa por hora de 100 USD para 2 meses de la iniciativa, los costes de personas de la iniciativa se calculan de la siguiente manera:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>Se trata de una entrada manual en la que puede estimar el beneficio general que obtendría su departamento al completar esta iniciativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value amount]</td> 
   <td> <p style="font-weight: normal;">Representa el valor de su iniciativa teniendo en cuenta sus costes generales y beneficio planificado estimado. [!DNL Workfront] calcula el valor neto de una iniciativa mediante la fórmula siguiente:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

Puede mostrar la información de la iniciativa en los informes, tal como se describe en la tabla siguiente. Esta información solo está disponible en su instancia de Workfront cuando la compañía ha adquirido una licencia de Workfront Scenario Planner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo de informe</b></td> 
   <td><b>Información de iniciativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Los campos Nombre, Duración, Fechas de inicio y finalización, Introducido por, ID, Última fecha de publicación*, Todo el proyecto, incluidos los campos personalizados*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Toda la información de la iniciativa enumerada anteriormente: campos ID (función), Proyecto*, Horas planificadas de asignación del proyecto*, Horas de función del proyecto, Recuento (función), Todo el proyecto, incluidos los campos personalizados*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>Toda la información de la iniciativa enumerada anteriormente*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Estos campos se rellenan con información del proyecto vinculado a la iniciativa, solo cuando la iniciativa se ha creado a partir de un proyecto o se ha publicado en un proyecto al menos una vez. Para obtener información sobre la publicación de iniciativas, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
