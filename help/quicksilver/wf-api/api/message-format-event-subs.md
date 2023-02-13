---
content-type: api
navigation-topic: api-navigation-topic
title: Formato de mensaje de salida para suscripciones de evento
description: Formato de mensaje de salida para suscripciones de evento
author: John
feature: Workfront API
exl-id: addcf5bc-a101-4bb0-93a6-46b4af67c848
source-git-commit: 2ec05c03a5bfa842008870ca47fb617b81fd6ebd
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Formato de mensaje de salida para suscripciones de evento

Con el lanzamiento de Adobe Workfront 2017.3, el formato de los mensajes salientes para las suscripciones de eventos cambiará para permitir un mejor rendimiento y un mejor uso de las suscripciones de eventos para sus integraciones.

## Actualizaciones del formato de mensaje saliente

Se realizarán los siguientes cambios en el formato de mensaje saliente:

* Los mensajes salientes incluirán oldState y newState para un recurso de Workfront.

   Estos valores muestran los cambios realizados en un objeto como resultado de un evento en Workfront.

* El campo de metadatos eventTime se agregará a todos los mensajes salientes.

   Este campo indicará, en Nanosegundos y EpochSeconds, el tiempo en que se produjo un evento. Utilice eventTime para ordenar eventos procesados por su integración.

* Se eliminará el campo al que se hace referencia owner:companyID en el recurso NOTE.
* Se eliminará el objeto objectOn del recurso DOCU (Document) al que se hace referencia currentVersion.

Si actualmente utiliza suscripciones de eventos de Workfront, deberá actualizar las integraciones de Workfront antes de la versión 2017.3 para tener en cuenta estos cambios.

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción de evento](../../wf-api/general/event-subs-api.md).

## Ejemplos de formatos de mensaje antiguos y nuevos

El siguiente mensaje CREATE, de formato antiguo, ya no se utilizará después del lanzamiento de 2017.3:

```
{
  "eventType": "CREATE",
  "subscriptionId": "8a0d839d5ef32c9a015ef33064b00001",
  "fields": {
     "ID": "59d7db3c0000014b05536251b669a3e4",
     "name": "EventSub Test 53350c27-ce58-40e9-af75-a2d45ff13046",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:36:28.722-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:36:28.785-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1891,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```

El siguiente mensaje CREATE con formato nuevo se utilizará después del lanzamiento de 2017.3:

```
{
   "eventType": "CREATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef32e2cde0000",
   "eventTime": {
      "nano": 414000000,
      "epochSecond": 1507318444
   },
   "newState": {
     "ID": "59d7daab0000011b8faebf0f60d25d08",
     "name": "EventSub Test 3700e224-0ef7-4571-b200-09109712152c",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:34:03.562-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:34:04.000-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1890,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   },
   "oldState": {}
```

El siguiente mensaje UPDATE en formato antiguo ya no se utilizará después de la versión 2017.3:

```
{
     "eventType": "UPDATE",
     "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
     "fields": {
     "ID": "59d7dcde000001b2330bda8ac63fee16",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:43:26.305-0600",<
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:43:49.265-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1892,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   }
 }
```

El siguiente mensaje UPDATE de formato nuevo se utilizará después del lanzamiento de 2017.3:

```
{
   "eventType": "UPDATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
   "eventTime": {
     "nano": 998000000,
     "epochSecond": 1507319336
   },
   "newState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  },
  "oldState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19"
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```
