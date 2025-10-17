---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar sucesoras entre proyectos incompletas'
description: Este filtro de tareas devuelve sucesoras entre proyectos incompletas.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 72%

---

# Filtro: mostrar sucesoras entre proyectos incompletas

Este filtro de tareas devuelve sucesoras entre proyectos incompletas.

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

## Filtrar sucesoras entre proyectos

Para aplicar este filtro:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Haga clic en **Modo de texto**.
1. En el área mostrada, pegue el siguiente código:
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>sucesorsMM:projectID=FIELD:projectID<br>sucesorsMM:projectID_Mod=ne</pre>

1. Haga clic en **Aplicar** > **Guardar como nuevo**.
