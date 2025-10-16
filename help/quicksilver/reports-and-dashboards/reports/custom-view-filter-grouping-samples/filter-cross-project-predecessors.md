---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar predecesoras entre proyectos incompletas'
description: Este filtro de tareas devuelve predecesoras entre proyectos incompletas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 33%

---

# Filtro: mostrar predecesoras entre proyectos incompletas

<!--Audited: 10/2024-->

Este filtro de tareas devuelve predecesoras entre proyectos incompletas.

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

## Filtrar predecesoras entre proyectos

Para aplicar este filtro:

1. Ir a una lista de tareas o a un informe de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. (Condicional) Haga clic en **Modo de texto** si accedió al filtro desde una lista o en **Cambiar al modo de texto** si accedió al filtro desde un informe.
1. En la nueva área, pegue el siguiente código:
   <pre>predecesorsMM:projectID=FIELD:projectID<br>predecesorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Condicional) Haga clic en **Guardar filtro** si accedió al filtro desde un informe, o en **Aplicar** y después en **Guardar como nuevo** si accedió al filtro desde una lista de tareas.
