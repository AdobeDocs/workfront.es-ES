---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Crear una historia Agile en una iteración
description: Este artículo describe cómo crear una nueva historia Agile cuando ya está en la iteración.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Crear una historia Agile en una iteración

Este artículo describe cómo crear una nueva historia Agile cuando ya está en la iteración. Para obtener información acerca de cómo crear una historia Agile a partir de una tarea, un problema u otra área de [!DNL Adobe Workfront], vea [Agregar historias a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Trabajo] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] al proyecto en el que se encuentra la historia</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Crear una historia Agile en una iteración

1. Vaya a la iteración Agile en la que desea crear la historia:

   1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront, y luego haga clic en **[!UICONTROL Equipos]**.

   1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

   1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]**.
   1. Haga clic en el nombre de la iteración específica en la que desea crear un artículo.
   1. En el panel izquierdo, seleccione **[!UICONTROL Historias]**.

1.  Haga clic en **[!UICONTROL Nueva historia].**
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
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong></td>
      <td>Escriba una descripción para la historia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Seleccione esta opción si el artículo está listo para añadirse a una iteración. Cuando se selecciona esta opción, se indica a los usuarios qué historias del registro de pendientes están listas para agregarse a una iteración.<br>Se puede agregar una historia a una iteración independientemente de si está marcada o no <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimar] (puntos)</strong></td>
      <td>Especifique la estimación para la historia. Si su equipo Agile está configurado para estimar las historias en puntos, por defecto 1 punto es igual a 8 horas. Las estimaciones se agregan como [!UICONTROL Horas planificadas] en la historia.<br>Por ejemplo, si estima una historia como 3 puntos, el comportamiento predeterminado es agregar 24 horas planificadas a la historia.<br>Si un artículo contiene subtareas, recuerde que las estimaciones combinadas de todas las subtareas determinan la estimación del artículo principal. Para obtener más información, vea <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Agregar una subtarea a una historia existente en el tablero [!UICONTROL Scrum]</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Proyecto principal]</strong></td>
      <td>Empiece a escribir el nombre del proyecto con el que se asociará esta historia.<br>De manera predeterminada, el color de la historia se muestra con el mismo color que otras historias de este proyecto.<br>El estado del proyecto debe establecerse en [!UICONTROL Actual]. Si el estado del proyecto es cualquier cosa excepto [!UICONTROL Actual], no se muestra en el menú desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarea principal]</strong></td>
      <td>Después de elegir un proyecto principal, tiene la opción de elegir una tarea principal. Al seleccionar una tarea principal, el artículo se crea como una subtarea de la tarea principal en el proyecto seleccionado.<br>Empiece a escribir el nombre de la tarea principal de la historia y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Seleccione cualquier formulario personalizado para agregar al artículo.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Guardar historia]**.
