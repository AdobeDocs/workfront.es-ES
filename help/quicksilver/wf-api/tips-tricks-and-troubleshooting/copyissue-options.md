---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuración de opciones para OPTASK copyIssue
description: Una explicación de los valores enteros esperados por el extremo copyIssue .
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Configuración de opciones para OPTASK copyIssue


Una de las propiedades de una llamada a la API copyIssue es un campo denominado `options`. Este campo espera un número entero.

Para incluir una de las siguientes opciones, introduzca el entero correspondiente. Para incluir más de una opción, introduzca la suma de los enteros coincidentes.

| option | value* |
|---|---|
| Borrar asignaciones | 2 |
| Borrar progreso | 4 |
| Borrar documentos | 128 |
| Borrar actualizaciones | 65536 |
| Borrar permisos | 524288 |
| Borrar datos personalizados | 1048576 |

*Todos los valores son poderes de 2.

Ejemplos:

* Para borrar el progreso al copiar el problema, introduzca un `options` valor de `4`.

* Para borrar el progreso y los documentos, introduzca un `options` valor de `132`.

   Borrar progreso = 4

   Borrar documentos = 128

   4 + 128 = 132
