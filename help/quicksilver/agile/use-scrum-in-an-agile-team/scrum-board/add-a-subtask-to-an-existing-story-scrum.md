---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Agregar una subtarea a una historia existente en el panel de exploración
description: Cuando cree subtareas para artículos existentes, tenga en cuenta la configuración del modo de finalización para el proyecto, ya que esto afecta a la forma en que se actualizan los artículos.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Agregar una subtarea a una historia existente en el tablero [!UICONTROL Scrum]

Al crear subtareas para artículos existentes, tenga en cuenta lo siguiente:

**Cuando la configuración de [!UICONTROL Modo de finalización] del proyecto está establecida en [!UICONTROL Manual]:**

* Al mover una historia principal con subtareas a [!UICONTROL Completar], se actualiza la historia principal al 100% y el [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas no se actualizan.
* Para actualizar el [!UICONTROL Porcentaje completado] de la historia, debe actualizarlo desde la ficha [!UICONTROL Historias] o desde la página [!UICONTROL Detalles] del objeto.

**Cuando la configuración de [!UICONTROL Modo de finalización] del proyecto está establecida en [!UICONTROL Automático]**:

* Al mover una historia principal con subtareas a [!UICONTROL Completar], se actualiza la historia principal al 100% y el [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas también se actualizan al 100% y [!UICONTROL Estado] se actualiza a [!UICONTROL Completado].
* Para actualizar el [!UICONTROL Porcentaje completado] de la historia, debe actualizar el [!UICONTROL Porcentaje completado] para cualquier subtarea. El [!UICONTROL porcentaje completado] para la historia se calcula en función del [!UICONTROL porcentaje completado] de todas las subtareas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p> 
   o
   <p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Acceso de [!UICONTROL Contribute] o [!UICONTROL Manage] a la tarea en la que se encuentra la subtarea </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar una subtarea a un artículo existente en el panel de exploración

{{step1-to-team}}

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya a la iteración Agile o al proyecto que contiene el artículo donde desea agregar una subtarea. Para obtener información sobre cómo navegar a una iteración, vea [Ver una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Vaya al mosaico de artículo del guion gráfico donde desee agregar una subtarea.
1. Haga clic en **[!UICONTROL Agregar subtarea]** en la tarjeta de historia principal para crear una subtarea para la historia.

   ![Agregar subtarea](assets/agile-story-addsubtask-NWE.png)

   O

   Haga clic en **[!UICONTROL Agregar subtarea]** en un mosaico de subtarea para crear una subtarea para la subtarea.

   [!DNL Workfront] admite infinitos niveles de subtareas, pero sólo se muestran dos niveles (subtareas de subtareas) en el panel de historias Agile.

   ![Agregar subtarea](assets/agile-story-addsubtask2-NWE.png)

   Al agregar una subtarea a una historia que actualmente no tiene una pista de natación, la tarea principal se promociona a la columna [!UICONTROL Historia principal] y la subtarea se mueve dentro de la pista de natación.

1. Especifique la siguiente información:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nombre de subtarea]</strong></td>
      <td> Especifique un nombre para la subtarea.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong></td>
      <td>Especifique una descripción para la subtarea.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimar]</strong></td>
      <td>Especifique la estimación para la subtarea.<br><p>Tenga en cuenta lo siguiente al crear estimaciones:</p>
       <ul>
        <li>Si su equipo Agile está configurado para estimar las historias en puntos, por defecto 1 punto es igual a 8 horas. Las estimaciones se agregan como [!UICONTROL Horas planificadas] en la historia.</li>
        <li>Las estimaciones combinadas para todas las subtareas determinan la estimación del artículo principal. Para obtener más información, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Actualizar el estado de las historias y subtareas en el panel de exploración</a>.</li>
        <li>Cuando se crea una nueva subtarea, el campo [!UICONTROL Estimate] ya está establecido. Si restablece la estimación en la subtarea, restablece la estimación en el artículo principal (porque el artículo principal es la suma de todas sus subtareas).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Horas planificadas]</strong></td>
      <td> (Disponible solo en proyectos) Especifique el número de horas planificadas para la tarea.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Asignación]</strong></td>
      <td>Empiece escribiendo el nombre del equipo al que desea asignar la subtarea y, a continuación, haga clic en él cuando aparezca en la lista desplegable.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Crear]**.
