---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: detalles de la emisión originaria de las tareas y los proyectos'
description: 'Cuando un problema se convierte en una tarea o un proyecto, se establece una relación de objeto de resolución entre la tarea o el proyecto y el problema. Esta vista muestra los siguientes campos del problema que se completan automáticamente cuando la tarea o el proyecto finaliza: EDITAR MI.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Ver: detalles de la emisión originaria de tareas y proyectos

Cuando un problema se convierte en una tarea o un proyecto, se establece una relación de objeto de resolución entre la tarea o el proyecto y el problema. Esta vista muestra los siguientes campos del problema que se completan automáticamente cuando se completa la tarea o el proyecto:

* Nombre
* Fecha de entrada
* Fecha planificada de finalización
* Fecha real de finalización
* Tipo de solicitud
* Nombre del creador
* Usuario asignado

![task_with_resolve_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Para obtener más información, consulte también [Ver: mostrar la información del problema original en las listas de tareas y proyectos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## Ver detalles de problemas de origen para tareas y proyectos

1. Vaya a una lista de tareas o a una lista de proyectos.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Haga clic en **Guardar vista**.
