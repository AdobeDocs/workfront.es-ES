---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Administrar historias y problemas en el panel de exploración
description: Puede mover una historia o un problema del panel de exploración a otra iteración o al registro de pendientes, o eliminarlo del panel de exploración. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.
author: Courtney
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ielfm99We9-fno0XOxp34XkWjtgLrmfCKhLx9kNAP8Q
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 471
ht-degree: 40%

---

# Administrar historias y problemas en el tablero [!UICONTROL Scrum]

Puede mover una historia o un problema del tablero [!UICONTROL Scrum] a otra iteración o al registro de pendientes, o eliminarlo del tablero [!UICONTROL Scrum]. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.

Para eliminar una tarea o un problema de la iteración sin eliminarlo ni enviarlo al registro de pendientes, vaya al proyecto y elimine el equipo de Agile de la columna de asignación. Esto elimina la tarea o el problema del panel de exploración, pero permanece en el proyecto.

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
   <td>Acceso de [!UICONTROL Manage] a la tarea o problema </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover una historia o un problema del tablero [!UICONTROL Scrum]

{{step1-to-team}}

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
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Seleccione para mover la historia o el problema al registro de asuntos pendientes del equipo.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Los elementos de trabajo [!UICONTROL Fecha de inicio planificada] y [!UICONTROL Fecha de finalización planificada] se ven afectados por un ajuste de la página [!UICONTROL Editar equipo]. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover]**.

## Eliminar una historia o un problema del tablero [!UICONTROL Scrum]

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.
1. Haga clic en el icono **[!UICONTROL Más]** del artículo o problema y seleccione **[!UICONTROL Eliminar artículo]** o **[!UICONTROL Eliminar problema]**.

   ![Eliminar o mover historia del panel de exploración](assets/scrum-delete-move-story.png)

1. En el mensaje de confirmación, haga clic en **[!UICONTROL Sí, eliminarlo]**.
