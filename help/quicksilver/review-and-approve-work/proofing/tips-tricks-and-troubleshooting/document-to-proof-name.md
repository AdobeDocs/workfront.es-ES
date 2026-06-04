---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: El nombre del documento ha cambiado después de la carga y contiene un carácter no válido
description: Algunos documentos no se pueden convertir en pruebas.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 98%

---

# El nombre del documento ha cambiado después de la carga y contiene un carácter no válido

## Problema

Algunos documentos no se pueden convertir en pruebas.

## Causa

Los archivos cargados en Workfront no pueden contener ciertos caracteres en los nombres de archivo. Si un archivo contiene cualquiera de los siguientes caracteres en el nombre de archivo, los caracteres se eliminan del nombre de archivo cuando se carga el archivo: `! # % * \ | ' " / ? < > { } [ ]`.

Si el nombre de un documento se actualiza para que incluya un carácter no válido después de la carga inicial, falla la generación de pruebas.

## Solución

Elimine el carácter no válido del nombre del documento:

1. Seleccione el documento y haga clic en **Detalles del documento**.
1. Haga clic en el nombre del documento, elimine el carácter no válido y pulse entrar.

   Caracteres no válidos: `! # % * \ | ' " / ? < > { } [ ]`

   ![Nombre de documento](assets/doc-name.png)

1. Actualice la página y genere la prueba.
