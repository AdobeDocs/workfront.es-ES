---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la duración del proyecto
description: Adobe Workfront calcula la duración de un proyecto teniendo en cuenta la fecha de inicio de la primera tarea y la fecha de finalización de la última tarea, y cuenta el número de días entre las dos fechas.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 96%

---

# Información general sobre la duración de un proyecto

Adobe Workfront calcula la duración de un proyecto teniendo en cuenta la fecha de inicio de la primera tarea y la fecha de finalización de la última tarea, y cuenta el número de días entre las dos fechas.

## Duración de proyecto

La duración del proyecto se calcula mediante la fórmula siguiente:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>La duración de los problemas del proyecto no afecta a la duración del proyecto.

La duración del proyecto cuenta el número de días entre las dos fechas de la tarea en función de la programación asociada con el proyecto o los usuarios asignados a las tareas. Para obtener información acerca de la programación que Workfront usa para calcular la duración, consulte [Información general sobre programaciones](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Tipos de duración del proyecto

Existen dos tipos de Duración del proyecto y las fórmulas mediante las cuales Workfront los calcula:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Duración planificada**:

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Duración real**:

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Buscar la duración del proyecto

Puede localizar las duraciones planificadas y reales del proyecto en las siguientes áreas de Workfront:

* . En el área Detalles del proyecto, en la sección Información general.

  Para obtener más información acerca de la subficha Información general de un proyecto, consulte el artículo [Administrar información en el área Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* En un informe de proyecto, incluyendo los campos Duración o Duración real en el informe.

  Para obtener más información acerca de la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
