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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 5%

---


# Eliminar un documento o una carpeta (aún no implementado)

Elimina un documento o una carpeta con el ID proporcionado en el sistema externo. Al eliminar una carpeta, también se elimina su contenido.

## URL

PUT /delete

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| documentId  | Identificador de documento que se va a eliminar |
| folderId  |  Identificador de carpeta que se va a eliminar |



## Respuesta

Una cadena JSON que indica éxito o error, como se especifica en la sección Gestión de errores a continuación.

### Ejemplo

PUT https://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234
* devuelve `status: "success"`

* devuelve `status: "failure", error: "File not found"`
