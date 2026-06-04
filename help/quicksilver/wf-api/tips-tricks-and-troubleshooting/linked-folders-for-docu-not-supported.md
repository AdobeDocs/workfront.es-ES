---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Las carpetas vinculadas no son compatibles con el objeto DOCU
description: Las carpetas vinculadas no son compatibles con el objeto DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 100%

---

# No se admite el uso de la API para añadir una carpeta vinculada

No se admite el uso de la API para añadir una carpeta vinculada a la matriz de carpetas para un objeto de documento (DOCU). La solicitud se realizará correctamente, pero algunos proveedores externos pueden eliminar el documento del sistema. Esto se debe a que el sistema externo se utilizará como la fuente final de la verdad. Por lo tanto, si se elimina el documento del proveedor externo, se considera que el documento ya no existe. Los documentos que no se encuentren en la carpeta vinculada (externa) pueden eliminarse automáticamente de [!DNL Workfront] sin posibilidad de recuperarlos.
