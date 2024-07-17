---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperar información de moneda para un proyecto cuando la moneda es nula
description: Recuperar información de moneda para un proyecto cuando la moneda es nula
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Recuperar información de moneda para un proyecto cuando la moneda es nula (no asignada)

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
