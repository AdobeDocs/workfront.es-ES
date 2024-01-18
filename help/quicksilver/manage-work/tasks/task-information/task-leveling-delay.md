---
product-area: projects
navigation-topic: task-information
title: Actualizar demora de nivelación de tarea
description: A veces, puede haber conflictos entre las programaciones de tareas de un proyecto. Puede redistribuir recursos o solucionar conflictos de recursos reprogramando recursos y tareas para que todas las tareas se puedan completar dentro de una programación realista. Para obtener información acerca de la redistribución de tareas, vea Redistribuir recursos en el diagrama de Gantt
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# Actualizar demora de nivelación de tarea

A veces, puede haber conflictos entre las programaciones de tareas de un proyecto. Puede redistribuir recursos o solucionar conflictos de recursos reprogramando recursos y tareas para que todas las tareas se puedan completar dentro de una programación realista. Para obtener información sobre la redistribución de tareas, consulte [Nivelar recursos en el gráfico Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Como jefe de proyecto o como encargado de la tarea, también puede agregar un Retraso por redistribución en tareas individuales para tener en cuenta los conflictos de recursos o de programación. En otras palabras, una tarea se puede programar con un retraso para garantizar que, cuando Adobe Workfront nivele las tareas, una programación más realista supere los conflictos de recursos.

Si se agrega un retraso de redistribución a una tarea, se ajusta la Fecha proyectada de finalización de la tarea. Para obtener información sobre la fecha proyectada de finalización, consulte [Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos para tareas </p> <p>Permisos de contribución o superiores para proyectos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Agregar un retraso de nivelación a una tarea

1. Vaya a una tarea para la que desee agregar un retraso de nivelación.
1. Haga clic en **Icono Más** a la derecha del nombre de la tarea y haga clic en **Editar**.

1. Clic **Configuración**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Especifique el **Retraso de nivelación**, en horas, y después elija una unidad de tiempo.\
   Este es el tiempo en que el recurso se retrasará al iniciar la tarea debido a conflictos de recursos.

   Seleccione entre las siguientes opciones para unidades de tiempo:

   * minutos
   * Horas. Esta es la opción predeterminada.
   * Días
   * Semanas
   * Meses
   * Minutos transcurridos
   * Horas transcurridas
   * Días transcurridos
   * Semanas transcurridas
   * Meses transcurridos

   >[!TIP]
   >
   >El tiempo transcurrido es una unidad de tiempo de la duración de una tarea. Es el tiempo entre la Fecha planificada de inicio y la Fecha planificada de finalización de una tarea que incluye días festivos, fines de semana y días libres. En otras palabras, el tiempo transcurrido es el paso de los días del calendario.

1. Clic **Guardar**. 

 
