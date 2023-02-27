---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Información general de Webhooks
description: Información general de Webhooks
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Información general de Webhooks

Adobe Workfront Document Webhooks define un conjunto de extremos de API a través de los cuales Workfront realiza llamadas de API autorizadas a un proveedor de documentos externo. Esto permite a cualquier persona crear un complemento de middleware para cualquier proveedor de almacenamiento de documentos.

![](assets/mceclip0-350x262.png)

La experiencia del usuario para las integraciones basadas en weblock será similar a la de las integraciones de documentos existentes, como Google Drive, Box y Dropbox. Por ejemplo, un usuario de Workfront podrá realizar las siguientes acciones:

* Navegar por la estructura de carpetas del proveedor de documentos externo
* Buscar archivos
* Vinculación de archivos a Workfront
* Cargar archivos al proveedor de documentos externo
* Ver una miniatura del documento

**Implementación de referencia**

Para ayudar a iniciar el desarrollo de una nueva implementación de enlaces web, Workfront proporciona una implementación de referencia. El código para esto se puede encontrar en [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . Esta implementación se basa en Java y permite a Workfront conectar documentos en un sistema de archivos de red. 

## Versiones

* Versión 1.0 (Fecha de versión - mayo de 2015): Especificación inicial

* Versión 1.1 (Fecha de versión - junio de 2015). Se ha actualizado /uploadInit - Se ha añadido documentId y documentVersionId

* Versión 1.2 (Fecha de versión - octubre de 2015): Se ha añadido /createFolder

* Próximas versiones (Fecha de versión - TBD):

   * Se ha añadido /delete
   * Se ha añadido /cambiar nombre
   * Se ha añadido /serviceInfo
   * Se ha añadido /customAction
   * Agregue paginación y parentId a /search
