---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Categorizar artículos por color en el tablero Anulación
description: La asociación de color predeterminada de los artículos de tablero de Anulación varía en función de si el tablero de artículos se encuentra en una iteración o en un proyecto.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Categorizar artículos por color en la variable [!UICONTROL Anulación] tablero

## Cambiar la asociación de color predeterminada de los artículos

La asociación de color predeterminada de los artículos varía en función de si el tablero de artículos se encuentra en una iteración o en un proyecto:

* **[!UICONTROL Iteración]**: En una iteración, los mosaicos del tablero de historia están codificados por colores según el proyecto al que esté asociado el artículo. (A cada proyecto se le asigna arbitrariamente un color en el tablero de artículos). Puede cambiar este comportamiento predeterminado para cada equipo ágil. Los colores de los artículos ágiles de una iteración se pueden asociar al proyecto (predeterminado), a la prioridad del artículo, al propietario o a la forma libre. Para obtener más información, consulte [Configurar cómo se utilizan los indicadores de color para los artículos en el tablero de artículos ágil](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) en el artículo [Configurar la anulación](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Proyecto]**: En un proyecto, todas las subtareas coinciden con el color de la tarea principal, de modo que los colores de todas las historias en cualquier espacio en blanco determinado sean los mismos. Los colores se asignan aleatoriamente a tareas cuando se crean si la tarea no tiene ninguna subtarea o no tiene una tarea principal. Puede cambiar este comportamiento predeterminado modificando la vista ágil. Los colores de artículos ágiles de un proyecto se pueden asociar al artículo principal (predeterminado), a la prioridad del artículo, al propietario o a la forma libre. Para obtener más información, consulte [Crear o personalizar un [!UICONTROL Águila] ver](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) en [Información general sobre vistas en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Cambiar el color de los artículos al utilizar el formato libre

Si la configuración del equipo ágil se ha configurado para que la variable [!UICONTROL Asociar color de tarjeta a] está configurada en [!UICONTROL Forma libre], los usuarios pueden cambiar manualmente el color de los mosaicos de artículos individuales. Esto puede resultar útil para comunicar otros tipos de información que son importantes para el equipo o la organización:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica, o seleccione **[!UICONTROL Iteración actual]**.
1. Pase el ratón sobre el banner de color que aparece en la parte superior del mosaico de la historia.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Haga clic en **[!UICONTROL Cambiar color]** y, a continuación, seleccione el color que desee.

   ![](assets/agile-story-color2-nwe-350x138.png)
