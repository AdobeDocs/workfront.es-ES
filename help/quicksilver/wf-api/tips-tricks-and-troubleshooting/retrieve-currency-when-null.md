---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperar información de moneda para un proyecto cuando la moneda es nula
description: Recuperar información de moneda para un proyecto cuando la moneda es nula
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
TQID: https://experienceleague.adobe.com/fWBcEeqoJFK6WzcEE2Ajqv6cdxk0J9IN1CiPPGU6pIg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 9%

---

# Recuperar información de moneda para un proyecto cuando la moneda tiene un valor nulo (no asignada)

El objeto de proyecto con el campo de moneda se puede recuperar mediante la siguiente solicitud:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Esto devolverá el siguiente cuerpo de respuesta:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Si la moneda no está establecida para el proyecto, esta respuesta incluiría una moneda con el valor `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Si necesita la divisa para el proyecto (por ejemplo, para cálculos), puede recuperar la divisa predeterminada para el cliente:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

La respuesta incluye la moneda que el usuario ha establecido como predeterminada, que se utilizaría en cualquier proyecto para ese cliente que no tenga la moneda configurada:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
