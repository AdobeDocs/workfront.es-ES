---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupación: patrocinador del proyecto para una lista de tareas'
description: Esta agrupación de tareas le permite agrupar tareas por el patrocinador del proyecto.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 79%

---

# Agrupación: patrocinador del proyecto para una lista de tareas

<!--Audited: 11/2024-->

Esta agrupación de tareas le permite agrupar tareas por el patrocinador del proyecto.

![Agrupar por patrocinador del proyecto](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## Agrupar por patrocinador del proyecto para una lista de tareas


Para aplicar esta agrupación:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Agrupación**, seleccione **Nueva agrupación**.

1. Haga clic en **Cambiar al modo de texto**.
1. Elimine el texto del área que se muestra y reemplácelo por el siguiente código:

   ```
   group.0.name=Project Sponsor
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=string
   ```

1. Haga clic en **Listo**.
1. Actualice el nombre de la agrupación y haga clic en **Guardar agrupación**.

