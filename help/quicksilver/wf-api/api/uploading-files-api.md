---
content-type: api
navigation-topic: api-navigation-topic
title: Carga de archivos mediante la API
description: Carga de archivos mediante la API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
TQID: https://experienceleague.adobe.com/Yd7byYJ1pYDXwdKvINXh4fKy-pWoEiNMj345jr1HHNs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 93%

---

# Carga de archivos mediante la API

Puede cargar archivos utilizando las API de WorkFront con herramientas API, como Postman o con comandos cURL simples.

Para cargar documentos, consulte las instrucciones en **Cargar Documentos** en el comportamiento de publicación de WorkFront [Post Behavior](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). También puede utilizar estas mismas instrucciones para las solicitudes cURL.

**Cuando utilice herramientas API para cargar archivos, siga estas directrices:**

* Utilice la opción de la herramienta API para cargar el archivo. A menudo hay un botón **Elegir archivo** en la pantalla de solicitud.

* Utilice el método HTTP del POST para realizar la solicitud y cargar el archivo.

* La solicitud debe generar una respuesta de que incluya un valor para su identificador.

* Utilice el valor del identificador, el tipo de objeto y el valor GUID para el objID en una carga útil JSON para realizar una llamada posterior. Esto sirve para crear el objeto para el archivo, como en el siguiente ejemplo:

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

Debe recibir un ID. para el objeto en la respuesta.

Consulte la ayuda de la herramienta API específica que está utilizando para obtener más información.
