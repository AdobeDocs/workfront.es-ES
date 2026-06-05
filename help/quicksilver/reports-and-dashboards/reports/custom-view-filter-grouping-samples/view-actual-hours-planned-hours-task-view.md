---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: Horas reales sobre Horas planificadas en la misma columna de una tarea Vista'
description: En esta vista de tareas, la cantidad real de horas registradas en una tarea se muestra a lo largo de las horas planificadas para cada tarea. La variación de horas entre las horas planificadas y las reales también se muestra en una columna independiente.
author: Courtney
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/F-2pvs6cYCOrQ9oGAg7iZa3nlLvZ7F-2durIiTykCbw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 269
ht-degree: 54%

---

# Vista: Horas reales sobre Horas planificadas en la misma columna de una tarea Vista

En esta vista de tareas, la cantidad real de horas registradas en una tarea se muestra a lo largo de las horas planificadas para cada tarea. La variación de horas entre las horas planificadas y las reales también se muestra en una columna independiente.

![actual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Requisitos de acceso

<!--Audited: 10/2024-->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vista Horas reales sobre Horas planificadas en una tarea Vista

Para aplicar este vista:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.
1. En el área **Vista previa de columnas**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Editar modo de texto**.
1. Quite el texto que encuentre en el cuadro de modo de texto y reemplácelo por el siguiente código:

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.viewalias=assignments
   column.1.displayname=
   column.1.linkedname=direct
   column.1.namekey=assignments
   column.1.valuefield=assignmentsListString
   column.1.valueformat=HTML
   column.1.tile.name=component.assignmentslist
   column.2.displayname=Actual/ Planned Hours
   column.2.linkedname=direct
   column.2.namekey=actualworkrequired
   column.2.querysort=actualWork
   column.2.textmode=true
   column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)
   column.2.valuefield=actualWorkRequired
   column.2.valueformat=compound
   column.2.viewalias=actualworkrequired
   column.3.aggregator.function=SUM
   column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})
   column.3.aggregator.valueformat=compound
   column.3.displayname=Hours Variance
   column.3.linkedname=direct
   column.3.textmode=true
   column.3.valueexpression=SUB({actualWork}, {workRequired})/60
   column.3.valueformat=customNumberAsString
   ```

1. Haga clic en **Listo** y luego en **Guardar vista**.
