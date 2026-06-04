---
content-type: api
keywords: API,data,sync,journal,entry,object
navigation-topic: general-api
title: Utilice la API para sincronizar datos de programas y servicios
description: Utilice la API para sincronizar datos de programas y servicios
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
TQID: https://experienceleague.adobe.com/7ozt2OXI0CWlPmtkJGlaD-n6pekapA0X-GBpwDhFZ4Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 478
ht-degree: 100%

---

# Uso de la API para sincronizar datos de programas y servicios

Estas son algunas formas comunes de utilizar la API para sincronizar datos para programas y servicios.

## Actualizaciones casi en tiempo real

Adobe Workfront utiliza “Suscripciones a eventos” (también denominadas comúnmente “webhooks”) para enviar actualizaciones casi en tiempo real sobre los objetos y las acciones compatibles, a través de la API, a los puntos finales deseados. Puede esperar recibir una actualización con respecto a los nuevos objetos y acciones en un plazo de 5 segundos, pero las actualizaciones promedio llegan en aproximadamente un segundo. Para obtener información adicional sobre qué tipo de objetos y acciones se admiten, detalles técnicos y ejemplos sobre cómo configurar suscripciones a eventos, consulte [API de suscripción a eventos](../../wf-api/general/event-subs-api.md) y [Requisitos de entrega de suscripción a eventos](../../wf-api/general/setup-event-sub-endpoint.md).

## Actualizaciones por lotes

Las actualizaciones por lotes son una forma de configurar el sistema para recibir actualizaciones mediante solicitudes periódicas a los servidores de Workfront. Hay muchas formas de hacerlo, pero generalmente el proceso consiste en hacer que el servicio realice una solicitud a los servidores de la API de Workfront y en buscar objetos que se hayan creado o modificado desde la última llamada de solicitud. Para obtener información sobre posibles solicitudes, llamadas y parámetros útiles, consulte la sección [Comportamiento de GET](../../wf-api/general/api-basics.md#get-behavior) del artículo [Conceptos básicos de la API](../../wf-api/general/api-basics.md).

A medida que configura el servicio para actualizaciones por lotes, hay que tener en cuenta algunos aspectos importantes:

### Fechas de entrada

Las fechas de entrada se almacenan utilizando el formato ISO 8601. Este estándar incluye información de fecha, hora y zona horaria.

**Ejemplo:** formato de fecha ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Tanto la fecha en que se crea un objeto como la última fecha en que se modificó se almacenan como “entryDate” y “lastUpdateDate”, respectivamente. Para obtener información detallada acerca de objetos de Workfront, sus campos asociados y nombres de campo, consulte [Explorador de API](../../wf-api/general/api-explorer.md). Observe que la entryDate de cualquier objeto de Workfront no cambia, mientras que la lastUpdatedDate cambia cada vez que se modifica el objeto.

**Ejemplo:** solicitud de GET para un objeto del problema, con el campo **lastUpdateDate**. Esta solicitud devolverá todos los problemas actualizados desde la fecha especificada.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objeto de entrada de cuaderno

Si está interesado en obtener cambios con respecto a un campo específico en un objeto, puede consultar el objeto “Entrada de cuaderno&quot;. El objeto de entrada de cuaderno de Workfront se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Cuando se configura un campo para que se registre como parte del objeto Entrada de cuaderno, se creará una entrada de cuaderno correspondiente cada vez que se modifique dicho campo. A continuación, puede consultar el objeto Entrada de cuaderno mediante una llamada de API similar a la siguiente:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>“entryDate&quot; se utiliza para ver la entrada de cuaderno de una modificación, en lugar de consultar el objeto modificado en sí.
