---
content-type: api
navigation-topic: api-navigation-topic
title: Carga de archivos mediante la API
description: Carga de archivos mediante la API
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3db01c329c005570b782ae3445f83b7c44ced676
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Carga de archivos mediante la API

Puede cargar archivos mediante las API de Workfront con herramientas de API como Postman o con comandos cURL simples.

Para cargar documentos, consulte las instrucciones de **Cargar documentos** en Workfront [Comportamiento de publicación](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). También puede utilizar estas mismas instrucciones para las solicitudes cURL.

**Cuando utilice herramientas API para cargar archivos, siga estas directrices:**

* Utilice la opción de la herramienta API para cargar el archivo. Estos suelen ser un **Elegir archivo** en la pantalla de solicitud.

* Utilice el método HTTP del POST para realizar la solicitud y cargar el archivo.

* La solicitud debe generar una respuesta de que incluya un valor para su identificador.

* Utilice el valor del identificador, el tipo de objeto y el valor GUID para el objID en una carga útil JSON para realizar una llamada posterior. Esto sirve para crear el objeto para el archivo, como en el siguiente ejemplo:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Debe recibir un ID. para el objeto en la respuesta.

Consulte la ayuda de la herramienta API específica que está utilizando para obtener más información.
