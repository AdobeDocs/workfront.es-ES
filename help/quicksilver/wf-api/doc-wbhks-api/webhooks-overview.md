---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Información general sobre webhooks
description: Información general sobre webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Información general sobre webhooks

Adobe Workfront Document Webhooks define un conjunto de extremos de API a través de los cuales Workfront realiza llamadas de API autorizadas a un proveedor de documentos externo. Esto permite a cualquier persona crear un complemento de middleware para cualquier proveedor de almacenamiento de documentos.

![](assets/mceclip0-350x262.png)

La experiencia del usuario para integraciones basadas en ganchos web será similar a la de integraciones de documentos existentes, como Google Drive, Box y Dropbox. Por ejemplo, un usuario de Workfront podrá realizar las siguientes acciones:

* Navegar por la estructura de carpetas del proveedor de documentos externo
* Buscar archivos
* Vinculación de archivos a Workfront
* Cargar archivos al proveedor de documentos externo
* Ver una miniatura del documento

**Implementación de referencia**

Para ayudar a impulsar el desarrollo de una nueva implementación de webhooks, Workfront proporciona ejemplos de una implementación de referencia. Estos ejemplos se encuentran en [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Los ejemplos están basados en Java y permiten a Workfront conectar documentos en un sistema de archivos de red. 

>[!NOTE]
>
>Los recursos de GitHub son solo ejemplos y no pueden ejecutar una implementación.

## Versiones

* Versión 1.0 (Fecha de versión: mayo de 2015): Especificación inicial

* Versión 1.1 (Fecha de versión: junio de 2015). Se ha actualizado /uploadInit: ID de documento y ID de versión de documento añadidos

* Versión 1.2 (Fecha de lanzamiento: octubre de 2015): Se ha añadido /createFolder

* Próximas versiones (fecha de lanzamiento: por determinar):

   * Añadido /delete
   * Añadido /name
   * Se ha añadido /serviceInfo
   * Se ha añadido /customAction
   * Añadir paginación y parentId a /search
