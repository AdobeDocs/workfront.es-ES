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
TQID: https://experienceleague.adobe.com/7-f8Z3qQQ2z7ZHHfSrGgJqIQCKdeqEoL96XlfCGzYSo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 75
ht-degree: 100%

---

# Eliminación de un documento o una carpeta (aún no implementado)

Elimina un documento o una carpeta con el ID proporcionado en el sistema externo. Al eliminar una carpeta, también se elimina su contenido.

## URL

PUT /delete

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| documentId  | El identificador de documento que se va a eliminar |
| folderId  |  El identificador de carpeta que se va a eliminar |



## Respuesta

Una cadena JSON que indica éxito o error, tal como se especifica en la sección Gestión de errores que viene a continuación.

### Ejemplo

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
