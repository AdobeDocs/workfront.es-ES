---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Gestión de errores de webhooks de documentos
description: Gestión de errores de webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 100%

---

# Gestión de errores de webhooks de documentos

Pueden surgir problemas al procesar solicitudes de API. Esto se debe gestionar de forma coherente en todos los puntos finales de la API. Cuando se produce un error, el proveedor de webhooks debe incluir un código de error en el encabezado de respuesta. Los códigos de error incluyen los siguientes:

* 403 - Prohibido. Indica que faltan los tókenes de solicitud o que no son válidos, o bien que las credenciales asociadas con los tókenes no tienen acceso al recurso especificado. Para los proveedores de webhooks basados en OAuth, Adobe Workfront intentará recuperar nuevos tokens de acceso.

* 404 - No se encuentra. Indica que el archivo o la carpeta especificados no existen.

* 500 - Error de servidor interno. Cualquier otro tipo de error.

* Descripción del error en el cuerpo de respuesta con el siguiente formato:

  ```
  {status: "error"
   error: "Sample error message"}
  ```
