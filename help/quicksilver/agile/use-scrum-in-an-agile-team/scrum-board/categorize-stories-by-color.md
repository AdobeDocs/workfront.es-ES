---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Categorizar historias por color en el panel Scrum
description: La asociación de colores predeterminada de las historias del guion gráfico de Scrum difiere según si el guion gráfico se encuentra en una iteración o en un proyecto.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Categorizar historias por color en el tablero [!UICONTROL Scrum]

## Cambiar la asociación de colores predeterminada de las historias

La asociación de colores predeterminada de las historias difiere según si el guion gráfico se encuentra en una iteración o en un proyecto:

* **[!UICONTROL Iteración]**: en una iteración, los mosaicos del guion gráfico tienen un código de color según el proyecto con el que esté asociado el artículo. (A cada proyecto se le asigna arbitrariamente un color en el guion gráfico). Puede cambiar este comportamiento predeterminado para cada equipo Agile. Los colores de las historias Agile en una iteración pueden vincularse al proyecto (predeterminado), a la prioridad de la historia, al propietario o a la forma libre. Para obtener más información, consulte [Configurar cómo se usan los indicadores de color para las historias en el panel de historias Agile](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Proyecto]**: en un proyecto, todas las subtareas coinciden con el color de la tarea principal, de modo que los colores de todas las historias de cualquier carril de baño son iguales. Los colores se asignan aleatoriamente a las tareas cuando se crean si la tarea no tiene subtareas o no tiene una tarea principal. Puede cambiar este comportamiento predeterminado modificando la vista Agile. Los colores de las historias Agile de un proyecto se pueden asociar a la historia principal (predeterminada), la prioridad de la historia, el propietario o la forma libre. Para obtener más información, consulte [Crear o personalizar una vista de [!UICONTROL Agile]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) en [Información general de vistas en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Cambiar el color de las historias al usar la forma libre

Si la configuración del equipo Agile se ha configurado de modo que la opción [!UICONTROL Asociar color de tarjeta a] se establezca en [!UICONTROL Forma libre], los usuarios podrán cambiar manualmente el color de los mosaicos de artículos individuales. Esto puede resultar útil para comunicar otros tipos de información que son importantes para el equipo o la organización:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront, y luego haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.
1. Pase el ratón sobre el titular de color que hay en la parte superior del mosaico de la historia.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Haga clic en **[!UICONTROL Cambiar color]** y, a continuación, seleccione el color que desee.

   ![](assets/agile-story-color2-nwe-350x138.png)
