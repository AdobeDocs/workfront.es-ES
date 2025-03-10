---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Consultas de KPI
description: Consultas mejoradas de Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 9ca5574d-7bc5-4d9d-9ed7-4d5fad6f7857
source-git-commit: 905aaaa5d300bc71058dd6ee2d568c8fc1229570
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 5%

---

# Consultas de KPI

Puede utilizar las consultas de este artículo para crear visualizaciones de datos similares a las de Enhanced Analytics.

>[!IMPORTANT]
>
>Las consultas producirán resultados similares a los que se muestran en el análisis mejorado, pero es posible que no coincidan exactamente.


## Requisitos previos

Antes de empezar, debe

1. Establezca una conexión con la herramienta Business Intelligence (BI):
   1. [Crear una cuenta de lector o una conexión para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Establezca una conexión con Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Una vez establecida una conexión, puede utilizar las consultas de este artículo para extraer y visualizar datos.

## Proyectos finalizados

El KPI de proyectos completados muestra cuántos proyectos se han completado dentro del período de tiempo filtrado, así como cómo ha aumentado o disminuido el porcentaje desde el período de tiempo anterior.

También puede ver el número de proyectos completados en el período de tiempo anterior, así como el número de días en el período de tiempo anterior.

![Proyectos KPI completados](assets/kpi-projects-completed-350x182.png)

### Consulta

```
WITH completedProjectsInRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
    SELECT 
        (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD 
    FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
    SELECT 
        CASE 
            WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
            WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
        END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
    FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
    a.PROJECT_COUNT, 
    b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## Proyectos finalizados a tiempo

El KPI Proyectos finalizados a tiempo muestra el porcentaje de proyectos dentro del período de tiempo filtrado que se finalizaron a tiempo, así como la forma en que el porcentaje aumentó o disminuyó desde el período de tiempo anterior.

También puede ver el porcentaje de proyectos completados a tiempo en el período de tiempo anterior, así como el número de días en el período de tiempo anterior.

![Proyectos KPI completados a tiempo](assets/kpi-projects-completed-on-time-350x180.png)

```
WITH completedProjectsInRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedOntimeProjectsInRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
        AND t0.PROGRESSSTATUS = 'ON' 
), percentOntimeProjects as ( 
    SELECT 
        CASE 
            WHEN a.PROJECT_COUNT = 0 THEN 0 
            ELSE ROUND(b.PROJECT_COUNT/a.PROJECT_COUNT) * 100 
        END as ONTIMEPROJECTPERCENT 
    FROM completedProjectsInRange a, completedOntimeProjectsInRange b 
), completedProjectsPreviousRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), completedOntimeProjectsPreviousRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
        AND t0.PROGRESSSTATUS = 'ON' 
), percentOntimeProjectsPreviousRange as ( 
    SELECT 
        CASE 
            WHEN a.PROJECT_COUNT = 0 THEN 0 
            ELSE ROUND(b.PROJECT_COUNT/a.PROJECT_COUNT) * 100 
        END as ONTIMEPROJECTPERCENT 
    FROM completedProjectsPreviousRange a, completedOntimeProjectsPreviousRange b 
), rawChange as ( 
    SELECT 
        (a.ONTIMEPROJECTPERCENT - b.ONTIMEPROJECTPERCENT) as CHANGE_FROM_PREVIOUS_PERIOD 
    FROM percentOntimeProjects a, percentOntimeProjectsPreviousRange b 
), percentChange as ( 
    SELECT  
        CASE 
            WHEN a.ONTIMEPROJECTPERCENT = b.ONTIMEPROJECTPERCENT THEN 0 
            WHEN b.ONTIMEPROJECTPERCENT > 0 THEN ((a.ONTIMEPROJECTPERCENT - b.ONTIMEPROJECTPERCENT) / b.ONTIMEPROJECTPERCENT * 100) 
        END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
    FROM percentOntimeProjects a, percentOntimeProjectsPreviousRange b 
) 

SELECT 
    a.ONTIMEPROJECTPERCENT, 
    b.ONTIMEPROJECTPERCENT as PREVIOUS_ONTIMEPROJECTPERCENT, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM percentOntimeProjects a, percentOntimeProjectsPreviousRange b, rawChange c, 
percentChange d
```

## Media  de duración del proyecto

El KPI promedio KPI de duración del proyecto muestra la cantidad promedio de tiempo de finalización (en días, semanas o años) para proyectos con fechas de finalización reales dentro del período de tiempo filtrado, así como la forma en que el porcentaje aumentó o disminuyó desde el período de tiempo anterior.

También puede ver la cantidad promedio de tiempo de finalización de los proyectos con fechas de finalización reales en el período de tiempo anterior, así como el número de días en el período de tiempo anterior.

>[!NOTE]
>
>Esto solo tiene en cuenta la duración de los proyectos completados.


![Duración promedio de proyecto de KPI](assets/kpi-avg.-project-duration-350x168.png)

```
WITH averageProjectDurationInRange as ( 
    SELECT 
        AVG(t0.ACTUALDURATIONMINUTES) as AVERAGE_PROJECT_DURATION 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), averageProjectPreviousRange as ( 
    SELECT AVG (t0. ACTUALDURATIONMINUTES) as AVERAGE_PROJECT_DURATION FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
    SELECT ((a.AVERAGE_PROJECT_DURATION - b.AVERAGE_PROJECT_DURATION) / 480) as CHANGE_FROM_PREVIOUS_PERIOD FROM averageProjectDurationInRange a, averageProjectPreviousRange b 
), percentChange as ( 
    SELECT  
        CASE 
            WHEN a.AVERAGE_PROJECT_DURATION = b.AVERAGE_PROJECT_DURATION THEN 0 
            WHEN b.AVERAGE_PROJECT_DURATION > 0 THEN ((a.AVERAGE_PROJECT_DURATION - b.AVERAGE_PROJECT_DURATION)  / b.AVERAGE_PROJECT_DURATION) * 100 
        END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
        FROM averageProjectDurationInRange a, averageProjectPreviousRange b 
) 
 
