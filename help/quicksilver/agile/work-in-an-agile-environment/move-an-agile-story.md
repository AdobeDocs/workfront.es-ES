---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover una historia de Agile
description: Puede mover una historia Agile a una iteración diferente (para equipos de Scrum) o al registro de pendientes (para equipos de Kanban y Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Mover una historia ágil

Puede mover una historia Agile a una iteración diferente (para equipos de Scrum) o al registro de pendientes (para equipos de Kanban y Scrum).

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

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover una historia de una iteración o panel Kanban al registro de pendientes

1. Vaya a la iteración o al panel Kanban que contiene el artículo que desea mover al registro de pendientes.
1. Haga clic en el encabezado de la iteración en la parte superior de la página.
1. En la ficha **[!UICONTROL Historias]**, seleccione las historias que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.

   Se muestra el cuadro de diálogo **[!UICONTROL Mover historia]**.

   ![Cuadro de diálogo Mover historia](assets/iteration-story-move.png)

1. Seleccione el registro de pendientes de **team_name**.
En el ejemplo anterior, el nombre del equipo es **Marketing**.

1. Haga clic en **[!UICONTROL Mover historia]**.

## Mover una historia a otra iteración

Puede mover una historia a una iteración diferente para su equipo de Scrum.

>[!NOTE]
>
>La opción **[!UICONTROL Mover a]** no está disponible para las historias principales en una iteración. Sólo puede mover subtareas a otra iteración.

1. Vaya a la iteración que contiene el artículo que desea mover.
1. Haga clic en el encabezado de la iteración en la parte superior de la página.
1. En la ficha **[!UICONTROL Historias]**, seleccione las historias que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.

   Se muestra el cuadro de diálogo **[!UICONTROL Mover historia]**.

   ![Cuadro de diálogo Mover historia](assets/iteration-story-move.png)

1. Seleccione **[!UICONTROL Otra iteración]** y, a continuación, en el menú desplegable, seleccione la iteración a la que desea mover la historia.

   >[!NOTE]
   >
   >El elemento de trabajo [!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fecha planificada de finalización] se ven afectados por una configuración en la página [!UICONTROL Editar equipo]. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) en el artículo [Configurar Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover historia]**.
