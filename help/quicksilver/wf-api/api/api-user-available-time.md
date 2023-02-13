---
content-type: api
navigation-topic: wf-api
title: Obtener la API de tiempo disponible de los usuarios
description: Obtener la API de tiempo disponible de los usuarios
author: John
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: aea37c1d200dfadf9ccbb7b36145eb04d5ab4b6d
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# API de tiempo disponible para usuarios

**URI: attask/api/v15.0/user/getUsersAvailableTime**

El punto final de tiempo disponible para los usuarios recupera los datos en el tiempo disponible para el usuario. Esto permite integraciones para la agregación de datos según los atributos del usuario y los intervalos de tiempo.

## Solicitud de ejemplo

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parámetros de solicitud

* **userIDs**: matriz de cadenas. Requerido. Ejemplo: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. cadena. Requerido. Ejemplo:  `"2022-07-10T00:00:00"`.

* **toDate**: datetime. cadena. Requerido. Ejemplo `"2022-07-20T23:59:59"`.

## Ejemplo de respuesta:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Parámetros de respuesta

* **AVL**: Horas disponibles reales. Matriz de números.
* **PAVL**: Horario disponible puro para la programación que no incluye días no laborables o tiempo libre del usuario. Cadena.