SELECT 
    a.AVERAGE_PROJECT_DURATION, 
    b.AVERAGE_PROJECT_DURATION as PREVIOUS_AVERAGE_PROJECT_DURATION, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM averageProjectDurationInRange a, averageProjectPreviousRange b, rawChange c, 
percentChange d
```

## Media de tareas por proyecto

El KPI Promedio de tareas por proyecto muestra el número promedio de tareas asignadas a proyectos dentro del período de tiempo filtrado, así como la forma en que el porcentaje de tareas ha aumentado o disminuido desde el período de tiempo anterior.

También puede ver el número promedio de tareas asignadas a proyectos en el período de tiempo anterior, así como el número de días en el período de tiempo anterior.

![Tareas promedio de KPI por proyecto](assets/kpi-average-tasks-per-project-350x179.png)

```
WITH tasksPerProjectInRange as ( 
    SELECT 
        COUNT(t0.TASKID) as TASK_COUNT 
    FROM TASKS_CURRENT t0 
        LEFT JOIN PROJECTS_CURRENT t1 ON t1.PROJECTID = t0.PROJECTID 
    WHERE 
        ( 
            t1.PLANNEDSTARTDATE >= '2025-01-01' 
            AND t1.PLANNEDSTARTDATE <= '2025-01-31' 
        ) 
        OR ( 
            t1.PLANNEDCOMPLETIONDATE >= '2025-01-01' 
            AND t1. PLANNEDCOMPLETIONDATE <= '2025-01-31' 
        ) 
        OR ( 
            t1.PLANNEDSTARTDATE <= '2025-01-01' 
            AND t1. PLANNEDCOMPLETIONDATE >= '2025-01-31' 
        ) 
    GROUP BY t0.PROJECTID 
), averageTasksPerProjectInRange as ( 
    SELECT AVG(TASK_COUNT) AS AVERAGE_TASK_COUNT FROM tasksPerProjectInRange 
), tasksPerProjectInPreviousRange as ( 
    SELECT 
        COUNT(t0.TASKID) as TASK_COUNT 
    FROM TASKS_CURRENT t0 
        LEFT JOIN PROJECTS_CURRENT t1 ON t1.PROJECTID = t0.PROJECTID 
    WHERE 
        ( 
            t1.PLANNEDSTARTDATE >= '2024-12-01' 
            AND t1.PLANNEDSTARTDATE <= '2024-12-31' 
        ) 
        OR ( 
            t1.PLANNEDCOMPLETIONDATE >= '2024-12-01' 
            AND t1. PLANNEDCOMPLETIONDATE <= '2024-12-31' 
        ) 
        OR ( 
            t1.PLANNEDSTARTDATE <= '2024-12-01' 
            AND t1. PLANNEDCOMPLETIONDATE >= '2024-12-31' 
        ) 
    GROUP BY t0.PROJECTID 
), averageTasksPerProjectInPreviousRange as ( 
    SELECT 
        AVG(TASK_COUNT) AS AVERAGE_TASK_COUNT 
        FROM tasksPerProjectInPreviousRange 
), rawChange as ( 
    SELECT 
        (a.AVERAGE_TASK_COUNT - b.AVERAGE_TASK_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD 
    FROM averageTasksPerProjectInRange a, averageTasksPerProjectInPreviousRange b 
), percentChange as ( 
    SELECT 
        CASE 
            WHEN a.AVERAGE_TASK_COUNT = b.AVERAGE_TASK_COUNT THEN 0 
            WHEN b.AVERAGE_TASK_COUNT > 0 THEN ((a.AVERAGE_TASK_COUNT - b.AVERAGE_TASK_COUNT) / b.AVERAGE_TASK_COUNT) * 100  
        END as PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
    FROM averageTasksPerProjectInRange a, averageTasksPerProjectInPreviousRange b 
) 
 
SELECT 
    a.AVERAGE_TASK_COUNT, 
    b.AVERAGE_TASK_COUNT as PREVIOUS_AVERAGE_TASK_COUNT, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM averageTasksPerProjectInRange a, averageTasksPerProjectInPreviousRange b, rawChange c, percentChange d
```

## Resolución de problemas

* **Sin resultados**: Si la consulta no devuelve ningún resultado, compruebe que las comillas dobles y simples se hayan copiado correctamente.