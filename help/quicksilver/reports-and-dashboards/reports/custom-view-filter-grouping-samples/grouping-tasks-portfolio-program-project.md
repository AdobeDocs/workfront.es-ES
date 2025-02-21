---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupación: Tareas por Portfolio, Programa y Proyecto'
description: Utilice esta agrupación de tareas para agrupar tareas por el portafolio, por programa y luego por el proyecto con el que están asociadas.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 58%

---

# Agrupación: tareas por portafolio, programa y proyecto

<!--Audited: 10/2024-->

Utilice esta agrupación de tareas para agrupar tareas por el portafolio, por programa y luego por el proyecto con el que están asociadas.

![Agrupación de proyectos de programas de Portfolio](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Agrupar tareas por portafolio, programa y proyecto

Para aplicar esta agrupación:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Agrupación**, seleccione **Nueva agrupación**.
1. Haga clic en **Agregar agrupación**.

1. Haga clic en **Cambiar a modo de texto**.
1. Quitar el texto del área **Agrupar por**.
1. Reemplace el texto por el código siguiente :

   ```
   group.0.linkedname=project
   group.0.namekey=portfolio
   group.0.notime=false
   group.0.valuefield=project:portfolio:name
   group.0.valueformat=string
   group.1.linkedname=project
   group.1.namekey=program
   group.1.notime=false
   group.1.valuefield=project:program:name
   group.1.valueformat=string
   group.2.name=Project
   group.2.valuefield=project:name
   group.2.valueformat=HTML
   textmode=true
   ```

1. Haga clic en **Listo** > **Guardar agrupación**.
1. (Opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.

