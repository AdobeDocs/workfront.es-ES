---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Información general sobre los campos financieros de Business Case
description: La subpestaña Caso de negocio incluye campos financieros para el proyecto. Para que algunos de los campos financieros tengan valores, se deben completar las áreas correspondientes del caso empresarial.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# Información general sobre los campos financieros de Business Case

La subpestaña Caso de negocio incluye campos financieros para el proyecto. Para que algunos de los campos financieros tengan valores, se deben completar las áreas correspondientes del caso empresarial.  

En el caso empresarial se muestran los siguientes campos financieros del proyecto:

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
   <td>Alineado </td> 
   <td> <p>Muestra la alineación del proyecto según su informe de valoración. Un alto valor porcentual indica que el proyecto está bien alineado con el propósito y los objetivos de la organización. <br>Para obtener más información sobre el uso de los informes de valoración, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Crear un informe de valoración</a>.</p> <p>Este campo se muestra en el área Resumen de casos comerciales . </p> </td> 
  </tr> 
  <tr> 
   <td>Costo presupuestado</td> 
   <td> <p>El coste total estimado que se asocia al proyecto cuando se inicia el proyecto.</p> <p>El coste presupuestado del proyecto se calcula mediante la fórmula siguiente:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront utiliza las horas presupuestadas del planificador de recursos para calcular el costo laboral presupuestado.<br>Para obtener más información sobre el cálculo de Coste presupuestado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular costo presupuestado</a>. </p> <p>Este campo se muestra en el área Resumen de casos comerciales .</p> </td> 
  </tr> 
  <tr> 
   <td>Costo de gasto presupuestado</td> 
   <td> <p>El costo presupuestado de todos los gastos del proyecto. </p> <p>Esto se calcula mediante la fórmula siguiente:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Para obtener más información sobre el cálculo de gastos, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Administrar los gastos del proyecto </a>.</p> <p>Este campo se muestra en el área Gastos .</p> </td> 
  </tr> 
  <tr> 
   <td>Costo de mano de obra presupuestado</td> 
   <td> <p>El coste asociado con los recursos asignados para completar el trabajo en el proyecto.</p> <p>El coste laboral presupuestado del proyecto se calcula mediante la fórmula siguiente:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Workfront utiliza las horas presupuestadas del planificador de recursos para calcular el costo laboral presupuestado.<br>Para obtener más información sobre el cálculo del coste laboral presupuestado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos</a>.</p> <p>Este campo se muestra en el área Presupuestación de recursos del caso empresarial. </p> </td> 
  </tr> 
  <tr> 
   <td>Gastos Planificados</td> 
   <td> <p>Es lo mismo que Coste de Gastos Presupuestados. </p> <p>Nota: El costo planeado de los gastos es diferente al costo planeado para el proyecto. El costo planeado de los gastos se calcula en el importe planeado de los gastos del proyecto, mientras que el costo planeado se calcula usando las horas planificadas del proyecto. </p> <p>Este campo se muestra en el área Gastos, para cada gasto.</p> </td> 
  </tr> 
  <tr> 
   <td>Valor neto</td> 
   <td> <p>Este es el valor total esperado del proyecto después de calcular su beneficio y eliminar los costes.</p> <p>El valor neto del proyecto se calcula mediante la fórmula siguiente:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Para obtener más información sobre el cálculo del valor neto, consulte <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor neto</a>.<br></p> <p>Este campo se muestra en el área Resumen de casos comerciales .</p> </td> 
  </tr> 
  <tr> 
   <td>Beneficio planificado</td> 
   <td>Una estimación manual de los beneficios monetarios para su organización cuando se complete este proyecto. Puede ser cualquier cantidad de moneda y es específica para usted y para cada proyecto que administra. El beneficio planeado no puede tener un valor negativo. Este campo se muestra en el área Resumen de casos comerciales y se puede editar en el área Información del proyecto del caso empresarial. </td> 
  </tr> 
  <tr> 
   <td>Costo potencial de los riesgos</td> 
   <td> <p>Este es el coste potencial de todos los riesgos del proyecto. </p> <p>Se calcula mediante la fórmula siguiente:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Para obtener más información sobre los riesgos en el proyecto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Crear y editar riesgos en proyectos</a>.</p> <p>Este campo se muestra en el área Resumen de casos comerciales .</p> </td> 
  </tr> 
  <tr> 
   <td>Riesgo potencial</td> 
   <td> <p>En el Resumen de Casos de Negocio, esta es la cantidad del coste de todos los riesgos si deben producirse, según su probabilidad. Por ejemplo, si un riesgo tiene un costo potencial de 100 dólares y una probabilidad de ocurrir del 10%, el riesgo potencial es de 10 dólares. El posible riesgo en el resumen del caso empresarial se calcula mediante la fórmula siguiente:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> para todos los riesgos. </p> </td> 
  </tr> 
  <tr> 
   <td>Coste de reducción de riesgos</td> 
   <td> <p>El costo del plan de mitigación de los riesgos que se estima podría ocurrir en el proyecto.<br>Para obtener más información sobre los riesgos en el proyecto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Crear y editar riesgos en proyectos</a>.</p> <p>Este campo se muestra en el área Riesgos para cada riesgo especificado en el proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo potencial para un riesgo</td> 
   <td> <p>El costo financiero estimado cuando los riesgos definidos en el proyecto se producirían, independientemente de su probabilidad. </p> <p>Se trata de un campo actualizado manualmente que se muestra en cada riesgo del área Riesgos del Caso de Negocio. </p> </td> 
  </tr> 
  <tr> 
   <td>Riesgos Total Coste Potencial</td> 
   <td> <p>Se trata del coste financiero total estimado de todos los riesgos definidos en el proyecto cuando realmente se produjeron. </p> <p>Esto se calcula mediante la fórmula siguiente:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Se muestra como un número de moneda junto al título del área Riesgos del Caso de negocio.</p> </td> 
  </tr> 
 </tbody> 
</table>
