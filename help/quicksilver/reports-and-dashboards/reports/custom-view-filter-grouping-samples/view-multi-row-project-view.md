---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: vista de proyecto de varias filas'
description: Obtenga información sobre la vista de proyecto de varias filas en los informes.
author: Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 56%

---

# Vista: vista de proyecto de varias filas

<!--Audited: 11/2024-->

En esta vista de proyecto se puede:

* Visualizar la información del proyecto en formato de varias filas.\
  La vista utiliza la etiqueta `sharecol=true` para combinar varios campos bajo el mismo encabezado de columna. Para obtener más información sobre esta etiqueta, consulte [Vista: combinar información de varias columnas en una columna compartida](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Utilice una columna de marcador de posición que contenga una etiqueta de salto de línea de HTML (`<br>`) para forzar la visualización de la descripción debajo del nombre del proyecto, por ejemplo.
* Visualizar el propietario del proyecto entre paréntesis después del nombre del proyecto.
* Visualizar el nombre del proyecto como un vínculo al proyecto.

![Fila del proyecto con vista apilada](assets/project-multi-row-stacked-view-350x219.png)

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

## Creación de una vista de proyecto de varias filas

1. Ir a una lista de proyectos.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.
1. Elimine todas las columnas de la vista, excepto una.
1. Seleccione la columna restante y haga clic en **Cambiar al modo de texto** y después en **Editar modo de texto**.
1. Elimine el texto en **Editar modo de texto** y, a continuación, copie y pegue el modo de texto siguiente dentro de la columna:

   ```
   column.0.linkedname=direct
   column.0.link.valueformat=val
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.valuefield=objCode
   column.0.link.lookup=link.view
   column.0.sharecol=true
   column.0.descriptionkey=name
   column.0.width=150
   column.0.querysort=name
   column.0.valuefield=name
   column.0.name=Project Name / Manager / Description
   column.0.shortview=false
   column.0.stretch=100
   column.0.textmode=true
   column.0.listsort=string(name)
   column.0.valueformat=HTML
   column.1.valueexpression=CONCAT(" (",{owner}.{name},")")
   column.1.listsort=nested(owner).string(name)
   column.1.width=1
   column.1.linkedname=direct
   column.1.querysort=owner:name
   column.1.textmode=true
   column.1.shortview=false
   column.1.stretch=0
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.width=1
   column.2.value=
   column.2.shortview=false
   column.2.sharecol=true
   column.2.stretch=0
   column.2.textmode=true
   column.2.valueformat=HTML
   column.3.styledef.style=font-color:#ccc;
   column.3.descriptionkey=description
   column.3.linkedname=direct
   column.3.valuefield=description
   column.3.listsort=string(description)
   column.3.querysort=description
   column.3.namekey=description.abbr
   column.3.textmode=true
   column.3.sharecol=true
   column.3.stretch=0
   column.3.shortview=false
   column.3.valueformat=HTML
   column.3.width=1
   column.4.shortview=false
   column.4.value=
   column.4.sharecol=true
   column.4.width=1
   column.4.textmode=true
   column.4.valueformat=HTML\
   column.4.stretch=0
   column.5.name=Planned Dates / Duration
   column.5.width=150
   column.5.querysort=plannedStartDate
   column.5.sharecol=true
   column.5.stretch=0
   column.5.textmode=true
   column.5.shortview=false
   column.5.linkedname=direct
   column.5.listsort=atDateAsAtDate(plannedStartDate)
   column.5.valuefield=plannedStartDate
   column.5.valueformat=atDate
   column.6.sharecol=true
   column.6.stretch=0
   column.6.width=1
   column.6.textmode=true
   column.6.value=-
   column.6.valueformat=HTML
   column.6.shortview=false
   column.7.namekey=plannedcompletiondate.abbr
   column.7.width=1
   column.7.sharecol=true
   column.7.shortview=false
   column.7.stretch=0
   column.7.listsort=atDateAsAtDate(plannedCompletionDate)
   column.7.linkedname=direct
   column.7.descriptionkey=plannedcompletiondate
   column.7.textmode=true
   column.7.querysort=plannedCompletionDate
   column.7.valueformat=atDate
   column.7.valuefield=plannedCompletionDate
   column.8.value=
   column.8.width=1
   column.8.textmode=true
   column.8.sharecol=true
   column.8.valueformat=HTML
   column.8.stretch=0
   column.9.textmode=true
   column.9.listsort=intAsInt(durationMinutes)
   column.9.stretch=0
   column.9.valuefield=durationFieldLong
   column.9.descriptionkey=duration
   column.9.viewalias=duration
   column.9.querysort=durationMinutes
   column.9.sharecol=true
   column.9.width=100
   column.9.shortview=false
   column.9.namekey=duration.abbr
   column.9.linkedname=direct
   column.9.valueformat=compound
   column.10.textmode=true
   column.10.stretch=0
   ```


1. Haga clic en **Listo** > **Guardar vista**.
