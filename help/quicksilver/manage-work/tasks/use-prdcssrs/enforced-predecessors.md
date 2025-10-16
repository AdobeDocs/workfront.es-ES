---
product-area: projects
navigation-topic: use-predecessors
title: Forzar predecesoras
description: Las predecesoras son tareas de las que dependen otras tareas para su finalización. Las relaciones de predecesora afectan a las fechas de inicio y finalización de las tareas y, en última instancia, afectan a la línea de tiempo del proyecto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 97%

---

# Forzar predecesoras

<!-- Audited: 2/2024 -->

Las predecesoras son tareas de las que dependen otras tareas para su finalización. Las relaciones de predecesora afectan a las fechas de inicio y finalización de las tareas y, en última instancia, afectan a la línea de tiempo del proyecto.

Para obtener información sobre las predecesoras, consulte [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Al establecer relaciones de predecesora entre las tareas, se define cómo el comienzo o la finalización de una tarea dependiente depende del comienzo o de la finalización de sus tareas predecesoras. Esto se realiza mediante diferentes tipos de dependencia.

Para obtener información acerca de los tipos de dependencia, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Información general sobre predecesoras forzadas

>[!IMPORTANT]
>
>Debe imponer predecesoras para exigir que se respeten las relaciones de predecesor. Si no se imponen predecesoras, las tareas dependientes pueden comenzar y finalizar independientemente del comienzo y la finalización de sus predecesoras, independientemente de sus tipos de dependencia.

Puede forzar la relación de predecesora al establecer predecesoras en un proyecto.

Si se fuerza una predecesora, la tarea sucesora no podrá iniciarse antes de que se complete la predecesora. Por ejemplo, si se fuerza una relación Finalizar-Iniciar entre la Tarea A y la Tarea B, la Tarea B no puede comenzar (el estado debe ser Nuevo y el porcentaje completado debe permanecer en 0 %) hasta que la Tarea A se marque como completada. Las relaciones de imposición se aplican a todos los tipos de predecesoras.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
      <p>New: Standard</p> 
      <p>OR</p>
      <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Forzar una predecesora a nivel de tarea

1. Vaya a la tarea sucesora cuya predecesora desea forzar.
1. Haga clic en **Predecesoras** en el panel izquierdo y luego haga clic en **Agregar predecesora**.
1. (Condicional) Si desea añadir una tarea predecesora entre proyectos, quite el nombre del proyecto en el campo **Proyecto principal** y reemplácelo por otro proyecto.
1. Especifique el nombre de la tarea predecesora en el campo **Tareas**.
1. Especifique el **Tipo de dependencia** entre estas dos tareas.

   El **Tipo de dependencia** predeterminado es **Finalizar-Iniciar**.

1. Seleccione el campo **Forzado** para forzar la predecesora.
1. Haga clic en **Guardar**.

## Forzar una predecesora en una lista de tareas

1. Vaya a una lista de tareas de un proyecto.
1. En el menú desplegable **Vista**, seleccione la **Vista estándar**.

1. Tome nota mentalmente del número de tareas que va a designar como predecesoras.
1. Busque la tarea sucesora cuya predecesora desea forzar.
1. En la columna **Predecesoras**, empiece a escribir el número de la tarea predecesora seguida de “e”. Por ejemplo, escriba &quot;1e&quot; para añadir la tarea número 1 como predecesora de la tarea seleccionada.
1. Haga clic en Entrar para guardar la información de predecesoras de la tarea.

   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
