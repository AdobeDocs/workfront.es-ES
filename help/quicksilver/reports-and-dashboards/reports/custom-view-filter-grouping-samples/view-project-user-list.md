---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: lista de usuarios del proyecto con funciones del puesto"
description: Puede aplicar esta vista en una lista de proyectos o un informe para mostrar una lista de los usuarios asociados al proyecto, así como una lista de las funciones que desempeñan en el proyecto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Vista: lista de usuarios del proyecto con funciones del puesto

Puede aplicar esta vista en una lista de proyectos o un informe para mostrar una lista de los usuarios asociados al proyecto, así como una lista de las funciones que desempeñan en el proyecto.

La información de este informe también se puede encontrar en el área Personas del proyecto.

>[!TIP]
>
>Si no se enumeran funciones del puesto para los usuarios, pero sabe que están asociados a funciones del puesto en sus perfiles de usuario, puede que esto signifique que están asignados a tareas y problemas, pero es posible que no estén asociados a una función del puesto en la tarea o el problema, o que los usuarios enumerados en el informe no sean los asignados a tareas y problemas, pero cumplan otras funciones en el proyecto (por ejemplo, Propietario o Patrocinador).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Ver una lista de usuarios del proyecto con roles

1. Ir a una lista de proyectos.
1. Desde el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Previsualización de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y luego haga clic en **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en la **Modo de texto** y reemplácelo por el siguiente código:
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Usuarios del proyecto<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}.{name}<br>column.1.valueformat=HTML<br>column.2.displayname=Funciones del proyecto<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={role}.{name}<br>column.2.valueformat=HTML</pre>

1. Clic **Guardar vista**.
