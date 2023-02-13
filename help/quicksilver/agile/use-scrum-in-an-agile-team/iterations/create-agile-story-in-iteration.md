---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Crear un artículo ágil en una iteración
description: Este artículo describe cómo crear un nuevo artículo ágil cuando ya se encuentra en la iteración.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Crear un artículo ágil en una iteración

Este artículo describe cómo crear un nuevo artículo ágil cuando ya se encuentra en la iteración. Para obtener información sobre la creación de un artículo ágil a partir de una tarea, un problema u otro área de [!DNL Adobe Workfront], consulte [Añadir artículos a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Administrar] al proyecto en el que se encuentra el artículo</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Crear un artículo ágil en una iteración

1. Vaya a la iteración ágil en la que desea crear el artículo:

   1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Equipos]**.

   1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

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
      <td>Escriba un nombre para el artículo.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong></td>
      <td>Escriba una descripción para el artículo.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Seleccione esta opción si el artículo está listo para agregarse a una iteración. Cuando se selecciona esta opción, indica a los usuarios qué artículos del "backlog" están listos para agregarse a una iteración.<br>Se puede añadir un artículo a una iteración tanto si está marcado como si no <strong>[!UICONTROL Listo].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimación] (puntos)</strong></td>
      <td>Especifique la estimación del artículo. Si su equipo ágil está configurado para estimar los artículos en puntos, de forma predeterminada 1 punto es igual a 8 horas. Las estimaciones se añaden como [!UICONTROL Horario planificado] en el artículo.<br>Por ejemplo, si calcula un artículo como 3 puntos, el comportamiento predeterminado es agregar 24 horas planificadas al artículo.<br>Si un artículo contiene subtareas, recuerde que las estimaciones combinadas para todas las subtareas determinan la estimación del artículo principal. Para obtener más información, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Agregue una subtarea a un artículo existente en la tarjeta [!UICONTROL Scrum]</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Proyecto principal]</strong></td>
      <td>Empiece a escribir el nombre del proyecto al que se asociará este artículo.<br>De forma predeterminada, el color del artículo se muestra con el mismo color que otros artículos de este proyecto.<br>El estado del proyecto debe establecerse en [!UICONTROL Current]. Si el estado del proyecto es distinto de [!UICONTROL Actual], no se muestra en el menú desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarea Principal]</strong></td>
      <td>Después de elegir un proyecto principal, tiene la opción de elegir una tarea principal. Cuando selecciona una tarea principal, el artículo se crea como una subtarea de la tarea principal en el proyecto que ha seleccionado.<br>Empiece a escribir el nombre de la tarea principal para el artículo y, a continuación, haga clic en él cuando aparezca en la lista desplegable.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Forms personalizado]</strong></td>
      <td>Seleccione los formularios personalizados que desee agregar al artículo.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Guardar artículo]**.
