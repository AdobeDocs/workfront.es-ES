---
title: Las asignaciones de un objeto eliminado aparecen inesperadamente en los informes de los responsables
description: Las asignaciones de un objeto eliminado aparecen inesperadamente en los informes de los responsables
author: Courtney
draft: Probably
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 1%

---

# Las asignaciones de un objeto eliminado aparecen inesperadamente en los informes de los responsables

## Problema

Después de eliminar un objeto que tiene una asignación, se eliminan tanto el objeto como la asignación. Sin embargo, es posible que la tarea aparezca en algunos informes.

Por ejemplo, si elimina una tarea asignada a un usuario, también se elimina la asignación al usuario. Sin embargo, si posteriormente ejecuta un informe de tareas filtrado por el asignado, con ese usuario especificado, el informe sigue mostrando la tarea eliminada si la tarea sigue estando en la Papelera de reciclaje.

## Causa

Esto se debe a limitaciones arquitectónicas de la Papelera de reciclaje. Actualmente no hay planes en la hoja de ruta para abordar esta cuestión debido a la escala del rediseño arquitectónico que sería necesario.
