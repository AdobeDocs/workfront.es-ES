---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vista: Problemas con la resolución de detalles del objeto"
description: Esta vista de problema muestra el nombre y el porcentaje completado del objeto de resolución del problema, lo que permite que el creador del problema tenga una perspectiva del progreso del problema incluso sin acceso a la tarea o al proyecto de resolución.
author: Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Ver: problemas con la resolución de detalles de objetos

<!--Audited: 11/2024-->

Esta vista de problema muestra el nombre y el porcentaje completado del objeto de resolución del problema, lo que permite que el creador del problema tenga una perspectiva del progreso del problema incluso sin acceso a la tarea o al proyecto de resolución.

Esta vista usa la etiqueta `sharecol=true` para combinar varios campos bajo el mismo encabezado de columna. Para obtener más información sobre la etiqueta `sharecol`, consulte [Ver: combinar información de varias columnas en una columna compartida](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolve_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo:<ul><li>Colaborador para modificar una vista</li><li>Estándar para modificar un informe</li></ul></p><p>O</p>Actual:<ul><li>Solicitud para modificar una vista</li><li>Plan para modificar un informe</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver problemas con la resolución de detalles del objeto

1. Ir a una lista de problemas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante, haga clic en **Cambiar al modo de texto** y, a continuación, haga clic en **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   column.0.querysort=name
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=sourceobject
   column.1.linkedname=direct
   column.1.listsort=nested(referenceObject).HTML(name)
   column.1.namekey=sourceobject.abbr
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=referenceObject:name
   column.1.valueformat=HTML
   column.1.viewalias=source
   column.1.width=100
   column.2.descriptionkey=assignedto
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=assignedTo:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=assignedTo:objCode
   column.2.link.valueformat=val
   column.2.linkedname=assignedTo
   column.2.listsort=nested(assignedTo).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=assignedTo:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=entrydate
   column.3.linkedname=direct
   column.3.listsort=atDateAsAtDate(entryDate)
   column.3.namekey=entrydate.abbr
   column.3.querysort=entryDate
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=entryDate
   column.3.valueformat=atDate
   column.3.width=150
   column.4.descriptionkey=description
   column.4.linkedname=direct
   column.4.listsort=string(description)
   column.4.namekey=description.abbr
   column.4.querysort=description
   column.4.shortview=false
   column.4.stretch=75
   column.4.valuefield=description
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=status
   column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum
   column.5.linkedname=direct
   column.5.listsort=string(status)
   column.5.namekey=status.abbr
   column.5.querysort=status
   column.5.shortview=false
   column.5.stretch=0
   column.5.type=enum
   column.5.valuefield=status
   column.5.valueformat=val
   column.5.width=150
   column.6.displayname=Resolving Object Name
   column.6.linkedname=resolveTask
   column.6.namekey=view.relatedcolumn
   column.6.namekeyargkey.0=resolveTask
   column.6.namekeyargkey.1=name
   column.6.querysort=resolveTask:name
   column.6.sharecol=true
   column.6.textmode=true
   column.6.valuefield=resolveTask:name
   column.6.valueformat=HTML
   column.7.displayname=
   column.7.linkedname=resolveOpTask
   column.7.namekey=view.relatedcolumn
   column.7.namekeyargkey.0=resolveOpTask
   column.7.namekeyargkey.1=name
   column.7.querysort=resolveOpTask:name
   column.7.sharecol=true
   column.7.textmode=true
   column.7.valuefield=resolveOpTask:name
   column.7.valueformat=HTML
   column.8.displayname=
   column.8.linkedname=resolveProject
   column.8.namekey=view.relatedcolumn
   column.8.namekeyargkey.0=resolveProject
   column.8.namekeyargkey.1=name
   column.8.querysort=resolveProject:name
   column.8.textmode=true
   column.8.valuefield=resolveProject:name
   column.8.valueformat=HTML
   column.9.displayname=Resolving Object Percent Complete
   column.9.textmode=true
   column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},''))
   column.9.valueformat=doubleAsPercentRounded
   ```

1. Haga clic en **Listo** > **Guardar vista**.
1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
