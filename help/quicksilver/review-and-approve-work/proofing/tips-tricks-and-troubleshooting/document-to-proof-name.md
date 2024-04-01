---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: El nombre del documento cambió después de la carga y contiene un carácter no válido
description: Algunos documentos no se pueden convertir en pruebas.
author: Courtney
source-git-commit: a01c2e42dad1a7c00ac73fcaeb1202c56238a8bb
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# El nombre del documento cambió después de la carga y contiene un carácter no válido

## Problema

Algunos documentos no se pueden convertir en pruebas.

## Causa

Los archivos cargados en Workfront no pueden contener ciertos caracteres en los nombres de archivo. Si un archivo contiene cualquiera de los siguientes caracteres en el nombre del archivo, los caracteres se quitan del nombre del archivo cuando se carga el archivo: `! # % * \ | ' " / ? < > { } [ ]`.

Si el nombre de un documento se actualiza para incluir un carácter no válido después de la carga inicial, la generación de pruebas fallará.

## Solución

Elimine el carácter no válido del nombre del documento:

1. Seleccione el documento y haga clic en **Detalles del documento**.
1. Haga clic en el nombre del documento, elimine el carácter no válido y pulse Intro.

   Caracteres no válidos: `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. Actualice la página y genere la prueba.