---
content-type: api
navigation-topic: api-navigation-topic
title: Obsolescencia de API interna
description: Obsolescencia de API interna
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Obsolescencia de API interna

API interna es una versión de la API de Adobe Workfront que no es compatible debido a su diseño y propósito. Aunque contiene las actualizaciones más recientes de la API de Workfront, está sujeto a cambios sin previo aviso y, por lo tanto, debe utilizarse con precaución en las integraciones de producción. Workfront recomienda encarecidamente actualizar todas las integraciones internas de la API a una API con versiones.

Para obtener más información sobre las versiones compatibles de la API de Workfront, consulte [Versiones de API y programación de asistencia](../../wf-api/api/api-version-support-schedule.md).

**Uso de API no admitida**

Si las integraciones requieren una funcionalidad que no está disponible en una API con versiones, Workfront recomienda utilizar API no admitida. Al igual que API interna, API no admitida no es compatible. API no admitida también incluye los cambios más recientes en la API de Workfront y está sujeta a cambios sin previo aviso. Workfront le recomienda utilizar API no admitidas en su entorno de prueba, donde puede explorar nuevas funciones y asegurarse de que la API esté libre de errores.

**Determinación de la versión de la API que está utilizando**

Puede determinar la versión de la API que utilizan las integraciones mediante REST para construir un URI que envíe una llamada a través de HTTPS a Workfront y que luego devuelva una respuesta JSON.

El siguiente ejemplo muestra un URI que llama a API-Internal:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

El siguiente ejemplo muestra un URI que llama a API-Unsupported:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

El siguiente ejemplo muestra un URI que llama a la versión 15.0 de la API:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
