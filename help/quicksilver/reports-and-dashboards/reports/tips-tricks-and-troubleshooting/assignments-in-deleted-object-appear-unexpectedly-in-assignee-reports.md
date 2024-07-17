---
title: Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes de usuarios asignados
description: Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes de usuarios asignados
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes de usuarios asignados

## Problema

Después de eliminar un objeto que tiene una asignación, se eliminan tanto el objeto como la asignación. Sin embargo, es posible que la asignación aparezca en algunos informes.

Por ejemplo, si elimina una tarea que se asignó a un usuario, también se elimina la asignación al usuario. Sin embargo, si más adelante ejecuta un informe de tareas que está filtrado por el usuario asignado, con ese usuario especificado, el informe sigue mostrando la tarea eliminada si la tarea sigue en la Papelera de reciclaje.

## Causa

Esto se debe a limitaciones arquitectónicas de la papelera de reciclaje. Actualmente no hay planes en la hoja de ruta para abordar esta cuestión debido a la escala de rediseño arquitectónico que sería necesario.
