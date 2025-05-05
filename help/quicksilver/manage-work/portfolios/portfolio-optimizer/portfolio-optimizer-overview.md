---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Información general del Optimizador de portafolios
description: El [!UICONTROL Optimizador de portafolios] es la herramienta que se usa para comparar y evaluar proyectos. El proceso de revisar y comparar los valores de caso empresarial de los proyectos asignados a un portafolio es la forma en que un administrador de portafolios puede priorizar los proyectos y generar el mayor valor para una organización.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: c53e7d2229032c59710a8f955de53cfbd7fc6df4
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 96%

---

# Información general del [!UICONTROL Optimizador de portafolios]

<!-- Audited: 01/2024 -->

El [!UICONTROL Optimizador de portafolios] es la herramienta que se usa para comparar y evaluar proyectos. El proceso de revisar y comparar los valores del [!UICONTROL Caso empresarial] de los proyectos asignados a un portafolio es el modo en que un administrador de portafolios puede priorizar los proyectos y generar el mayor valor para una organización.

![Optimizador de Portfolio con proyectos](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

El propósito del [!UICONTROL Optimizador de portafolios] es proporcionar una interfaz a través de la cual un administrador de portafolios, un comité directivo o una oficina de administración de productos puedan ver información resumida sobre el caso empresarial de cada proyecto. Los proyectos se pueden priorizar según los valores y metas estratégicos, o según su puntuación general.

El [!UICONTROL Optimizador de portafolios] solo puede ayudarle si ha completado los siguientes requisitos previos:

* Se han completado los [!UICONTROL Business Cases] de los proyectos. Para obtener más información, consulte los artículos incluidos en [Definir un caso empresarial: índice de artículos](../../projects/define-a-business-case/define-business-case.md).
* Un portafolio se define en el área Información general del proyecto de la sección Detalles del proyecto para los proyectos que desea revisar.
* Ha indicado el presupuesto del proyecto y el beneficio planificado de los proyectos que desea revisar. El coste fijo y los ingresos fijos son opcionales pero añaden valor adicional. Para obtener más información, consulte [Campos de finanzas del proyecto](../../projects/project-finances/project-finances-overview-1.md).

Para obtener información sobre la localización del [!UICONTROL Optimizador de portafolios], consulte [Localizar el [!UICONTROL Optimizador de portafolios]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanzas en el [!UICONTROL Optimizador de portafolios]

Puede ver el estado financiero del portafolio en cualquier momento mientras duren los proyectos al usar el [!UICONTROL Optimizador de portafolios].

Tenga en cuenta lo siguiente al trabajar en finanzas en el [!UICONTROL Optimizador de portafolios]:

* A cada proyecto se le asigna una puntuación cuando se completan sus [!UICONTROL Casos empresariales], según los criterios del [!UICONTROL Optimizador de portafolios] con los que coincidan. Por ejemplo, los proyectos de bajo coste o de alta alineación reciben una puntuación más alta.

  Para obtener más información sobre el cálculo de la puntuación del Optimizador de portafolios de un proyecto, consulte [Información general sobre la puntuación del [!UICONTROL Optimizador de portafolios]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Los cálculos financieros del [!UICONTROL Optimizador de portafolios] usan el [!UICONTROL Coste presupuestado] del [!UICONTROL Caso empresarial] del proyecto.
* Puede priorizar manualmente los proyectos en el [!UICONTROL Optimizador de portafolios], teniendo en cuenta toda la información que se tiene sobre ellos. Esta incluye, por ejemplo, los datos financieros, la alineación con sus cuadros de resultados y el retorno de la inversión.

### Áreas financieras del [!UICONTROL Optimizador de portafolios] {#the-financial-areas-in-the-portfolio-optimizer}

Puede ver información financiera en las siguientes áreas del [!UICONTROL Optimizador de portafolios]:

* **[!UICONTROL Encabezado del portafolios]**: esta área muestra información financiera recopilada de todos los proyectos del portafolio. Se muestra en todas las pestañas del objeto Portafolio.
* **[!UICONTROL Finanzas del portafolio para proyectos seleccionados]**: esta área muestra información financiera recopilada de los proyectos seleccionados en el [!UICONTROL Optimizador de portafolios]. Puede añadir o quitar proyectos y comprender el efecto que tendrá en las finanzas del portafolio al consultar la información de esta área.
* **[!UICONTROL Finanzas de los proyectos]**: esta área muestra la información financiera de cada proyecto enumerado en el [!UICONTROL Optimizador de portafolios].

### Campos financieros del [!UICONTROL Optimizador de portafolios] {#the-financial-fields-in-the-portfolio-optimizer}

En el [!UICONTROL Optimizador de portafolios] se muestran los siguientes campos:

* [Encabezado del portafolio](#portfolio-header)
* [Finanzas del portafolio para los proyectos seleccionados](#portfolio-finances-for-selected-projects)

#### Encabezado del portafolio {#portfolio-header}

![Encabezado de Portfolio](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcula los campos financieros del encabezado del portafolio mediante el uso de información de proyectos con estados equivalentes exclusivamente a [!UICONTROL Aprobado] o [!UICONTROL Actual].

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
   <td> <p>Porcentaje de proyectos del portafolio que se consideran [!UICONTROL On Time]. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>Se considera que un proyecto está [!UICONTROL On Time], cuando la <strong>[!UICONTROL Condition]</strong> del proyecto es <strong>[!UICONTROL On Target]</strong>. <br>Para obtener más información sobre las [!UICONTROL Project Conditions], consulte el artículo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Información general sobre la condición y el tipo de condición del proyecto</a>.</p> <p>El porcentaje <strong>[!UICONTROL On Time]</strong> se calcula con la siguiente fórmula:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Número de proyectos [!UICONTROL On Time] / Número total de proyectos que están en el estado [!UICONTROL Current] o [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>Porcentaje de proyectos del portafolio que se consideran [!UICONTROL On Budget]. Esto es visible desde cualquier pestaña de un [!UICONTROL portfolio].</p> <p>Los proyectos son <strong>[!UICONTROL On Budget]</strong> cuando no han excedido su presupuesto predefinido. <br>Para obtener más información sobre el presupuesto de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Manage] información en el área Finanzas del proyecto</a>.</p> <p>El porcentaje de [!UICONTROL On Budget] se calcula mediante la siguiente fórmula:</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Número de proyectos [!UICONTROL On Budget]/número total de proyectos </em><em>con estado [!UICONTROL Current] o [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (para portafolios)</td> 
   <td> <p>El [!UICONTROL Return on Investment] (ROI) del portafolio se calcula teniendo en cuenta el [!UICONTROL Benefit] total del [!UICONTROL Portfolio] y el total de los [!UICONTROL Budgeted Costs] de los proyectos. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>El valor de ROI del portafolio se calcula con la siguiente fórmula:</p> <p><em>ROI del portafolio = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Para obtener más información sobre cómo se calcula el ROI de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcular el retorno de la inversión (ROI)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] o [!UICONTROL Alignment Score] </td> 
   <td> <p>Promedio de todos los valores de [!UICONTROL Project Alignment Score], que se calculan después de completar el [!UICONTROL Scorecard] en el [!UICONTROL Business Case] del proyecto. La puntuación de alineación de cada proyecto se indica en la columna [!UICONTROL Alignment] del [!UICONTROL Portfolio Optimizer]. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>Para obtener más información sobre cómo generar una puntuación de alineación para un proyecto, consulte el artículo <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>Suma de todos los [!UICONTROL Net Values] de todos los proyectos del portafolio. Esto es visible desde cualquier pestaña dentro de un portafolio.</p> <p>Para obtener más información sobre cómo se calcula el [!UICONTROL Net Value] para un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor neto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finanzas del portafolio para los proyectos seleccionados {#portfolio-finances-for-selected-projects}

![Finanzas de Portfolio](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nombre de campo</strong> </th> 
   <th><strong>Descripción</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Number of projects]</td> 
   <td> <p>Número total de proyectos activos en el portafolio. Los proyectos que se consideran activos en un portafolio pueden estar en cualquiera de los siguientes estados:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approved]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>Puede actualizar manualmente este campo para indicar cuál es el presupuesto total para todo el portafolio. Este presupuesto se utiliza para todos los proyectos dentro del portafolio. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining]</td> 
   <td> <p>El presupuesto restante después del [!UICONTROL Costo total] en todos los proyectos dentro del portafolio se ha restado del Presupuesto del portafolio.</p> <p>El [!UICONTROL Remaining Portfolio Budget] se calcula mediante la siguiente fórmula:</p> <p><em>[!UICONTROL Remaining Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - [!UICONTROL Budgeted Cost] total de todos los proyectos del portafolio</em> </p> <p>El presupuesto del portafolio es una entrada manual en el campo Presupuesto de Portfolio Optimizer. </p> <p>Para obtener más información sobre el seguimiento de los costes de un proyecto, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Cost]</td> 
   <td> <p>Suma de los costes de todos los proyectos mostrados en el [!UICONTROL Portfolio Optimizer]. El coste de cada proyecto es el mismo que el [!UICONTROL Budgeted Cost] del proyecto, tal como se muestra en el [!UICONTROL Business Case Summary]. </p> <p>Para obtener más información sobre los campos financieros de los proyectos en el [!UICONTROL Business Case], consulte la sección “Explicación de los campos financieros en el caso empresarial” en el artículo <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Crear un caso empresarial para un proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>Suma de todos los [!UICONTROL Potential Risk Costs] de todos los proyectos del portafolio. El [!UICONTROL Potential Risk Cost] de cada proyecto se indica en la columna [!UICONTROL Risk] del [!UICONTROL Portfolio Optimizer]. </p> <p>Para obtener más información sobre cómo calcular los riesgos de los proyectos, consulte el artículo <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular el coste potencial de riesgos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>Suma de todos los valores de [!UICONTROL Planned Benefit] de todos los proyectos del portafolio. El valor de Beneficio planificado de cada proyecto se indica en la columna [!UICONTROL Benefit] del [!UICONTROL Portfolio Optimizer]. </p> <p>Para obtener más información sobre el [!UICONTROL Planned Benefit] de un proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Información general sobre el beneficio planificado del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicador de [!UICONTROL Risk to Net Value]</td> 
   <td> <p>Mide el valor de [!UICONTROL Potential Risk], teniendo en cuenta el [!UICONTROL Net Value] proporcionado por todos los proyectos del portafolio. Para lograr la máxima eficiencia dentro del portafolio, es conveniente que el indicador [!UICONTROL Risk] sea bajo y el indicador [!UICONTROL Net Value] sea alto. </p> <p>Para obtener más información acerca del cálculo del riesgo del [!UICONTROL Net Value], consulte el artículo <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcular el riesgo del valor neto en un portafolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar el [!UICONTROL Optimizador de portafolios]

Puede personalizar solo el área de la lista de proyectos del [!UICONTROL Optimizador de portafolios] mediante la configuración para cambiar la información de la lista.

Los siguientes iconos y opciones están disponibles para el [!UICONTROL Optimizador de portafolios]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icono en el Optimizador de portafolios</strong></td> 
   <td><strong>Nombre</strong></td> 
   <td><strong>Función</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Set project priority]</td> 
   <td><p>Utilice este icono cuando desee guardar el pedido del proyecto, según su prioridad.</p>
   <p>Debe tener permisos de administración en todos los proyectos de la lista para poder usar <b>Establecer prioridad de proyecto</b></p>.
    </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimize portfolio]</td> 
   <td>Utilice este icono para optimizar el portafolio en función de los siguientes valores financieros de los proyectos:
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>[!UICONTROL Value]</li>
     <li>[!UICONTROL Risk to Benefit]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Para obtener más información acerca de cómo optimizar su portafolio, consulte el artículo <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimizar proyectos en el [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Iconos de [!UICONTROL Undo]/ [!UICONTROL Redo]</td> 
   <td>Utilice estos iconos para cancelar o rehacer los cambios realizados en [!UICONTROL Portfolio Optimizer] antes de guardar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/[!UICONTROL Hide] proyectos sin marcar</td> 
   <td>Utilice estos iconos para mostrar u ocultar los proyectos del portafolio que haya desmarcado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilice este icono para exportar los datos del área de [!UICONTROL Project Prioritization] del [!UICONTROL Portfolio Optimizer]. Se puede exportar a los siguientes formatos:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>Delimitado por [!UICONTROL Tab]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Utilice este icono para modificar los campos de proyecto mostrados en las columnas del [!UICONTROL Portfolio Optimizer] o para modificar los proyectos que se muestran en el [!UICONTROL Optimizer] según sus estados. </p> <p>Sugerencia:  
     <ul> 
      <li> <p>No todos los campos estándar de [!DNL Workfront]están disponibles para añadir en las columnas. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Solo puede añadir los campos personalizados que tengan un valor distinto de cero en cualquiera de los proyectos del portafolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
