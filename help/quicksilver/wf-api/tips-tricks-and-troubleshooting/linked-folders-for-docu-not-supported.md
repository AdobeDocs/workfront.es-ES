---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Las carpetas vinculadas no son compatibles con el objeto DOCU
description: Las carpetas vinculadas no son compatibles con el objeto DOCU
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# No se admite el uso de la API para añadir una carpeta vinculada

No se admite el uso de la API para añadir una carpeta vinculada a la matriz de carpetas para un objeto Document (DOCU). La solicitud se realizará correctamente, pero algunos proveedores externos pueden eliminar el documento del sistema. Esto se debe a que el sistema externo se utilizará como la fuente final de la verdad. Por lo tanto, si el documento se elimina del proveedor externo, se considera que ya no existe. Cualquier documento que no se encuentre en la carpeta vinculada (externa) puede eliminarse automáticamente de [!DNL Workfront] sin forma de recuperarlos.
