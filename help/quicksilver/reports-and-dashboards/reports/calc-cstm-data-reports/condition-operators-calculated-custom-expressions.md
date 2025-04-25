---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operadores de condición en expresiones personalizadas calculadas
description: Puede utilizar operadores o modificadores de condición al crear datos personalizados calculados en Adobe Workfront cuando utilice el modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 100%

---

# Operadores de condición en campos personalizados calculados

<!-- Audited: 2/2024 -->

Puede utilizar operadores o modificadores de condición al crear datos personalizados calculados en Adobe Workfront cuando utilice el modo de texto. Para obtener información acerca del uso del modo de texto en Workfront, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Los operadores o modificadores de condición ayudan a crear una instrucción de condición conectando los campos de Workfront existentes en las instrucciones y generando un nuevo campo. El uso más común de los operadores de condición es generar la condición de una instrucción &quot;IF&quot;.

Puede utilizar instrucciones &quot;IF&quot; en Workfront para comparar, dar formato y agrupar campos de datos con fines de creación de informes y datos personalizados.

Puede crear instrucciones &quot;IF&quot; para los siguientes elementos de Workfront:

* Vistas
* Agrupaciones
* Campos personalizados calculados

Para obtener más información acerca de la creación de instrucciones &quot;IF&quot;, consulte [Información general sobre instrucciones &quot;IF&quot;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Los ejemplos de esta guía ilustran el uso de operadores de condición en campos personalizados calculados. También puede utilizarlos en columnas o agrupaciones personalizadas calculadas cuando siga la sintaxis correcta para los campos personalizados calculados en los informes.

Para obtener información acerca de la diferencia de sintaxis entre los campos personalizados calculados y los datos personalizados calculados en los informes, consulte [Campos personalizados calculados frente a columnas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Consulte el Explorador de API para buscar los campos a los que desea hacer referencia en las expresiones personalizadas calculadas. Para obtener información sobre el Explorador de API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

Puede utilizar los siguientes modificadores de condición en Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operador de condición</th> 
   <th>Sintaxis del operador de condición</th> 
   <th>Definición del operador de condición</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Igual (no distingue mayúsculas y minúsculas)</td> 
   <td>= </td> 
   <td> <p>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es igual al segundo campo.</p> <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha planificada de finalización con la Fecha proyectada de finalización de una tarea: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Mayor que </td> 
   <td>&gt; </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es mayor que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha planificada de finalización con la Fecha proyectada de finalización de una tarea: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Mayor o igual que </td> 
   <td>&gt;= </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es mayor o igual que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha planificada de finalización con la Fecha proyectada de finalización de una tarea: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Menor que </td> 
   <td>&lt; </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es menor que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha planificada de finalización con la Fecha proyectada de finalización de una tarea: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Menor o igual que </td> 
   <td>&lt;= </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es menor o igual que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha planificada de finalización con la Fecha proyectada de finalización de una tarea: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>No es </td> 
   <td>! </td> 
   <td> <p>Añada este operador delante de cualquiera de los operadores anteriores para negar el operador. </p> <p>Por ejemplo: </p> 
    <ul> 
     <li>Es igual a: = </li> 
     <li>No es igual a: != </li> 
    </ul> <p>Añadir este operador delante de las siguientes expresiones de datos añade una instrucción negativa a las expresiones: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>EN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Para obtener información acerca de estas expresiones de datos y una lista completa, consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Información general sobre expresiones de datos calculados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>O </td> 
   <td>|| </td> 
   <td> <p>Utilice este operador para indicar que la condición se cumple cuando la expresión encuentra el primer o el segundo valor de la instrucción. </p> <p>Por ejemplo, utilice la instrucción siguiente en un campo personalizado calculado para generar una instrucción “IF” que marque los proyectos en los estados actuales o planificados como “Activos”: </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> Y </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Utilice este operador para indicar que la condición se cumple cuando la expresión encuentra un elemento que cumple dos condiciones al mismo tiempo. </p> <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción “IF” que encuentre proyectos que están en estado actual y tienen una condición de riesgo y los marque como “Mediación necesaria”. </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
