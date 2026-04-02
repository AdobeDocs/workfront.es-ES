---
title: Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes de usuarios asignados
description: Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes de usuarios asignados
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 1%

---

# Las asignaciones de un objeto eliminado aparecen de forma inesperada en los informes de usuarios asignados

## Problema

Después de eliminar un objeto que tiene una asignación, se eliminan tanto el objeto como la asignación. Sin embargo, es posible que la asignación aparezca en algunos informes.

Por ejemplo, si elimina una tarea que se asignó a un usuario, también se elimina la asignación al usuario. Sin embargo, si más adelante ejecuta un informe de tareas que está filtrado por el usuario asignado, con ese usuario especificado, el informe sigue mostrando la tarea eliminada si la tarea sigue en la Papelera de reciclaje.

## Causa

Esto se debe a limitaciones arquitectónicas de la papelera de reciclaje. Actualmente no hay planes en la hoja de ruta para abordar esta cuestión debido a la escala de rediseño arquitectónico que sería necesario.
