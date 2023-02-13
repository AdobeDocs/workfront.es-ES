---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Información general sobre Portfolio Optimizer
description: La variable [!UICONTROL Optimizador de Portfolio] es la herramienta utilizada para la evaluación y comparación de proyectos. El proceso de revisión y comparación de los valores de Caso de negocio de los proyectos asignados a un portafolio es la forma en que un administrador de portafolios puede priorizar los proyectos y generar el mayor valor para una organización.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 0%

---

# [!UICONTROL Optimizador de Portfolio] información general

La variable [!UICONTROL Optimizador de Portfolio] es la herramienta utilizada para la evaluación y comparación de proyectos. El proceso de revisión y comparación [!UICONTROL Caso empresarial] los valores de los proyectos asignados a un portafolio son la forma en que un administrador de portafolios puede priorizar los proyectos y generar el mayor valor para una organización.

El propósito del [!UICONTROL optimizador de portafolio] es proporcionar una interfaz a través de la cual un administrador de portafolios, un comité directivo o una oficina de gestión de productos pueden ver información resumida sobre el caso empresarial de cada proyecto. A continuación, se puede priorizar los proyectos según los valores y objetivos estratégicos o según su puntuación general.

La variable [!UICONTROL Optimizador de Portfolio] solo puede ayudarle si ha completado los siguientes requisitos previos:


* La variable [!UICONTROL Casos de uso] se han completado los proyectos. Para obtener más información, consulte los artículos de la sección [Definir un caso empresarial](../../projects/define-a-business-case/define-business-case.md).
* Un portafolio se define en el área Información general del proyecto de la sección Detalles del proyecto para los proyectos que desea revisar
* Ha indicado el presupuesto del proyecto y el beneficio planeado para los proyectos que desea revisar. Coste fijo e Ingresos fijos son opcionales, pero agregan valor adicional. Para obtener más información, consulte [Campos de finanzas de proyecto](../../projects/project-finances/project-finances-overview-1.md).


