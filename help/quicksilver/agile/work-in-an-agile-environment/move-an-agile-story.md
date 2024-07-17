---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover una historia ágil
description: Puede mover una historia Agile a una iteración diferente (para equipos de Scrum) o al registro de pendientes (para equipos de Kanban y Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Mover una historia ágil

Puede mover una historia Agile a una iteración diferente (para equipos de Scrum) o al registro de pendientes (para equipos de Kanban y Scrum).

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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] a la historia</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Mover una historia de una iteración o panel Kanban al registro de pendientes

1. Vaya a la iteración o al panel Kanban que contiene el artículo que desea mover al registro de pendientes.
1. Haga clic en el encabezado de la iteración en la parte superior de la página.
1. En la ficha **[!UICONTROL Historias]**, seleccione las historias que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.

   Se muestra el cuadro de diálogo **[!UICONTROL Mover historia]**.

   ![Cuadro de diálogo Mover historia](assets/iteration-story-move.png)

1. Seleccione el registro de pendientes de *team_name*.\
   En el ejemplo anterior, el nombre del equipo es&#x200B; **Marketing.**

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
   >El elemento de trabajo [!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fecha planificada de finalización] se ven afectados por una configuración en la página [!UICONTROL Editar equipo]. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover historia]**.
