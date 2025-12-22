---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Crear una historia de Agile
description: Puede crear una historia de Agile en una iteración de varias formas. Después de crear una historia de Agile, puede agregar subtareas a la historia.
author: Jenny
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 17%

---

# Crear una historia de Agile

Puede crear una historia de Agile en una iteración de varias formas. Después de crear una historia de Agile, puede agregar subtareas a la historia.

Cuando agrega una historia o subtarea en una iteración, el tipo de duración se establece en [!UICONTROL Simple] y la restricción de tarea se establece en Fechas fijas, con las fechas bloqueadas dentro de la iteración. No se puede modificar el tipo de duración ni la restricción de tarea en una iteración. Además, la duración de la tarea debe ser mayor que 0 minutos.

Para obtener información acerca de cómo administrar la historia después de agregarla a la iteración, vea [Iteraciones](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso al proyecto en el que se encuentra la historia </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una historia de Agile en una iteración

1. Vaya a la iteración Agile en la que desea crear la historia:

   {{step1-to-team}}

   1. (Opcional) Haga clic en el icono de **[!UICONTROL Cambiar equipo]** ![icono de Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

   1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.
   1. Haga clic en el nombre de la iteración específica en la que desea crear un artículo.

   ![Agregar nueva historia a la iteración](assets/iteration-stories-list.png)

1. Haga clic en **[!UICONTROL Nueva historia].**
1. Especifique la siguiente información:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nombre de artículo]</strong></td>
      <td>Escriba un nombre para la historia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Escriba una descripción para la historia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Seleccione esta opción si el artículo está listo para añadirse a una iteración. Cuando se selecciona esta opción, se indica a los usuarios qué historias del registro de pendientes están listas para agregarse a una iteración.<br>Se puede agregar una historia a una iteración independientemente de si está marcada o no <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimar] (puntos)</strong></td>
      <td>Especifique la estimación para la historia. Si su equipo de Agile está configurado para estimar las historias en puntos, por defecto 1 punto es igual a 8 horas. Las estimaciones se añaden como [!UICONTROL Planned Hours] en la historia.<br>Por ejemplo, si calcula una historia como 3 puntos, el comportamiento predeterminado es agregar 24 [!UICONTROL Horas planificadas] a la historia.<br>Si un artículo contiene subtareas, recuerde que las estimaciones combinadas de todas las subtareas determinan la estimación del artículo principal. Para obtener más información, consulte <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Añadir historias a una iteración existente</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Empiece a escribir el nombre del proyecto con el que se asociará esta historia.<br>De manera predeterminada, el color de la historia se muestra con el mismo color que otras historias de este proyecto.<br>El estado del proyecto debe establecerse en [!UICONTROL Actual]. Si el estado del proyecto es cualquier cosa excepto [!UICONTROL Actual], no se muestra en el menú desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>Después de elegir un proyecto principal, tiene la opción de elegir una tarea principal. Al seleccionar una tarea principal, el artículo se crea como una subtarea de la tarea principal en el proyecto seleccionado.<br>Empiece a escribir el nombre de la tarea principal de la historia y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Seleccione cualquier formulario personalizado para agregar al artículo.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Guardar historia]**.

## Crear una historia de Agile en el registro de pendientes

Puede crear una historia Agile a partir del registro de pendientes Agile, tal como se describe en la sección [Crear nuevas historias en el registro de asuntos pendientes](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) del artículo [[!UICONTROL Administrar] el registro de asuntos pendientes Agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Agregar una tarea o un problema como historia de Agile

Puede agregar una tarea o un problema existente como artículo a una iteración. Para obtener más información, consulte [Agregar historias a una iteración existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) o [Agregar historias y problemas del tablero [!UICONTROL Scrum]](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Crear subtareas en una historia de Agile

Puede crear una subtarea en un artículo de Agile mediante cualquiera de los métodos siguientes:

* Utilizando la ficha **[!UICONTROL Subtareas]**, tal como se describe en [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) en [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Directamente desde el guion gráfico, como se describe en [Crear una iteración](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
