---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver y agrupar: mostrar la duración real del proyecto agregada por la media en un grupo"
description: Puede agregar la siguiente columna en un informe de proyecto para mostrar la duración real agregada como promedio en una agrupación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Ver y agrupar: mostrar la duración real del proyecto agregada por el promedio en una agrupación

Puede agregar la siguiente columna en un informe de proyecto para mostrar la duración real agregada como promedio en una agrupación.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Mostrar la duración real del proyecto agregada por el promedio en una agrupación

Para agregar esta columna a una vista de proyecto:

1. (Recomendado) Para obtener mejores resultados y ver el valor promedio agregado de la duración real, debe tener un Grupo agregado a la lista o informe del proyecto.\
   Para obtener más información sobre la creación de agrupaciones, consulte el artículo [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Vaya a una vista de proyecto existente.
1. Expanda el menú desplegable Ver y seleccione **Personalizar vista**.
1. Haga clic en **Agregar columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre la **Mostrar en esta columna** y haga clic en **Haga clic para editar texto**.

1. Elimine todo el texto del cuadro Modo de texto y sustitúyalo por el siguiente código:

   <pre>agregador.displayformat=compuesto <br>agregador.función=AVG <br>gregator.namekey=view.relatedcolumn <br>agregator.namekeyargkey=actualduration <br>gregator.valueField=realDurationMinutes <br>agregator.value eformat=val <br>nombreDePantalla=Duración real del proyecto <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinutes <br>textmode=true <br>valueField=actualDurationMinutes <br>value eformat=compuesto#M:D <br>viewalias=actualduration</pre>

1. Haga clic en **Guardar vista**.
