---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Realización de asignaciones inteligentes
description: Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias para usuarios, roles o equipos que Adobe Workfront presenta al asignar elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo. Para obtener información sobre las asignaciones inteligentes, consulte Información general sobre las asignaciones inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Realización de asignaciones inteligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes o en el entorno de producción para los clientes que habilitaron versiones rápidas.</span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener información acerca de la versión actual, consulte [Información general sobre la versión del cuarto trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo.

Las asignaciones inteligentes son sugerencias para usuarios, funciones o equipos que Adobe Workfront presenta al asignar elementos de trabajo a recursos. Workfront basa sus sugerencias en un algoritmo que determina el recurso más apropiado para el trabajo.

<span class="preview">Workfront cuenta con dos algoritmos independientes que calculan asignaciones inteligentes que funcionan de forma diferente en las tareas y en los problemas.</span>

Para obtener más información acerca de los criterios utilizados para determinar las asignaciones inteligentes, vea [Información general sobre las asignaciones inteligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Nuevo: estándar</p>
      O
      <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas y Problemas</p> <p>Acceso de visualización o superior a Proyectos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores con la capacidad de asignar tareas y problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Realización de asignaciones inteligentes

Las asignaciones inteligentes están disponibles en la mayoría de las ubicaciones donde puede realizar asignaciones en Workfront.

1. Vaya a una de las siguientes áreas y haga clic en el campo **Asignaciones** o **Asignar esto a**:

   * Una lista de tareas o problemas o un informe
   * Un encabezado de tarea o problema
   * El panel Resumen de tareas o problemas
   * <span class="preview">Nueva tarea</span> o nuevo cuadro de problema al agregar <span class="preview">una nueva tarea</span> o problema a un proyecto
   * Una tarea o un problema en el Distribuidor de cargas de trabajo

1. Coloque el cursor en el campo Asignaciones y espere dos segundos.

   En el caso de los problemas, las asignaciones inteligentes se muestran en las siguientes secciones:

   * **Usuarios y equipos**
   * **Funciones del puesto**

   ![](assets/smart-assignments-issue-header.png)

   En el caso de las tareas, las asignaciones inteligentes se muestran en las secciones siguientes, según la fase del cálculo del algoritmo en la que se hayan identificado las asignaciones:

   * <span class="preview">**Asignaciones sugeridas**: Muestra las asignaciones identificadas en la primera fase del algoritmo de asignación inteligente de tareas.</span>
   * **Usuarios y equipos**, **Funciones del puesto** o <span class="preview">**Funciones del puesto de la tarjeta de tarifas**</span>: Asignaciones identificadas en la segunda fase del cálculo del algoritmo de la asignación inteligente de tareas.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Para obtener más información, vea [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Seleccione el recurso en la lista de recomendaciones haciendo clic en su nombre.

1. (Opcional) Haga clic en **Asignármelo** para asignarse a sí mismo el elemento de trabajo.

   >[!TIP]
   >
   >Si no hay sugerencias, la lista de sugerencias no se abre.

1. (Opcional) Si no desea utilizar uno de los usuarios recomendados de la lista de asignaciones inteligentes, empiece a escribir el nombre del recurso deseado y selecciónelo cuando aparezca en la lista.
1. Haga clic en **Introducir** para realizar la asignación.

   El usuario seleccionado está asignado a la tarea o al problema.
