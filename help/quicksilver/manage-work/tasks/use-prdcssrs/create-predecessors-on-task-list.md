---
product-area: projects
navigation-topic: use-predecessors
title: Crear una relación de predecesoras en la lista de tareas
description: Puede utilizar tareas predecesoras (o sólo predecesoras) para vincular tareas que dependen de otras tareas para comenzar o finalizar. Por ejemplo, no desea organizar una fiesta (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Crear una relación de predecesoras en la lista de tareas

Puede utilizar tareas predecesoras (o sólo predecesoras) para vincular tareas que dependen de otras tareas para comenzar o finalizar. Por ejemplo, no desea organizar una fiesta (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).

Este artículo muestra cómo crear predecesoras en la lista de tareas.

Puede ver las tareas predecesoras de las siguientes áreas de Adobe Workfront:

* En la lista de tareas de la columna Predecesoras.
* En el gráfico Gantt
* En la sección Predecesoras de una tarea dependiente

Para obtener más información, vea [Información general sobre tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acceso

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
   <td> <p>Nuevo: estándar </p><p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront. Para obtener más información acerca de los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creación de un predecesor

1. Vaya a un proyecto.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Asegúrese de que la vista actual muestre la columna **Predecesora**.

   Si la vista no muestra la columna Predecesoras, cambie a una vista que sí la muestre o agregue la columna a la vista.

1. Seleccione la tarea que desee designar como tarea dependiente.
1. Haga clic dentro de la columna **Predecesoras**.
1. Escriba el número de tarea que desea designar como predecesora de la tarea seleccionada y, a continuación, presione **Entrar**.

   >[!TIP]
   >
   >Para agregar una predecesora entre proyectos, haga lo siguiente:
   >
   >1. Haz clic en el icono **Modo de planificación** y elige **Guardar automáticamente**.
   >
   >1. Escriba el Número de referencia del proyecto del predecesor seguido de dos puntos y el número de la tarea. Por ejemplo, escriba: 765021:12. Esto indica que el número de referencia del proyecto del predecesor es 765021 y el predecesor es el número de tarea 12 del proyecto.
   >
   >1. Agregue el tipo de dependencia para este predecesor. Para obtener más información, vea [Crear predecesoras entre proyectos](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Presione **Intro**.
   >
   >**IMPORTANTE**
   >
   >No puede agregar una tarea predecesora entre proyectos cuando la lista de tareas se muestra en el modo de guardado manual.

   El icono del predecesor se vuelve verde cuando la tarea del predecesor se marca como completada. Esto indica que la tarea dependiente está lista para trabajar.

   Para obtener más información acerca de los tipos de relación disponibles en la columna Predecesoras, vea [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) en [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Ver detalles del predecesor

Puede ver rápidamente los detalles sobre el predecesor desde la lista de tareas.

1. En la lista de tareas, pase el ratón sobre el número de predecesora en la columna **Predecesoras**.

   Se muestra un cuadro con los detalles del predecesor.

   ![Detalles de la predecesora](assets/predecessor-details-in-task-list.png)

   Se muestran los siguientes detalles:

   **Nombre de predecesora:** Nombre del predecesor al que se hace referencia. Se incluye el número de tarea del predecesor. Haga clic en el nombre de la tarea para abrirla. En el ejemplo anterior, el predecesor es Production/Execution/Delivery.

   **Nombre del proyecto:** Nombre del proyecto donde reside el predecesor. El proyecto se identifica como el proyecto actual si el predecesor pertenece a los mismos proyectos que la tarea, o como proyecto cruzado, si el predecesor pertenece a un proyecto diferente. En el ejemplo anterior, el nombre del proyecto es Producción de activos digitales (integrada) - Proyecto. Para obtener más información sobre las tareas predecesoras entre proyectos, vea [Crear tareas predecesoras entre proyectos](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Puede ampliar los detalles del proyecto para ver las fechas de inicio y finalización planificadas del proyecto, la condición, el estado, el porcentaje completado y el propietario. Para un proyecto cruzado, puede hacer clic en **Ver proyecto** para abrir el proyecto.

   **ID.:** Número de referencia del proyecto donde se encuentra el predecesor.

   **Inicio planificado:** La fecha planificada de inicio de la tarea predecesora.

   **Fin planificado:** La fecha planificada de finalización de la tarea predecesora.

   **Número de predecesoras:** Número de predecesoras para la predecesora a la que se hace referencia. En el ejemplo anterior, la predecesora a la que se hace referencia tiene 1 predecesora.

   **Número de sucesoras:** Número de tareas sucesoras (o dependientes) para la predecesora a la que se hace referencia. En el ejemplo anterior, se hace referencia al predecesor con 1 sucesor.
