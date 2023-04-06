---
product-area: reporting
navigation-topic: reporting-elements
title: Modificadores de filtro y condición
description: Los modificadores de filtro y condición permiten crear filtros y establecer condiciones para dar formato a los resultados del informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# Modificadores de filtro y condición

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Los modificadores de filtro y condición permiten crear filtros y establecer condiciones para dar formato a los resultados del informe.

Para obtener más información sobre la creación de filtros, consulte el artículo [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obtener más información sobre el uso del formato condicional en las vistas, consulte el artículo [Utilizar el formato condicional en las vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificadores de filtro y condición

Para obtener una lista de modificadores de lapso de tiempo integrados, consulte el artículo [Filtrado de informes por intervalos de tiempo](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Algunos modificadores están integrados y puede seleccionarlos en un menú desplegable dentro del filtro o de la afirmación de formato condicional. Otros modificadores solo se pueden utilizar en filtros de modo de texto. Para obtener más información sobre la comprensión del modo de texto, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Puede utilizar los siguientes modificadores de condición en filtros y afirmaciones de formato condicional:

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
   <td> <p><strong>En blanco</strong> </p> </td> 
   <td> <p><strong>en blanco</strong> </p> </td> 
   <td> <p>El campo existe para el objeto, pero aún no se ha dado un valor al campo.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>No en blanco</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>El campo que está filtrando existe y se le ha dado un valor.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>El campo está en blanco o no existe. Por ejemplo, desea buscar elementos sin un ID de tarea principal. Esto significa que desea ver solo tareas independientes. El calificador para el "ID de tarea principal" sería <strong>null</strong>, ya que una tarea sin ID (en este caso el principal) no existe. </p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>El campo que está filtrando existe y contiene un valor que no es nulo.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contiene</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>(Sin distinción de mayúsculas y minúsculas) Esta es una versión de <strong>contains</strong>. Por ejemplo: "cicontains inf" captura cualquier valor que contenga "Inf" o "inf".</p> <p> <p>Nota: Adobe Workfront busca la palabra o frase exacta que está especificando para cada instrucción de filtro. Por ejemplo, si está buscando cualquier proyecto que contenga la frase "nuevo proyecto" en el nombre, Workfront no muestra proyectos que solo tengan "nuevo", "proyecto" o "nuevo proyecto principal" en el nombre. El filtro encuentra solo proyectos con la frase exacta "nuevo proyecto" en el nombre.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(Sin distinción de mayúsculas y minúsculas) Esta es una opción que no distingue entre mayúsculas y minúsculas de <strong>eq</strong>. Solo devuelve una coincidencia exacta del valor buscado.</p> <p>Por ejemplo, al buscar una tarea con un nombre específico, "nombre de tarea cieq test" encuentra tareas donde el nombre es "Prueba", "PRUEBA" o "Prueba", pero no encuentra una tarea con el nombre "prueba 123".</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cin</strong> </p> </td> 
   <td> <p>(Sin distinción de mayúsculas y minúsculas) Esta es una versión de <strong>en</strong>.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Esta es una versión de <strong>like</strong>. Por ejemplo: "cilike %Current% %Dead%" devuelve cualquier nota que contenga "Current to Dead" o "current to Death".</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>(Sin distinción de mayúsculas y minúsculas) Esta es una versión de <strong>notin</strong>.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre la creación de filtros mediante el modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contiene</strong> </p> </td> 
   <td> <p>(Distinción entre mayúsculas y minúsculas) Busca el texto especificado en toda una cadena de texto.</p> <p>Por ejemplo, si se usa "contiene información", se capturará cualquier cosa que contenga "información", como la palabra "infinito".</p> <p>Este modificador solo se puede usar en filtros de modo de texto. Para obtener más información acerca del modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>No contiene</strong> </p> </td> 
   <td> <p><strong>cinotcontiene</strong> </p> </td> 
   <td> <p>(Sin distinción de mayúsculas y minúsculas) Filtra los elementos que no tienen el valor especificado.</p> <p>Por ejemplo, "no contiene inf" captura cualquier cosa sin "Inf" o "inf" en el nombre.</p> <p>Nota: <span>Si el campo que está filtrando tiene varias opciones, filtrará los resultados que contienen tanto la opción que especifique, así como la opción que especifique y cualquier opción adicional.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>No existe</strong> </td> 
   <td><strong>NOTEXISTAS</strong> </td> 
   <td> <p>Este modificador solo se utiliza con filtros complejos en una instrucción EXISTS. Estos filtros solo hacen referencia a los siguientes objetos: </p> 
    <ul> 
     <li>Objetos que abarcan varios niveles en la jerarquía de objetos </li> 
     <li>Objetos que faltan </li> 
    </ul> <p>Para obtener información sobre la creación de filtros complejos mediante instrucciones EXISTS, consulte el artículo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Crear filtros complejos en modo texto usando instrucciones EXISTS</a>. Este es el único modificador utilizado en las instrucciones EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Igual (no distingue mayúsculas y minúsculas)</strong> </p> </td> 
   <td> <p><strong>en</strong> </p> </td> 
   <td> <p>(Distinción entre mayúsculas y minúsculas) Este modificador permite crear una lista de variables separadas por coma para compararlas con un único atributo evaluado en un filtro. La lista completa se trata como una instrucción OR y devuelve los resultados que cumplen los criterios de una o más de las variables.</p> <p>Por ejemplo, cuando se buscan proyectos, el uso de "en CUR, PLN, CPL" devuelve todos los proyectos que están en estado Actual, O Planificación, O Completado.</p> <p>El modificador integrado <strong>Igual</strong> corresponde al modificador de modo de texto de <strong>en</strong>. Esto significa que puede elegir Equal with multiple values para el campo .</p> <p>Por ejemplo, puede elegir un "Estado es igual a Actual, Planificación, Muerto" en un informe de proyecto y puede ver los proyectos en cualquiera de estos estados.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(Con distinción de mayúsculas y minúsculas) Esto solo devuelve una coincidencia exacta del valor buscado.</p> <p>Por ejemplo, al buscar proyectos completos, "eq CPL" devuelve todos los proyectos en estado completo. "eq CPL, CUR" no devuelve un resultado porque un proyecto no puede estar completo y actualizado al mismo tiempo.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el uso del modo de texto para crear filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mayor que</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con un valor bueno al valor introducido, sin incluir el valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>(Distinción entre mayúsculas y minúsculas) Busca partes de una cadena de texto de forma similar a <strong>contains</strong>. Sin embargo, <strong>like</strong> permite insertar caracteres comodín para dividir el texto.</p> <p>Por ejemplo, cuando se buscan notas, el uso de "como %Current% %Dead%" devuelve cualquier nota que contenga la frase "De actual a muerto". No incluye ninguna nota que contenga "Muerta a la actual". Cada valor se busca en el orden en que aparece en la lista. El % representa un comodín para reemplazar caracteres o segmentos de texto.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor que</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con un valor inferior al introducido, sin incluir el valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mayor o igual a</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con valores buenos o iguales al valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Menor o igual a</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Esto busca todos los resultados con un valor menor o igual que el valor introducido.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Entre</strong> </p> </td> 
   <td> <p><strong>entre</strong> </p> </td> 
   <td> <p>Proporciona dos valores de campo requeridos y busca todos los resultados dentro del rango de ambos campos, incluidos los valores introducidos.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>(Distinción entre mayúsculas y minúsculas) Filtra los elementos que no tengan el valor especificado.</p> <p>Por ejemplo, "notcontains inf" captura cualquier cosa con sin "inf", pero muestra valores que contienen "Inf".</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Esto es lo contrario de <strong>entre</strong>. Proporciona dos campos de valor requeridos y busca todos los resultados fuera del rango de ambos campos, incluidos los valores introducidos.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>no es igual</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>(Con distinción de mayúsculas y minúsculas) Es lo contrario a <strong>en</strong>. Solo devuelve resultados que no están en la lista especificada.</p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> <p>Nota: <span>Si el campo que está filtrando tiene varias opciones, filtrará los resultados que contienen tanto la opción que especifique, así como la opción que especifique y cualquier opción adicional.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(Con distinción de mayúsculas y minúsculas) Es lo contrario a <strong>eq</strong>. Devuelve solo los resultados que no coinciden exactamente con el valor buscado, y también coincide con el caso del valor.</p> <p>Por ejemplo, <b>ne</b> devuelve cualquier valor que no sea igual a "Actual", pero que no devuelva ningún valor que no sea igual a "actual". </p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>(Sin distinción de mayúsculas y minúsculas) Esta es una opción que no distingue entre mayúsculas y minúsculas de <strong>ne</strong> y es lo opuesto al <b>cieq</b> modificador. Solo devuelve resultados que no coinciden exactamente con el valor buscado, sin tener en cuenta las mayúsculas y minúsculas del valor.</p> <p>Por ejemplo, <b>cine</b> devuelve cualquier valor que no sea igual a "actual" o "actual". </p> <p>Este modificador solo se puede utilizar en filtros de modo de texto. Para obtener más información sobre el modo de texto en los filtros, consulte <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edición de un filtro mediante el modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
