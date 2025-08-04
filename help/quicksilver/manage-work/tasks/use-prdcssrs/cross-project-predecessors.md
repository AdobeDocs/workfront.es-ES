---
product-area: projects
navigation-topic: use-predecessors
title: Crear predecesoras entre proyectos
description: Una tarea predecesora entre proyectos es una tarea de la que depende otra tarea (denominada tarea sucesora) de otro proyecto. La predecesora es la tarea que tiene prioridad sobre la tarea dependiente (sucesora). Por ejemplo, puede crear una dependencia que requiera que la tarea predecesora se marque como Completada antes de poder iniciar la tarea dependiente.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 94%

---

# Crear predecesoras entre proyectos

<!--Audited: 12/2024-->

Una tarea predecesora entre proyectos es una tarea de la que depende otra tarea (denominada tarea sucesora) de otro proyecto. La predecesora es la tarea que tiene prioridad sobre la tarea dependiente (sucesora). Por ejemplo, puede crear una dependencia que requiera que la tarea predecesora se marque como Completada antes de poder iniciar la tarea dependiente.

Adobe Workfront permite que las tareas dependan de tareas de otros proyectos, al igual que permite predecesoras dentro de un solo proyecto.

>[!INFO]
>
>Por ejemplo, una compañía excavadora tiene una sola retroexcavadora y dos proyectos tienen tareas que requieren el uso de la retroexcavadora. El administrador del proyecto puede convertir la tarea del primer proyecto en predecesora de la tarea del segundo proyecto. Esto muestra que el segundo proyecto puede empezar a utilizar la retroexcavadora cuando el primer proyecto termina con ella.

Al vincular proyectos mediante predecesoras entre proyectos, las fechas del proyecto principal (el que tiene la tarea predecesora) afectarán al proyecto secundario (el que tiene la tarea sucesora).

>[!TIP]
>
>Debe recalcular las líneas de tiempo de los proyectos para ver las fechas actualizadas del proyecto secundario. Para obtener más información sobre cómo recalcular líneas de tiempo, consulte [Configurar el recálculo de la línea de tiempo para los proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para obtener más información acerca de las relaciones de predecesoras, consulte [Información general sobre las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Estándar </p>

<p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y los proyectos</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una predecesora entre proyectos

>[!TIP]
>
>Aunque la creación de tareas de plantilla predecesoras es similar a la creación de tareas de proyecto predecesoras, no se pueden crear tareas de plantilla predecesoras entre plantillas para tareas de plantilla.


1. Vaya a la tarea que va a ser su sucesora (tarea dependiente).
1. Haga clic en **Predecesoras** en el panel izquierdo.

   >[!TIP]
   >
   >   El administrador del grupo o de Workfront podría quitar la sección **Predecesoras** u otras secciones del panel izquierdo.

1. Haga clic en **Añadir predecesora.**
1. En el campo **Proyecto principal**, empiece a escribir el nombre del proyecto que contiene la tarea que desea que sea la predecesora de la tarea actual.
1. Haga clic sobre el nombre cuando aparezca en la lista.
1. En el campo **Tareas**, empiece a escribir el nombre de la tarea que desea que sea la predecesora de la tarea actual.
1. Especifique la siguiente información para definir la relación entre la tarea predecesora y la dependiente:


   * **Tipo de dependencia:** seleccione la relación que desea que tenga la tarea predecesora con la tarea dependiente. La relación predeterminada es “Finalizar-Iniciar”, lo que significa que la tarea predecesora debe finalizar antes de que pueda comenzar la tarea dependiente. Para obtener más información acerca de los distintos tipos de dependencias, consulte [Información general sobre los tipos de dependencias entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Retardo:** especifique la cantidad de tiempo que debe transcurrir después de la finalización de una predecesora forzada hasta que pueda comenzar la tarea dependiente. Para obtener más información acerca de los distintos tipos de retardo, consulte [Información general sobre los tipos de retardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Forzada:** cuando se selecciona esta opción, la relación de dependencia entre las dos tareas no se puede evitar si los usuarios inician las tareas de forma anticipada. Por ejemplo, si se aplica una relación entre la tarea A y la tarea B, la tarea B no se puede iniciar hasta que se complete la tarea A. Para obtener más información sobre el uso de predecesoras, consulte [Forzar predecesoras](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Cuando esta opción no está seleccionada, la dependencia se trata como una sugerencia a los usuarios. Por ejemplo, los usuarios pueden iniciar la Tarea B antes de que se complete la Tarea A.

1. Haga clic en **Guardar**.

   Las tareas que tienen una tarea predecesora entre proyectos muestran el número de referencia del proyecto al que pertenece la tarea predecesora y el número de la tarea, separados por dos puntos, en la columna Predecesoras de una lista de tareas.

   ![Predecesora entre proyectos](assets/cross-project-predecessor-in-list-view.png)

   El icono de la predecesora se vuelve verde cuando la tarea predecesora se marca como completada. Esto indica que la tarea dependiente está lista para trabajar.

   Pase el puntero por encima de este valor para obtener más información sobre el predecesor, el proyecto y las fechas. Haga clic en la predecesora entre proyectos en el cuadro de detalles para abrir la tarea.

   Haga clic cerca de la parte superior de la ventana flotante para ver más información sobre el proyecto de la predecesora.

   Haga clic en **Ver proyecto** para abrir el proyecto de la predecesora.

   ![Detalles de predecesoras entre proyectos](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   La opción **Ver proyecto** solo se muestra al visualizar una predecesora entre proyectos.

