---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: patrocinador del proyecto para horas"
description: Este grupo de horas organiza las horas por el patrocinador del proyecto en el que se registran. La interfaz estándar del Report Builder para las agrupaciones de horas no proporciona una asignación al campo Patrocinador de proyecto. Debe utilizar la interfaz del modo Texto para acceder a este campo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Agrupación: patrocinador del proyecto por horas

Este grupo de horas organiza las horas por el patrocinador del proyecto en el que se registran. La interfaz estándar del Report Builder para las agrupaciones de horas no proporciona una asignación al campo Patrocinador de proyecto. Debe utilizar la interfaz del modo Texto para acceder a este campo.

![hour_report_agrupado_by_patrocinador.png](assets/hour-report-grouped-by-sponsor-350x39.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar una agrupación </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una agrupación</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Agrupar por patrocinador del proyecto durante horas

Para aplicar esta agrupación:

1. Ir a una lista de horas.
1. En el menú desplegable **Agrupación**, seleccione **Nueva agrupación**.

1. Haga clic **Cambiar al modo de texto**.
1. Elimine el texto del área **Agrupar su informe**.

1. Reemplace el texto con el siguiente código:
   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. Haga clic en **Guardar agrupación**.
