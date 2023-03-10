---
product-area: templates
navigation-topic: templates-navigation-topic
title: Creación de una plantilla de proyecto
description: Puede crear y eliminar plantillas desde el área Plantillas . Al crear una plantilla nueva, puede introducir la información de todas las tareas y toda la información de la configuración futura del proyecto. Esta información se transfiere al proyecto cuando lo cree desde la plantilla.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Creación de una plantilla de proyecto

Puede crear y eliminar plantillas desde el área Plantillas . Al crear una plantilla nueva, puede introducir la información de todas las tareas y toda la información de la configuración futura del proyecto. Esta información se transfiere al proyecto cuando lo cree desde la plantilla.

Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero, como se describe en este artículo.
* A partir de proyectos existentes, guardando un proyecto como plantilla.

   Para obtener más información sobre la creación de plantillas a partir de proyectos existentes, consulte [Guardar un proyecto como plantilla](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiándolo desde otra plantilla.

   Para obtener más información sobre cómo copiar una plantilla existente, consulte [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Si es administrador de Workfront, puede crear plantillas importando modelos. Para obtener más información, consulte [Configuración de un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisitos de acceso

Debe tener lo siguiente:

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
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Administrador del sistema para importar plantillas desde modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Plantillas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>De forma predeterminada, tiene permisos de gestión para las plantillas que crea</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Creación de una plantilla

1. En el **Menú principal** ![](assets/main-menu-icon.png) click **Plantillas**.

1. Haga clic en **Nueva plantilla**.

   La plantilla no tiene título.

   ![Nueva plantilla](assets/create-template-nwe-2022-350x102.png)

1. Especifique un nombre para la nueva plantilla en el encabezado de la plantilla y, a continuación, pulse **Escriba.**
1. Haga clic en el **Tareas de plantilla** en el panel izquierdo.
1. Haga clic en **Empezar a añadir tareas de plantilla**.

   O

   Haga clic en **Nueva tarea de plantilla** para empezar a añadir tareas a la plantilla.

   Añadir tareas de plantilla a una plantilla es idéntico a añadir tareas a un proyecto.

   Para obtener más información sobre cómo agregar tareas a un proyecto, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >No se pueden agregar tareas recurrentes a una plantilla.

1. (Opcional) Haga clic en el **Diagrama de Gantt** en la esquina superior derecha de la Lista de tareas para ver una representación visual de la lista de tareas de la plantilla.

   >[!TIP]
   >
   >No puede editar tareas directamente desde este diagrama de Gantt.

1. Para agregar información a la nueva plantilla, haga clic en el botón **Más** menú ![](assets/more-icon.png)y haga clic en **Editar**.

   Para obtener información sobre cómo editar una plantilla, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Haga clic en **Guardar cambios**.
1. (Opcional) Si desea agregar más elementos a la plantilla, consulte la sección [Agregar elementos adicionales a una plantilla](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configuración de plantilla determinada por la asociación de grupos

La asociación de una plantilla de proyecto con un grupo (o su ausencia) afecta a la forma en que el proyecto, la tarea y las preferencias de problema determinan ciertos ajustes de la plantilla. Para obtener más información, consulte la sección [Creación y modificación de las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) en el artículo [Creación y modificación de las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
