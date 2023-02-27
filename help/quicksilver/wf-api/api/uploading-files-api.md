---
content-type: api
navigation-topic: api-navigation-topic
title: Carga de archivos mediante la API
description: Carga de archivos mediante la API
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Carga de archivos mediante la API

Puede cargar archivos mediante las API de Workfront con herramientas de API como Postman o con comandos cURL sencillos.

Para cargar documentos, consulte las instrucciones para **Carga de documentos** en Workfront [Comportamiento del anuncio](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). También puede utilizar las mismas instrucciones para las solicitudes cURL.

**Cuando utilice herramientas de API para cargar archivos, siga estas directrices:**

* Utilice la opción de la herramienta API para cargar el archivo. A menudo, se trata de un **Elegir archivo** en la pantalla de solicitud.

* Utilice el método HTTP del POST para realizar la solicitud de carga del archivo.

* El resultado de la solicitud debe ser una respuesta que incluya un valor para su controlador.

* Utilice el valor de controlador, el tipo de objeto y el valor GUID para objID en una carga útil JSON para realizar una llamada posterior. Esto es para crear el objeto para el archivo, como en el siguiente ejemplo:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Debe recibir un ID para el objeto en la respuesta.

Consulte la ayuda de la herramienta API específica que está utilizando para obtener más información.
