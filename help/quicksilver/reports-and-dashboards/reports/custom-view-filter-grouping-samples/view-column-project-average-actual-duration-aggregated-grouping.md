---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver y agrupar: mostrar la duración real del proyecto agregada por el promedio en una agrupación"
description: Puede agregar la siguiente columna en un informe de proyecto para mostrar la duración real agregada como promedio en una agrupación.
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Ver y agrupar: muestra la duración real del proyecto agregada por el promedio en una agrupación

<!--Audited: 11/2024-->

Puede agregar la siguiente columna en una vista de proyecto para mostrar la duración real agregada como promedio en una agrupación.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar la duración real del proyecto agregada por el promedio en una agrupación

Para agregar esta columna a una vista de proyecto:

1. Ir a una lista de proyectos.
1. (Obligatorio) Para ver el valor promedio agregado de la duración real del proyecto, debe tener una agrupación agregada a la lista de proyectos.\
   Para obtener más información acerca de cómo crear agrupaciones, vea el artículo [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
1. Expanda el menú desplegable **Vista** y seleccione **Personalizar vista**.
1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto** y luego haga clic en **Editar modo de texto**.
1. Elimine todo el texto del cuadro **Editar modo de texto** y reemplácelo por el código siguiente:

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. Haga clic en **Listo** y luego en **Guardar vista**.
1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
