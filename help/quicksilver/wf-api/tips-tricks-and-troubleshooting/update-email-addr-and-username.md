---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Al actualizarse emailAddress no se actualiza username
description: Al actualizarse emailAddress no se actualiza username
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
TQID: https://experienceleague.adobe.com/dkceJuJ6WfaZTnbD6zdP6TsHR5bvkERD-EiBgVmrCck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 100%

---

# Al actualizarse emailAddress no se actualiza username

## Problema

Normalmente, `emailAddr` y `username` son el mismo atributo. Por lo tanto, si cambia el atributo `emailAddr` de un usuario, el atributo `username` se actualiza automáticamente para que coincida.

Cuando `username` no coincide con `emailAddr`, la actualización de `emailAddr` no actualiza `username` automáticamente. Esto es así para los cambios de `emailAddr` realizados en la interfaz de usuario y la API.

## Causa

Este desajuste puede generarse debido a lo siguiente:

* Por usuarios que se crearon antes de que existiera la regla de sincronización. Puede ser que los atributos de las cuentas de usuario muy antiguas que no estén sincronizados.

* Por usuarios que se crearon mediante SSO en un momento en que la dirección de correo electrónico de Workfront distinguía entre mayúsculas y minúsculas. La opción de aprovisionamiento automático de SSO ejecutaba una comprobación que distinguía entre mayúsculas y minúsculas para los usuarios basándose en los atributos del usuario del proveedor de identidad. Si no existía una coincidencia exacta, los servicios de aprovisionamiento automático creaban un nuevo usuario. Si ya existía un usuario, existía la posibilidad de que las mayúsculas y minúsculas del nombre de usuario y de `emailAddr` no coincidieran.

* Los usuarios a los que se les ha actualizado el atributo `username` directamente a través de la API y cuyo atributo `emailAddr` no se ha actualizado. Es posible que `username` y `emailAddr` no coincidan.

## Solución

Utilice la API para cambiar el atributo `username` para que sea el mismo que `emailAddr`. Después de sincronizar los atributos, cualquier actualización de `emailAddr` actualizará también `username` para que coincidan (cuando el campo de nombre de usuario no esté incluido en la actualización).
