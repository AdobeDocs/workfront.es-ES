---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Realizar asignaciones inteligentes
description: Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias sobre usuarios, funciones o equipos que Adobe Workfront le presenta cuando asigna elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo. Para obtener información sobre las asignaciones inteligentes, consulte Información general sobre las asignaciones inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 89%

---

# Realizar asignaciones inteligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">La información resaltada en esta página hace referencia a la funcionalidad disponible solamente en el entorno de producción para los clientes que habilitaron versiones rápidas.</span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Esta funcionalidad se eliminará del entorno de producción para los clientes que habilitaron la versión rápida con la versión 25.1 en enero de 2025. Para obtener más información sobre la versión 25.1, consulte [Información general sobre la versión del primer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo.

Las asignaciones inteligentes son sugerencias sobre usuarios, funciones o equipos que Adobe Workfront le presenta cuando asigna elementos de trabajo a recursos. Workfront basa sus sugerencias en un algoritmo que determina el recurso más apropiado para el trabajo.

<span class="preview">Workfront cuenta con dos algoritmos independientes que calculan asignaciones inteligentes que funcionan de forma diferente según se trate de tareas o problemas.</span>

Para obtener más información acerca de los criterios utilizados para determinar las asignaciones inteligentes, consulte [Información general sobre las asignaciones inteligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Nuevo: estándar</p>
      O
      <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Problemas</p> <p>Acceso de visualización o superior a los proyectos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de aportación o superiores con capacidad para realizar asignaciones a tareas y problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Realizar asignaciones inteligentes

Las asignaciones inteligentes están disponibles en la mayoría de las ubicaciones donde puede realizar asignaciones en Workfront.

1. Vaya a una de las siguientes áreas y haga clic en el campo **Asignaciones** o **Asignar esto a**:

   * Una lista de tareas o problemas o un informe
   * Un encabezado de tarea o problema
   * El panel Resumen de tareas o problemas
   * Un cuadro <span class="preview">Nueva tarea</span> o Nuevo problema, cuando añade <span class="preview">una nueva tarea</span> o problema a un proyecto
   * Una tarea o un problema en el Distribuidor de cargas de trabajo

1. Coloque el cursor en el campo Asignaciones y espere dos segundos.

   En el caso de los problemas, las asignaciones inteligentes se muestran en las siguientes secciones:

   * **Usuarios y equipos**
   * **Funciones del puesto**

   ![](assets/smart-assignments-issue-header.png)

   En el caso de las tareas, las asignaciones inteligentes se muestran en las secciones siguientes, según la fase de cálculo del algoritmo en la que se hayan identificado las asignaciones:

   * <span class="preview">**Asignaciones sugeridas**: muestra las asignaciones identificadas en la primera fase del algoritmo de asignación inteligente de tareas.</span>
   * **Usuarios y equipos**, **Funciones del puesto** o <span class="preview">**Puestos de trabajo de tarjeta de tarifas**</span>: asignaciones identificadas en la segunda fase de cálculo del algoritmo de la asignación inteligente de tareas.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Para obtener más información, consulte [Información general sobre las asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Seleccione el recurso en la lista de recomendaciones haciendo clic en su nombre.

1. (Opcional) Haga clic en **Asignármelo a mí** para asignarse a sí mismo el elemento de trabajo.

   >[!TIP]
   >
   >Si no hay sugerencias, la lista de sugerencias no se abre.

1. (Opcional) Si no desea utilizar alguno de los usuarios recomendados en la lista de asignaciones inteligentes, empiece a escribir el nombre del recurso deseado y selecciónelo cuando aparezca en la lista.
1. Haga clic en **Introducir** para realizar la asignación.

   El usuario seleccionado es asignado a la tarea o el problema.
