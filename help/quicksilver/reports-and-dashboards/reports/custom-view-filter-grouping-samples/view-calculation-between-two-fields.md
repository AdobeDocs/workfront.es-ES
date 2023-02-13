---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: mostrar el resultado de un cálculo entre dos campos de una columna"'
description: Se puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Ver: mostrar el resultado de un cálculo entre dos campos de una columna

Se puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos.

Por ejemplo, si desea averiguar el número de días de la semana que transcurrieron entre dos fechas, puede utilizar la sintaxis del modo de texto y las expresiones de datos para calcular esta diferencia.\
Por ejemplo, puede calcular la diferencia de día de la semana entre la Fecha de Finalización Planificada y la Fecha de Finalización Real de una tarea y mostrar el resultado en una columna.

Puede utilizar otras dos fechas en este cálculo (Inicio real, Finalización real, Inicio proyectado, Finalización proyectada, etc.).\
Para obtener más información sobre las expresiones de datos calculadas, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar el resultado de un cálculo entre dos campos de una columna

Para agregar esta columna a una vista de tareas:

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna**, luego **Cambiar al modo de texto**.

1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre>display_name=Week Day Diferencia<br>textmode=true<br>valueexpression=WEEKDAYDIFF({scheduledCompletionDate},{actualCompletionDate})<br>value=format=HTML</pre>

1. (Opcional) Para acumular los valores mostrados en la vista en una agrupación, siga los pasos descritos en [Agrupación: mostrar el resultado de agregar varios valores calculados en una agrupación](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Haga clic en **Guardar**, luego **Guardar vista**.
