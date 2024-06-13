---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: La acción moverAcarpeta del documento no funciona
description: Al utilizar la acción Documento moveToFolder, se devuelve un error 422.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# La acción moverAcarpeta del documento no funciona

## Problema

Cuando se utiliza el objeto Document `moveToFolder` acción, se devuelve un error 422.

O

Si se utiliza esta acción a través del módulo Adobe Authenticator en Workfront Fusion, el documento no se mueve, pero no hay indicación del error. El error es el mismo, pero el módulo Adobe Authenticator no lo muestra.

## Solución

Una posible causa de un error 422 para esta acción es que la acción está intentando mover un documento de una carpeta vinculada a otra carpeta vinculada.

Compruebe que el documento que desea mover no esté ya en una carpeta vinculada.
