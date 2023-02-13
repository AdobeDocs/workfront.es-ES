---
product-area: templates
navigation-topic: templates-navigation-topic
title: Eliminar información de plantilla de un proyecto
description: No se puede quitar una plantilla de un proyecto. Solo puede eliminar manualmente la información que se añadió al proyecto después de adjuntar una plantilla al proyecto. Para obtener información sobre cómo adjuntar plantillas, consulte Adjuntar una plantilla a un proyecto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Eliminar información de plantilla de un proyecto

No se puede quitar una plantilla de un proyecto. Solo puede eliminar manualmente la información que se añadió al proyecto después de adjuntar una plantilla al proyecto. Para obtener información sobre cómo adjuntar plantillas, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso a las tareas </p> <p>Contribución o acceso superior al proyecto </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Opciones para quitar información de plantilla de un proyecto

Para eliminar la información de plantilla que se agregó al proyecto, puede realizar una de las siguientes acciones:

* Elimine manualmente la información del proyecto después de adjuntar la plantilla.

   Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Elimine las tareas del proyecto que se añadieron con la plantilla.

   Para obtener más información, consulte la [Eliminar tareas creadas a partir de una plantilla](#delete-tasks-created-from-a-template) en este artículo.

* Elimine la plantilla de Workfront. Al eliminar la plantilla de Workfront, no se eliminan las tareas agregadas de la plantilla a los proyectos.

   Para obtener más información, consulte [Eliminar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Eliminar tareas creadas a partir de una plantilla {#delete-tasks-created-from-a-template}

1. Vaya a la **Tareas** del proyecto.
1. Realice una de las siguientes acciones:

   * Cree un filtro para que la lista de tareas muestre solo las tareas creadas a partir de una plantilla con la siguiente instrucción:

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      Para obtener información sobre cómo crear un filtro, consulte [Crear o editar filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      Al aplicar el filtro, solo se muestran en la lista las tareas asociadas con un ID de tarea de plantilla.

   * Cree una vista para que la lista de tareas muestre la variable **ID de tarea de plantilla** o **Nombre de tarea de plantilla** campos de una columna.

      Cuando se aplica la vista, las tareas que contienen información en la columna ID de tarea de plantilla o nombre de tarea de plantilla se crean mediante una plantilla.

      Para obtener información sobre cómo crear una vista, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Seleccione todas las tareas identificadas en el paso 2 como creadas a partir de una plantilla y, a continuación, haga clic en **el icono Eliminar****> Sí, Eliminarlo**. Para obtener más información, consulte [Eliminar tareas](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
