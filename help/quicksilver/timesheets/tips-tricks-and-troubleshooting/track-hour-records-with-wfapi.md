---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Seguimiento de registros de horas con la API de Adobe Workfront
description: En caso de que la organización use Adobe Workfront para introducir las horas trabajadas, pero use otra herramienta como sistema de registro de esos datos, será posible utilizar la API de Workfront para sincronizar datos entre los dos sistemas.
author: Lisa
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 100%

---

# Seguimiento de registros de horas con la API de Adobe Workfront

En caso de que la organización use Adobe Workfront para introducir las horas trabajadas, pero use otra herramienta como sistema de registro de esos datos, será posible usar la API de Workfront para sincronizar datos entre los dos sistemas.

El simple seguimiento del registro de horas no es viable porque, en caso de eliminar la entrada de horas, se eliminará todo el registro, requiriendo la extracción de todo el conjunto de datos y su comparación con el conjunto de datos antiguo. Afortunadamente, todas las transacciones horarias se registran en las entradas del historial de Workfront.

Después de recuperar un conjunto inicial de todas las horas actuales del sistema, es posible realizar un seguimiento de todos y cada uno de los cambios a través de las entradas del historial.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"datos": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjVal Código": "HORA",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D" <br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HORA",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f0 08db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HORA",<br>"subObjID": "57854160 08db05d9d2925c12b10f521"<br>,<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler", <br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HORA",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>A continuación, se muestra una descripción de los campos incluidos:

* **changeType:** tipo de cambio que se realiza en el objeto:

   * **A:** añadir

   * **E:** editar

   * **D:** eliminar

* **aux2:** nombre del usuario del registro de horas.

* **newNumberVal:** nuevo valor del registro de horas (será nulo si changeType es D).

* **oldNumberVal:** valor anterior del registro de horas.

* **subObjCode:** tipo de registro que se modifica (siempre debe ser HORA).

* **subObjID:** ID del registro de horas.

Use esta información para saber qué registros de horas se cambiaron, editaron o eliminaron. A continuación, use subObjID para recuperar más información de los registros de horas si fuera necesario.
