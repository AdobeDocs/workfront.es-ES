---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuración de opciones para OPTASK copyIssue
description: Una explicación de los valores enteros esperados por el extremo copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Configuración de opciones para OPTASK copyIssue


Una de las propiedades de una llamada a la API copyIssue es un campo llamado `options`. Este campo espera un entero.

Para incluir una de las siguientes opciones, introduzca el entero coincidente. Para incluir más de una opción, introduzca la suma de los enteros coincidentes.

| opción | valor* |
|---|---|
| Borrar asignaciones | 2 |
| Borrar progreso | 4 |
| Borrar documentos | 128 |
| Borrar actualizaciones | 65536 |
| Borrar permisos | 524288 |
| Borrar datos personalizados | 1048576 |

*Todos los valores son potencias de 2.

Ejemplos:

* Para borrar el progreso al copiar el problema, introduzca un `options` valor de `4`.

* Para borrar tanto el progreso como los documentos, introduzca un `options` valor de `132`.

  Borrar progreso = 4

  Borrar documentos = 128

  4 + 128 = 132
