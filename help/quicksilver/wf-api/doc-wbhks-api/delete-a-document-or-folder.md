---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Eliminar un documento o una carpeta
description: Eliminar un documento o una carpeta
author: Becky
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# Eliminar un documento o carpeta (aún no implementado)

Elimina un documento o carpeta con el ID dado en el sistema externo. Al eliminar una carpeta, también se elimina el contenido de la misma.

## Dirección URL

PUT /delete

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| documentId  | El ID del documento que se va a eliminar |
| folderId  |  El ID de carpeta que se va a eliminar |



## respuesta

Una cadena JSON que indica que se ha realizado correctamente o que se ha producido un error, tal como se especifica en la sección Error Handling a continuación.

### Ejemplo

PUT https://www.example.com/api/deleteid=1234
* return `status: “success”`

* return `status: “failure”, error: “File not found”`
