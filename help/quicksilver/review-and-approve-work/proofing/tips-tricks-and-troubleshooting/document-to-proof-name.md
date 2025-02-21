---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: El nombre del documento ha cambiado después de la carga y contiene un carácter no válido
description: Algunos documentos no se pueden convertir en pruebas.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
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
