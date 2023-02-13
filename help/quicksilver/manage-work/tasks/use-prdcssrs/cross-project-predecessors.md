---
product-area: projects
navigation-topic: use-predecessors
title: Crear predecesores entre proyectos
description: Un predecesor entre proyectos es una tarea de la que depende otra tarea (denominada tarea sucesora) en otro proyecto. El predecesor es la tarea que tiene prioridad sobre la tarea dependiente (sucesora). Por ejemplo, puede crear una dependencia que requiera que la tarea predecesora esté marcada como Completa antes de que la tarea dependiente pueda comenzar.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Crear predecesores entre proyectos

Un predecesor entre proyectos es una tarea de la que depende otra tarea (denominada tarea sucesora) en otro proyecto. El predecesor es la tarea que tiene prioridad sobre la tarea dependiente (sucesora). Por ejemplo, puede crear una dependencia que requiera que la tarea predecesora esté marcada como Completa antes de que la tarea dependiente pueda comenzar.

Al igual que los predecesores dentro de un solo proyecto, Adobe Workfront permite que las tareas dependan de tareas de otros proyectos.

**EJEMPLO**

Si una empresa de excavación tiene una sola plataforma y dos proyectos simultáneos tienen tareas que requieren el uso de la plataforma, el administrador del proyecto puede hacer que la tarea del primer proyecto dependa de la tarea del segundo proyecto para ilustrar que la excavación puede iniciarse cuando el proyecto anterior renuncie a la plataforma de fondo.
Al vincular proyectos mediante predecesores entre proyectos, las fechas del proyecto principal (la que tiene la tarea predecesora) afectarán al proyecto secundario (el que tiene la tarea sucesora).

>[!TIP]
>
>Debe volver a calcular las cronologías de los proyectos para ver las fechas actualizadas para el proyecto secundario. Para obtener más información sobre cómo volver a calcular las líneas de tiempo, consulte [Configurar nuevos cálculos de cronología para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para obtener más información sobre las relaciones predecesoras, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acceso

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Administrar permisos para las tareas y los proyectos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un predecesor entre proyectos

1. Vaya a la tarea que será su sucesor.
1. Haga clic en **Predecesores** en el panel izquierdo.
1. Haga clic en **Agregar predecesor.**
1. En el **Proyecto principal** , empiece a escribir el nombre del proyecto que contiene la tarea que desea que dependa de la tarea actual.
1. Haga clic en el nombre cuando aparezca en la lista desplegable.
1. En el **Tareas** , empiece a escribir el nombre de la tarea que desea que dependa de la tarea actual.
1. Especifique la siguiente información para definir la relación entre la tarea predecesora y la tarea dependiente:

   * **Tipo de dependencia:** Seleccione la relación que desea que tenga la tarea con la tarea dependiente. La relación predeterminada es &quot;Finish-Start&quot;, lo que significa que la tarea predecesora debe finalizar antes de que pueda iniciarse la tarea dependiente. Para obtener más información sobre los distintos tipos de dependencias, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Retraso:** Especifique la cantidad de tiempo que debe transcurrir después de completar un predecesor forzado hasta que pueda comenzar la tarea dependiente. Para obtener más información sobre los distintos tipos de retraso, consulte [Descripción general de los tipos de retraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Aplicado:** Cuando se selecciona esta opción, los usuarios que inician tareas antes no pueden eludir la relación de dependencia entre las dos tareas. Por ejemplo, si aplica una relación entre la tarea A y la tarea B, la tarea B no se puede iniciar hasta que la tarea A no se haya completado. Para obtener más información sobre cómo aplicar predecesores, consulte [Aplicar predecesores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      Cuando no se selecciona esta opción, la dependencia se trata como una sugerencia para los usuarios. Por ejemplo, los usuarios pueden iniciar la tarea B antes de que la tarea A se complete.

1. Haga clic en **Guardar**.

   Las tareas que tienen un predecesor entre proyectos muestran el número de referencia del proyecto al que pertenece el predecesor y el número de la tarea, separados por dos puntos en la columna Predecesores de una lista de tareas.

   ![predecesor entre proyectos](assets/cross-project-predecessor-in-list-view.png)

   El icono predecesor se vuelve verde cuando la tarea predecesora se marca como completada. Esto indica que la tarea dependiente está lista para funcionar.

   Pase el ratón sobre este valor para obtener más información sobre el predecesor, el proyecto y las fechas. Haga clic en el predecesor entre proyectos en el cuadro de detalles para abrir la tarea. Haga clic en **Consulte Proyecto** para abrir el proyecto cruzado.

   ![Detalles del predecesor entre proyectos](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   La variable **Consulte Proyecto** solo se muestra al visualizar un predecesor entre proyectos.

