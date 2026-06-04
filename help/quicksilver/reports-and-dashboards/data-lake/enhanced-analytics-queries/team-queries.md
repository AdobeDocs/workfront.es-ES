---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Actividad por consultas de equipo
description: Consultas de análisis mejorado
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 6f07e52b-b813-4b3a-9333-0c9300e051ca
TQID: https://experienceleague.adobe.com/q4x3b0G-hwtFUAkNyRp1oWnAi09Kh8qFO77U8aDEl98
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 172
ht-degree: 18%

---

# Actividad por consultas de equipo

Puede utilizar las consultas de este artículo para crear visualizaciones de datos similares a las de Enhanced Analytics.

>[!IMPORTANT]
>
>Las consultas producirán resultados similares a los que se muestran en el análisis mejorado, pero es posible que no coincidan exactamente.


## Requisitos previos

Antes de empezar, debe

1. Establezca una conexión con la herramienta Business Intelligence (BI):
   1. [Crear una cuenta de lector o una conexión para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Establecimiento de una conexión con Workfront Data Conect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Una vez establecida una conexión, puede utilizar las consultas de este artículo para extraer y visualizar datos.

## Eventos de inicio de sesión de los usuarios de Home Teams 

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(ul.lastlogindate) 
```

### Eventos de inicio de sesión de usuarios de equipos de inicio: explorar en profundidad

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(ul.lastlogindate)
```

## Eventos de inicio de sesión de usuarios de Teams

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM teammembers_current tmc 
    inner join teams_current tc on tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    inner join userlogins ul on tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(ul.lastlogindate)
```

### Eventos de inicio de sesión de los usuarios de Teams: explorar en profundidad

```
WITH userlogins as ( 
    SELECT userid, lastlogindate 
    FROM ( 
        SELECT userid, lastlogindate, lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid  ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate), count(*) 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN userlogins ul ON tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate)
```



## Eventos de cambio de estado de las tareas de los usuarios de Home Teams 

```
WITH task_status_changes as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    ) 
    WHERE status != previous_status 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid,  TO_DATE(tsc.begin_effective_timestamp)
```

### Eventos de cambio de estado de las tareas de los usuarios de Equipos de inicio: explorar en profundidad

```
WITH task_status_changes as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    ) 
    WHERE status != previous_status 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tsc.begin_effective_timestamp)
```

## Eventos de cambio de estado de tareas de usuarios de equipos

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
) 

SELECT tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp), count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp) 
```

### Eventos de cambio de estado de tareas de usuarios de equipos: explorar en profundidad

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
WHERE status != previous_status  
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    inner join teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    inner join assignments_current ac ON tmc.userid = ac.assignedtoid  
    inner join task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tsc.begin_effective_timestamp) 
```

## Eventos de finalización de tareas de los usuarios de Equipos de inicio

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(tasks_done.task_completion_date)
```

### Eventos de finalización de tareas de usuarios de equipos de inicio: explorar en profundidad

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        ) 
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tasks_done.task_completion_date) 
```

## Eventos de finalización de tareas de usuarios de equipos

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(tasks_done.task_completion_date) 
```

### Eventos de finalización de tareas de usuarios de equipos: explorar en profundidad

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT taskid, actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tasks_done.task_completion_date) 
```
