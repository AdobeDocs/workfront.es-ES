---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: compañía y grupo de inicio del usuario asignado"
description: Esta vista de tarea muestra la compañía y el grupo de inicio del propietario principal de la tarea. Son valores que no están disponibles en la interfaz estándar, pero a los que se puede acceder mediante el modo de texto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Ver: compañía y grupo de inicio del usuario asignado

Esta vista de tarea muestra la compañía y el grupo de inicio del propietario principal de la tarea. Son valores que no están disponibles en la interfaz estándar, pero a los que se puede acceder mediante el modo de texto.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Ver la compañía y el grupo de inicio del usuario asignado

1. Ir a una lista de tareas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en el cuadro **Modo de texto** y reemplácelo por el siguiente código:
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0 .namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> .1.link.linkproperty.0.valuefield=assignedTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo:objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo).string(name)<br> 0.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=Asignado a la compañía<br> column.2.displayname=Asignado a la compañía{3 3} column.2.linkedname=assignedTo:company<br> column.2.listsort=nested(assignedTo:company).string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:nombre<br> column.2.shortview=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:nombre<br> column.2.valuevalue format=HTML<br> column.2.width=150<br> column.3.description=Assigned To Home Group<br> column.3.displayname=Assigned To Home Group<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo{50 {name<br> column.3.shortview=false<br> column.3.stretch=0<br> column.3.valuefield=assignedTo:homeGroup:nombre<br> column.3.valueformat=HTML<br> column.3.width=150<br>:homeGroup:</pre>

1. Haga clic en **Guardar cambios**.
