---
product-area: projects
navigation-topic: use-predecessors
title: Crear una relación de predecesora en la lista de tareas
description: Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras para comenzar o finalizar. Por ejemplo, no querría organizar una fiesta (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 69%

---

# Crear una relación de predecesora en la lista de tareas

<!-- Audited: 5/2025 -->

Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras para comenzar o finalizar. Por ejemplo, no querría organizar una fiesta (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).

En este artículo se muestra cómo crear predecesoras en la lista de tareas.

Puede ver las tareas predecesoras de las siguientes áreas de Adobe Workfront:

* En la lista de tareas de la columna Predecesoras.
* En el gráfico Gantt.
* En la sección Predecesoras de una tarea dependiente.

Para obtener más información, consulte [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Estándar </p><p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una predecesora

{{step1-to-projects}}

1. Seleccione un proyecto en la página **Proyectos**.
1. Haga clic en **Tareas** en el panel izquierdo.
1. En la lista desplegable **Vistas**, seleccione una vista que muestre la columna **Predecesora** o agregue la columna a la vista actual.

1. Seleccione la tarea que desee designar como tarea dependiente.
1. Haga clic dentro de la columna **Predecesoras** de la tarea.
1. Escriba el número de tarea que desee designar como predecesora de la tarea seleccionada y, a continuación, presione **Entrar**.

   >[!TIP]
   >
   >Para añadir una predecesora entre proyectos, haga lo siguiente:
   >
   >1. Haga clic en el icono **Modo de planificación** y elija **Guardar automáticamente**.
   >
   >1. Escriba el Número de referencia del proyecto del predecesor seguido de dos puntos y el número de la tarea. Por ejemplo, al escribir *765021:12* se indica que el número de referencia del proyecto del predecesor es 765021 y que el predecesor es el número de tarea 12 del proyecto.
   >
   >1. Añada el tipo de dependencia para esta predecesora. Para obtener más información, consulte [Crear predecesoras entre proyectos](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >1. Pulse **Intro**.
   >
   >**IMPORTANTE**
   >
   >No puede agregar una tarea predecesora entre proyectos cuando la lista de tareas se muestra en el modo de guardado manual.

   El icono de la predecesora se vuelve verde cuando la tarea predecesora se marca como completada. Esto indica que la tarea dependiente está lista para trabajar.

   Para obtener más información acerca de los tipos de relación disponibles en la columna Predecesoras, vea [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Ver detalles de la predecesora

Puede ver rápidamente los detalles sobre la predecesora desde la lista de tareas.

1. En la lista de tareas, pase el ratón sobre el número de predecesora en la columna **Predecesoras**. Se muestra un cuadro con los detalles del predecesor.

   ![Detalles de la predecesora](assets/predecessor-details-in-task-list.png)

   Se muestran los siguientes detalles:

   **Nombre de predecesora:** el nombre de la predecesora a la que se hace referencia. Se incluye el número de tarea de la predecesora. Haga clic en el nombre de la tarea para abrirla.

   **Nombre del proyecto:** el nombre del proyecto donde reside la predecesora. El proyecto se identifica como el proyecto actual si la predecesora pertenece a los mismos proyectos que la tarea, o como entre proyectos, si la predecesora pertenece a un proyecto diferente. Para obtener más información sobre las tareas predecesoras entre proyectos, consulte [Comprender las predecesoras entre proyectos](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Puede ampliar los detalles del proyecto para ver las fechas de inicio y de finalización planificadas del proyecto, la condición, el estado, el porcentaje completado y el propietario. Para un entre proyecto, puede hacer clic en **Ver proyecto** para abrirlo.

   **ID.:** el número de referencia del proyecto donde se encuentra la predecesora.

   **Inicio planificado:** la fecha de inicio planificada de la tarea predecesora.

   **Fin planificado:** la fecha planificada de finalización de la tarea predecesora.

   **Número de predecesoras:** Número de predecesoras para la predecesora a la que se hace referencia.

   **Número de sucesoras:** Número de tareas sucesoras (o dependientes) para la predecesora a la que se hace referencia.
