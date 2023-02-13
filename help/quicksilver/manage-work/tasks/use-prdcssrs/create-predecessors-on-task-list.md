---
product-area: projects
navigation-topic: use-predecessors
title: Crear una relación predecesora en la lista de tareas
description: Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras tareas para iniciarse o completarse. Por ejemplo, no desea alojar una parte (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Crear una relación predecesora en la lista de tareas

Puede utilizar tareas predecesoras (o solo predecesoras) para vincular tareas que dependen de otras tareas para iniciarse o completarse. Por ejemplo, no desea alojar una parte (tarea dependiente) antes de enviar las invitaciones (tarea predecesora).

Este artículo muestra cómo crear predecesores en la lista de tareas.

Puede ver las tareas anteriores en las siguientes áreas de Adobe Workfront:

* En la lista de tareas de la columna Predecesores .
* En el diagrama de Gantt
* En la sección Predecesores de una tarea dependiente

Para obtener más información, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Editar acceso a Tareas y proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un predecesor

1. Vaya a un proyecto.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Asegúrese de que la vista actual muestre la variable **Predecesor** para abrir el Navegador.

   Si la vista no muestra la columna Predecesores, cambie a una vista que lo haga o agregue la columna a la vista.

1. Seleccione la tarea que desea designar como tarea dependiente.
1. Haga clic dentro del **Predecesores** para abrir el Navegador.
1. Escriba el número de tarea que desea designar como predecesor de la tarea seleccionada y, a continuación, pulse **Entrar**.

   El icono predecesor se vuelve verde cuando la tarea predecesora se marca como completada. Esto indica que la tarea dependiente está lista para funcionar.

   Para obtener más información sobre los tipos de relación disponibles en la columna Predecesores , consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) en [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Ver detalles del predecesor

Puede ver rápidamente los detalles sobre el predecesor desde la lista de tareas.

1. En la lista de tareas, pase el ratón sobre el número de predecesor en la **Predecesores** para abrir el Navegador.

   Aparece un cuadro con los detalles del predecesor.

   ![Detalles del predecesor](assets/predecessor-details-in-task-list.png)

   Se muestran los siguientes detalles:

   **Nombre del predecesor:** Nombre del predecesor al que se hace referencia. Se incluye el número de tarea del predecesor. Haga clic en el nombre de la tarea para abrirla. En el ejemplo anterior, el predecesor es Production/Execution/Delivery.

   **Nombre del proyecto:** Nombre del proyecto en el que reside el predecesor. El proyecto se identifica como el proyecto actual si el predecesor pertenece a los mismos proyectos que la tarea, o como un proyecto cruzado, si el predecesor pertenece a un proyecto diferente. En el ejemplo anterior, el nombre del proyecto es Producción de recursos digitales (integrada) - Proyecto. Para obtener más información sobre los predecesores entre proyectos, consulte [Crear predecesores entre proyectos](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Puede ampliar los detalles del proyecto para ver las fechas de inicio y finalización, la condición, el estado, el porcentaje completado y el propietario del proyecto. Para un proyecto cruzado, puede hacer clic en **Consulte Proyecto** para abrir el proyecto.

   **ID:** Número de referencia del proyecto en el que se encuentra el predecesor.

   **Inicio planificado:** Fecha de inicio planeada de la tarea predecesora.

   **Fin planificado:** Fecha de finalización planeada de la tarea predecesora.

   **Número de predecesores:** Número de predecesores a los que se hace referencia para el predecesor. En el ejemplo anterior, el predecesor al que se hace referencia tiene 1 predecesor.

   **Número de sucesores:** Número de tareas sucesoras (o dependientes) a las que se hace referencia en el predecesor. En el ejemplo anterior, el predecesor al que se hace referencia tiene 1 sucesor.
