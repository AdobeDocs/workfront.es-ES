---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupación: desglose de porcentaje de tarea 1'''
description: '"En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por un rango de sus valores de porcentaje completado. Los desgloses muestran el valor de porcentaje completado de incrementos de 25 puntos porcentuales: 0-25 %, 25-50 %, etc.'''
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# Agrupación: desglose de porcentaje de tarea 1

En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por un rango de sus valores de porcentaje completado. Los desgloses muestran el valor de porcentaje completado de incrementos de 25 puntos porcentuales: 0-25 %, 25-50 %, etc. 

La siguiente agrupación organiza las tareas por el valor de porcentaje completado en 6 agrupaciones diferentes:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25_split_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Agrupar por desglose de porcentaje de tarea

Para aplicar esta agrupación:

1. Vaya a una lista de tareas.
1. En el **Agrupación** menú desplegable, seleccione **Nuevo grupo**.

1. Haga clic en **Cambiar al modo de texto**.
1. Elimine el texto de la sección **Agrupar su informe** .
1. Reemplace el texto por el siguiente código:

   <pre>group.0.linkedname=direct<br>group.0.name=Desglose porcentual<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}) &lt;100,"75-99 %","100 %"))))<br>group.0.valueformat=string</pre>

1. Haga clic en **Guardar agrupación**.
