---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Agregar una subtarea a un artículo existente en el panel Anular
description: Cuando cree subtareas para artículos existentes, tenga en cuenta la configuración del modo de finalización para el proyecto, ya que esto afecta a la forma en que se actualizan los artículos.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Agregue una subtarea a un artículo existente en el [!UICONTROL Anulación] tablero

Al crear subtareas para artículos existentes, tenga en cuenta lo siguiente:

**Cuando la variable [!UICONTROL Modo de finalización] la configuración del proyecto se establece en [!UICONTROL Manual]:**

* Mover un artículo principal con subtareas a [!UICONTROL Completar] actualiza el artículo principal al 100 % y la variable [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas no se actualizan.
* Para actualizar el [!UICONTROL Porcentaje completado] para el artículo, debe actualizarlo desde el [!UICONTROL Historias] o desde la pestaña [!UICONTROL Detalles] del objeto.

**Cuando la variable [!UICONTROL Modo de finalización] la configuración del proyecto se establece en [!UICONTROL Automático]**:

* Mover un artículo principal con subtareas a [!UICONTROL Completar] actualiza el artículo principal al 100 % y la variable [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas también se actualizan al 100% y la variable [!UICONTROL Estado] se actualiza a [!UICONTROL Completar].
* Para actualizar el [!UICONTROL Porcentaje completado] para el artículo, debe actualizar el [!UICONTROL Porcentaje completado] para cualquier subtarea. La variable [!UICONTROL Porcentaje completado] para el artículo se calcula en función de la variable [!UICONTROL Porcentaje completado] de todas las subtareas.

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
   <td> <p>Acceso de [!UICONTROL Contribute] o [!UICONTROL Manage] a la tarea en la que se encuentra la subtarea</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Agregar una subtarea a un artículo existente en el panel Anular

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya a la iteración ágil o al proyecto que contiene el artículo en el que desea agregar una subtarea. Para obtener información sobre cómo navegar a una iteración, consulte [Ver una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Vaya al mosaico del artículo en el panel del artículo en el que desea agregar una subtarea.
1. Haga clic en **[!UICONTROL Agregar subtarea]** en la tarjeta del artículo principal para crear una subtarea del artículo.

   ![Agregar subtarea](assets/agile-story-addsubtask-NWE.png)

   O

   Haga clic en **[!UICONTROL Agregar subtarea]** en un mosaico de subtarea para crear una subtarea a la subtarea.

   [!DNL Workfront] admite niveles infinitos de subtareas, pero solo se muestran dos niveles (subtareas de subtareas) en el tablero de artículos ágil.

   ![Agregar subtarea](assets/agile-story-addsubtask2-NWE.png)

   Al añadir una subtarea a un artículo que actualmente no tiene una vista panorámica, la tarea principal se promociona a la función [!UICONTROL Artículo principal] y la subtarea se desplaza dentro de swimlane.

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
      <td role="rowheader"><strong>[!UICONTROL Estimación]</strong></td>
      <td>Especifique la estimación de la subtarea.<br><p>Tenga en cuenta lo siguiente al crear estimaciones:</p>
       <ul>
        <li>Si su equipo ágil está configurado para estimar los artículos en puntos, de forma predeterminada 1 punto es igual a 8 horas. Las estimaciones se añaden como [!UICONTROL Horario planificado] en el artículo.</li>
        <li>Las estimaciones combinadas para todas las subtareas determinan la estimación del artículo principal. Para obtener más información, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Actualizar el estado de los artículos y las subtareas en el panel Anulación</a>.</li>
        <li>Cuando se crea una nueva subtarea, el campo [!UICONTROL Estimate] ya está establecido. Si restablece la estimación en la subtarea, restablece la estimación en el artículo principal (porque el artículo principal es la suma de todas sus subtareas).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Horario planificado]</strong></td>
      <td> (Disponible solo en proyectos) Especifique el número de horas planificadas para la tarea.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>Empiece a escribir el nombre del equipo al que desea asignar la subtarea y, a continuación, haga clic en él cuando aparezca en la lista desplegable.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Crear]**.
