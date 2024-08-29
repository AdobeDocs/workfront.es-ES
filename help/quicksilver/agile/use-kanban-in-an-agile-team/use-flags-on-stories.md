---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usar indicadores en historias en el Panel Kanban
description: En el tablero  [!DNL Kanban] , los indicadores proporcionan una indicación visual de cuándo una historia está lista para pasar al siguiente estado. Esto permite a los equipos de Kanban utilizar un enfoque de "extracción" en lugar de "inserción" al mover historias entre estados.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Usar marcas en las historias del tablero [!UICONTROL Kanban]

En el tablero [!DNL Kanban], los indicadores proporcionan una indicación visual de cuándo una historia está lista para pasar al siguiente estado. Esto permite a los equipos de [!UICONTROL Kanban] usar un enfoque de &quot;extracción&quot; en lugar de un enfoque de &quot;inserción&quot; al mover historias entre estados.

**Ejemplo:** Considere el siguiente ejemplo de un equipo que usa un enfoque de &quot;extracción&quot;: Olivia, la diseñadora gráfica del equipo, finaliza su trabajo y, a continuación, establece la marca de historia como &quot;[!UICONTROL Listo para extracción]&quot;. Esta bandera proporciona una indicación visual a Tony, el redactor del equipo, de que la historia está lista para que pase al siguiente estado. A continuación, Tony pasa la historia al siguiente estado cuando esté listo para comenzar a trabajar en ella.

Tenga en cuenta lo siguiente al utilizar indicadores en historias:

* Las marcas no son un estado, sino una indicación visual de que la historia está lista para ser trasladada al siguiente estado por otro miembro del equipo.
* Los indicadores no aparecen en ninguna tarjeta de historia que esté en la columna [!UICONTROL Registro de pendientes] ni en la columna [!UICONTROL Completar] (ni en ninguna columna en la que el estado de la columna sea igual a [!UICONTROL Completar]).

  Para obtener más información sobre los estados de los artículos, consulte [Usar indicadores en los artículos del Panel Kanban](#updating-the-status-of-stories-and-subtasks)

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
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar marcas en las historias del tablero [!UICONTROL Kanban]

Para cambiar un indicador en una historia:

{{step1-to-team}}

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo [!UICONTROL Kanban] en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya al tablero [!UICONTROL Kanban] donde desee cambiar un marcador de una historia.
1. Expanda el mosaico de la historia para ver el indicador.
De manera predeterminada, el indicador se establece en **[!UICONTROL On Track]** para cada artículo.
   ![Tarjeta Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Haga clic en el indicador actual y, a continuación, seleccione una de las siguientes opciones de indicador:

   * **[!UICONTROL En seguimiento]:** La historia se encuentra en el estado apropiado y no es necesario realizar ninguna acción en este momento.

     Este es el indicador predeterminado para cada artículo del Panel Kanban.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Está bloqueado]:** La historia no puede pasar al siguiente estado. Cuando este indicador se establece en un artículo, este no se cuenta para el límite de trabajo en curso. (Para obtener más información sobre los límites de WIP, consulte el artículo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)).

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Listo para extraer]:** La historia está lista para que otro miembro del equipo la mueva al siguiente estado.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
