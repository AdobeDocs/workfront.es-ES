---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupación: Proyectos por fecha de entrada'
description: En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por sus valores de Fecha de entrada.
author: Courtney
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/173W6SSSF18yuWOs0wD684ZmYQlQE-H24MZNVXZsomE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 220
ht-degree: 79%

---

# Agrupación: proyectos por fecha de entrada

<!--Audited: 10/2024-->

En esta agrupación de proyectos personalizada, puede mostrar los proyectos agrupados por sus valores de Fecha de entrada.

Cada agrupación muestra los proyectos con una fecha de entrada en:

* Los últimos 30 días
* entre 30 y 60 días
* 60 días o más

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
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

## Agrupar proyectos por fecha de entrada

Para aplicar esta agrupación:

1. Vaya a un informe de proyecto existente o cree un nuevo informe de proyecto.\
   Para obtener más información acerca de cómo crear un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Haga clic en **Acciones de informe** > **Editar**.
1. En la pestaña **Agrupación**, haga clic en **Añadir agrupación**.
1. Haga clic en **Cambiar a modo texto**.
1. Quitar el texto del área **Agrupar por**.
1. Reemplace el texto por el código siguiente :


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. Haga clic en **Listo** > **Guardar agrupación**.
1. (Opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.
