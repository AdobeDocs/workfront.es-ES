---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Descripción general de los tipos de dependencia de tareas
description: Los tipos de dependencia hacen referencia a las relaciones predecesoras entre tareas. Definen cuándo puede comenzar o finalizar la tarea dependiente en función del inicio o final de su predecesor.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Descripción general de los tipos de dependencia de tareas

Los tipos de dependencia hacen referencia a las relaciones predecesoras entre tareas. Definen cuándo puede comenzar o finalizar la tarea dependiente en función del inicio o final de su predecesor.

>[!IMPORTANT]
>
>Adobe Workfront no restringe que las tareas dependientes se inicien o terminen según los tipos de dependencia a menos que se refuercen las relaciones predecesoras. Para obtener información sobre cómo aplicar predecesores, consulte [Aplicar predecesores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Debe especificar el Tipo de dependencia de una relación predecesora cuando establezca esta relación entre las tareas.

Para obtener más información sobre las predecesoras, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Los siguientes son los tipos de dependencia de Workfront:

* **Fin-Inicio (fs)**: La tarea predecesora debe finalizar antes de que pueda iniciarse la tarea dependiente. Es el tipo de dependencia predeterminado, que se usa cuando no se especifica ningún otro tipo de dependencia.
* **Fin-fin (ff)**: La tarea predecesora debe finalizar antes de que la tarea dependiente pueda finalizar.
* **Inicio (ss)**: La tarea predecesora debe iniciarse antes de que se pueda iniciar la tarea dependiente. No se puede iniciar la tarea dependiente a menos que el predecesor haya iniciado al menos.
* **Start-Finish (sf)**: La tarea predecesora debe iniciarse antes de que la tarea dependiente pueda finalizar. Puede iniciar la tarea dependiente antes de que se inicie el predecesor, pero no podrá terminarla a menos que se inicie el predecesor.
* **Inicio programado (sd)**: Esto programa una tarea como Finish-Start, pero el tipo de aplicación real es Finish-Finish. Cuando se utiliza esto, la tarea dependiente está programada para iniciarse después de completar la tarea predecesora. Sin embargo, la aplicación lo hace para que la tarea dependiente pueda iniciarse en cualquier momento, pero no puede finalizar hasta que la tarea predecesora haya finalizado.
