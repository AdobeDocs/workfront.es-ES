---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Crear una historia de Agile en una iteración
description: Este artículo describe cómo crear una nueva historia Agile cuando ya está en la iteración.
author: Jenny
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 26%

---

# Crear una historia Agile en una iteración

Este artículo describe cómo crear una nueva historia Agile cuando ya está en la iteración. Para obtener información acerca de cómo crear una historia Agile a partir de una tarea, un problema u otra área de [!DNL Adobe Workfront], vea [Agregar historias a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

## Crear una historia Agile en una iteración

1. Vaya a la iteración Agile en la que desea crear la historia:

   {{step1-to-team}}

   1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![icono Cambiar de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

   1. En el panel izquierdo, seleccione **[!UICONTROL Iterations]**.
   1. Haga clic en el nombre de la iteración específica en la que desea crear un artículo.
   1. En el panel izquierdo, seleccione **[!UICONTROL Historias]**.

1.  Haga clic en **[!UICONTROL Nueva historia]**.
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
      <td>Especifique la estimación para la historia. Si su equipo Agile está configurado para estimar las historias en puntos, de forma predeterminada 1 punto equivale a 8 horas. Las estimaciones se añaden como [!UICONTROL Planned Hours] en la historia.<br>Por ejemplo, si estima una historia como 3 puntos, el comportamiento predeterminado es agregar 24 horas planificadas a la historia.<br>Si un artículo contiene subtareas, recuerde que las estimaciones combinadas de todas las subtareas determinan la estimación del artículo principal. Para obtener más información, vea <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Agregar una subtarea a una historia existente en el tablero [!UICONTROL Scrum]</a>.</td>
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
