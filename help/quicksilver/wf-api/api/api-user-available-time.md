---
content-type: api
navigation-topic: wf-api
title: Obtener la API de tiempo disponible de los usuarios
description: Obtener la API de tiempo disponible de los usuarios
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 100%

---

# API de tiempo disponible de los usuarios

**URI: attask/api/v15.0/user/getUsersAvailableTime**

El punto final de tiempo disponible de los usuarios recupera datos sobre el tiempo disponible del usuario. Esto permite integraciones para la agregación de datos según los atributos del usuario y los intervalos de tiempo.

## Solicitud de ejemplo

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parámetros de solicitud

* **userIDs**: matriz de cadenas. necesario. Ejemplo: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. cadena. necesario. Ejemplo: `"2022-07-10T00:00:00"`.

* **toDate**: datetime. cadena. necesario. Ejemplo `"2022-07-20T23:59:59"`.

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

* **AVL**: horas disponibles reales. Matriz de números.
* **PAVL**: horas puras disponibles para la programación que no incluyen los días no laborables ni los días libres del usuario. Cadena.
