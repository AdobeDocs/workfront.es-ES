---
content-type: api
keywords: API,datos,sincronizar,historial,entrada,objeto
navigation-topic: general-api
title: Utilice la API para sincronizar datos para programas y servicios
description: Utilice la API para sincronizar datos para programas y servicios
author: John
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: e6bad8cbe84d0f116e9679ecaba5178973a2604f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Uso de la API para sincronizar datos para programas y servicios

Estas son algunas formas comunes de utilizar la API para sincronizar datos para programas y servicios.

## Actualizaciones casi en tiempo real

Adobe Workfront utiliza &quot;Suscripciones de eventos&quot; (también conocidos como webhooks) para enviar actualizaciones casi en tiempo real sobre objetos y acciones compatibles, a través de la API, a los puntos de conexión deseados. Puede esperar recibir una actualización con respecto a nuevos objetos y acciones en un plazo de 5 segundos, pero las actualizaciones promedio llegan en aproximadamente 1 segundo. Para obtener información adicional sobre qué tipo de objetos son compatibles, qué tipos de acciones se admiten, detalles técnicos y ejemplos de cómo configurar suscripciones de eventos, consulte [API de suscripción de evento](../../wf-api/general/event-subs-api.md) y [Requisitos de entrega de suscripción de evento](../../wf-api/general/setup-event-sub-endpoint.md).

## Actualizaciones por lotes

Las actualizaciones por lotes son una forma de configurar el sistema para las actualizaciones mediante solicitudes periódicas a los servidores de Workfront. Existen muchas formas de hacerlo, pero por lo general el proceso consiste en hacer que el servicio realice una solicitud a los servidores de la API de Workfront y en buscar objetos que se hayan creado o modificado desde la última llamada de solicitud. Para obtener información sobre posibles solicitudes llamadas y parámetros útiles, consulte la [Comportamiento del GET](../../wf-api/general/api-basics.md#get-behavior) de la sección [Conceptos básicos de API](../../wf-api/general/api-basics.md) artículo.

Como está configurando su servicio para las actualizaciones por lotes, hay que tener en cuenta algunos aspectos importantes:

### Fechas de entrada

Las fechas de entrada se almacenan utilizando el formato ISO 8601. Este estándar incluye información de fecha, hora y zona horaria.

**Ejemplo:** Formato de fecha ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Tanto la fecha de creación de un objeto como la última fecha de modificación del objeto se almacenan como &quot;entryDate&quot; y &quot;lastUpdateDate&quot;, respectivamente. Para obtener información detallada sobre los objetos de Workfront, sus campos asociados y nombres de campo, consulte la [Explorador de API](../../wf-api/general/api-explorer.md). Observe que entryDate para cualquier objeto Workfront dado no cambia, ya que lastUpdatedDate cambia cada vez que se modifica el objeto.

**Ejemplo:** solicitud de GET para un objeto de problema, utilizando la variable **lastUpdateDate** campo . Esta solicitud devolverá todos los problemas actualizados desde esa fecha especificada.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v11.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objeto de entrada de diario

Si le interesa obtener cambios relativos a un campo específico de un objeto, puede consultar el objeto &quot;Entrada de diario&quot;. El objeto Workfront Journal Entry se puede configurar para registrar información sobre campos de objeto específicos cada vez que se modifiquen dichos campos; consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) para obtener más información.

Cuando se configura un campo para que se registre como parte del objeto Entrada de diario, se crea una Entrada de diario correspondiente cada vez que se modifica ese campo. A continuación, puede consultar el objeto Entrada de diario mediante una llamada de API similar a la siguiente:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v11.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; se utiliza para ver una entrada de diario de un cambio, en lugar de mirar el propio objeto modificado.
