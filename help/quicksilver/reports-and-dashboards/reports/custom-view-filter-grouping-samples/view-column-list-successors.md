---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: añadir una lista de tareas sucesoras en una columna'
description: Puede añadir una columna a una vista de tareas para mostrar una lista de los sucesores de las tareas. La columna Sucesores de tareas incluye el número del sucesor y el nombre.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Ver: añadir una lista de tareas sucesoras en una columna

Puede añadir una columna a una vista de tareas para mostrar una lista de los sucesores de las tareas. La variable **Sucesores de tareas** incluye el número del sucesor y el nombre.

![task_view_with_a_list_of_sucesors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Añadir una lista de tareas sucesoras en una columna

Para agregar esta columna a una vista de tareas:

1. Vaya a una vista de tarea existente.
1. Expanda el menú desplegable Ver y seleccione **Personalizar vista**.
1. Haga clic en **Agregar columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre la **Mostrar en esta columna** y haga clic en **Haga clic para editar texto**.

1. Elimine todo el texto del cuadro Modo de texto y sustitúyalo por el siguiente código:

   <pre>displayname=Sucesores de tarea<br>listdelimiter=<br><br>listmethod=nested(sucesors).lists<br>textmode=true<br>type=iterate<br>valueExpression=CONCAT({sucessor}.{taskNumber},' - ',{sucesor}.{name})<br>value=format=HTML</pre>

1. Haga clic en **Guardar vista**.
