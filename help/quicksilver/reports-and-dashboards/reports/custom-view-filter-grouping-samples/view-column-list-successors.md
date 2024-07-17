---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: agregar una lista de tareas sucesoras en una columna"
description: Puede agregar una columna a una vista de tareas para mostrar una lista de las sucesoras de las tareas. La columna Sucesoras de tareas incluye el número de la tarea sucesora así como el nombre.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 2%

---

# Ver: Agregar una lista de tareas sucesoras en una columna

Puede agregar una columna a una vista de tareas para mostrar una lista de las sucesoras de las tareas. La columna **Sucesoras de tareas** incluye el número de la sucesora y el nombre.

![task_view_with_a_list_of_sucesors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Agregar una lista de tareas sucesoras en una columna

Para agregar esta columna a una vista de tareas:

1. Ir a una vista de tareas existente.
1. Expanda el menú desplegable Vista y seleccione **Personalizar vista**.
1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área **Mostrar en esta columna** y haga clic en **Haga clic para editar el texto**.

1. Elimine todo el texto del cuadro Modo de texto y sustitúyalo por el siguiente código:
   <pre>displayname=Sucesoras de tareas<br>listdelimiter=<br><br>listmethod=nested(sucesors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}).{taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>

1. Pulse **Guardar vista**.
