---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Información general sobre los tipos de dependencia entre tareas
description: Los tipos de dependencias hacen referencia a las relaciones de predecesoras entre tareas. Definen cuándo puede comenzar o finalizar la tarea dependiente en función del comienzo o del fin de su predecesora.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Información general sobre los tipos de dependencia entre tareas

<!-- Audited: 12/2023 -->

Los tipos de dependencias hacen referencia a las relaciones de predecesoras entre tareas. Definen cuándo puede comenzar o finalizar la tarea dependiente en función del comienzo o del fin de su predecesora.

>[!IMPORTANT]
>
>Adobe Workfront no restringe el inicio o el final de las tareas dependientes en función de los tipos de dependencia a menos que se apliquen las relaciones de predecesoras. Para obtener información acerca de cómo aplicar predecesoras, consulte [Forzar predecesoras](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Debe especificar el Tipo de dependencia de una relación predecesora al establecer esta relación entre las tareas.

Para obtener más información sobre predecesoras, consulte [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Los siguientes son los tipos de dependencias de Workfront:

* **Finalizar-Iniciar (fs)**: la tarea predecesora debe finalizar antes de que pueda iniciarse la tarea dependiente. Es el tipo de dependencia predeterminado que se usa cuando no se especifica ningún otro tipo de dependencia.
* **Finalizar-Finalizar (ff)**: la tarea predecesora debe finalizar antes de que pueda finalizar la tarea dependiente.
* **Inicio-Inicio (ss)**: la tarea predecesora debe iniciarse antes de que pueda iniciarse la tarea dependiente. No puede iniciar la tarea dependiente a menos que la predecesora haya comenzado por lo menos.
* **Inicio-Fin (sf)**: la tarea predecesora debe comenzar antes de que pueda finalizar la tarea dependiente. Puede iniciar la tarea dependiente antes de que comience el predecesor, pero no puede finalizarla a menos que comience el predecesor.
* **Inicio programado (sd)**: esto programa una tarea como Fin-Comienzo, pero el tipo de aplicación real es Fin-Fin. Cuando se utiliza esta opción, la tarea dependiente se programa para iniciarse una vez completada la tarea predecesora. Sin embargo, la aplicación hace que la tarea dependiente pueda comenzar en cualquier momento, pero no puede finalizar hasta que finalice la tarea predecesora.

>[!NOTE]
>
>Las abreviaciones de los tipos de dependencia se utilizan en listas de tareas para definir relaciones de predecesoras. Para obtener más información, consulte [Ejemplos de valores de predecesoras en una lista de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Información general sobre predecesoras de tareas](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

