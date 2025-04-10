---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover una historia de Agile
description: Puede mover una historia Agile a una iteración diferente (para equipos de Scrum) o al registro de asuntos pendientes (para equipos de Kanban y Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 68aafe63ff8b60a542ed9dd0900b3742c26a1e4f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 75%

---

# Mover una historia Agile

Puede mover una historia Agile a una iteración diferente (para equipos de Scrum) o al registro de asuntos pendientes (para equipos de Kanban y Scrum).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>Acceso de [!UICONTROL Manage] a la historia</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover una historia de una iteración o tablero Kanban al registro de asuntos pendientes

1. Vaya a la iteración o al tablero Kanban que contiene la historia que desea mover al registro de asuntos pendientes.
1. Haga clic en el encabezado de la iteración en la parte superior de la página.
1. En la ficha **[!UICONTROL Historias]**, seleccione las historias que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**. Se muestra el cuadro de diálogo **[!UICONTROL Mover a]**.

   ![Cuadro de diálogo Mover historia](assets/iteration-story-move.png)

1. Seleccione el registro de pendientes de **team_name**. En el ejemplo anterior, el nombre del equipo es **Marketing**.

1. Haga clic en **[!UICONTROL Mover]**.

## Mover una historia a una iteración diferente

Puede mover una historia a una iteración diferente para su equipo de Scrum si es administrador del sistema o miembro del equipo al que está asociada la iteración.

>[!NOTE]
>
> La opción **[!UICONTROL Mover a]** no está disponible para las historias principales en una iteración. Solo puede mover subtareas a otra iteración.


1. Vaya a la iteración que contiene la historia que desea mover.
1. Haga clic en el encabezado de la iteración en la parte superior de la página.
1. En la ficha **[!UICONTROL Historias]**, seleccione las historias que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**. Se muestra el cuadro de diálogo **[!UICONTROL Mover a]**.

   ![Cuadro de diálogo Mover historia](assets/iteration-story-move.png)

1. Seleccione **[!UICONTROL Otra Iteración]**.
1. En el menú desplegable que aparece, seleccione la iteración a la que desea mover el artículo.

   >[!NOTE]
   >
   >Los elementos de trabajo [!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fecha planificada de finalización] se ven afectados por un ajuste de la página [!UICONTROL Editar equipo]. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) en el artículo [Configurar Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover]**.
