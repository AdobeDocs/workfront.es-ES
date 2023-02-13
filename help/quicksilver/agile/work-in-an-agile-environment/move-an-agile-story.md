---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Mover una historia ágil
description: Puede mover una historia ágil a una iteración diferente (para equipos de depuración) o a la pendiente (para equipos de Kanban y Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Mover una historia ágil

Puede mover una historia ágil a una iteración diferente (para equipos de depuración) o a la pendiente (para equipos de Kanban y Scrum).

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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Administrar] al artículo</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Mover un artículo de una iteración o panel kanban al registro

1. Vaya a la iteración o el tablero Kanban que contiene el artículo que desea mover al registro pendiente.
1. Haga clic en el encabezado de iteración en la parte superior de la página.
1. En el **[!UICONTROL Historias]** , seleccione los artículos que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.

   La variable **[!UICONTROL Mover artículo]** se muestra.

   ![Cuadro de diálogo Mover artículo](assets/iteration-story-move.png)

1. Select *nombre_equipo* El retraso de .\
   En el ejemplo anterior, el nombre del equipo es &#x200B; **Marketing.**

1. Haga clic en **[!UICONTROL Mover artículo]**.

## Mover un artículo a otra iteración

Puede mover una historia a otra iteración para su equipo de Anulación de errores.

>[!NOTE]
>
>La variable **[!UICONTROL Mover a]** no está disponible para artículos principales en una iteración. Solo puede mover subtareas a otra iteración.

1. Vaya a la iteración que contiene el artículo que desea mover.
1. Haga clic en el encabezado de iteración en la parte superior de la página.
1. En el **[!UICONTROL Historias]** , seleccione los artículos que desee mover.
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Mover a]**.

   La variable **[!UICONTROL Mover artículo]** se muestra.

   ![Cuadro de diálogo Mover artículo](assets/iteration-story-move.png)

1. Select **[!UICONTROL Otra iteración]** y, a continuación, en el menú desplegable, seleccione la iteración donde desee mover el artículo.

   >[!NOTE]
   >
   >El elemento de trabajo [!UICONTROL Fecha de inicio planeada] y [!UICONTROL Fecha de finalización planeada] se ven afectados por una configuración en la variable [!UICONTROL Editar equipo] página. Para obtener más información, consulte la sección [[!UICONTROL Configurar] cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar la anulación](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Haga clic en **[!UICONTROL Mover artículo]**.
