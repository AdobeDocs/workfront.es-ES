---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperar información de moneda para un proyecto cuando la moneda es nula
description: Recuperar información de moneda para un proyecto cuando la moneda es nula
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Recuperar información de moneda para un proyecto cuando la moneda es nula (no está asignada)

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

Si la moneda no está configurada para el proyecto, esta respuesta incluiría una moneda con el valor `null`:

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

Si necesita la moneda para el proyecto (por ejemplo, para los cálculos), puede recuperar la moneda predeterminada para el cliente:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

La respuesta incluye la moneda que el usuario ha establecido como predeterminada, que sería utilizada por cualquier proyecto para ese cliente que no tenga configurada la moneda:

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
