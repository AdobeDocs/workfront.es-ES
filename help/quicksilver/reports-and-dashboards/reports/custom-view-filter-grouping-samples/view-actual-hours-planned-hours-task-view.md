---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: Horas reales sobre horas planificadas en la misma columna de una vista de tarea"'
description: En esta vista de tareas, la cantidad real de horas registradas en una tarea se muestra a lo largo de las horas planificadas para cada tarea.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Ver: Horas reales sobre horas planificadas en la misma columna de una vista de tarea

En esta vista de tareas, la cantidad real de horas registradas en una tarea se muestra a lo largo de las horas planificadas para cada tarea.

![actual_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

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

## Ver horas reales sobre horas planificadas en una vista de tareas

Para aplicar esta vista:

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.value.format=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.value.format=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.name=name.abbr<br>column.0.querysort=name<br>column.0.abreviview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=asignaciones<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=asignaciones<br>column.1.valuefield=assignedListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignments.list<br>column.2.displayname=Real/ Horario planificado<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({realWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.value eformat=complex<br>column.2.viewalias=actualworkrequired<br>column.3.agregator.function=SUM<br>column.3.agregator.valueexpression=SUB({realWork}, {workRequired})<br>column.3.gregator.value.format=components<br>column.3.displayname=Variación de horas<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({realWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Haga clic en **Guardar vista**.
