---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: Empresa y grupo de inicio del usuario asignado"
description: Esta vista de tareas muestra la empresa y el grupo principal del propietario principal de la tarea. Estos son valores que no están disponibles en la interfaz estándar, pero se puede acceder a ellos mediante el modo de texto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Ver: empresa y grupo de inicio del usuario asignado

Esta vista de tareas muestra la empresa y el grupo principal del propietario principal de la tarea. Estos son valores que no están disponibles en la interfaz estándar, pero se puede acceder a ellos mediante el modo de texto.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Ver la empresa y el grupo de inicio del usuario asignado

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valueField=ID<br> column.0.link.linkproperty.0.value.format=int<br> column.0.link.lookup=link.view<br> column.0.link.value.field=objCode<br> column.0.link.value.format=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.name=name.abbr<br> column.0.querysort=name<br> column.0.abreviview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valueField=assignedTo:ID<br> column.1.link.linkproperty.0.value.format=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo:objCode<br> column.1.link.value.format=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo).string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.abreviview=false<br> column.1.stretch=0<br> column.1.valueField=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=Assigned To Company<br> column.2.displayname=Assigned To Company<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nested(assignedTo:company).string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:name<br> column.2.abreviview=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:name<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=Assigned To Home Group<br> column.3.displayname=Assigned To Home Group<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:name<br> column.3.abreviview=false<br> column.3.stretch=0<br> column.3.valuefield=assignedTo:homeGroup:name<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. Haga clic en **Guardar cambios**.
