---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: problemas con la información de aprobación"
description: La siguiente vista de problema muestra el proceso de aprobación, el paso, los nombres de los aprobadores y el estado del problema antes de que se concediera la aprobación. Algunos de estos campos no son accesibles a través del generador de interfaces estándar.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Ver: problemas con la información de aprobación

La siguiente vista de problema muestra el proceso de aprobación, el paso, los nombres de los aprobadores y el estado del problema antes de que se concediera la aprobación. Algunos de estos campos no son accesibles a través del generador de interfaces estándar.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver problemas con la información de aprobación

1. Ir a una lista de problemas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en el cuadro **Modo de texto** y reemplácelo por el siguiente código:
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0 .namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=40<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name)<br>column.1.namekey=assignedto<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.stretch=0<br>column.1.valuefield=assignedTo:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=rol column.2.linkedname=role<br>column.2.listsort=nested(role).string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=role:name<br>column.2.valueformat=HTML<br>column.2.width=150 35}column.3.description=Approval Process Name<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Approval Process Name<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.stretch=35<br>column.3.valuefield=approvalProcess:name<br>column.3.valueformat=HTML<br>column.3 .width=220<br>column.4.description=Approval Step Name<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Approval Step Name<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovalStep:name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Estado anterior<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Estado anterior<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=previousStatus<br>column.5.valuevaluefield format=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=approver.plural.abbr<br>column.6.querysort=approversString<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br><br><br></pre>

1. Pulse **Guardar vista**.
