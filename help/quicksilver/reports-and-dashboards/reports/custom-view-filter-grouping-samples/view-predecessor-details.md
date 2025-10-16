---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Detalles de predecesoras'
description: Esta vista de tareas muestra detalles de las tareas predecesoras de las tareas mediante una vista de colección. En una vista de colección, puede mostrar información sobre objetos que están en una relación "uno a varios". En este caso, cada tarea (una) puede tener varias predecesoras (muchas). La vista muestra el nombre de las tareas, así como los nombres de sus predecesoras, los nombres de proyecto de sus predecesoras, las fechas planificadas de finalización de sus predecesoras y los estados de sus predecesoras.
author: Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 30%

---

# Ver: detalles de predecesoras

<!--Audited: 11/2024-->

Esta vista de tareas muestra detalles de las tareas predecesoras de las tareas mediante una vista de colección. En una vista de colección, puede mostrar información sobre objetos que están en una relación &quot;uno a varios&quot;. En este caso, cada tarea (una) puede tener varias predecesoras (muchas). La vista muestra el nombre de las tareas, así como los nombres de sus predecesoras, los nombres de proyecto de sus predecesoras, las fechas planificadas de finalización de sus predecesoras y los estados de sus predecesoras.

Para obtener información acerca de las referencias a colecciones en los informes, vea [Colecciones de referencia en un informe](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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
   <p>Colaborador o solicitud para modificar una vista </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Ver detalles de la predecesora

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columnas**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   column.0.displayname=
   column.0.linkedname=direct
   column.0.namekey=name
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.1.displayname=Predecessors Numbers & Names
   column.1.listdelimiter=
   column.1.listmethod=nested(predecessors).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})
   column.1.valueformat=HTML
   column.2.displayname=Predecessors Project Names
   column.2.listdelimiter=
   column.2.listmethod=nested(predecessors).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={predecessor}.{project}.{name}
   column.2.valueformat=HTML
   column.3.displayname=Predecessors Completion Dates
   column.3.listdelimiter=
   column.3.listmethod=nested(predecessors).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={predecessor}.{plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Predecessors Status
   column.4.listdelimiter=
   column.4.listmethod=nested(predecessors).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={predecessor}.{status}
   column.4.valueformat=HTML
   ```

1. Haga clic en **Listo** > **Guardar vista**.
