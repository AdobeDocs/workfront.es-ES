---
product-area: projects
navigation-topic: create-tasks
title: Información general sobre Crear tareas
description: Solo puede crear tareas en un proyecto una vez creado el proyecto.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 9%

---

# Información general sobre Crear tareas

Solo puede crear tareas en un proyecto una vez creado el proyecto.

Por ejemplo, después de crear un proyecto, puede que desee añadir tareas y modificarlas para organizar el plan del proyecto. Para obtener más información sobre cómo crear un proyecto, vea [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md). Para obtener información sobre cómo crear tareas, vea [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Este artículo describe las consideraciones, limitaciones y valores predeterminados que se aplican al crear tareas.

## Formas de crear tareas en un proyecto

Puede crear tareas en un proyecto de las siguientes maneras:

* Desde cero, como se describe en [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copie tareas al mismo proyecto o a un nuevo proyecto, o duplique tareas en el mismo proyecto, como se describe en [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Mover tareas de un proyecto a otro, como se describe en [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitaciones en la creación de tareas

Cuando tenga los permisos y el acceso correctos, podrá crear tareas en un proyecto. Sin embargo, los siguientes son casos en los que es posible que no pueda crear tareas:

* El administrador de Adobe Workfront o de un grupo debe habilitar la adición de tareas a un proyecto que se encuentre en estado completo o muerto en el área de Preferencias del proyecto. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* No puede agregar tareas a un proyecto que tenga Aprobación pendiente.

## Número máximo de tareas permitidas en un proyecto

Un proyecto puede contener hasta 5000 tareas. Aparece un mensaje de advertencia en el proyecto cuando se acerca al límite, cuando se ha alcanzado y se intenta superar el límite.

Según el número de tareas de los proyectos en los que se impuso esta limitación, la instancia de Workfront podría permitir más de 5000 tareas en un solo proyecto.

Si puede incluir más de 5000 tareas en un solo proyecto, tenga en cuenta lo siguiente:

* El límite de tareas para su entorno de Workfront se establece en el número actual de tareas en su proyecto más grande, más un 10 % adicional.

  Por ejemplo, si un proyecto de la instancia de Workfront contiene 10 000 tareas, el límite de cada proyecto de la instancia de Workfront es de 11 000 tareas.

* Los proyectos más pequeños mejoran el rendimiento y minimizan los desafíos de administración que acompañan a los proyectos grandes.

## Valores predeterminados de tarea al agregar tareas a un proyecto

Existen dos tipos de información predeterminada que Workfront actualiza automáticamente para las tareas cuando las crea:

* Información predeterminada de nivel del sistema

  El administrador de Workfront o de un grupo establece los valores predeterminados de nivel del sistema para las tareas del área Tareas y problemas de las Preferencias del proyecto. Para obtener información acerca de las preferencias de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) o [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Información predeterminada de nivel de proyecto

  El resto de esta sección describe los valores predeterminados de nivel de proyecto que usted, como jefe de proyecto, puede definir para todas las tareas nuevas que se agregan a un proyecto

Al agregar una tarea a un proyecto, según la configuración del proyecto, Workfront podría adjuntar automáticamente un proceso de aprobación o formularios personalizados a la tarea.

Para obtener información sobre cómo configurar un proyecto para agregarlo de manera predeterminada, consulte la sección &quot;Tareas&quot; en el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Al definir la información predeterminada que se asociará con las tareas agregadas a un proyecto en el nivel de proyecto, tenga en cuenta lo siguiente:

* Debe tener permisos de administración en el proyecto para definir la configuración predeterminada para el proceso de aprobación de tareas y los formularios personalizados.
* Todas las tareas nuevas se crean con el proceso de aprobación y los formularios personalizados definidos al editar el proyecto.
* Puede modificar esta configuración predeterminada al agregar tareas mediante el cuadro Editar tarea, pero no al agregar tareas en la edición en línea.
* Puede definir el proceso de aprobación y los formularios personalizados para las tareas de una plantilla.

   * Cuando se crea un proyecto a partir de esta plantilla, el proceso de aprobación y los formularios personalizados se aplican automáticamente al proyecto.
   * Cuando se adjunta una plantilla a un proyecto existente, el proyecto conserva el proceso de aprobación de tareas original y la configuración de los formularios personalizados si están definidos. Si no están definidos, los ajustes de la plantilla se convertirán en los ajustes del proyecto.
   * Cuando se adjunta una plantilla a un proyecto existente, las tareas agregadas al proyecto desde la plantilla conservan el proceso de aprobación y la configuración de formularios personalizados que tenían en la plantilla, independientemente de la configuración de tareas del proyecto.

  Para obtener información acerca de cómo adjuntar una plantilla a un proyecto, vea [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Al copiar el proyecto, la configuración predeterminada de la tarea se transfiere al nuevo proyecto.

  Para obtener información sobre la copia de un proyecto, consulte [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

* Cuando se copian tareas de un proyecto a otro y el proyecto de destino tiene una configuración predeterminada diferente para las tareas, las tareas copiadas conservan la configuración predeterminada del proyecto original, a menos que se borren en el proceso de copia.
* Al duplicar una tarea en el mismo proyecto, los formularios personalizados y el proceso de aprobación se transfieren a la tarea duplicada.

  Para obtener información sobre cómo copiar y duplicar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Al mover la tarea a otro proyecto, la configuración predeterminada de la tarea se guarda en las tareas del proyecto original, independientemente de la configuración predeterminada de la tarea en el nuevo proyecto.

  Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).
