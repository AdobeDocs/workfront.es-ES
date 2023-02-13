---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Administrar artículos y problemas en el tablero Anulación
description: Puede mover un artículo o un número del panel Anulación a otra iteración o al acumulado, o eliminarlo del panel Anulación. Cuando elimina un artículo o problema, este se mueve a la Papelera de reciclaje durante 30 días y solo puede recuperarlo el administrador del sistema.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Administrar artículos y problemas en [!UICONTROL Anulación] tablero

Puede mover un artículo o un número desde el [!UICONTROL Anulación] a otra iteración o al trabajo pendiente, o elimínelo de la [!UICONTROL Anulación] tablero. Cuando elimina un artículo o problema, este se mueve a la Papelera de reciclaje durante 30 días y solo puede recuperarlo el administrador del sistema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Acceso de [!UICONTROL Administrar] a la tarea o problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Mover artículo o problema desde el [!UICONTROL Anulación] tablero

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png)y, a continuación, seleccione un equipo Anular en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica, o seleccione **[!UICONTROL Iteración actual]**.
1. Haga clic en el **[!UICONTROL Más]** en el artículo o problema y seleccione **[!UICONTROL Mover a]**.

   ![Eliminar o mover un artículo del tablero Anulación](assets/scrum-delete-move-story.png)

1. En el mensaje de confirmación, elija:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Otra iteración]</strong></td>
        <td>Seleccione para mover el elemento a otra iteración y, a continuación, elija a qué iteración se moverá el artículo o el problema. Si no se definen iteraciones futuras, no se puede mover el elemento.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Seleccione para mover el artículo o el problema al trabajo acumulado del equipo.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >El elemento de trabajo [!UICONTROL Fecha de inicio planeada] y [!UICONTROL Fecha de finalización planeada] se ven afectados por una configuración en la variable [!UICONTROL Editar equipo] página. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar la anulación](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover]**.

## Eliminar artículo o número del [!UICONTROL Anulación] tablero

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png)y, a continuación, seleccione un equipo Anular en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica, o seleccione **[!UICONTROL Iteración actual]**.
1. Haga clic en el **[!UICONTROL Más]** en el artículo o problema y seleccione **[!UICONTROL Eliminar artículo]** o **[!UICONTROL Eliminar problema]**.

   ![Eliminar o mover un artículo del tablero Anulación](assets/scrum-delete-move-story.png)

1. En el mensaje de confirmación, haga clic en **[!UICONTROL Sí, elimínelo]**.
