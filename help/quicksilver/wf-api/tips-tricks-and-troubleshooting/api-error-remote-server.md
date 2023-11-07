---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Mensaje de error de API 400 Solicitud incorrecta
description: Mensaje de error de API 400 Solicitud incorrecta
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Error de API: &quot;El servidor remoto devolvió un error (400) Solicitud incorrecta&quot;

## Problema

Se obtiene el siguiente error al intentar utilizar la API para importar un campo personalizado a un problema:

`The remote server returned an error: (400) Bad Request`

## Causa

Este error se produce cuando intenta importar, a través de la API, un campo personalizado de un proyecto que no tiene un formulario personalizado asociado a un tema de la cola.

## Solución

Agregue el formulario personalizado correcto al tema de la cola.

Para obtener más información sobre los temas de colas, consulte [Crear temas de cola](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
