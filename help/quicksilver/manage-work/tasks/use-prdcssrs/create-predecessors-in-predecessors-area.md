---
product-area: projects
navigation-topic: use-predecessors
title: Crear una relación predecesora con el área Predecesoras
description: Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras tareas para iniciarse o completarse. Por ejemplo, no desea alojar una parte (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Crear una relación predecesora con el área Predecesoras

Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras tareas para iniciarse o completarse. Por ejemplo, no desea alojar una parte (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).

Este artículo muestra cómo se pueden configurar predecesores con la ficha Predecesores de una tarea.

Para obtener información sobre la configuración de predecesores en una lista de tareas, consulte [Crear una relación predecesora en la lista de tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Puede ver las tareas anteriores en las siguientes áreas de Adobe Workfront:

* En la sección Predecesores de las tareas dependientes
* En el diagrama de Gantt
* En la lista de tareas de la columna Predecesores

Para obtener información sobre las predecesoras, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Creación de un predecesor para una tarea

1. Vaya a una tarea que desee designar como tarea dependiente y, a continuación, haga clic en **Predecesores** en el panel izquierdo.

   Es posible que tenga que hacer clic en **Mostrar más**, luego **Predecesores**.

1. Haga clic en **+Agregar predecesor**.
1. (Opcional) Para agregar un predecesor entre proyectos, reemplace el nombre del proyecto en la variable **Proyecto principal** con otro proyecto y, a continuación, escriba el nombre de la tarea o tareas que desee como predecesoras.

   Para obtener información sobre cómo agregar predecesores entre proyectos, consulte [Crear predecesores entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Escriba el nombre de la tarea o tareas que desea designar como predecesoras.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Seleccione un **Tipo de dependencia**.

   Para obtener información sobre los tipos de dependencias de tareas, consulte una [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique un **Lag** cantidad en días.

   Para obtener información sobre los tipos de retraso, consulte &#x200B; [Descripción general de los tipos de retraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Select **Enforzado** si desea aplicar la relación predecesora entre las dos tareas.

   Para obtener información sobre cómo aplicar predecesores, consulte [Aplicar predecesores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Haga clic en **Guardar**.
