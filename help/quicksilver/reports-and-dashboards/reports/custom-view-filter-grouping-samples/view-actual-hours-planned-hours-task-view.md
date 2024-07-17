---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Horas reales sobre horas planificadas en la misma columna de un tarea Ver'
description: En este tarea vista, la cantidad real de horas registradas en una tarea se muestra a lo largo de las horas planificadas para cada tarea.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# Ver: Horas reales sobre horas planificadas en la misma columna de una tarea Ver

En esta vista de tareas, la cantidad real de horas registradas en una tarea se muestra a lo largo de las horas planificadas para cada tarea.

![informe_de_tareas_real_vs_planificado_en.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems Plan Workfront*</td> 
   <td> <p>Cualquier</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Licencia Workfront*</td> 
   <td> <p>Solicitud de modificación de un vista </p>
   <p>plan modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si aún no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objetos</td> 
   <td> <p>Administrar permisos para un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, tipo de licencia o acceso tiene, comuníquese con el administrador de Workfront.

## Ver horas reales sobre las horas planificadas en un tarea vista

Para aplicar este vista:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar a modo de texto**.
1. Pase el ratón sobre el área Modo de texto y haga clic en Haga clic **para editar el texto**.
1. Quitar el texto que encuentra en el **cuadro Modo de** texto y sustitúyalo por el siguiente código:
   <pre>column.0.descriptionkey=name<br>column.0.vincular.linkproperty.0.name=ID<br>column.0.vincular.linkproperty.0.valuefield=ID<br>column.0.vincular.linkproperty.0.valueformat=int<br>column.0.vincular.lookup=vincular.vista<br>column.0.vincular.valuefield=objCode<br>column.0.vincular.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Actual/ Planned Hours<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours Variance<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Pulse **Guardar vista**.
