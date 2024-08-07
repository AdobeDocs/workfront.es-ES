---
product-area: projects
navigation-topic: use-predecessors
title: Forzar predecesoras
description: Las tareas predecesoras son tareas de las que dependen otras tareas para su finalización. Las relaciones de predecesoras afectan a las fechas de inicio y finalización de las tareas y, en última instancia, afectan a la cronología del proyecto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Forzar predecesoras

<!-- Audited: 2/2024 -->

Las tareas predecesoras son tareas de las que dependen otras tareas para su finalización. Las relaciones de predecesoras afectan a las fechas de inicio y finalización de las tareas y, en última instancia, afectan a la cronología del proyecto.

Para obtener información acerca de las tareas predecesoras, vea [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Al establecer relaciones de predecesoras entre tareas, se define cómo el comienzo o el fin de una tarea dependiente depende del comienzo o del fin de sus tareas predecesoras. Esto se realiza mediante diferentes tipos de dependencia.

Para obtener información acerca de los tipos de dependencia, vea [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Información general sobre predecesoras forzadas

>[!IMPORTANT]
>
>Debe hacer cumplir las predecesoras para exigir que se respeten las relaciones de predecesoras. Sin aplicar las tareas predecesoras, las tareas dependientes pueden comenzar y finalizar independientemente del comienzo y el fin de sus predecesoras, independientemente de sus tipos de dependencia.

Puede forzar la relación de predecesoras al establecer predecesoras en un proyecto.

Si se fuerza una tarea predecesora, la tarea sucesora no puede iniciarse antes de que finalice la predecesora. Por ejemplo, si se aplica una relación Fin-Comienzo entre la Tarea A y la Tarea B, la Tarea B no puede comenzar (el estado debe ser Nuevo y el porcentaje completado debe permanecer en 0%) hasta que la Tarea A se marque como completada. Las relaciones obligatorias se aplican a todos los tipos de predecesoras.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
      <p>Nuevo: estándar</p> 
      <p>O</p>
      <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Administrar permisos para las tareas y el proyecto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exigir un predecesor en el nivel de tarea

1. Vaya a la tarea sucesora cuyo predecesor desea aplicar.
1. Haga clic en **Predecesoras** en el panel izquierdo y luego haga clic en **Agregar predecesora**. Es posible que tengas que hacer clic en **Mostrar más** y luego en **Predecesoras**.
1. (Condicional) Si desea agregar una tarea predecesora entre proyectos, quite el nombre del proyecto en el campo **Proyecto principal** y reemplácelo por otro proyecto.
1. Especifique el nombre de las tareas predecesoras en el campo **Tareas**.
1. Especifique el **Tipo de dependencia** entre estas dos tareas.

   El **tipo de dependencia** predeterminado es **Finalizar-Inicio**.

1. Seleccione el campo **Forzado** para forzar el predecesor.
1. Haga clic en **Guardar**.

## Forzar un predecesor en una lista de tareas

1. Ir a una lista de tareas de un proyecto.
1. En el menú desplegable **Vista**, seleccione la **Vista estándar**.

1. Tome nota mentalmente del número de tareas que va a designar como predecesoras.
1. Busque la tarea sucesora cuyo predecesor desea aplicar.
1. En la columna **Predecesoras**, empiece a escribir el número de la tarea predecesora seguida de &quot;e&quot;. Por ejemplo, escriba &quot;1e&quot; para agregar la tarea número 1 como predecesora de la tarea seleccionada.
1. Haga clic en Entrar para guardar la información de predecesoras de la tarea.

   ![predecesora_forzada_en_lista.png](assets/predecessor-enforced-in-list-350x308.png)
