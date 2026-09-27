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
TQID: 'https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 70%
---
# Cambiar el nombre de un documento o carpeta (aún no implementado)

Cambia el nombre de un documento o carpeta con el ID proporcionado en el sistema externo.

**URL**

PUT /rename

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id | El identificador de documento o carpeta cuyo nombre se va a cambiar |
| name  | El nuevo nombre del documento o la carpeta |


## Respuesta

Una cadena JSON que indica éxito o error, tal como se especifica en la sección Gestión de errores que viene a continuación.

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
