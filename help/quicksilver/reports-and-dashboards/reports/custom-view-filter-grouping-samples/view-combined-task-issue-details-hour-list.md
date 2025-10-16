---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Detalles combinados de tareas y problemas en una lista de horas'
description: Esta vista de horas combina las columnas de nombre de tarea y nombre de problema, así como las Horas planificadas de tarea y problema usando la etiqueta sharecol. Dado que una entrada de hora solo puede pertenecer a una tarea o a un problema, ambos objetos no pueden aparecer en la misma columna al mismo tiempo. Cada línea de la vista se rellena con la información de una tarea o de un problema.
author: Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 65%

---

# Vista: detalles combinados de tareas y problemas en una lista de horas

<!--Audited:11/2024-->

Esta vista de horas combina las columnas Nombre de tarea y Nombre de problema, así como las Horas planificadas de tarea y Problema usando la etiqueta `sharecol`. Dado que una entrada de hora solo puede pertenecer a una tarea o a un problema, ambos objetos no pueden aparecer en la misma columna al mismo tiempo. Cada línea de la vista se rellena con la información de una tarea o de un problema.

Para obtener más información sobre la etiqueta `sharecol`, consulte [Ver: combinar información de varias columnas en una columna compartida](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

## Ver detalles combinados de tareas y problemas en una lista de horas

1. Vaya a una lista de horas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.
1. En el área **Vista previa de columnas**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   column.1.querysort=project:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=project:name
   column.1.valueformat=HTML
   column.1.width=100
   column.2.description=Task or Issue
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=task:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=task:objCode
   column.2.link.valueformat=val
   column.2.linkedname=task
   column.2.listsort=nested(task).string(name)
   column.2.name=Task or Issue
   column.2.querysort=task:name
   column.2.sharecol=true
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=task:name
   column.2.valueformat=HTML
   column.2.width=100
   column.3.descriptionkey=optask
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=opTask:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=opTask:objCode
   column.3.link.valueformat=val
   column.3.linkedname=optask
   column.3.listsort=nested(opTask).string(name)
   column.3.namekey=opTask
   column.3.querysort=opTask:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=opTask:name
   column.3.valueformat=HTML
   column.3.width=1
   column.4.valuefield=task:work
   column.4.sharecol=true
   column.4.linkedname=task
   column.4.valueformat=doubleAsInt
   column.4.namekey=view.relatedcolumn
   column.4.querysort=task:work
   column.4.textmode=true
   column.4.namekeyargkey.0=task
   column.4.namekeyargkey.1=work
   column.4.displayname=Planned Effort
   column.5.displayname=Planned Effort
   column.5.viewalias=opTask:workrequired
   column.5.linkedname=opTask
   column.5.valuefield=opTask:workRequired
   column.5.valueformat=compound
   column.5.querysort=opTask:workRequired
   column.5.namekeyargkey.0=opTask
   column.5.namekeyargkey.1=workrequired
   column.5.namekey=view.relatedcolumn
   column.5.textmode=true
   column.6.descriptionkey=hours
   column.6.linkedname=direct
   column.6.listsort=doubleAsDouble(hours)
   column.6.namekey=hours.abbr
   column.6.querysort=hours
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=hours
   column.6.valueformat=doubleAsString
   column.6.width=75
   column.7.descriptionkey=entrydate
   column.7.linkedname=direct
   column.7.listsort=atDateAsAtDate(entryDate)
   column.7.namekey=entrydate.abbr
   column.7.querysort=entryDate
   column.7.shortview=false
   column.7.stretch=0
   column.7.valuefield=entryDate
   column.7.valueformat=atDate
   column.7.width=75
   column.8.descriptionkey=description
   column.8.linkedname=direct
   column.8.listsort=string(description)
   column.8.namekey=description.abbr
   column.8.querysort=description
   column.8.shortview=false
   column.8.stretch=0
   column.8.valuefield=description
   column.8.valueformat=HTML
   column.8.width=150
   ```

1. Haga clic en **Listo** > **Guardar vista**.
1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
