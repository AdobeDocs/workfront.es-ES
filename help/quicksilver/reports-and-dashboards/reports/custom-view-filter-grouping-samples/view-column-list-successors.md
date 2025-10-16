---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Agregar una lista de sucesores de tareas en una columna'
description: Puede agregar una columna a una vista de tareas para mostrar una lista de las sucesoras de las tareas. La columna Sucesoras de tareas incluye el número de la tarea sucesora así como el nombre.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# Ver: Agregar una lista de tareas sucesoras en una columna

<!--Audited: 11/2024-->

Puede agregar una columna a una vista de tareas para mostrar una lista de las sucesoras de las tareas. La columna **Sucesoras de tareas** incluye el número de la sucesora y el nombre.

![task_view_with_a_list_of_sucesors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Agregar una lista de tareas sucesoras en una columna

Para añadir esta columna a una vista de tareas:

1. Ir a una lista de tareas.
1. Expanda el menú desplegable **Vista** y haga clic en **Nueva vista**.
1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto** y luego haga clic en **Editar modo de texto**.
1. Elimine todo el texto del cuadro **Editar modo de texto** y reemplácelo por el código siguiente:

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. Haga clic en **Listo** y luego en **Guardar vista**.
