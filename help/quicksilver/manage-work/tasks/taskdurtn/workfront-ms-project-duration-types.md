---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipos de duración en Adobe Workfront y Microsoft Project
description: Los tipos de duración disponibles en Adobe Workfront son diferentes a sus equivalentes en Microsoft Project, que se denominan Tipos de tareas. Esto puede resultar confuso a veces al exportar o importar proyectos entre Workfront y Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 17%

---

# Tipos de duración en Adobe Workfront y Microsoft Project

Los tipos de duración disponibles en Adobe Workfront son diferentes a sus equivalentes en Microsoft Project, que se denominan Tipos de tareas. Esto puede resultar confuso a veces al exportar o importar proyectos entre Workfront y Microsoft Project.

Para obtener información sobre cómo importar y exportar proyectos entre Workfront y Microsoft Project, consulte los siguientes artículos:

* [Exportar un proyecto a un proyecto de Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importar un proyecto desde Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Tipos de duración en proyectos de Workfront y Microsoft

Workfront tiene cuatro tipos de duración de tareas:

* Simple
* Condicionada por el esfuerzo
* Trabajo calculado
* Asignación calculada

Para obtener más información, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Microsoft Project no reconoce estos tipos de duración. En la actualidad, Microsoft Project tiene tres tipos de tareas similares a los tipos de duración de Workfront:

* Unidades fijas
* Trabajo fijo
* Duración fija

## El tipo de duración cambia al exportar de Workfront a MS Project

Al exportar proyectos de Workfront a un proyecto de Microsoft, las tareas impulsadas por el esfuerzo se convierten en trabajo fijo. Simple, Trabajo calculado y Asignación calculada pasan a ser Unidades fijas.

## El tipo de duración cambia al importar de MS Project a Workfront

Al importar proyectos desde un proyecto de Microsoft en Workfront, las unidades fijas pasan a depender del esfuerzo. Trabajo fijo y Duración fija reciben el tipo de duración predeterminado que el administrador de Workfront seleccionó para su sistema. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
