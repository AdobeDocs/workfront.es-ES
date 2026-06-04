---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuración de opciones para OPTASK copyIssue
description: Una explicación de los valores enteros esperados por el extremo copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 100%

---

# Configuración de opciones para OPTASK copyIssue


Una de las propiedades de una llamada API copyIssue es un campo denominado `options`. Este campo espera un número entero.

Para incluir una de las siguientes opciones, introduzca el número entero correspondiente. Para incluir más de una opción, introduzca la suma de los números enteros correspondientes.

| Opción | valor * |
|---|---|
| Borrar asignaciones | 2 |
| Borrar progreso | 4 |
| Borrar documentos | 128 |
| Borrar actualizaciones | 65536 |
| Borrar permisos | 524288 |
| Borrar datos personalizados | 1048576 |

*Todos los valores son potencias de 2.

Ejemplos:

* Para borrar el progreso al copiar el problema, introduzca un valor `options` de `4`.

* Para borrar tanto el progreso como los documentos, introduzca un valor `options` de `132`.

  Borrar progreso = 4

  Borrar documentos = 128

  4 + 128 = 132
