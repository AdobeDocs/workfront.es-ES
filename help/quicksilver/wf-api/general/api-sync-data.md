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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Uso de la API para sincronizar datos de programas y servicios

Estas son algunas formas comunes de utilizar la API para sincronizar datos para programas y servicios.

## Actualizaciones casi en tiempo real

Adobe Workfront utiliza &quot;Suscripciones de eventos&quot; (también denominadas comúnmente &quot;webhooks&quot;) para enviar actualizaciones casi en tiempo real sobre los objetos y las acciones compatibles, a través de la API, a los puntos de conexión deseados. Puede esperar recibir una actualización con respecto a los nuevos objetos y acciones en un plazo de 5 segundos, pero las actualizaciones promedio llegan en aproximadamente 1 segundo. Para obtener información adicional sobre qué tipo de objetos se admiten, qué tipos de acciones se admiten, detalles técnicos y ejemplos sobre cómo configurar suscripciones a eventos, consulte [API de suscripción a eventos](../../wf-api/general/event-subs-api.md) y [Requisitos de entrega de suscripción a eventos](../../wf-api/general/setup-event-sub-endpoint.md).

## Actualizaciones por lotes

Las actualizaciones por lotes son una forma de configurar el sistema para recibir actualizaciones mediante solicitudes periódicas a los servidores de Workfront. Hay muchas formas de hacerlo, pero generalmente el proceso consiste en hacer que el servicio realice una solicitud a los servidores de la API de Workfront y en buscar objetos que se hayan creado o modificado desde la última llamada de solicitud. Para obtener información sobre posibles solicitudes, llamadas y parámetros útiles, consulte la sección [Comportamiento de GET](../../wf-api/general/api-basics.md#get-behavior) del artículo [Conceptos básicos de la API](../../wf-api/general/api-basics.md).

A medida que configura el servicio para actualizaciones por lotes, hay que tener en cuenta algunos aspectos importantes:

### Fechas de entrada

Las fechas de entrada se almacenan utilizando el formato ISO 8601. Este estándar incluye información de fecha, hora y zona horaria.

**Ejemplo:** formato de fecha ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Tanto la fecha en que se crea un objeto como la última fecha en que se modificó se almacenan como &quot;entryDate&quot; y &quot;lastUpdateDate&quot;, respectivamente. Para obtener información detallada acerca de objetos de Workfront, sus campos asociados y nombres de campo, consulte [Explorador de API](../../wf-api/general/api-explorer.md). Observe que entryDate de cualquier objeto Workfront dado no cambia, mientras que lastUpdatedDate cambia cada vez que se modifica el objeto.

**Ejemplo:** solicitud de GET para un objeto de problema, con el campo **lastUpdateDate**. Esta solicitud devolverá todos los problemas actualizados desde la fecha especificada.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objeto de entrada de diario

Si está interesado en obtener cambios con respecto a un campo específico en un objeto, puede consultar el objeto &quot;Entrada de cuaderno&quot;. El objeto de entrada de diario de Workfront se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Para obtener más información, vea [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Cuando se configura un campo para que se registre como parte del objeto de entrada de cuaderno, se creará una entrada de cuaderno correspondiente cada vez que se modifique ese campo. A continuación, puede consultar el objeto Entrada de cuaderno mediante una llamada de API similar a la siguiente:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; se utiliza para ver una entrada de diario de un cambio, en lugar de ver el propio objeto modificado.
