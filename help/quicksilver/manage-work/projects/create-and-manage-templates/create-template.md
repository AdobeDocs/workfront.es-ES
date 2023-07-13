---
product-area: templates
navigation-topic: templates-navigation-topic
title: Crear una plantilla de proyecto
description: Puede crear y eliminar plantillas desde el área Plantillas. Al crear una plantilla nueva, puede introducir la información de todas las tareas y toda la información de la configuración futura del proyecto. Esta información se transferirá al proyecto cuando lo cree a partir de la plantilla.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Crear una plantilla de proyecto

Puede crear y eliminar plantillas desde el área Plantillas. Al crear una plantilla nueva, puede introducir la información de todas las tareas y toda la información de la configuración futura del proyecto. Esta información se transferirá al proyecto cuando lo cree a partir de la plantilla.

>[!NOTE]
>
>Una plantilla y sus tareas no tienen fechas reales, sino una indicación de qué día (a partir de cuándo podría comenzar el proyecto futuro) podría comenzar una tarea y en qué día debería completarse la tarea. Al utilizar plantillas para crear proyectos futuros, los proyectos recibirán fechas reales. Para obtener más información, consulte [Creación de un proyecto](../create-projects/create-project.md).


Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero, como se describe en este artículo.
* Desde proyectos existentes, guardando un proyecto como plantilla.

  Para obtener más información sobre la creación de plantillas a partir de proyectos existentes, consulte [Guardar un proyecto como plantilla](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiándolo desde otra plantilla.

  Para obtener más información sobre cómo copiar una plantilla existente, consulte [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Si es administrador de Workfront, puede crear plantillas importando modelos. Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Administrador del sistema para importar plantillas de modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a plantillas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>De forma predeterminada, tiene permisos de administración para las plantillas que crea</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Creación de una plantilla

1. Desde el **Menú principal** ![](assets/main-menu-icon.png) click **Plantillas**.

1. Clic **Nueva plantilla**.

   La plantilla no tiene título.

   ![Nueva plantilla](assets/create-template-nwe-2022-350x102.png)

1. Especifique un nombre para la nueva plantilla en el encabezado de la plantilla y pulse **Entrar.**
1. Haga clic en **Tareas de plantilla** en el panel izquierdo.
1. Clic **Comenzar a agregar tareas de plantilla**.

   O

   Clic **Nueva tarea de plantilla** para empezar a añadir tareas a la plantilla.

   Agregar tareas de plantilla a una plantilla es idéntico a agregar tareas a un proyecto.

   Para obtener más información sobre cómo agregar tareas a un proyecto, consulte [Creación de tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >No puede agregar tareas recurrentes a una plantilla.

1. (Opcional) Haga clic en **Gráfico Gantt** en la esquina superior derecha de la Lista de tareas para ver una representación visual de la lista de tareas de la plantilla.

   >[!TIP]
   >
   >No puede editar tareas directamente desde este gráfico Gantt.

1. Para añadir información a la nueva plantilla, haga clic en **Más** menú ![](assets/more-icon.png), luego haga clic en **Editar**.

   Para obtener información sobre cómo editar una plantilla, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Haga clic en **Guardar cambios**.
1. (Opcional) Si desea agregar elementos adicionales a la plantilla, consulte la sección [Adición de elementos adicionales a una plantilla](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configuración de plantilla determinada por asociación de grupo

La asociación de una plantilla de proyecto con un grupo (o la falta de asociación) afecta a la forma en que las preferencias de proyecto, tarea y problema determinan ciertas configuraciones en la plantilla. Para obtener más información, consulte la sección [Crear y modificar las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) en el artículo [Crear y modificar las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
