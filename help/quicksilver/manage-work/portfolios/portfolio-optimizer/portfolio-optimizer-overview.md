---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Información general de Portfolio Optimizer
description: El [!UICONTROL Portfolio Optimizer] es la herramienta utilizada para la evaluación y comparación de proyectos. El proceso de revisar y comparar los valores de los casos comerciales de los proyectos asignados a un portafolio es la forma en que un administrador de portafolios puede priorizar los proyectos y generar el mayor valor para una organización.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '1629'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] descripción general

<!-- Audited: 01/2024 -->

El [!UICONTROL Portfolio Optimizer] es la herramienta utilizada para la evaluación y comparación de proyectos. Proceso de revisión y comparación [!UICONTROL Caso comercial] los valores de los proyectos asignados a un portafolio son la forma en que un administrador de portafolios puede priorizar los proyectos y generar el mayor valor para una organización.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

El propósito de la [!UICONTROL optimizador de portafolios] es proporcionar una interfaz a través de la cual un administrador de portafolios, un comité directivo o una oficina de administración de productos pueden ver información resumida sobre el caso comercial de cada proyecto. Los proyectos se pueden priorizar según los valores estratégicos y los objetivos, o según su puntuación general.

El [!UICONTROL Portfolio Optimizer] Solo puede ayudarle si ha completado los siguientes requisitos previos:

* El [!UICONTROL Casos comerciales] se han completado en los proyectos. Para obtener más información, consulte los artículos de [Definir un caso comercial: índice de artículos](../../projects/define-a-business-case/define-business-case.md).
* Un portafolio se define en el área Información general del proyecto de la sección Detalles del proyecto para los proyectos que desea revisar.
* Ha indicado el presupuesto del proyecto y el beneficio planificado de los proyectos que desea revisar. Costo fijo e ingresos fijos son opcionales pero agregan valor adicional. Para obtener más información, consulte [Campos de finanzas del proyecto](../../projects/project-finances/project-finances-overview-1.md).

