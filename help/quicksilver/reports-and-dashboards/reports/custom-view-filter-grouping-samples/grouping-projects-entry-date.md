---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: proyectos por fecha de entrada"
description: En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por sus valores de Fecha de entrada.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Agrupación: proyectos por fecha de entrada

En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por sus valores de Fecha de entrada.

Cada agrupación muestra los proyectos con una fecha de entrada en:

* Los últimos 30 días
* 30 a 60 días
* 60 días o más

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

## Agrupar proyectos por fecha de entrada

Para aplicar esta agrupación:

1. Vaya a un informe de proyecto existente o cree un nuevo informe de proyecto.\
   Para obtener más información acerca de cómo crear un informe, vea el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Haga clic en **Acciones de informe** > **Editar**.
1. En la ficha **Agrupación**, haga clic en **Agregar agrupación**.
1. Haga clic en **Cambiar al modo de texto**.
1. Quitar el texto del área **Agrupar por**.
1. Reemplace el texto con el siguiente código:

   group.0.linkedname=direct
group.0.name=Entrada de proyecto
group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))&lt;=30,&quot;Last 30 Days&quot;,IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&amp;&amp;ABS(DATEDIFF({entryDate},$$TODAY))&lt;=60,&quot;30-60 Days&quot;,&quot;Older than 60 days&quot;)
group.0.valueformat=atDateAsMonthString
textmode=true

1. Haga clic en **Listo** > **Guardar agrupación**.
1. (Opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.
