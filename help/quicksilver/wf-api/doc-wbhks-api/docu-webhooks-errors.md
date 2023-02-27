---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Gestión de errores de los Webhooks de documento
description: Gestión de errores de los Webhooks de documento
author: Becky
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Gestión de errores de los Webhooks de documento

Pueden surgir problemas al procesar solicitudes de API. Esto debe gestionarse de forma coherente en todos los extremos de la API. Cuando se produce un error, el proveedor de vínculos web debe incluir un código de error en el encabezado de respuesta. Los códigos de error incluyen:

* 403 - Prohibido. Indica que faltan tokens de solicitud o que no son válidos, o que las credenciales asociadas con los tokens no tienen acceso al recurso especificado. Para los proveedores de vínculos web basados en OAuth, Adobe Workfront intentará recuperar nuevos tokens de acceso.

* 404 - No encontrado. Indica que el archivo o la carpeta especificados no existen.

* 500 - Error interno del servidor. Cualquier otro tipo de error.

* Descripción del error en el cuerpo de respuesta con el siguiente formato:

   ```
   {status: “error”
    error: “Sample error message”}
   ```
