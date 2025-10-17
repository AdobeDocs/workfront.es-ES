---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usar indicadores en historias en el Panel Kanban
description: En el tablero  [!DNL Kanban] , los indicadores proporcionan una indicación visual de cuándo una historia está lista para moverse al siguiente estado. Esto permite a los equipos de Kanban utilizar un enfoque de “extracción” en lugar de “inserción” al mover historias entre estados.
author: Jenny
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 85%

---

# Usar indicadores en las historias del tablero [!UICONTROL Kanban]

En el tablero [!DNL Kanban], los indicadores proporcionan una indicación visual de cuándo una historia está lista para moverse al siguiente estado. Esto permite a los equipos de [!UICONTROL Kanban] usar un enfoque de “extracción” en lugar de “inserción” al mover historias entre estados.

**Ejemplo:** Supongamos que un equipo usa un enfoque de “extracción”: Ana, la diseñadora gráfica del equipo, finaliza su trabajo y, a continuación, establece el indicador de historia en “[!UICONTROL Listo para extraer]”. Este indicador proporciona una indicación visual a Jorge, el redactor del equipo, de que la historia está lista para moverse al siguiente estado. A continuación, Jorge moverá la historia al siguiente estado cuando esté listo para comenzar a trabajar en ella.

Tenga en cuenta lo siguiente al utilizar indicadores en historias:

* Los indicadores no son un estado, sino una indicación visual de que la historia está lista para que otro integrante del equipo la mueva al siguiente estado.
* Los indicadores no aparecen en ninguna tarjeta de historia que esté en la columna [!UICONTROL Backlog] ni en la columna [!UICONTROL Complete] (ni en ninguna columna en la que el estado de la columna sea igual a [!UICONTROL Complete]).

  Para obtener más información sobre los estados de las historias, consulte [Usar indicadores en las historias del tablero Kanban](#updating-the-status-of-stories-and-subtasks)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar indicadores en las historias del tablero [!UICONTROL Kanban]

Para cambiar un indicador en una historia:

{{step1-to-team}}

1. (Opcional) Haga clic en el icono **[!UICONTROL Switch team]** ![Switch team](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo [!UICONTROL Kanban] en el menú desplegable o busque uno en la barra de búsqueda.

1. Vaya al tablero [!UICONTROL Kanban] donde desee cambiar un indicador en una historia.
1. Expanda el mosaico de la historia para ver el indicador.
De manera predeterminada, el indicador se establece en **[!UICONTROL On Track]** para cada historia.
   ![Kanban card](assets/agile-storycard-kanban-2021-350x308.png)

1. Haga clic en el indicador actual y, a continuación, seleccione una de las siguientes opciones de indicador:

   * **[!UICONTROL En seguimiento]:** La historia se encuentra en el estado apropiado y no es necesario realizar ninguna acción en este momento.

     Este es el indicador predeterminado de cada historia del tablero Kanban.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Is Blocked]:** la historia no puede pasar al siguiente estado. Cuando se establece este indicador en una historia, esta no cuenta para el límite de WIP. (Para obtener más información sobre los límites de WIP, consulte el artículo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)).

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Listo para extraer]:** La historia está lista para que otro miembro del equipo la mueva al siguiente estado.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
