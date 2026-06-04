---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipos de duración en Adobe Workfront y Microsoft Project
description: Los tipos de duración disponibles en Adobe Workfront son diferentes a sus equivalentes en Microsoft Project, que se denominan Tipos de tareas. Esto puede resultar confuso a veces al exportar o importar proyectos entre Workfront y Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
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
 
(drafting this because it is misleading)
 
</note>
-->
