---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: detalles del predecesor'
description: Esta vista de tareas muestra detalles de los predecesores de las tareas utilizando una vista de colección. En una vista de colección, puede mostrar información sobre los objetos que están en una relación "uno a varios". En este caso, cada tarea (una) puede tener varias predecesoras (muchas). La vista muestra el nombre de las tareas, así como los nombres de sus predecesores, los nombres de proyecto de los predecesores, las fechas de finalización previstas por los predecesores y los estados de los predecesores.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Ver: detalles del predecesor

Esta vista de tareas muestra detalles de los predecesores de las tareas utilizando una vista de colección. En una vista de colección, puede mostrar información sobre los objetos que están en una relación &quot;uno a varios&quot;. En este caso, cada tarea (una) puede tener varias predecesoras (muchas). La vista muestra el nombre de las tareas, así como los nombres de sus predecesores, los nombres de proyecto de los predecesores, las fechas de finalización previstas por los predecesores y los estados de los predecesores.

Para obtener información sobre referencias a colecciones en informes, consulte [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecesor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Ver detalles del predecesor

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecesors Números y nombres<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(predecessors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecesor}.{taskNumber},' - ',{predecesor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Predecesors Nombres de proyecto<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecessors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.value expression={predecessor}.{proyecto}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Fechas de finalización de los predecesores<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}.{scheduledCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Predecesors Status<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(predecessors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.value expression={predecessor}.{status}<br>column.4.valueformat=HTML</pre>

1. Haga clic en **Guardar vista**.
