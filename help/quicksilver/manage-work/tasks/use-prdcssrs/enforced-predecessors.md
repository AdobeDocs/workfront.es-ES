---
product-area: projects
navigation-topic: use-predecessors
title: Aplicar predecesores
description: Los predecesores son tareas en las que otras tareas dependen de la finalización. Las relaciones de los predecesores afectan a las fechas de inicio y finalización de las tareas y, en última instancia, afectan a la cronología del proyecto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Aplicar predecesores

Los predecesores son tareas en las que otras tareas dependen de la finalización. Las relaciones de los predecesores afectan a las fechas de inicio y finalización de las tareas y, en última instancia, afectan a la cronología del proyecto.

Para obtener información sobre las predecesoras, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Al establecer relaciones predecesoras entre tareas, se define cómo el inicio o el fin de una tarea dependiente depende del inicio o el fin de sus tareas predecesoras. Esto se hace usando diferentes tipos de dependencias.

Para obtener información sobre los tipos de dependencia, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Resumen de predecesores reforzados

>[!IMPORTANT]
>
>Debe hacer cumplir a los predecesores para exigir que se respeten las relaciones predecesoras. Sin aplicar los predecesores, las tareas dependientes pueden iniciarse y finalizar de forma independiente desde el inicio y el fin de sus predecesores, independientemente de sus tipos de dependencia.

Puede aplicar la relación de predecesor al configurar predecesores en un proyecto.

Si se aplica un predecesor, la tarea sucesora no puede iniciarse antes de que finalice el predecesor. Por ejemplo, la aplicación de una relación Fin-Inicio entre la tarea A y la tarea B significa que la tarea B no puede iniciarse (el estado debe permanecer como Nuevo y el porcentaje completado debe permanecer en 0%) hasta que la tarea A se marque como completada. Las relaciones de aplicación se aplican a todos los tipos de predecesores.

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

## Aplicar un predecesor en el nivel de tarea

1. Vaya a la tarea sucesora cuyo predecesor desea aplicar.
1. Haga clic en **Predecesores** en el panel izquierdo y, a continuación, haga clic en **Agregar predecesor**. Es posible que tenga que hacer clic en **Mostrar más**, luego **Predecesores**.
1. (Condicional) Si desea agregar un predecesor de varios proyectos, elimine el nombre del proyecto en la sección **Proyecto principal** y reemplácelo por otro proyecto.
1. Especifique el nombre de la tarea o tareas predecesoras en la variable **Tareas** campo .
1. Especifique la variable **Tipo de dependencia** entre estas dos tareas.

   El valor predeterminado **Tipo de dependencia** es **Finish-Start**.

1. Seleccione el **Enforzado** para aplicar el predecesor.
1. Haga clic en **Guardar**.

## Aplicar un predecesor en una lista de tareas

1. Vaya a la lista de tareas de un proyecto.
1. En el **Ver** menú desplegable, seleccione la **Vista estándar**.

1. Anote el número de tareas que va a designar como predecesor.
1. Busque la tarea sucesora cuyo predecesor desee aplicar.
1. En el **Predecesores** , empiece a introducir el número de la tarea predecesora seguida de &quot;e&quot;. Por ejemplo, escriba &quot;1e&quot; para agregar el número de tarea 1 como predecesor a la tarea seleccionada.
1. Haga clic en Intro para guardar la información predecesora de la tarea.

   ![predecesor_forced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
