---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Cambiar el nombre de un documento o carpeta (aún no implementado)
description: Cambiar el nombre de un documento o carpeta
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# Cambiar el nombre de un documento o carpeta (aún no implementado)

Cambia el nombre de un documento o carpeta por el ID dado en el sistema externo.

**Dirección URL**

PUT /cambiar nombre

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id | El ID de documento o carpeta al que cambiar el nombre |
| name  | El nuevo nombre del documento o carpeta |


## respuesta

Una cadena JSON que indica que se ha realizado correctamente o que se ha producido un error, tal como se especifica en la sección Error Handling a continuación.

**Ejemplo:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

return

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