Para obtener información sobre cómo localizar el [!UICONTROL Portfolio Optimizer], consulte [Busque el [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanzas en la UE [!UICONTROL Portfolio Optimizer]

Puede ver el estado financiero de su cartera en cualquier momento durante la duración de sus proyectos al utilizar el [!UICONTROL Portfolio Optimizer].

Tenga en cuenta lo siguiente al trabajar con finanzas en [!UICONTROL Portfolio Optimizer]:

* A cada proyecto se le asigna una puntuación cuando [!UICONTROL Casos comerciales] se completan según los criterios con los que coincidan en la [!UICONTROL Portfolio Optimizer]. Por ejemplo, los proyectos de bajo coste o de alta alineación reciben una puntuación más alta.

  Para obtener más información sobre el cálculo de la puntuación del optimizador de portafolios de un proyecto, consulte [Descripción general de [!UICONTROL Portfolio Optimizer] Puntuación](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Los cálculos financieros para [!UICONTROL Portfolio Optimizer] use el [!UICONTROL Costo presupuestado] en el [!UICONTROL Caso comercial] del proyecto.
* Puede priorizar manualmente sus proyectos en la [!UICONTROL Portfolio Optimizer], teniendo en cuenta toda la información sobre ellos. Esto incluye datos financieros, alineación en sus cuadros de resultados y ROI, por ejemplo.

### Las áreas financieras en la [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Puede ver información financiera en las siguientes áreas del [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL Encabezado de Portfolio]**: Esta área muestra información financiera recopilada de todos los proyectos del portafolio. Se muestra en todas las pestañas del objeto Portfolio.
* **[!UICONTROL Finanzas del Portfolio para los proyectos seleccionados]**: Esta área muestra información financiera recopilada de los proyectos seleccionados en la [!UICONTROL Portfolio Optimizer]. Puede agregar o eliminar proyectos y comprender cómo afectará esto a las finanzas del portafolio consultando la información de esta área.
* **[!UICONTROL Finanzas de proyectos]**: Esta área muestra la información financiera de cada proyecto enumerado en la [!UICONTROL Portfolio Optimizer].

### Los campos financieros en la [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Los siguientes campos financieros se muestran en la variable [!UICONTROL Portfolio Optimizer]:

* [encabezado del Portfolio](#portfolio-header)
* [Finanzas de Portfolio para proyectos seleccionados](#portfolio-finances-for-selected-projects)

#### encabezado del Portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcula los campos financieros en el encabezado del portafolio utilizando información de proyectos con estados que solo equivalen a [!UICONTROL Aprobado] o [!UICONTROL Actual].

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
   <td> <p>Porcentaje de proyectos del portafolio que se consideran [!UICONTROL a tiempo]. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>Se considera que un proyecto es [!UICONTROL On Time] cuando el proyecto <strong>[!UICONTROL Condición]</strong> es <strong>[!UICONTROL En Destino]</strong>. <br>Para obtener más información acerca de [!UICONTROL Condiciones del proyecto], vea el artículo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Descripción general de la condición y el tipo de condición del proyecto</a>.</p> <p>El <strong>[!UICONTROL On Time]</strong> El porcentaje de se calcula mediante la fórmula siguiente:</p> <p><em>[!UICONTROL Porcentaje de Portfolio de Tiempo Activado] = Número de proyectos de [!UICONTROL A Tiempo]/ Número total de proyectos en estado [!UICONTROL Actual] o [!UICONTROL Aprobado]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Según Presupuesto]</td> 
   <td> <p>Porcentaje de proyectos del portafolio que se consideran [!UICONTROL según el presupuesto]. Esto es visible desde cualquier ficha dentro de un portafolio de [!UICONTROL].</p> <p>Los proyectos son <strong>[!UICONTROL Según Presupuesto]</strong> cuando no hayan superado su presupuesto predefinido. <br>Para obtener más información sobre el presupuesto de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Información de [!UICONTROL Manage] en el área de finanzas del proyecto</a>.</p> <p>El porcentaje [!UICONTROL On Budget] se calcula mediante la siguiente fórmula:</p> <p><em>[!UICONTROL Porcentaje de Portfolio de presupuesto] = Número de proyectos de [!UICONTROL de presupuesto]/ Número total de proyectos </em><em>en un estado [!UICONTROL Actual] o [!UICONTROL Aprobado]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (para portafolios)</td> 
   <td> <p>El [!UICONTROL Retorno de la inversión] (ROI) del portafolio se calcula teniendo en cuenta el [!UICONTROL Beneficio] total del [!UICONTROL Portfolio] y el total de los [!UICONTROL Costos presupuestados] de los proyectos. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>El valor de ROI del Portfolio se calcula mediante la siguiente fórmula:</p> <p><em>ROI del Portfolio = ([!UICONTROL Beneficio total] - [!UICONTROL Costo total presupuestado])/ [!UICONTROL Costo total] * 100</em> </p> <p>Para obtener más información sobre cómo se calcula el retorno de la inversión de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcular el retorno de la inversión (ROI)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL alineado] o [!UICONTROL puntuación de alineación] </td> 
   <td> <p>Promedio de todos los valores de [!UICONTROL Puntuación de alineación del proyecto], que se calculan después de completar el informe de valoración de [!UICONTROL] en el [!UICONTROL Caso comercial] del proyecto. La puntuación de alineación de cada proyecto se muestra en la columna [!UICONTROL Alignment] de [!UICONTROL Portfolio Optimizer]. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>Para obtener más información sobre cómo generar una puntuación de alineación para un proyecto, consulte el artículo <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor neto]</td> 
   <td> <p>Suma de todos los [!UICONTROL Valores de red] de todos los proyectos del portafolio. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>Para obtener más información acerca de cómo se calcula el valor neto de [!UICONTROL] para un proyecto, vea el artículo <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor neto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finanzas de Portfolio para proyectos seleccionados {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nombre del campo</strong> </th> 
   <th><strong>Descripción</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Número de proyectos]</td> 
   <td> <p>Número total de proyectos activos en el portafolio. Los proyectos que se consideran activos en un portafolio pueden estar en cualquiera de los siguientes estados:</p> 
    <ul> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Planificación]</li> 
     <li>[!UICONTROL Aprobado]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Presupuesto]</td> 
   <td>Puede actualizar manualmente este campo para indicar cuál es el presupuesto total para todo el portafolio. Este presupuesto se utiliza para todos los proyectos dentro del portafolio. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restante]</td> 
   <td> <p>El presupuesto restante después de que todos los [!UICONTROL Costos presupuestados] de todos los proyectos dentro del portafolio se hayan restado del Presupuesto del portafolio.</p> <p>El [!UICONTROL Presupuesto de Portfolio restante] se calcula mediante la siguiente fórmula:</p> <p><em>[!UICONTROL Presupuesto de Portfolio restante] = [!UICONTROL Presupuesto de Portfolio total] - Total [!UICONTROL Costo presupuestado] de todos los proyectos de Portfolio</em> </p> <p>El [!UICONTROL Costo presupuestado] general de todos los proyectos del portafolio se representa en la barra de indicadores debajo del campo Presupuesto. </p> <p>Para obtener más información sobre el seguimiento de los costes de un proyecto, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo total]</td> 
   <td> <p>Suma de los costos de todos los proyectos mostrados en [!UICONTROL Portfolio Optimizer]. El costo de cada proyecto es el mismo que el [!UICONTROL Costo presupuestado] del proyecto, tal como se muestra en el [!UICONTROL Resumen de caso comercial]. </p> <p>Para obtener más información acerca de los campos financieros de los proyectos en [!UICONTROL Business Case], vea la sección "Comprensión de los campos financieros en el caso comercial" en el artículo <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Crear un caso comercial para un proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Riesgo] </td> 
   <td> <p>Suma de todos los [!UICONTROL Costos de riesgo potencial] de todos los proyectos del portafolio. El [!UICONTROL Costo de riesgo potencial] de cada proyecto se muestra en la columna [!UICONTROL Riesgo] de [!UICONTROL Portfolio Optimizer]. </p> <p>Para obtener más información sobre el cálculo de riesgos para los proyectos, vea el artículo <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular costo de riesgo potencial</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Beneficio]</td> 
   <td> <p>Suma de todos los valores de [!UICONTROL Beneficio planificado] de todos los proyectos del portafolio. El valor de Beneficio planificado de cada proyecto se muestra en la columna [!UICONTROL Beneficio] de [!UICONTROL Portfolio Optimizer]. </p> <p>Para obtener más información acerca del [!UICONTROL Beneficio planificado] de un proyecto, vea el artículo <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Visión General de Beneficio Planificado del Proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicador de [!UICONTROL Riesgo de valor neto]</td> 
   <td> <p>Mide el valor de [!UICONTROL Riesgo potencial], teniendo en cuenta el [!UICONTROL Valor neto] proporcionado por todos los proyectos del portafolio. Para lograr la máxima eficiencia dentro del portafolio, desea ver que el indicador de [!UICONTROL Riesgo] es bajo y el indicador de [!UICONTROL Valor neto] es alto. </p> <p>Para obtener más información acerca del cálculo de Riesgo para [!UICONTROL Valor neto], vea el artículo <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcular el riesgo de valor neto en un portafolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalización de [!UICONTROL Portfolio Optimizer]

