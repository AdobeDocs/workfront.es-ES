---
product-area: templates
navigation-topic: templates-navigation-topic
title: Quitar información de plantilla de un proyecto
description: No se puede quitar una plantilla de un proyecto. Solo puede quitar manualmente la información que se agregó al proyecto después de adjuntar una plantilla al proyecto. Para obtener información sobre cómo adjuntar plantillas, consulte Adjuntar una plantilla a un proyecto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# Quitar información de plantilla de un proyecto

No se puede quitar una plantilla de un proyecto. Solo puede quitar manualmente la información que se agregó al proyecto después de adjuntar una plantilla al proyecto. Para obtener información acerca de cómo adjuntar plantillas, vea [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso a las tareas </p> <p>Contribute o acceso superior al proyecto </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Opciones para quitar información de plantilla de un proyecto

Para quitar la información de plantilla agregada al proyecto, puede realizar una de las siguientes acciones:

* Elimine manualmente la información del proyecto después de adjuntar la plantilla.

  Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Elimine las tareas del proyecto que se agregaron con la plantilla.

  Para obtener más información, consulte la sección [Eliminar tareas creadas a partir de una plantilla](#delete-tasks-created-from-a-template) en este artículo.

* Elimine la plantilla de Workfront. Al eliminar la plantilla de Workfront, no se eliminan de los proyectos las tareas agregadas desde la plantilla.

  Para obtener más información, consulte [Eliminar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Eliminar tareas creadas a partir de una plantilla {#delete-tasks-created-from-a-template}

1. Vaya a la sección **Tareas** del proyecto.
1. Realice una de las siguientes acciones:

   * Cree un filtro para la lista de tareas para mostrar solo las tareas que se crearon a partir de una plantilla con la siguiente instrucción:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Para obtener información sobre cómo crear un filtro, consulte [Crear o editar filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Al aplicar el filtro, solo se muestran en la lista las tareas asociadas con un ID de tarea de plantilla.

   * Cree una vista para la lista de tareas con el fin de mostrar los campos **Identificador de tarea de plantilla** o **Nombre de tarea de plantilla** en una columna.

     Al aplicar la vista, las tareas que contienen información en las columnas Identificador de tarea de plantilla o Nombre de tarea de plantilla se crearon mediante una plantilla.

     Para obtener información acerca de cómo crear una vista, vea [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Seleccione todas las tareas identificadas en el paso 2 como creadas a partir de una plantilla, luego haga clic en **el icono Eliminar**&#x200B;**> Sí, eliminarla**. Para obtener más información, consulte [Eliminar tareas](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
