---
content-type: api
navigation-topic: api-navigation-topic
title: Obsolescencia de la API interna
description: Obsolescencia de la API interna
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
TQID: https://experienceleague.adobe.com/LGyk8MIATMQj6JHqKmjkeL2pXW-b6xtxo2heMd4h0y4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 241
ht-degree: 100%

---

# Obsolescencia de la API interna

La API interna es una versión de la API de Adobe Workfront que no es compatible debido a su diseño y propósito. Aunque contiene las actualizaciones más recientes de la API de Workfront, está sujeta a cambios sin previo aviso y, por lo tanto, debe utilizarse con precaución en las integraciones de producción. Workfront recomienda encarecidamente actualizar todas las integraciones de la API interna a una API con diversas versiones.

Para obtener más información sobre las versiones compatibles de la API de Workfront, consulte [Versiones de API y programación de compatibilidad](../../wf-api/api/api-version-support-schedule.md).

**Uso de una API no compatible**

Si las integraciones requieren una funcionalidad que no está disponible en una API con diversas versiones, Workfront recomienda utilizar una API no compatible. Al igual que la API interna, una API no compatible no recibe soporte. La API no compatible también incluye los cambios más recientes en la API de Workfront y está sujeta a cambios sin previo aviso. Workfront le recomienda utilizar la API no compatible en su entorno de prueba, donde puede explorar nuevas funciones y asegurarse de que la API no contiene errores.

**Determinar la versión de la API que está usando**

Puede determinar la versión de la API que utilizan sus integraciones mediante REST para construir un URI que envíe una llamada a través de HTTPS a Workfront y que luego devuelva una respuesta JSON.

El siguiente ejemplo muestra un URI que llama a una API interna:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

El siguiente ejemplo muestra un URI que llama a una API no compatible:

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>Las llamadas a la API no compatible omiten la sección `/api` de la dirección URL.

El siguiente ejemplo muestra un URI que llama a la versión 15.0 de la API:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
