---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Cambiar el nombre de un documento o carpeta (aún no implementado)
description: Cambiar el nombre de un documento o carpeta
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 8%

---


# Cambiar el nombre de un documento o carpeta (aún no implementado)

Cambia el nombre de un documento o carpeta con el ID proporcionado en el sistema externo.

**URL**

PUT /name

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id | Identificador de documento o carpeta cuyo nombre se va a cambiar |
| name  | El nuevo nombre del documento o la carpeta |


## respuesta

Una cadena JSON que indica éxito o error, como se especifica en la sección Gestión de errores a continuación.

**Ejemplo:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

devoluciones

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
