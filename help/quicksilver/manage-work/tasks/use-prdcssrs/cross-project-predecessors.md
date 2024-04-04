---
product-area: projects
navigation-topic: use-predecessors
title: Crear predecesoras entre proyectos
description: Una tarea predecesora entre proyectos es una tarea de la que depende otra tarea (denominada tarea sucesora) de otro proyecto. El predecesor es la tarea que tiene prioridad sobre la tarea dependiente (sucesora). Por ejemplo, puede crear una dependencia que requiera que la tarea predecesora se marque como Completada antes de que pueda iniciarse la tarea dependiente.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 0%

---

# Crear predecesoras entre proyectos

<!--Audited: 12/2023-->

Una tarea predecesora entre proyectos es una tarea de la que depende otra tarea (denominada tarea sucesora) de otro proyecto. El predecesor es la tarea que tiene prioridad sobre la tarea dependiente (sucesora). Por ejemplo, puede crear una dependencia que requiera que la tarea predecesora se marque como Completada antes de que pueda iniciarse la tarea dependiente.

Adobe Workfront permite que las tareas dependan de tareas de otros proyectos, al igual que permite predecesoras dentro de un solo proyecto.

>[!INFO]
>
>Por ejemplo, una empresa excavadora tiene una sola retroexcavadora y dos proyectos tienen tareas que requieren el uso de la retroexcavadora. El jefe de proyecto puede convertir la tarea del primer proyecto en predecesora de la tarea del segundo proyecto. Esto muestra que el segundo proyecto puede empezar a utilizar la retroexcavadora cuando el primer proyecto termina con ella.

Al vincular proyectos mediante predecesoras entre proyectos, las fechas del proyecto principal (el que tiene la tarea predecesora) afectarán al proyecto secundario (el que tiene la tarea sucesora).

>[!TIP]
>
>Debe recalcular las escalas de tiempo de los proyectos para ver las fechas actualizadas del proyecto secundario. Para obtener más información sobre cómo recalcular las escalas de tiempo, consulte [Configurar cálculos de escala de tiempo para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para obtener más información sobre las relaciones de predecesoras, consulte [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar </p> 
   O
   <p>Actual: plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y los proyectos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Creación de una predecesora entre proyectos

1. Vaya a la tarea que va a ser su sucesora (tarea dependiente).
1. Clic **Predecesoras** en el panel izquierdo.
1. Clic **Agregar predecesora.**
1. En el **Proyecto principal** , empiece a escribir el nombre del proyecto que contiene la tarea que desea que sea la predecesora de la tarea actual.
1. Haga clic en el nombre cuando aparezca en la lista desplegable.
1. En el **Tareas** , empiece a escribir el nombre de la tarea que desea que sea la predecesora de la tarea actual.
1. Especifique la siguiente información para definir la relación entre la tarea predecesora y la dependiente:

   * **Tipo de dependencia:** Seleccione la relación que desea que tenga la tarea predecesora con la tarea dependiente. La relación predeterminada es &quot;Finalizar-Iniciar&quot;, lo que significa que la tarea predecesora debe finalizar antes de que pueda comenzar la tarea dependiente. Para obtener más información sobre los distintos tipos de dependencias, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Retardo:** Especifique la cantidad de tiempo que debe transcurrir después de la finalización de un predecesor forzado hasta que pueda comenzar la tarea dependiente. Para obtener más información sobre los distintos tipos de retardo, consulte [Resumen de tipos de retardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Forzado:** Si se selecciona esta opción, los usuarios que comienzan las tareas antes no pueden eludir la relación de dependencia entre las dos tareas. Por ejemplo, si se aplica una relación entre la Tarea A y la Tarea B, la Tarea B no se puede iniciar hasta que se complete la Tarea A. Para obtener más información acerca de cómo aplicar predecesoras, consulte [Forzar predecesoras](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Cuando esta opción no está seleccionada, la dependencia se trata como una sugerencia a los usuarios. Por ejemplo, los usuarios pueden iniciar la Tarea B antes de que se complete la Tarea A.

1. Haga clic en **Guardar**.

   Las tareas que tienen una tarea predecesora entre proyectos muestran el número de referencia del proyecto al que pertenece la tarea predecesora y el número de la tarea, separados por dos puntos, en la columna Predecesoras de una lista de tareas.

   ![Predecesora entre proyectos](assets/cross-project-predecessor-in-list-view.png)

   El icono del predecesor se vuelve verde cuando la tarea del predecesor se marca como completada. Esto indica que la tarea dependiente está lista para trabajar.

   Pase el ratón sobre este valor para obtener más información sobre el predecesor, el proyecto y las fechas. Haga clic en la predecesora entre proyectos en el cuadro de detalles para abrir la tarea.

   Haga clic cerca de la parte superior de la ventana flotante para ver más información sobre el proyecto del predecesor.

   Clic **Ver proyecto** para abrir el proyecto del predecesor.

   ![Detalles de predecesoras entre proyectos](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   El **Ver proyecto** Esta opción solo se muestra al ver una predecesora entre proyectos.

