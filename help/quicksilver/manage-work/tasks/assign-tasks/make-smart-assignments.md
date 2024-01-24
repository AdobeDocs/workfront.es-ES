---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Realización de asignaciones inteligentes
description: Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias para los usuarios que Adobe Workfront presenta al asignar elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo. Para obtener información sobre las asignaciones inteligentes, consulte Información general sobre las asignaciones inteligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 03894773e61fc0706148695572a164a2e778da9b
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Realización de asignaciones inteligentes

<!--update "Results" to "Other assignments" with Prod-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes.</span>

<span class="preview">Para obtener más información sobre la programación actual de versiones, consulte [Información general sobre la versión del primer trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

Puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo.

Las asignaciones inteligentes son sugerencias para los usuarios que Adobe Workfront presenta al asignar elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo.

<span class="preview">Hay dos algoritmos independientes en Workfront para tareas y problemas. </span>
Para obtener información sobre las asignaciones inteligentes, consulte [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
      O
      <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Problemas</p> <p>Acceso de visualización o superior a Proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de contribución o superiores con la capacidad de asignar tareas y problemas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Realización de asignaciones inteligentes

Las asignaciones inteligentes están disponibles en la mayoría de las ubicaciones donde puede realizar asignaciones en Workfront.

1. Vaya a y, a continuación, haga clic en **Asignaciones** o **Asignar esto a** campo:

   * Una lista de tareas o problemas o un informe
   * Un encabezado de tarea o problema
   * El panel Resumen de tareas o problemas
   * El campo Asignaciones de un elemento enumerado en el área de Inicio
   * Una tarea o un problema en el Distribuidor de cargas de trabajo

1. Coloque el cursor en el campo de asignación y espere dos segundos.

   <span class="preview">El **Asignaciones sugeridas** se muestra la lista.</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   Se muestra el encabezado de la lista **Estas son algunas recomendaciones** en lugar de **Asignaciones sugeridas** en una lista de problemas.

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   Si tiene problemas, las sugerencias de asignación inteligente se muestran en **Asignaciones sugeridas** área.

   En el caso de las tareas, las asignaciones inteligentes se muestran en las secciones siguientes, según la fase del cálculo del algoritmo en la que se hayan identificado las asignaciones:

   * **Asignaciones sugeridas**: Asignaciones identificadas en la primera fase del cálculo del algoritmo de asignación inteligente de tareas.
   * <span class="preview">**Resultados**: Asignaciones identificadas en la segunda fase del cálculo del algoritmo de asignación inteligente de tareas. Esta sección no está disponible para problemas. </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   Para obtener más información, consulte [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. Seleccione el usuario en la lista de recomendaciones haciendo clic en su nombre.

1. (Opcional) Haga clic en **Asignármelo a mí** para asignarse el elemento de trabajo.

   >[!TIP]
   >
   >Si no hay sugerencias, la lista de sugerencias no se abre.

1. (Opcional) Si no desea utilizar uno de los usuarios recomendados de la lista de asignaciones inteligentes, empiece a escribir el nombre del usuario deseado y selecciónelo cuando aparezca en la lista.
1. Clic **Entrar** para realizar la asignación.

   El usuario seleccionado está asignado a la tarea o al problema.
