---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: mostrar sangría de tareas en una lista de tareas'
description: En esta vista de tareas, puede agregar código a la columna Nombre de la tarea para mostrar las tareas con sangría según la estructura de desglose de trabajo del proyecto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Ver: mostrar sangría de tareas en una lista de tareas

En esta vista de tareas, puede agregar código a la columna Nombre de la tarea para mostrar las tareas con sangría según la estructura de desglose de trabajo del proyecto.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Mostrar sangría de tareas en una columna de una lista de tareas

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y empiece a escribir &quot;Nombre de tarea&quot; en la sección **Mostrar en esta columna** a continuación, selecciónelo cuando aparezca en la lista.

1. En la nueva columna, haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección

   ```
   valuefield=
   ```

   y reemplácelo por el siguiente código:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Haga clic en **Guardar**, luego **Guardar vista**.
