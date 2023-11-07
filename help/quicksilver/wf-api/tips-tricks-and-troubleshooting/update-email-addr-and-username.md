---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: La actualización a emailAddress no actualiza el nombre de usuario
description: La actualización a emailAddress no actualiza el nombre de usuario
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# La actualización a emailAddress no actualiza el nombre de usuario

## Problema

Normalmente, `emailAddr` y `username` son el mismo atributo. Por lo tanto, si cambia el de un usuario `emailAddr` atributo, el `username` se actualiza automáticamente para que coincida con.

Si la variable `username` no coincide con el `emailAddr`, una actualización del `emailAddr` no actualiza el `username` automáticamente. Esto es así para ambos `emailAddr` cambios a través de la interfaz de usuario y de la API.

## Causa

El desajuste puede crearse de varias formas:

* Usuarios creados antes de que existiera la regla de sincronización. Las cuentas de usuario muy antiguas pueden no tener estos atributos sincronizados.

* Los usuarios creados mediante SSO en un momento en que la dirección de correo electrónico de Workfront distinguía entre mayúsculas y minúsculas. La opción de aprovisionamiento automático de SSO ejecutaría una comprobación que distingue entre mayúsculas y minúsculas para los usuarios en función de los atributos del usuario del proveedor de identidad. Cuando no existía una coincidencia exacta, los servicios de aprovisionamiento automático creaban un nuevo usuario. Si ya existía un usuario, era posible que el nombre de usuario y `emailAddr` no tendría la misma carcasa.

* Usuarios que han tenido la `username` se actualizan directamente a través de la API y sus `emailAddr` no se ha actualizado. El `username` y `emailAddr` posiblemente no coincidan.

## Solución

Utilice la API para cambiar el `username` el atributo debe ser el mismo que `emailAddr`. Después de sincronizar los atributos, cualquier actualización del `emailAddr` también actualizará el `username` para que coincida (cuando el campo de nombre de usuario no se incluye en la actualización).
