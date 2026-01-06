---
product-area: templates
navigation-topic: templates-navigation-topic
title: Eliminación de información de plantilla de un proyecto
description: No se puede quitar una plantilla de un proyecto. Solo puede quitar manualmente la información que se añadió al proyecto después de adjuntar una plantilla al proyecto. Para obtener información sobre cómo adjuntar plantillas, consulte Adjuntar una plantilla a un proyecto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 93%

---

# Eliminación de información de plantilla de un proyecto

No se puede quitar una plantilla de un proyecto. Solo puede quitar manualmente la información que se añadió al proyecto después de adjuntar una plantilla al proyecto. Para obtener información acerca de cómo adjuntar plantillas, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso a las tareas </p> <p>Contribución o un acceso superior al proyecto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Opciones para quitar información de la plantilla de un proyecto

Para quitar la información de la plantilla añadida al proyecto, puede realizar una de las siguientes acciones:

* Elimine manualmente la información del proyecto después de adjuntar la plantilla.

  Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Elimine las tareas del proyecto que se añadieron con la plantilla.

  Para obtener más información, consulte la sección [Eliminar tareas creadas a partir de una plantilla](#delete-tasks-created-from-a-template) en este artículo.

* Elimine la plantilla de Workfront. Al eliminar la plantilla de Workfront, no se eliminan de los proyectos las tareas añadidas desde la plantilla.

  Para obtener más información, consulte [Eliminar plantillas del proyecto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Eliminación de tareas creadas a partir de una plantilla {#delete-tasks-created-from-a-template}

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

     Para obtener información acerca de cómo crear una vista, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Seleccione todas las tareas identificadas en el paso 2 como creadas a partir de una plantilla, luego haga clic en **el icono Eliminar****> Sí, eliminarla**. Para obtener más información, consulte [Eliminar tareas](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
