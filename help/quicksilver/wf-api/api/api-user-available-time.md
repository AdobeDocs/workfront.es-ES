---
content-type: api
navigation-topic: wf-api
title: Obtener los usuarios disponibles API de tiempo
description: Obtener los usuarios disponibles API de tiempo
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 9%

---

# API de tiempo de usuarios disponible

**URI: attask/api/v15.0/user/getUsersAvailableTime**

El punto final de tiempo de los usuarios disponibles recupera los datos en el tiempo disponible del usuario. Esto permite realizar integraciones para agregar datos de acuerdo con los atributos del usuario y los intervalos de tiempo.

## Solicitud de ejemplo

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parámetros de solicitud

* **userIDs**: matriz de cadenas. Requerido. Ejemplo: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. cadena. Requerido. Ejemplo:  `"2022-07-10T00:00:00"`.

* **toDate**: datetime. cadena. Requerido. Ejemplo `"2022-07-20T23:59:59"`.

## Respuesta de ejemplo:

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
* **PAVL**: Horas puramente disponibles para la programación que no incluyen días no laborables o días libres del usuario. Cadena.
