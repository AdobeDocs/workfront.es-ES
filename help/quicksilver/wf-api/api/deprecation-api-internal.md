---
content-type: api
navigation-topic: api-navigation-topic
title: 'Obsolescencia de API: interna'
description: 'Obsolescencia de API: interna'
author: John
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Obsolescencia de API: interna

API interna es una versión de la API de Adobe Workfront que no es compatible debido a su diseño y finalidad. Aunque contiene las actualizaciones más recientes de la API de Workfront, está sujeta a cambios sin previo aviso y, por lo tanto, debe utilizarse con precaución en las integraciones de producción. Workfront recomienda actualizar todas las integraciones API-internas a una API con versiones.

Para obtener más información sobre las versiones compatibles de la API de Workfront, consulte [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

**Uso de API no admitida**

Si las integraciones requieren funciones que no están disponibles en una API con versiones, Workfront recomienda utilizar API no admitidas. De forma similar a API-interna, no se admite API-Unsupported. No compatible con API también incluye los cambios más recientes en la API de Workfront y está sujeto a cambios sin previo aviso. Workfront le recomienda utilizar API no admitida en su entorno de prueba, donde puede explorar nuevas funciones y asegurarse de que la API no contenga errores.

**Determinación de la versión de API que utiliza**

Puede determinar la versión de la API que utilizan sus integraciones mediante REST para construir un URI que envíe una llamada a través de HTTPS a Workfront y, a continuación, devuelva una respuesta JSON.

El siguiente ejemplo muestra un URI que llama a API-Internal:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

El siguiente ejemplo muestra el URI que llama a API-Unsupported:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

El siguiente ejemplo muestra un URI que llama a la versión 15.0 de la API:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
