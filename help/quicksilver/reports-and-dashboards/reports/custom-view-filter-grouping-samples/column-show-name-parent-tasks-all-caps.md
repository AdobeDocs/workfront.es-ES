---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Mostrar el nombre de las tareas principales en mayúsculas'
description: Puede añadir esta columna a una vista de tareas para mostrar el nombre de las tareas principales en mayúsculas.
author: Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 74%

---

# Ver: mostrar el nombre de las tareas principales en mayúsculas

<!--Audited: 10/2024-->

Puede añadir esta columna a una vista de tareas para mostrar el nombre de las tareas principales en mayúsculas.

![Columna con tarea principal en mayúsculas](assets/column-task-with-all-caps-parent-350x112.png)

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

## Mostrar el nombre de las tareas principales todo en mayúsculas

Para generar esta columna en una vista de tareas:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, selecciona una vista y luego haz clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).
O\
   En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, haga clic en el encabezado de la columna que muestra el nombre de la tarea en la lista.
1. Haz clic en **Cambiar al modo de texto** y luego haz clic en **Editar modo de texto**.
1. Quite el texto que encuentra en el cuadro **Modo de texto** y sustitúyalo por el siguiente código:

   ```
   linkedname=direct
   namekey=name
   querysort=name
   styledef.case.0.comparison.icon=false
   styledef.case.0.comparison.leftmethod=numberOfChildren
   styledef.case.0.comparison.lefttext=numberOfChildren
   styledef.case.0.comparison.operator=gt
   styledef.case.0.comparison.operatortype=int
   styledef.case.0.comparison.righttext=0
   styledef.case.0.comparison.trueproperty.0.name=fontstyle
   styledef.case.0.comparison.trueproperty.0.value=bold
   valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})
   valueformat=HTML
   ```

1. Haga clic en **Listo** y luego haga clic en **Guardar vista**.
