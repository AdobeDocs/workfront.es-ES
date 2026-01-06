---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Información general sobre los campos financieros del caso empresarial
description: La subpestaña Caso comercial incluye los campos financieros del proyecto. Para que algunos de los campos financieros tengan valores, se deben completar las áreas correspondientes del caso empresarial.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 82%

---

# Información general sobre los campos financieros del caso empresarial

La subpestaña Caso comercial incluye los campos financieros del proyecto. Para que algunos de los campos financieros tengan valores, se deben completar las áreas correspondientes del caso empresarial.

Se muestran los siguientes campos financieros del proyecto en el caso comercial:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Nombre del campo</th> 
   <th scope="col">Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Alineado </td> 
   <td> <p>Muestra la alineación del proyecto según su cuadro de resultados. Un valor porcentual alto indica que el proyecto está bien alineado con la finalidad y los objetivos de la organización. <br>Para obtener más información sobre el uso de los cuadros de resultados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Crear un cuadro de resultados</a>.</p> <p>Este campo se muestra en el área Resumen de caso empresarial. </p> </td> 
  </tr> 
  <tr> 
   <td>Costo presupuestado</td> 
   <td> <p>El coste total estimado que se asociará al proyecto cuando se inicia.</p> <p>El coste presupuestado del proyecto se calcula mediante la siguiente fórmula:<br></p> <p><code>Budgeted Cost = Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront utiliza las horas presupuestadas del planificador de recursos para calcular el costo de mano de obra presupuestado.<br>Para obtener más información sobre el cálculo del costo presupuestado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular costo presupuestado</a>. </p> <p>Este campo se muestra en el área Resumen de caso empresarial.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo de gasto presupuestado</td> 
   <td> <p>El coste presupuestado de todos los gastos del proyecto. </p> <p>Esto se calcula mediante la fórmula siguiente:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Para obtener más información sobre el cálculo de gastos, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Administrar gastos de proyecto </a>.</p> <p>Este campo se muestra en el área Gastos.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo de mano de obra presupuestado</td> 
   <td> <p>Coste asociado a los recursos asignados para completar el trabajo en el proyecto.</p> <p>El coste de mano de obra presupuestado para el proyecto se calcula mediante la siguiente fórmula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront utiliza las horas presupuestadas del planificador de recursos para calcular el costo de mano de obra presupuestado.<br>Para obtener más información sobre el cálculo del coste de mano de obra presupuestado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el coste de mano de obra presupuestado y las horas presupuestadas para los proyectos</a>.</p> <p>Este campo se muestra en el área de Presupuestación de recursos del caso empresarial. </p> </td> 
  </tr> 
  <tr> 
   <td>Coste planificado de gastos</td> 
   <td> <p>Es igual que el coste presupuestado de gastos. </p> <p>Nota: El coste planificado de gastos es diferente del coste planificado del proyecto. El coste planificado de gastos se calcula a partir del importe planificado de los gastos del proyecto, mientras que el coste planificado se calcula usando las horas planificadas del proyecto. </p> <p>Este campo se muestra en el área Gastos para cada gasto.</p> </td> 
  </tr> 
  <tr> 
   <td>Valor neto</td> 
   <td> <p>Es el valor total previsto del proyecto después de calcular su beneficio y eliminar los costes.</p> <p>El valor neto del proyecto se calcula mediante la siguiente fórmula:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Para obtener más información sobre el cálculo del valor neto, consulte <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor neto</a>.<br></p> <p>Este campo se muestra en el área Resumen de caso empresarial.</p> </td> 
  </tr> 
  <tr> 
   <td>Beneficio planificado</td> 
   <td>Una estimación manual del beneficio monetario para su organización cuando se complete este proyecto. Puede ser cualquier cantidad de dinero y es específico para usted y para cada proyecto que administre. El Beneficio planificado no puede tener un valor negativo. Este campo se muestra en el área Resumen de caso comercial y se puede editar en el área Información del proyecto del caso empresarial. </td> 
  </tr> 
  <tr> 
   <td>Costo potencial de los riesgos</td> 
   <td> <p>Este es el coste potencial de todos los riesgos del proyecto. </p> <p>Se calcula mediante la fórmula siguiente:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Para obtener más información sobre los riesgos del proyecto, vea <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Crear y editar riesgos en proyectos</a>.</p> <p>Este campo se muestra en el área Resumen de caso empresarial.</p> </td> 
  </tr> 
  <tr> 
   <td>Riesgo potencial</td> 
   <td> <p>En el Resumen de caso comercial, se trata del importe del coste de todos los riesgos en caso de que se produzcan, en función de su probabilidad. Por ejemplo, si un riesgo tiene un costo potencial de 100 dólares y una probabilidad de que ocurra del 10%, el riesgo potencial es de 10 dólares. El riesgo potencial en el resumen del caso empresarial se calcula mediante la siguiente fórmula:</p> <p><code>Potential Risk = SUM(Risk Potential Cost x Probability)</code> para todos los riesgos. </p> </td> 
  </tr> 
  <tr> 
   <td>Coste de mitigación del riesgo</td> 
   <td> <p>El costo del plan de mitigación para los riesgos que está estimando podría ocurrir en el proyecto.<br>Para obtener más información acerca de los riesgos del proyecto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Crear y editar riesgos en proyectos</a>.</p> <p>Este campo se muestra en el área Riesgos para cada riesgo especificado en el proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Coste potencial de un riesgo</td> 
   <td> <p>El coste financiero estimado cuando los riesgos definidos en el proyecto se producirían de forma efectiva, independientemente de su probabilidad. </p> <p>Este es un campo actualizado manualmente que se muestra en cada riesgo del área Riesgos del caso empresarial. </p> </td> 
  </tr> 
  <tr> 
   <td>Coste potencial total de los riesgos</td> 
   <td> <p>Es el coste financiero total estimado de todos los riesgos definidos en el proyecto cuando realmente se han producido. </p> <p>Esto se calcula mediante la fórmula siguiente:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Se muestra como un número de moneda junto al título del área Riesgos del caso empresarial.</p> </td> 
  </tr> 
 </tbody> 
</table>
