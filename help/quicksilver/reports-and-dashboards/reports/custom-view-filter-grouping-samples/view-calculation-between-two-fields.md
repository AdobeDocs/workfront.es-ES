---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: mostrar el resultado de un cálculo entre dos campos de una columna'
description: Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ggwDFu-5dxDHNvX7JR9tWf730CFUrk0RF7Bu9QHgu9w
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
source-wordcount: 324
ht-degree: 90%

---

# Vista: mostrar el resultado de un cálculo entre dos campos de una columna

<!--Audited: 11/2024-->

Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos.

Por ejemplo, si desea averiguar el número de días de la semana que han transcurrido entre dos fechas, puede utilizar la sintaxis del modo de texto y expresiones de datos para calcular esta diferencia.\
Por ejemplo, puede calcular la diferencia de días de la semana entre la fecha planificada de finalización y la fecha real de finalización de una tarea y mostrar el resultado en una columna.

Puede utilizar otras dos fechas en este cálculo (inicio real, finalización real, inicio proyectado, finalización proyectada, etc.).\
Para obtener más información sobre las expresiones de datos calculados, consulte [Información general sobre las expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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


## Mostrar el resultado de un cálculo entre dos campos en una columna

Para añadir esta columna a una vista de tareas:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y, a continuación, **Cambiar al modo de texto** > **Editar modo de texto**.
1. Quite el texto que encuentra en el cuadro **Modo de texto** y sustitúyalo por el siguiente código:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Opcional) Para añadir los valores mostrados en la vista en una agrupación, siga los pasos descritos en [Agrupación: mostrar el resultado de agregar varios valores calculados en una agrupación](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Haga clic en **Listo** y luego en **Guardar vista**.
