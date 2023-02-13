---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operadores de condición en expresiones personalizadas calculadas
description: Puede utilizar operadores de condición o modificadores al crear datos personalizados calculados en Adobe Workfront al utilizar el modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# Operadores de condición en campos personalizados calculados

Puede utilizar operadores de condición o modificadores al crear datos personalizados calculados en Adobe Workfront al utilizar el modo de texto.

Para obtener información sobre el uso del modo de texto en Workfront, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Los operadores o modificadores de condición ayudan a crear una instrucción de condición conectando los campos Workfront existentes en las instrucciones y generando un nuevo campo. El uso más común de los operadores de condición es crear la condición de una instrucción &quot;IF&quot;.

Puede utilizar las instrucciones &quot;IF&quot; en Workfront para comparar, dar formato y agrupar campos de datos para generar informes y datos personalizados.

Puede crear instrucciones &quot;IF&quot; para los siguientes elementos de Workfront:

* Vistas
* Agrupaciones
* Campos personalizados calculados

Para obtener más información sobre la creación de instrucciones &quot;IF&quot;, consulte [Resumen de las instrucciones &quot;IF&quot;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Los ejemplos de esta guía ilustran el uso de operadores de condición en campos personalizados calculados. También puede utilizarlos en columnas o agrupaciones personalizadas calculadas, cuando siga la sintaxis correcta para los campos personalizados calculados en los informes.

Para obtener información sobre la diferencia de sintaxis entre los campos personalizados calculados y los datos personalizados calculados en los informes, consulte [Campos personalizados calculados vs. columnas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Consulte el Explorador de API para encontrar los campos a los que desea hacer referencia en las expresiones personalizadas calculadas. Para obtener información sobre el Explorador de API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

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
   <td> <p>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es igual al segundo campo.</p> <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha de Finalización Planificada con la Fecha de Finalización Prevista de una tarea: </p><pre>IF({estimatedCompletionDate}={scheduledCompletionDate},"On Track","Off Track")</pre> </td> 
  </tr> 
  <tr> 
   <td>Bueno que </td> 
   <td>&gt; </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es bueno que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha de Finalización Planificada con la Fecha de Finalización Prevista de una tarea: </p><pre>IF({estimatedCompletionDate}&gt;{scheduledCompletionDate},"Late",")</pre></td> 
  </tr> 
  <tr> 
   <td>Bueno que o igual a </td> 
   <td>&gt;= </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es bueno o igual al segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha de Finalización Planificada con la Fecha de Finalización Prevista de una tarea: </p><pre>IF({estimatedCompletionDate}&gt;={scheduledCompletionDate},"Late","Pre")</pre></td> 
  </tr> 
  <tr> 
   <td>Menor que </td> 
   <td>&lt; </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es menor que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha de Finalización Planificada con la Fecha de Finalización Prevista de una tarea: </p><pre>IF({estimatedCompletionDate}&lt;{scheduledCompletionDate},"Temprano",")</pre></td> 
  </tr> 
  <tr> 
   <td>Menor o igual que </td> 
   <td>&lt;= </td> 
   <td>Utilice este operador para indicar que la condición se cumple cuando el primer campo de la instrucción es menor o igual que el segundo campo. <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que compare la Fecha de Finalización Planificada con la Fecha de Finalización Prevista de una tarea: </p><pre>IF({estimatedCompletionDate}&lt;={scheduledCompletionDate},"Pre","Late")</pre></td> 
  </tr> 
  <tr> 
   <td>No </td> 
   <td>! </td> 
   <td> <p>Agregue este operador delante de cualquiera de los operadores anteriores para denegar el operador. </p> <p>Por ejemplo: </p> 
    <ul> 
     <li>Es igual a: = </li> 
     <li>No es igual a: != </li> 
    </ul> <p>Al agregar este operador delante de las siguientes expresiones de datos, se agrega una sentencia negativa a las expresiones: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>EN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Para obtener información sobre estas expresiones de datos y una lista completa, consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Expresiones de datos calculadas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>O </td> 
   <td>|| </td> 
   <td> <p>Utilice este operador para indicar que la condición se cumple cuando la expresión encuentra el primer o el segundo valor de la instrucción. </p> <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que marque los proyectos en los estados Actual o Planning como "Activo": </p><pre>IF({status}="PLN"||{status}="CUR","Activo","No activo")</pre> </td> 
  </tr> 
  <tr> 
   <td> Y </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Utilice este operador para indicar que la condición se cumple cuando la expresión encuentra un elemento que cumple dos condiciones al mismo tiempo. </p> <p>Por ejemplo, utilice la siguiente instrucción en un campo personalizado calculado para generar una instrucción "IF" que encuentre proyectos que estén en estado actual y que tengan una condición de en riesgo y los marque como "Mediación necesaria". </p><pre>IF({status}="CUR"&amp;{condition}="AR","Mediación necesaria",")</pre> </td> 
  </tr> 
 </tbody> 
</table>
