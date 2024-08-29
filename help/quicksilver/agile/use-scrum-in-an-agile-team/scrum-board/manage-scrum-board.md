---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Administrar historias y problemas en el panel de exploración
description: Puede mover una historia o un problema del panel de exploración a otra iteración o al registro de pendientes, o eliminarlo del panel de exploración. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Administrar historias y problemas en el tablero [!UICONTROL Scrum]

Puede mover una historia o un problema del tablero [!UICONTROL Scrum] a otra iteración o al registro de pendientes, o eliminarlo del tablero [!UICONTROL Scrum]. Cuando elimina una historia o un problema, se mueve a la papelera de reciclaje durante 30 días y solo el administrador del sistema puede recuperarlo.

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
   <td>Acceso de [!UICONTROL Manage] a la tarea o al problema </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
        <td><strong>[!UICONTROL Registro de pendientes]</strong></td>
        <td>Seleccione para mover la historia o el problema al registro de asuntos pendientes del equipo.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >El elemento de trabajo [!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fecha planificada de finalización] se ven afectados por una configuración en la página [!UICONTROL Editar equipo]. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover]**.

## Eliminar una historia o un problema del tablero [!UICONTROL Scrum]

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.
1. Haga clic en el icono **[!UICONTROL Más]** del artículo o problema y seleccione **[!UICONTROL Eliminar artículo]** o **[!UICONTROL Eliminar problema]**.

   ![Eliminar o mover historia del panel de exploración](assets/scrum-delete-move-story.png)

1. En el mensaje de confirmación, haga clic en **[!UICONTROL Sí, eliminarlo]**.
