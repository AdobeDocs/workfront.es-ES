---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Administrar historias y problemas en el panel de exploración
description: Puede mover una historia o un problema del panel de exploración a otra iteración o al registro de pendientes, o eliminarlo del panel de exploración. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Administrar historias y problemas en el tablero [!UICONTROL Scrum]

Puede mover una historia o un problema del tablero [!UICONTROL Scrum] a otra iteración o al registro de pendientes, o eliminarlo del tablero [!UICONTROL Scrum]. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.

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
   <td> <p>[!UICONTROL Trabajo] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] a la tarea o al problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Mover historia o problema del tablero [!UICONTROL Scrum]

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y luego haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.
1. Haz clic en el icono **[!UICONTROL Más]** de la historia o el problema y selecciona **[!UICONTROL Mover a]**.

   ![Eliminar o mover historia del panel de exploración](assets/scrum-delete-move-story.png)

1. En el mensaje de confirmación, elija:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Otra iteración]</strong></td>
        <td>Seleccione para mover el elemento a otra iteración y, a continuación, elija a qué iteración se moverá la historia o el problema. Si no se definen iteraciones futuras, no se puede mover el elemento.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Registro de pendientes]</strong></td>
        <td>Seleccione para mover la historia o el problema al registro de asuntos pendientes del equipo.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >El elemento de trabajo [!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fecha planificada de finalización] se ven afectados por una configuración en la página [!UICONTROL Editar equipo]. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover]**.

## Eliminar historia o problema del tablero [!UICONTROL Scrum]

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y luego haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.
1. Haga clic en el icono **[!UICONTROL Más]** del artículo o problema y seleccione **[!UICONTROL Eliminar artículo]** o **[!UICONTROL Eliminar problema]**.

   ![Eliminar o mover historia del panel de exploración](assets/scrum-delete-move-story.png)

1. En el mensaje de confirmación, haga clic en **[!UICONTROL Sí, eliminarlo]**.