Para obtener información sobre cómo localizar la variable [!UICONTROL Optimizador de Portfolio], consulte [Busque la variable [!UICONTROL Optimizador de Portfolio]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Las finanzas en el [!UICONTROL Optimizador de Portfolio]

* [Las áreas financieras de [!UICONTROL Optimizador de Portfolio]](#the-financial-areas-in-the-portfolio-optimizer)
* [Los campos financieros de la variable [!UICONTROL Optimizador de Portfolio]](#the-financial-fields-in-the-portfolio-optimizer)

Puede ver el estado financiero de su portafolio en cualquier momento durante la vida de sus proyectos al usar la variable [!UICONTROL Optimizador de Portfolio].

Tenga en cuenta lo siguiente cuando trabaje con finanzas en la variable [!UICONTROL Optimizador de Portfolio]:

* A los proyectos se les asigna una puntuación cuando [!UICONTROL Casos de uso] se completan según los criterios que coincidan en la variable [!UICONTROL Optimizador de Portfolio]. Por ejemplo, los proyectos de bajo costo o alta alineación reciben una puntuación más alta.

   Para obtener más información sobre el cálculo de la puntuación del optimizador de portafolio de un proyecto, consulte el artículo [Información general sobre [!UICONTROL Optimizador de Portfolio] Puntuación](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Los cálculos financieros para la variable [!UICONTROL Optimizador de Portfolio] use el [!UICONTROL Coste presupuestado] en el [!UICONTROL Caso empresarial] del proyecto.
* Puede priorizar manualmente sus proyectos en la [!UICONTROL Optimizador de Portfolio], teniendo en cuenta toda la información sobre ellos. Esto incluye datos financieros, alineación con sus informes de valoración, ROI, por ejemplo.

### Las áreas financieras de [!UICONTROL Optimizador de Portfolio] {#the-financial-areas-in-the-portfolio-optimizer}

Puede ver información financiera en las siguientes áreas de la [!UICONTROL Optimizador de Portfolio]:

* **[!UICONTROL Encabezado del Portfolio]**: Esta área muestra la información financiera recopilada de todos los proyectos del portafolio. Se muestra en todas las fichas del objeto Portfolio.
* **[!UICONTROL Finanzas de Portfolio para proyectos seleccionados]**: Esta área muestra la información financiera recopilada de los proyectos seleccionados en la [!UICONTROL Optimizador de Portfolio]. Puede agregar o eliminar proyectos y comprender cómo esto afectará a las finanzas del portafolio consultando la información de esta área.
* **[!UICONTROL Fondos de proyectos]**: Esta área muestra la información financiera de cada proyecto enumerado en la variable [!UICONTROL Optimizador de Portfolio].

### Los campos financieros de la variable [!UICONTROL Optimizador de Portfolio] {#the-financial-fields-in-the-portfolio-optimizer}

Los siguientes campos financieros se muestran en la sección [!UICONTROL Optimizador de Portfolio]:

* [encabezado del Portfolio](#portfolio-header)
* [Portfolio financieros para proyectos seleccionados](#portfolio-finances-for-selected-projects)

#### encabezado del Portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcula los campos financieros del encabezado del portafolio utilizando información de proyectos con estados que solo se corresponden con [!UICONTROL Aprobado] o [!UICONTROL Actual].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nombre del campo</strong> </th> 
   <th><strong>Descripción</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>El porcentaje de proyectos del portafolio que se consideran [!UICONTROL On Time]. Esto se puede ver desde cualquier pestaña dentro de un Portfolio.</p> <p>Se considera que un proyecto es [!UICONTROL On Time] cuando se ejecuta el proyecto <strong>[!UICONTROL Condition]</strong> es <strong>[!UICONTROL En Target]</strong>. <br>Para obtener más información sobre [!UICONTROL Project Conditions], consulte el artículo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Descripción general de la condición y el tipo de condición del proyecto</a>.</p> <p>La variable <strong>[!UICONTROL On Time]</strong> el porcentaje se calcula mediante la fórmula siguiente:</p> <p><em>[!UICONTROL On Time Portfolio centage] = Número de proyectos [!UICONTROL On Time]/ Número total de proyectos en estado [!UICONTROL Current] o [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL En El Presupuesto]</td> 
   <td> <p>El porcentaje de proyectos del portafolio que se consideran [!UICONTROL On Budget]. Esto se puede ver desde cualquier pestaña dentro de un [!UICONTROL Portfolio].</p> <p>Los proyectos son <strong>[!UICONTROL En El Presupuesto]</strong> cuando no hayan superado su presupuesto predefinido. <br>Para obtener más información sobre el presupuesto de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Información de [!UICONTROL Administrar] en el área de finanzas del proyecto</a>.</p> <p>El porcentaje [!UICONTROL On Budget] se calcula mediante la fórmula siguiente:</p> <p><em>[!UICONTROL En el porcentaje del Portfolio presupuestario] = Número de proyectos [!UICONTROL en el presupuesto]/ Número total de proyectos </em><em>en un estado [!UICONTROL Current] o [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (para portafolio)</td> 
   <td> <p>El [!UICONTROL Return on Investment] (ROI) del portafolio se calcula teniendo en cuenta el [!UICONTROL Benefit] total del [!UICONTROL Portfolio] y el total de los [!UICONTROL Budgeted Costs] de los proyectos. Esto se puede ver desde cualquier pestaña dentro de un Portfolio.</p> <p>El valor de ROI del Portfolio se calcula mediante la fórmula siguiente:</p> <p><em>ROI de Portfolio = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Para obtener más información sobre cómo se calcula el ROI de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcular el rendimiento de la inversión (ROI)</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alineado] o [!UICONTROL Puntuación de alineación] </td> 
   <td> <p>Media de todos los valores de la [!UICONTROL Project Alignment Score] que se calculan después de completar el [!UICONTROL Scorecard] en el [!UICONTROL Business Case] del proyecto. La puntuación de alineación de cada proyecto se muestra en la columna [!UICONTROL Alignment] del [!UICONTROL Portfolio Optimizer]. Esto se puede ver desde cualquier pestaña dentro de un portafolio.</p> <p>Para obtener más información sobre la generación de una puntuación de alineación para un proyecto, consulte el artículo <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Aplicar un informe de valoración a un proyecto y generar una puntuación de alineación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor neto]</td> 
   <td> <p>La suma de todos los [!UICONTROL Net Values] de todos los proyectos del portafolio. Esto se puede ver desde cualquier pestaña dentro de un portafolio.</p> <p>Para obtener más información sobre cómo se calcula el [!UICONTROL Net Value] para un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor neto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio financieros para proyectos seleccionados {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nombre del campo</strong> </th> 
   <th> <p><strong>Descripción</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Número de proyectos]</td> 
   <td> <p>El número total de proyectos activos en el portafolio. Los proyectos que se consideran activos en un portafolio pueden tener cualquiera de los siguientes estados:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Aprobado]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Presupuesto]</td> 
   <td>Puede actualizar manualmente este campo para indicar cuál es el presupuesto total para todo el portafolio. Este presupuesto se utiliza para todos los proyectos dentro de la cartera. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restante]</td> 
   <td> <p>El presupuesto restante después de todos los [!UICONTROL Costes presupuestados] de todos los proyectos incluidos en la cartera se ha restado del presupuesto de la cartera.</p> <p>El [!UICONTROL Presupuesto Portfolio restante] se calcula mediante la fórmula siguiente:</p> <p><em>[!UICONTROL Presupuesto Portfolio restante] = [!UICONTROL Total Presupuesto Portfolio] - Total [!UICONTROL Costo presupuestado] de todos los proyectos Portfolio</em> </p> <p>El [!UICONTROL Costo presupuestado] general de todos los proyectos del portafolio se representa en la barra de indicadores del campo Presupuesto . </p> <p>Para obtener más información sobre el seguimiento de costes en un proyecto, consulte el artículo<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo total]</td> 
   <td> <p>La suma de los costes de todos los proyectos mostrados en el [!UICONTROL Portfolio Optimizer]. El coste de cada proyecto es el mismo que el [!UICONTROL Costo presupuestado] del proyecto que se muestra en el [!UICONTROL Resumen de caso empresarial]. </p> <p>Para obtener más información sobre los campos financieros de los proyectos en el [!UICONTROL Business Case], consulte la sección "Explicación de los campos financieros en el caso empresarial" en el artículo <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Creación de un caso empresarial para un proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Riesgo] </td> 
   <td> <p>La suma de todos los [!UICONTROL Potencial Risk Costs] de todos los proyectos de la cartera. El [!UICONTROL Potencial Risk Cost] de cada proyecto se enumera en la columna [!UICONTROL Risk] del [!UICONTROL Portfolio Optimizer]. </p> <p>Para obtener más información sobre el cálculo de riesgos para los proyectos, consulte el artículo <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Coste de Riesgo Potencial </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ventaja]</td> 
   <td> <p>La suma de todos los valores de [!UICONTROL Planificado Beneficio] de todos los proyectos del portafolio. El valor de beneficio planeado de cada proyecto se enumera en la columna [!UICONTROL Benefit] del [!UICONTROL Portfolio Optimizer]. </p> <p>Para obtener más información sobre los [!UICONTROL Beneficios planificados] de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Descripción general de los beneficios previstos para el proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicador [!UICONTROL Riesgo a valor neto]</td> 
   <td> <p>Mide el valor [!UICONTROL Potencial Risk] teniendo en cuenta el [!UICONTROL Net Value] proporcionado por todos los proyectos del portafolio. Para lograr la mayor eficiencia dentro del portafolio, debe comprobarse que el indicador [!UICONTROL Risk] es bajo y que el indicador [!UICONTROL Net Value] es alto. </p> <p>Para obtener más información sobre el cálculo del riesgo en [!UICONTROL Valor neto], consulte el artículo <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcular el riesgo para el valor neto en un portafolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalice el [!UICONTROL Optimizador de Portfolio]

