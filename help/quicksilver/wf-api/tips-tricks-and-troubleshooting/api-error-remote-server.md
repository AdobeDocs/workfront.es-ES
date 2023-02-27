---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Mensaje de error de API 400 Solicitud incorrecta
description: Mensaje de error de API 400 Solicitud incorrecta
author: Becky
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Error de API: &quot;El servidor remoto devolvió un error (400) Solicitud incorrecta&quot;

## Problema

Se produce el siguiente error al intentar utilizar la API para importar un campo personalizado en un problema:

`The remote server returned an error: (400) Bad Request`

## Causa

Este error se produce cuando intenta importar, a través de la API, un campo personalizado de un proyecto que no tiene un formulario personalizado asociado a un tema de cola.

## Solución

Agregue el formulario personalizado correcto al tema de cola.

Para obtener más información sobre los temas de cola, consulte [Crear temas de cola](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
