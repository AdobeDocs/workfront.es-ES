---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: detalles del problema de origen para tareas y proyectos"
description: 'Cuando un problema se convierte en una tarea o un proyecto, se establece una relación de objeto de resolución entre la tarea o el proyecto y el problema. Esta vista muestra los siguientes campos del problema que se resuelve automáticamente cuando se completa la tarea o el proyecto: EDITARME.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# Ver: detalles del problema de origen para tareas y proyectos.

Cuando un problema se convierte en una tarea o un proyecto, se establece una relación de objeto de resolución entre la tarea o el proyecto y el problema. Esta vista muestra los siguientes campos del problema que se resuelve automáticamente al finalizar la tarea o el proyecto:

* Nombre
* Fecha de entrada
* Fecha planificada de finalización
* Fecha real de finalización
* Tipo de solicitud
* Nombre del creador
* Asignado a usuario

![task_with_resolve_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Para obtener más información, consulte [Ver: mostrar la información original del problema en las listas de tareas y proyectos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## Ver detalles del problema de origen de tareas y proyectos

1. Ir a una lista de tareas o de proyectos.
1. Desde el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Previsualización de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y luego haga clic en **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en la **Modo de texto** y reemplácelo por el siguiente código:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Clic **Guardar vista**.
