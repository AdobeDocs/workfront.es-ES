---
title: Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes asignados
description: Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes asignados
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes asignados

## Problema

Después de eliminar un objeto que tiene una asignación, se eliminan tanto el objeto como la asignación. Sin embargo, la asignación podría aparecer en algunos informes.

Por ejemplo, si elimina una tarea asignada a un usuario, también se elimina la asignación al usuario. Sin embargo, si posteriormente ejecuta un informe de tareas filtrado por el usuario asignado, con ese usuario especificado, el informe seguirá enumerando la tarea eliminada si la tarea sigue en la Papelera de reciclaje.

## Causa

Esto se debe a las limitaciones arquitectónicas de la Papelera de Reciclaje. Actualmente no hay planes en la hoja de ruta para abordar esta cuestión debido a la escala del rediseño arquitectónico que sería necesario.
