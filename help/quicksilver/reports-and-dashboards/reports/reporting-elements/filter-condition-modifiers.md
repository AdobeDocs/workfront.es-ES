---
product-area: reporting
navigation-topic: reporting-elements
title: Modificadores de filtro y condición
description: Los modificadores de filtro y condición permiten crear filtros y establecer condiciones para dar formato a los resultados del informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 0%

---

# Modificadores de filtro y condición

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Los modificadores de filtro y condición permiten crear filtros y establecer condiciones para dar formato a los resultados del informe.

Para obtener más información acerca de cómo generar filtros, vea el artículo [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obtener más información acerca del uso del formato condicional en Vistas, vea el artículo [Uso del formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificadores de filtro y condición

Algunos modificadores están integrados y puede elegirlos en un menú desplegable dentro del filtro o de la instrucción de formato condicional. Otros modificadores solo se pueden utilizar en filtros de modo de texto.

Para obtener más información sobre cómo entender el modo de texto, vea [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obtener una lista de modificadores de lapso de tiempo integrados, consulte el artículo [Filtrar informes por lapsos de tiempo](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Puede utilizar los siguientes modificadores de condición en filtros e instrucciones de formato condicional:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificador integrado</strong> </p> </th> 
   <th> <p><strong>Modificador de modo de texto</strong> </p> </th> 
   <th> <p><strong>Descripción</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>En Blanco</strong> </p> </td> 
   <td> <p><strong>en blanco</strong> </p> </td> 
   <td> <p>El campo existe para el objeto, pero actualmente el campo no tiene un valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>No Está En Blanco</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>El campo por el que está filtrando existe y se le ha dado un valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nulo</strong> </p> </td> 
   <td> <p>El campo está en blanco o no existe. Por ejemplo, desea buscar elementos sin un ID de tarea principal. Esto significa que solo desea ver tareas independientes. El calificador para el "ID de tarea principal" sería <strong>null</strong>, ya que una tarea sin ID (en este caso el principal) no existe. </p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>El campo por el que está filtrando existe y contiene un valor distinto de nulo.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contiene</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>Esta es la versión <i>sin distinción de mayúsculas y minúsculas</i> de <strong>contiene</strong>. Por ejemplo: <code>cicontains inf</code> captura cualquier valor que contenga <code>Inf</code> o <code>inf</code>.</p> <p> <p>Nota: Adobe Workfront busca la palabra o frase exacta que está especificando para cada instrucción de filtro. Por ejemplo, si está buscando un proyecto que contenga la frase <code>new project</code> en el nombre, Workfront no muestra los proyectos que tengan sólo <code>new</code>, solo <code>project</code> o <code>new main project</code> en el nombre. El filtro solo encuentra proyectos con la frase exacta <code>new project</code> en el nombre.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>No Contiene</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Esta es la versión <i>sin distinción de mayúsculas y minúsculas</i> de <strong>notcontains</strong>.</p><p>Este modificador filtra los elementos a los que les falta el valor especificado.</p> <p>Por ejemplo, <code>does not contain inf</code> captura todo lo que no contenga <code>Inf</code> o <code>inf</code> en el nombre.</p> <p>Nota: <span>Si el campo por el que está filtrando tiene varias opciones, se filtrarán los resultados que contengan tanto la opción especificada como la especificada y cualquier otra opción adicional.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contiene</strong> </p> </td> 
   <td> <p> Busca el texto <i>especificado que distingue entre mayúsculas y minúsculas</i> en toda una cadena de texto.</p> <p>Por ejemplo, al usar <code>contains Inf</code> se captura todo lo que contenga <code>Inf</code>, como la palabra <code>Infinity.</code></p> <p>Este modificador solo se puede usar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Filtra los elementos a los que les falta el valor <i>con distinción de mayúsculas y minúsculas</i> especificado.</p> <p>Por ejemplo, <code>notcontains inf</code> captura cualquier elemento sin <code>inf</code>, pero muestra los valores que contienen <code>Inf</code>.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Esta es la opción <i>sin distinción de mayúsculas y minúsculas</i> de <strong>eq</strong>. Solo devuelve una coincidencia exacta del valor buscado.</p> <p>Por ejemplo, al buscar una tarea con un nombre específico, <code>task name cieq test</code> encuentra tareas donde el nombre es <code>Test</code>, <code>TEST</code> o <code>Test</code>, pero no encuentra una tarea con el nombre <code>test 123.</code></p> <p>Al buscar un estado, no se admite el modificador <strong>cieq</strong>. Debe usar el modificador que distingue entre mayúsculas y minúsculas, <strong>eq</strong>, para buscar un estado.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Esta es la opción <i>sin distinción de mayúsculas y minúsculas</i> de <strong>ne</strong>, y es la opuesta al modificador <b>cieq</b>. Solo devuelve resultados que no coinciden exactamente con el valor buscado, sin tener en cuenta las mayúsculas y minúsculas del valor.</p> <p>Por ejemplo, <b>cine</b> devuelve cualquier valor que no sea igual a "actual" o "Actual". </p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Este modificador devuelve solamente una coincidencia exacta, <i>distingue entre mayúsculas y minúsculas</i> del valor buscado.</p> <p>Por ejemplo, al buscar proyectos completos, <code>eq CPL</code> devuelve todos los proyectos con el estado Completo. <code>eq CPL, CUR</code> no devuelve un resultado porque un proyecto no puede estar completo y ser actual al mismo tiempo.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Este es <i>el opuesto de <strong>eq</strong> que distingue entre mayúsculas y minúsculas</i>. Devuelve solo los resultados que no coinciden exactamente con el valor buscado, y también coincide con las mayúsculas y minúsculas del valor.</p> <p>Por ejemplo, <b>ne</b> devuelve cualquier valor que no sea igual a "Actual", pero no devuelve ningún valor que no sea igual a "actual". </p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> Esta es la versión <i>sin distinción de mayúsculas y minúsculas</i> de <strong>en</strong>.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>Esta es la versión <i>sin distinción de mayúsculas y minúsculas</i> de <strong>notin</strong>.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Igual</strong> </p> </td> 
   <td> <p><strong>en</strong> </p> </td> 
   <td> <p>Este modificador le permite crear una lista separada por comas de <i>variables que distinguen entre mayúsculas y minúsculas</i> para compararlas con un único atributo evaluado en un filtro. Toda la lista se trata como una instrucción OR y devuelve cualquier resultado que cumpla los criterios de una o varias variables.</p> <p>Por ejemplo, al buscar proyectos, al usar <code>in CUR, PLN, CPL</code> se devuelven todos los proyectos que están en el estado Actual, O Planificación, O Finalización.</p> <p>El modificador integrado <strong>Equal</strong> corresponde al modificador de modo de texto <strong>in</strong>. Esto significa que puede elegir Igual con varios valores para el campo.</p> <p>Por ejemplo, puede elegir "Estado es igual a Actual, Planificación, Muerto" en un informe de proyecto y puede ver proyectos en cualquiera de estos estados.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>No es igual a</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>Este es el <i>extremo que distingue entre mayúsculas y minúsculas</i> opuesto a <strong>en</strong>. Devuelve solo los resultados que no están en la lista especificada.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> <p>Nota: <span>Si el campo por el que está filtrando tiene varias opciones, se filtrarán los resultados que contengan tanto la opción especificada como la especificada y cualquier otra opción adicional.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>me gusta</strong> </p> </td> 
   <td> <p>Este modificador busca partes de una cadena de texto <i>que distingue entre mayúsculas y minúsculas</i> de manera similar a <strong>contiene</strong>. Sin embargo, <strong>like</strong> permite insertar caracteres comodín para dividir el texto.</p> <p>Por ejemplo, al buscar notas, al usar <code>like %Current% %Dead%</code> se devuelve cualquier nota que contenga la frase "Actual a Inactivo". No incluye ninguna nota que contenga "De muerto a actual". Cada valor se busca en el orden en que aparece en la lista. % representa un comodín para reemplazar caracteres o segmentos de texto. También se puede utilizar un guion bajo para un solo carácter comodín, como en <code>like Project_</code>, que devuelve "Proyecto" y "Proyectos". Si tiene intención de usar un modificador <strong>like</strong> o <strong>click</strong> en el filtro, le recomendamos que evite los caracteres % o _ en los nombres de los campos de datos personalizados, los valores de opciones de parámetros u otros nombres de objetos.</p><p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Esta es la versión <i>sin distinción de mayúsculas y minúsculas</i> de <strong>like</strong>. Por ejemplo: <code>cilike %Current% %Dead%</code> devuelve todas las notas que contienen <code>Current to Dead</code> o <code>current to dead</code>.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>No Existe</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Este modificador solo se utiliza con filtros complejos en una instrucción EXISTS. Estos filtros solo hacen referencia a los siguientes objetos: </p> 
    <ul> 
     <li>Objetos que abarcan varios niveles de la jerarquía de objetos </li> 
     <li>Objetos que faltan </li> 
    </ul> <p>Para obtener información acerca de cómo crear filtros complejos mediante instrucciones EXISTS, vea el artículo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Crear filtros complejos de modo de texto mediante instrucciones EXISTS</a>. Este es el único modificador utilizado en las instrucciones EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mayor Que</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con un valor mayor que el valor introducido, sin incluir el valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menos De</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con un valor menor que el introducido, sin incluir el valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mayor o igual que</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con valores mayores o iguales al valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor o igual que</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con un valor menor o igual que el valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Entre</strong> </p> </td> 
   <td> <p><strong>entre</strong> </p> </td> 
   <td> <p>Proporciona dos valores de campo requeridos y busca todos los resultados dentro del intervalo de ambos campos, incluidos los valores introducidos.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Esto es lo contrario a <strong>between</strong>. Proporciona dos campos de valor requeridos y busca todos los resultados fuera del intervalo de ambos campos, incluidos los valores introducidos.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, vea <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p> </td> 
  </tr>

</tbody> 
</table>
