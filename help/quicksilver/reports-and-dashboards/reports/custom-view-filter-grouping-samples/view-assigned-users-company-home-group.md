---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Compañía y grupo de inicio del usuario asignado'
description: Esta vista de tarea muestra la compañía y el grupo de inicio del propietario principal de la tarea. Son valores que no están disponibles en la interfaz estándar, pero a los que se puede acceder mediante el modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 75%

---

# Vista: compañía y grupo de inicio del usuario asignado

<!--Audited: 11/2024-->

Esta vista de tarea muestra la compañía y el grupo de inicio del propietario principal de la tarea. Son valores que no están disponibles en la interfaz estándar, pero a los que se puede acceder mediante el modo de texto.

![Ver la compañía y el grupo de inicio del usuario asignado](assets/view--assigned-user-s-company-and-home-group-350x80.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
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
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver la compañía y el grupo de inicio del usuario asignado

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Haga clic en **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=assignedto
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=assignedTo:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=assignedTo:objCode
   column.1.link.valueformat=val
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Assigned To Company
   column.2.displayname=Assigned To Company
   column.2.linkedname=assignedTo:company
   column.2.listsort=nested(assignedTo:company).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:company:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=assignedTo:company:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Assigned To Home Group
   column.3.displayname=Assigned To Home Group
   column.3.linkedname=assignedTo:homeGroup
   column.3.listsort=nested(assignedTo:homeGroup).string(name)
   column.3.namekey=assignedto
   column.3.querysort=assignedTo:homeGroup:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=assignedTo:homeGroup:name
   column.3.valueformat=HTML
   column.3.width=150
   ```

1. Haga clic en **Listo** > **Guardar vista**.
1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
