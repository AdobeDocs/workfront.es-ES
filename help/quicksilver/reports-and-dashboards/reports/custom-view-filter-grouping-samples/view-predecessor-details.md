---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: detalles de predecesoras"
description: Esta vista de tareas muestra detalles de las tareas predecesoras de las tareas mediante una vista de colección. En una vista de colección, puede mostrar información sobre objetos que están en una relación "uno a varios". En este caso, cada tarea (una) puede tener varias predecesoras (muchas). La vista muestra el nombre de las tareas, así como los nombres de sus predecesoras, los nombres de proyecto de sus predecesoras, las fechas planificadas de finalización de sus predecesoras y los estados de sus predecesoras.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Ver: detalles de predecesoras

Esta vista de tareas muestra detalles de las tareas predecesoras de las tareas mediante una vista de colección. En una vista de colección, puede mostrar información sobre objetos que están en una relación &quot;uno a varios&quot;. En este caso, cada tarea (una) puede tener varias predecesoras (muchas). La vista muestra el nombre de las tareas, así como los nombres de sus predecesoras, los nombres de proyecto de sus predecesoras, las fechas planificadas de finalización de sus predecesoras y los estados de sus predecesoras.

Para obtener información sobre las referencias a colecciones en los informes, consulte [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Ver detalles del predecesor

1. Ir a una lista de tareas.
1. Desde el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Previsualización de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y luego haga clic en **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en la **Modo de texto** y reemplácelo por el siguiente código:
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecesores Números y nombres<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(predecesors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecessor}).{taskNumber},' - ',{predecessor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Predecesores Nombres de proyecto<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecesors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}.{proyecto}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Fechas de finalización de predecesoras<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecesors).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}.{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Estado de predecesoras<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(predecesors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}.{status}<br>column.4.valueformat=HTML</pre>

1. Clic **Guardar vista**.
