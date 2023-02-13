---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipos de duración en proyectos de Adobe Workfront y Microsoft
description: Los tipos de duración disponibles en Adobe Workfront son diferentes a los de sus homólogos en el proyecto de Microsoft, que se denominan Tipos de tareas. Esto puede resultar confuso a veces al exportar o importar proyectos entre Workfront y Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Tipos de duración en proyectos de Adobe Workfront y Microsoft

Los tipos de duración disponibles en Adobe Workfront son diferentes a los de sus homólogos en el proyecto de Microsoft, que se denominan Tipos de tareas. Esto puede resultar confuso a veces al exportar o importar proyectos entre Workfront y Microsoft Project.

Para obtener información sobre la importación y exportación de proyectos entre Workfront y Microsoft Project, consulte los siguientes artículos:

* [Exportar un proyecto a un proyecto de Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importar un proyecto desde un proyecto de Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Tipos de duración en proyectos de Workfront y Microsoft

Workfront tiene cuatro tipos de duración de tarea:

* Sencilla
* Condicionada por el esfuerzo
* Trabajo calculado
* Asignación calculada

Para obtener más información, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Microsoft Project no reconoce estos tipos de duración. Actualmente, el proyecto de Microsoft tiene tres tipos de tarea similares a los tipos de duración de Workfront:

* Unidades fijas
* Trabajo fijo
* Duración fija

## El tipo de duración cambia al exportar de Workfront a un proyecto de MS

Al exportar proyectos de Workfront a Microsoft Project, las tareas impulsadas por el esfuerzo se convierten en trabajo fijo. Simple, Calculated Work y Calculated Assignment se convierten en unidades fijas.

## El tipo de duración cambia al importar de MS Project a Workfront

Al importar proyectos de Microsoft Project en Workfront, las unidades fijas se convierten en unidades de esfuerzo. Trabajo fijo y Duración fija reciben el tipo de duración predeterminada que el administrador de Workfront seleccionó para su sistema. Para obtener más información, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
