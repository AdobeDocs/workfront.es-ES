---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usar banderas en historias en el tablero Kanban
description: En el [!DNL Kanban] tablero, los indicadores proporcionan una indicación visual de cuándo un artículo está listo para pasar al siguiente estado. Esto permite a los equipos de Kanban usar un enfoque "pull" en lugar de un enfoque "push" al mover historias entre estados.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Use indicadores en los artículos del [!UICONTROL Kanban] tablero

En el [!DNL Kanban] tablero, los indicadores proporcionan una indicación visual de cuándo un artículo está listo para pasar al siguiente estado. Esto habilita [!UICONTROL Kanban] Los equipos utilizan un enfoque &quot;pull&quot; en lugar de un enfoque &quot;push&quot; al mover artículos entre estados.

**Ejemplo:** Consideremos el siguiente ejemplo de un equipo que utiliza un enfoque &quot;pull&quot;: Olivia, la diseñadora gráfica del equipo, finaliza su trabajo y luego marca la historia como &quot;[!UICONTROL Listo para extraer].&quot; Esta bandera proporciona una indicación visual a Tony, el redactor del equipo, de que la historia está listo para que pase al siguiente estado. Tony luego mueve la historia al siguiente estado cuando está listo para empezar a trabajar en ella.

Tenga en cuenta lo siguiente al usar indicadores en artículos:

* Los indicadores no son un estado, sino una indicación visual de que el artículo está listo para que otro miembro del equipo lo mueva al siguiente estado.
* Los indicadores no aparecen en ninguna tarjeta de artículo que se encuentre en la sección [!UICONTROL Retraso] o en la [!UICONTROL Completar] (o en cualquier columna donde el estado de la columna sea igual a [!UICONTROL Completar]).

   Para obtener más información sobre los estados de artículo, consulte [Usar banderas en historias en el tablero Kanban](#updating-the-status-of-stories-and-subtasks)

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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Use indicadores en los artículos del [!UICONTROL Kanban] tablero

Para cambiar una bandera en un artículo:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png)y, a continuación, seleccione una nueva [!UICONTROL Kanban] del menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya a la [!UICONTROL Kanban] tablero en el que desea cambiar un indicador de un artículo.
1. Expanda el mosaico del artículo para ver el indicador.\
   El indicador se establece en **[!UICONTROL On Track]** para cada artículo de forma predeterminada.\
   ![Tarjeta kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Haga clic en el indicador actual y, a continuación, seleccione entre las siguientes opciones de indicador:

   * **[!UICONTROL On Track]:** El artículo se encuentra en el estado adecuado y no es necesario realizar ninguna acción en este momento.\

      Esta es la bandera predeterminada para cada artículo del panel Kanban.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Está bloqueado]:** El artículo no puede continuar con el siguiente estado. Cuando este indicador se establece en un artículo, el artículo no se cuenta hacia el límite de WIP. (Para obtener más información sobre los límites de WIP, consulte el artículo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Listo para extraer]:** El artículo está listo para que otro miembro del equipo lo mueva al siguiente estado.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
