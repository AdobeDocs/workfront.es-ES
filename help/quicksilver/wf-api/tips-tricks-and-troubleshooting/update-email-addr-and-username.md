---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Actualizar a emailAddr no actualiza el nombre de usuario
description: La actualización a emailAddr no actualiza el usernam
author: John
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Actualizar a emailAddr no actualiza el nombre de usuario

## Problema

Normalmente, `emailAddr` y `username` son el mismo atributo. Por lo tanto, si cambia la `emailAddr` el atributo `username` se actualiza automáticamente para que coincida.

Cuando la variable `username` no coincide con la variable `emailAddr`, una actualización de `emailAddr` no actualiza el `username` automáticamente. Esto se aplica a ambos `emailAddr` cambia a través de la interfaz de usuario y a través de la API .

## Causa

El desajuste puede crearse de varias formas:

* Usuarios creados antes de que existiera la regla de sincronización. Es posible que las cuentas de usuario muy antiguas no tengan estos atributos sincronizados.

* Los usuarios creados mediante SSO en un momento en el que el emailAddr de Workfront distingue entre mayúsculas y minúsculas. La opción de aprovisionamiento automático de SSO ejecutaría una comprobación que distingue entre mayúsculas y minúsculas para los usuarios en función de los atributos del usuario del proveedor de identidad. Cuando no existía una coincidencia exacta, los servicios de aprovisionamiento automático creaban un nuevo usuario. Si un usuario ya existía, era posible que el nombre de usuario y `emailAddr` no tendría la misma carcasa.

* Usuarios que han tenido la variable `username` se actualiza directamente mediante la API y sus `emailAddr` no se actualizó. La variable `username` y `emailAddr` posiblemente no coincidan.

## Solución

Utilice la API para cambiar la variable `username` para que sea el mismo que el `emailAddr`. Después de sincronizar los atributos, cualquier actualización a la variable `emailAddr` también actualizará la variable `username` para que coincida (cuando el campo de nombre de usuario no está incluido en la actualización).
