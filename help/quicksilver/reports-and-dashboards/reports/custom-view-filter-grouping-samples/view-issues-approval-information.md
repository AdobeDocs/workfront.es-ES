---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: problemas con la información de aprobación"'
description: La siguiente vista de problemas muestra el proceso de aprobación, el paso, los nombres de los aprobadores y el estado del problema antes de conceder la aprobación. Algunos de estos campos no son accesibles a través del generador de interfaz estándar.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Ver: problemas con información de aprobación

La siguiente vista de problemas muestra el proceso de aprobación, el paso, los nombres de los aprobadores y el estado del problema antes de conceder la aprobación. Algunos de estos campos no son accesibles a través del generador de interfaz estándar.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Ver problemas con la información de aprobación

1. Vaya a una lista de problemas.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.value.format=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.value.format=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.name=name.abbr<br>column.0.querysort=name<br>column.0.abreviview=false<br>column.0.stretch=40<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name)<br>column.1.namekey=assignedto<br>column.1.querysort=assignedTo:name<br>column.1.abreviview=true<br>column.1.stretch=0<br>column.1.valueField=assignedTo:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nested(role).string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.abreviview=false<br>column.2.stretch=25<br>column.2.valuefield=role:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=Approval Process Name<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Approval Process Name<br>column.3.querysort=name<br>column.3.abreviview=false<br>column.3.stretch=35<br>column.3.valuefield=approvalProcess:name<br>column.3.valueformat=HTML<br>column.3.width=220<br>column.4.description=Approval Step Name<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Approval Step Name<br>column.4.querysort=name<br>column.4.shorview=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovalStep:name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Previous Status<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Previous Status<br>column.5.querysort=name<br>column.5.abreviview=false<br>column.5.stretch=0<br>column.5.valueField=previousStatus<br>column.5.valueformat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=approver.plural.abbr<br>column.6.querysort=approversString<br>column.6.abreviview=false<br>column.6.stretch=0<br>column.6.valueField=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br></pre>

1. Haga clic en **Guardar vista**.
