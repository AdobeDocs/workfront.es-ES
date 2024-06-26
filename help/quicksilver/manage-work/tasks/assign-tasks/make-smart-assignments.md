---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Realización de asignaciones inteligentes
description: Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias para usuarios, roles o equipos que Adobe Workfront presenta al asignar elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo. Para obtener información sobre las asignaciones inteligentes, consulte Información general sobre las asignaciones inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Realización de asignaciones inteligentes

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en el entorno de producción para los clientes que habilitaron versiones rápidas de.</span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la versión actual, consulte [Información general sobre la versión del tercer trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo.

Las asignaciones inteligentes son sugerencias para usuarios, funciones o equipos que Adobe Workfront presenta al asignar elementos de trabajo a recursos. Workfront basa sus sugerencias en un algoritmo que determina el recurso más apropiado para el trabajo.

<span class="preview">Hay dos algoritmos independientes en Workfront que calculan las asignaciones inteligentes que funcionan de forma diferente para las tareas y para los problemas. </span>

Para obtener más información sobre los criterios utilizados para determinar las asignaciones inteligentes, consulte [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

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
   <td> <p>Permisos de contribución o superiores con la capacidad de asignar tareas y problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Realización de asignaciones inteligentes

Las asignaciones inteligentes están disponibles en la mayoría de las ubicaciones donde puede realizar asignaciones en Workfront.

1. Vaya a y, a continuación, haga clic en **Asignaciones** o **Asignar esto a** campo:

   * Una lista de tareas o problemas o un informe
   * Un encabezado de tarea o problema
   * El panel Resumen de tareas o problemas
   * <span class="preview">Cuadro Nueva tarea o Nuevo problema a medida que agrega una nueva tarea o problema a un proyecto</span>
   * El campo Asignaciones de un elemento enumerado en el área de Inicio
   * Una tarea o un problema en el Distribuidor de cargas de trabajo

1. Coloque el cursor en el campo Asignaciones y espere dos segundos.

   <div class="preview">
   Se muestra una o varias de las siguientes secciones con sugerencias de asignación inteligente:

   * **Asignaciones sugeridas**: se muestra para las tareas. <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   Se muestra el encabezado de la lista **Estas son algunas recomendaciones** en lugar de **Asignaciones sugeridas** en el entorno Producción.
     >
   * **Usuarios y equipos**: se muestra para tareas y problemas.
   * **Funciones del puesto**: Muestra las tareas y los problemas.
   * **Valorar roles de trabajo de tarjeta**: se muestra para las tareas. Para obtener más información, consulte [Administrar tarjetas de tarifa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   En el caso de las tareas, las asignaciones inteligentes se muestran en las secciones siguientes, según la fase del cálculo del algoritmo en la que se hayan identificado las asignaciones:

   * **Asignaciones sugeridas**: Asignaciones identificadas en la primera fase del cálculo del algoritmo de asignación inteligente de tareas. <span class="preview">Esta sección no está disponible para problemas.</span>
   * <span class="preview">**Usuarios y equipos**, **Funciones del puesto**, o **Valorar roles de trabajo de tarjeta**: Asignaciones identificadas en la segunda fase del cálculo del algoritmo de asignación inteligente de tareas. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Para obtener más información, consulte [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Seleccione el usuario en la lista de recomendaciones haciendo clic en su nombre.

1. (Opcional) Haga clic en **Asignármelo a mí** para asignarse el elemento de trabajo.

   >[!TIP]
   >
   >Si no hay sugerencias, la lista de sugerencias no se abre.

1. (Opcional) Si no desea utilizar uno de los usuarios recomendados de la lista de asignaciones inteligentes, empiece a escribir el nombre del recurso deseado y selecciónelo cuando aparezca en la lista.
1. Clic **Entrar** para realizar la asignación.

   El usuario seleccionado está asignado a la tarea o al problema.
