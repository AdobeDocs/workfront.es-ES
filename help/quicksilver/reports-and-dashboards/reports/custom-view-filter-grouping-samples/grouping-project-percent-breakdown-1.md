---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupación: desglose del porcentaje del proyecto 1'''
description: En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por un rango de sus valores de porcentaje completado.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# Agrupación: desglose del porcentaje del proyecto 1

En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por un rango de sus valores de porcentaje completado.

La siguiente agrupación organiza los proyectos según el valor del porcentaje completado en una de estas agrupaciones:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![percent_complete_split_custom_project_grouping_25__increments.png](assets/percent-complete-breakdown-custom-350x56.png)

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

## Desglose de grupo por porcentaje del proyecto

Para aplicar esta agrupación:

1. Vaya a una lista de proyectos.
1. En el **Agrupación** menú desplegable, seleccione **Nuevo grupo**.

1. Haga clic en **Cambiar al modo de texto**.
1. Elimine el texto del cuadro y pegue el siguiente código en el espacio disponible:
   <pre>group.0.linkedname=direct<br>group.0.name=Desglose porcentual<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}) &lt;100,"75-99 %","100 %"))))<br>group.0.valueformat=string</pre>

1. Haga clic en **Guardar agrupación**.