Puede personalizar únicamente el área de la lista de proyectos de [!UICONTROL Portfolio Optimizer] usando la configuración para cambiar la información de la lista.

Los iconos y las opciones siguientes están disponibles para [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icono en Portfolio Optimizer</strong></td> 
   <td><strong>Nombre</strong></td> 
   <td><strong>Función</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Establecer prioridad de proyecto]</td> 
   <td>Utilice este icono cuando desee guardar el orden del proyecto, según su prioridad. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimizar portafolio]</td> 
   <td>Utilice este icono para optimizar el portafolio en función de los siguientes valores financieros de los proyectos:
    <ul>
     <li>[!UICONTROL Costo]</li>
     <li>[!UICONTROL Alineación]</li>
     <li>[!UICONTROL Valor]</li>
     <li>[!UICONTROL Riesgo de beneficio]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Para obtener más información sobre cómo optimizar su portafolio, consulte el artículo <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimizar proyectos en [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Iconos de [!UICONTROL Deshacer]/ [!UICONTROL Rehacer]</td> 
   <td>Utilice estos iconos para cancelar o rehacer los cambios realizados en [!UICONTROL Portfolio Optimizer] antes de guardar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Mostrar]/[!UICONTROL Ocultar] proyectos sin marcar</td> 
   <td>Utilice estos iconos para mostrar u ocultar los proyectos del portafolio que haya desmarcado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilice este icono para exportar los datos del área de [!UICONTROL Project Prioritization] de [!UICONTROL Portfolio Optimizer]. Se puede exportar a los siguientes formatos:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>Delimitado por [!UICONTROL Tab]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferencias]</td> 
   <td> <p>Utilice este icono para modificar los campos de proyecto mostrados en las columnas de [!UICONTROL Portfolio Optimizer] o para modificar los proyectos que se muestran en [!UICONTROL Optimizer] según sus estados. </p> <p>Sugerencia:  
     <ul> 
      <li> <p>No todos [!DNL Workfront] hay campos estándar disponibles para añadir en las columnas. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Solo puede agregar los campos personalizados que tengan un valor distinto de cero en cualquiera de los proyectos del portafolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
