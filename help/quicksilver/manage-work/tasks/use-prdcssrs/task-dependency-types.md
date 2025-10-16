---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Información general sobre los tipos de dependencia de tareas
description: Los tipos de dependencia hacen referencia a las relaciones de predecesoras entre tareas. Definen cuándo puede empezar o finalizar la tarea dependiente en función del comienzo o del fin de su predecesora.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 98%

---

# Información general sobre los tipos de dependencia entre tareas

<!-- Audited: 12/2023 -->

Los tipos de dependencia hacen referencia a las relaciones de predecesoras entre tareas. Definen cuándo puede empezar o finalizar la tarea dependiente en función del comienzo o del fin de su predecesora.

>[!IMPORTANT]
>
>Adobe Workfront no restringe el inicio o el final de las tareas dependientes en función de los tipos de dependencia a menos que se fuercen las relaciones de predecesoras. Para obtener información acerca de cómo forzar predecesoras, consulte [Forzar predecesoras](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Debe especificar el Tipo de dependencia de una relación predecesora al establecer esta relación entre las tareas.

Para obtener más información sobre el uso de predecesoras, consulte [Información general sobre las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Los siguientes son los tipos de dependencias de Workfront:

* **Finalizar-Iniciar (fs)**: la tarea predecesora debe finalizar para que pueda iniciarse la tarea dependiente. Es el tipo de dependencia predeterminado que se usa cuando no se especifica ningún otro tipo de dependencia.
* **Finalizar-Finalizar (ff)**: la tarea predecesora debe finalizar antes de que finalice la tarea dependiente.
* **Iniciar-Iniciar (ss)**: la tarea predecesora debe iniciarse antes de que pueda iniciarse la tarea dependiente. No puede iniciar la tarea dependiente a menos que la predecesora se haya iniciado como mínimo.
* **Iniciar-Finalizar (sf)**: la tarea predecesora debe empezar antes de que finalice la tarea dependiente. Puede iniciar la tarea dependiente antes de que empiece la predecesora, pero no puede finalizarla a menos que empiece la predecesora.
* **Programado-Iniciar (sd)**: esto programa una tarea como Finalizar-Iniciar, pero el tipo de aplicación real es Finalizar-Finalizar. Cuando se utiliza esta opción, la tarea dependiente se programa para iniciarse una vez completada la tarea predecesora. Sin embargo, la aplicación hace que la tarea dependiente pueda empezar en cualquier momento, pero no puede finalizar hasta que finalice la tarea predecesora.

>[!NOTE]
>
>Las abreviaciones de los tipos de dependencia se utilizan en listas de tareas para definir relaciones de predecesoras. Para obtener más información, consulte [Ejemplos de valores de tareas predecesoras en una lista de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) en [Información general sobre las predecesoras de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

