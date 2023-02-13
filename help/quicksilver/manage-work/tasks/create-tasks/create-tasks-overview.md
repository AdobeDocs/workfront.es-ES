---
product-area: projects
navigation-topic: create-tasks
title: Información general sobre la creación de tareas
description: Solo puede crear tareas en un proyecto una vez creado el proyecto.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Información general sobre la creación de tareas

Solo puede crear tareas en un proyecto una vez creado el proyecto.

Por ejemplo, después de crear un proyecto, es posible que desee agregar tareas y modificarlas para organizar el plan del proyecto. Para obtener más información sobre cómo crear un proyecto, consulte [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md). Para obtener información sobre la creación de tareas, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

En este artículo se describen consideraciones, limitaciones y valores predeterminados que se aplican al crear tareas.

## Formas de crear tareas en un proyecto

Puede crear tareas en un proyecto de las siguientes maneras:

* Desde cero, tal como se describe en [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copie tareas en el mismo proyecto o en un nuevo proyecto o en tareas duplicadas en el mismo proyecto, tal como se describe en [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Mover tareas de un proyecto a otro, tal como se describe en [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitaciones en la creación de tareas

Cuando tenga el acceso y los permisos correctos, puede crear tareas en un proyecto. Sin embargo, los siguientes son casos en los que es posible que no pueda crear tareas:

* El administrador de Adobe Workfront o un administrador de grupo deben habilitar la adición de tareas a un proyecto que esté en estado Finalizado o Muerto en el área Preferencias del proyecto . Para obtener información sobre cómo definir las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* No puede agregar tareas a un proyecto que esté en Pendiente de aprobación.

## El número máximo de tareas permitidas en un proyecto

Un proyecto puede contener hasta 5000 tareas. Aparece un mensaje de advertencia en el proyecto cuando se está acercando al límite, cuando ha alcanzado el límite y si intenta superar el límite.

Según el número de tareas en los proyectos cuando se impuso esta limitación, la instancia de Workfront podría permitir más de 5000 tareas en un solo proyecto.

Si puede incluir más de 5000 tareas en un solo proyecto, tenga en cuenta lo siguiente:

* El límite de tareas del entorno de Workfront se establece en el número actual de tareas del proyecto más grande, más un 10 % adicional.

   Por ejemplo, si un proyecto de la instancia de Workfront contiene 10 000 tareas, el límite de cada proyecto de la instancia de Workfront es de 11 000 tareas.

* Los proyectos más pequeños mejoran el rendimiento y minimizan los desafíos de administración que acompañan a los grandes proyectos.

## Valores predeterminados de tarea al agregar tareas a un proyecto

Existen dos tipos de información predeterminada que Workfront actualiza automáticamente para las tareas cuando las crea:

* Información predeterminada de nivel de sistema

   El administrador de Workfront o un administrador de grupo establecen los valores predeterminados de nivel de sistema para las tareas del área Tareas y problemas de Preferencias de proyecto. Para obtener información sobre las preferencias de tareas y problemas, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) o [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Información predeterminada de nivel de proyecto

   El resto de esta sección describe los valores predeterminados a nivel de proyecto que usted, como administrador de proyectos, puede definir para todas las tareas nuevas que se agregan a un proyecto

Cuando agregue una tarea a un proyecto, según cómo se configure el proyecto, Workfront podría adjuntar automáticamente a la tarea un proceso de aprobación o formularios personalizados.

Para obtener información sobre cómo configurar un proyecto para agregarlos de forma predeterminada, consulte la sección &quot;Tareas&quot; en la sección [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md) artículo.

Cuando defina la información predeterminada para asociarla con tareas agregadas a un proyecto en el nivel de proyecto, tenga en cuenta lo siguiente:

* Debe tener permisos de gestión en el proyecto para definir la configuración predeterminada para el proceso de aprobación de tareas y los formularios personalizados.
* Todas las tareas nuevas se crean con el proceso de aprobación y los formularios personalizados definidos al editar el proyecto.
* Puede modificar esta configuración predeterminada al agregar tareas mediante el cuadro Editar tarea, pero no al agregar tareas en la edición en línea.
* Puede definir el proceso de aprobación y los formularios personalizados para las tareas de una plantilla.

   * Cuando se crea un proyecto a partir de esta plantilla, el proceso de aprobación y los formularios personalizados se aplican automáticamente al proyecto.
   * Cuando una plantilla está adjunta a un proyecto existente, el proyecto conserva el proceso de aprobación de tareas original y la configuración de formularios personalizados si están definidos. Si no están definidos, la configuración de la plantilla se convierte en la configuración del proyecto.
   * Cuando una plantilla está adjunta a un proyecto existente, las tareas agregadas al proyecto desde la plantilla conservan el proceso de aprobación y la configuración de formularios personalizados que tenían en la plantilla, independientemente de la configuración de tareas del proyecto.

   Para obtener información sobre cómo adjuntar una plantilla a un proyecto, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Cuando copia el proyecto, la configuración predeterminada de la tarea se transfiere al nuevo proyecto.

   Para obtener información sobre cómo copiar un proyecto, consulte [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

* Cuando copia tareas de un proyecto a otro y el proyecto de destino tiene diferentes configuraciones predeterminadas para las tareas, las tareas copiadas conservan la configuración predeterminada del proyecto original, a menos que se borren en el proceso de copia.
* Cuando se duplica una tarea en el mismo proyecto, los formularios personalizados y el proceso de aprobación se transfieren a la tarea duplicada.

   Para obtener información sobre cómo copiar y duplicar tareas, consulte [ [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Al mover la tarea a otro proyecto, la configuración predeterminada de la tarea se guarda en las tareas del proyecto original, independientemente de la configuración predeterminada de la tarea en el nuevo proyecto.

   Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).