Puede personalizar solo el área de la lista de proyectos de la variable [!UICONTROL Optimizador de Portfolio] utilizando la configuración para cambiar la información de la lista.

Los iconos y las opciones disponibles para la variable [!UICONTROL Optimizador de Portfolio]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Icono en el Optimizador de Portfolio</td> 
   <td>Nombre</td> 
   <td>Función</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Establecer prioridad del proyecto]</td> 
   <td>Utilice este icono cuando desee guardar el orden del proyecto según su prioridad. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimizar portafolio]</td> 
   <td>Utilice este icono para optimizar el portafolio en función de los siguientes valores financieros de los proyectos:
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Alineación]</li>
     <li>[!UICONTROL Valor]</li>
     <li>[!UICONTROL Riesgo de beneficio]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Para obtener más información sobre la optimización del portafolio, consulte el artículo <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimizar proyectos en el [!UICONTROL Portfolio Optimizer] </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Iconos [!UICONTROL Deshacer]/ [!UICONTROL Rehacer]</td> 
   <td>Utilice estos iconos para cancelar o rehacer los cambios realizados en el [!UICONTROL Portfolio Optimizer] antes de guardarlos.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portafolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>Proyectos [!UICONTROL Mostrar]/ [!UICONTROL Ocultar sin marcar]</td> 
   <td>Utilice estos iconos para mostrar u ocultar los proyectos del portafolio que no haya seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilice este icono para exportar los datos del área [!UICONTROL Project Prioritization] del [!UICONTROL Portfolio Optimizer]. Puede exportarlo a los siguientes formatos:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Delimitado</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferencias_portafolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferencias]</td> 
   <td> <p>Utilice este icono para modificar los campos del proyecto que se muestran en las columnas del [!UICONTROL Portfolio Optimizer] o para modificar los proyectos que se muestran en el [!UICONTROL Optimizer], según sus estados. </p> <p>Sugerencia:  
     <ul> 
      <li> <p>No es todo [!DNL Workfront] los campos estándar están disponibles para añadirlos en las columnas. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Solo puede añadir los campos personalizados que tengan un valor distinto de cero en cualquiera de los proyectos del portafolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
