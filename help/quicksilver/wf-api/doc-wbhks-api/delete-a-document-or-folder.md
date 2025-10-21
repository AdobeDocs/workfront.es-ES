---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Eliminar un documento o una carpeta
description: Eliminar un documento o una carpeta
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '75'
ht-degree: 89%

---


# Eliminar un documento o una carpeta (aún no implementados)

Elimina un documento o una carpeta con el ID proporcionado en el sistema externo. Al eliminar una carpeta, también se elimina su contenido.

## URL

PUT /delete

## Parámetros de consulta

| Nombre | Descripción |
|---|---|
| documentId  | El identificador de documento que se va a eliminar |
| folderId  | El identificador de carpeta que se va a eliminar |



## Respuesta

Una cadena JSON que indica éxito o error, tal como se especifica en la sección Gestión de errores que viene a continuación.

### Ejemplo

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
