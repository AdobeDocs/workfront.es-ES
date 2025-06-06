---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Seguimiento de registros de horas con la API de Adobe Workfront
description: Si su organización utiliza Adobe Workfront para introducir las horas trabajadas, pero utiliza otra herramienta como sistema de registro para esos datos, puede utilizar la API de Workfront para sincronizar datos entre los dos sistemas.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Seguimiento de registros de horas con la API de Adobe Workfront

Si su organización utiliza Adobe Workfront para introducir las horas trabajadas, pero utiliza otra herramienta como sistema de registro para esos datos, puede utilizar la API de Workfront para sincronizar datos entre los dos sistemas.

El simple seguimiento del registro de horas no es viable porque, si se elimina la entrada de horas, se elimina todo el registro, lo que requiere extraer todo el conjunto de datos y compararlo con el conjunto de datos antiguo. Afortunadamente, todas las transacciones horarias se registran en las entradas de diario de Workfront.

Después de recuperar un conjunto inicial de todas las horas actuales del sistema, puede realizar un seguimiento de todos y cada uno de los cambios a través de las entradas de cuaderno.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>&lbrace;<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjVal Código": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D" <br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f0 08db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "57854160 08db05d9d2925c12b10f521"<br>,<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler", <br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>A continuación se muestra una descripción de los campos incluidos:

* **changeType:** Tipo de cambio que se está realizando en el objeto:

   * **A:** Agregar

   * **E:** Editar

   * **D:** Eliminar

* **aux2:** El nombre del usuario para el que está el registro de horas.

* **newNumberVal:** Nuevo valor del registro de hora (será nulo si changeType es D).

* **oldNumberVal:** Valor anterior del registro de hora.

* **subObjCode:** Tipo de registro que se modifica (siempre debe ser HOUR).

* **subObjID:** ID del registro de hora.

Puede utilizar esta información para descubrir qué registros de horas se han cambiado, editado o eliminado. A continuación, puede utilizar subObjID para recuperar más información de los registros de horas si es necesario.
