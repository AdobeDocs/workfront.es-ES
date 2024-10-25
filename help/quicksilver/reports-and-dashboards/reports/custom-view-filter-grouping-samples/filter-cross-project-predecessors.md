---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: mostrar predecesoras entre proyectos incompletas"
description: Este filtro de tareas devuelve predecesoras entre proyectos incompletas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Filtro: mostrar predecesoras entre proyectos incompletas

<!--Audited: 10/2024-->

Este filtro de tareas devuelve predecesoras entre proyectos incompletas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
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
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar predecesoras entre proyectos

Para aplicar este filtro:

1. Ir a una lista de tareas o a un informe de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. (Condicional) Haga clic en **Modo de texto** si accedió al filtro desde una lista o en **Cambiar al modo de texto** si accedió al filtro desde un informe.
1. En la nueva área, pegue el siguiente código:
   <pre>predecesorsMM:projectID=FIELD:projectID<br>predecesorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Condicional) Haga clic en **Guardar filtro** si accedió al filtro desde un informe, o en **Aplicar** y después en **Guardar como nuevo** si accedió al filtro desde una lista de tareas.
