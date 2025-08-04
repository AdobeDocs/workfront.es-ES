---
product-area: projects
navigation-topic: use-predecessors
title: Cree una relación de predecesoras mediante el área Predecesoras
description: Puede utilizar tareas predecesoras (o sólo predecesoras) para vincular tareas que dependen de otras tareas para comenzar o finalizar.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 46%

---

# Cree una relación de predecesoras mediante el área Predecesoras

<!-- Audited: 5/2025 -->

Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras para comenzar o finalizar. Por ejemplo, no desea organizar una fiesta (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).

En este artículo se muestra cómo puede establecer predecesoras mediante la pestaña Predecesoras dentro de una tarea.

Para obtener información acerca de cómo configurar predecesoras en una lista de tareas, consulte [Crear una relación de predecesoras en la lista de tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Puede ver las tareas predecesoras de las siguientes áreas de Adobe Workfront:

* En la sección Predecesoras de las tareas dependientes
* En el gráfico Gantt
* En la lista de tareas de la columna Predecesoras

Para obtener información acerca de las predecesoras, consulte [Información general sobre las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una predecesora para una tarea

Crear una tarea predecesora para una tarea de proyecto mediante el área Predecesoras es similar a crear predecesoras para tareas de plantilla en una plantilla.

Para crear una tarea predecesora para una tarea de proyecto:

1. Desplácese hasta la tarea que desee designar como tarea dependiente.

1. En el panel izquierdo, haga clic en **Predecesoras**.

1. En la sección **Predecesoras**, haga clic en **Agregar predecesora**. Se abre el cuadro de diálogo **Agregar predecesora**.

1. (Opcional) Para agregar una tarea predecesora entre proyectos, reemplace el nombre del proyecto en el campo **Proyecto principal** por otro proyecto.

   Para obtener más información, vea [Crear predecesoras entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

   >[!TIP]
   >
   >No se pueden crear predecesoras entre plantillas para tareas de plantilla.


1. En el campo **Tareas**, escriba el nombre de la tarea o tareas que desee designar como predecesoras y, a continuación, selecciónelas cuando aparezcan en la lista desplegable.

1. Seleccionar un **tipo de dependencia**.

   Para obtener más información, vea [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Escriba un importe de **retardo**.

   Para obtener más información, consulte[Resumen de tipos de retardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Cuadro de diálogo Agregar predecesora](assets/add-predecessor-dialog-box.png)

1. Seleccione la casilla de verificación **Forzado** si desea forzar la relación de predecesoras entre las dos tareas.

   Para obtener más información, vea [Aplicar predecesoras](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Haga clic en **Guardar**.

1. (Opcional) Para quitar un predecesor, selecciónelo de la lista de predecesores y luego haga clic en el icono **Quitar** ![Quitar icono](assets/remove-or-delete-icon.png).

   La tarea predecesora se elimina de la lista. La tarea predecesora no se elimina de su proyecto.
