---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Consultas de diagrama de proyecto
description: Consultas mejoradas de Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
source-git-commit: bd39c5794c55e27a876da185e67bf8c654a003b2
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 5%

---

# Consultas de diagrama de proyecto

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

## Horas planificadas de proyectos retiradas

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Horas planificadas de proyectos retiradas: evolución

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## Duración planificada de proyectos retirada 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Duración planificada de proyectos retirada: evolución

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```
