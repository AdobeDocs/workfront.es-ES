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
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 90%

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

PUT https://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234 ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­
* devuelve `status: "success"`

* devuelve `status: "failure", error: "File not found"`
