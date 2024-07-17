---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: El nombre del documento cambió después de la carga y contiene un carácter no válido
description: Algunos documentos no se pueden convertir en pruebas.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 3e16f69f5b3c2b37093b00841945e6529394fa94
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---

# El nombre del documento cambió después de la carga y contiene un carácter no válido

## Problema

Algunos documentos no se pueden convertir en pruebas.

## Causa

Los archivos cargados en Workfront no pueden contener ciertos caracteres en los nombres de archivo. Si un archivo contiene cualquiera de los siguientes caracteres en el nombre de archivo, los caracteres se quitarán del nombre de archivo cuando se cargue el archivo: `! # % * \ | ' " / ? < > { } [ ]`.

Si el nombre de un documento se actualiza para incluir un carácter no válido después de la carga inicial, la generación de pruebas fallará.

## Solución

Elimine el carácter no válido del nombre del documento:

1. Seleccione el documento y haga clic en **Detalles del documento**.
1. Haga clic en el nombre del documento, elimine el carácter no válido y pulse Intro.

   Caracteres no válidos: `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. Actualice la página y genere la prueba.
