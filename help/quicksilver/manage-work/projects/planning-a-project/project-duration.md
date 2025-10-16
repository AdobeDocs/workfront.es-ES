---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la duración del proyecto
description: Adobe Workfront calcula la duración de un proyecto teniendo en cuenta la fecha de inicio de la primera tarea y la fecha de finalización de la última tarea, y cuenta el número de días entre las dos fechas.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 98%

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
