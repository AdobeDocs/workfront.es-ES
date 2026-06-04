---
product-area: agile-and-teams
navigation-topic: burndown
title: Usar un horario de equipo alternativo para los gráficos de evolución
description: Los horarios definidos en  [!DNL Adobe Workfront]  afectan al gráfico de evolución al excluir los días libres (fines de semana y festivos) de la evolución.
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/BWnnytUMaoygpGpDdjQ5dmdBZrR1IWAu7onkwVizvUc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 29%

---

# Usar un horario de equipo alternativo para los gráficos de evolución

Los horarios definidos en [!DNL Adobe Workfront] afectan el gráfico de evolución al excluir los días libres (fines de semana y festivos) de la evolución.

De forma predeterminada, el gráfico de evolución utiliza la programación predeterminada. Además del horario predeterminado, los equipos de Agile pueden elegir utilizar también un horario alternativo para incorporar días no laborables específicos del equipo. Esta programación alternativa se refleja en el gráfico de evolución de cualquier iteración asignada al equipo. La programación alternativa solo afecta al gráfico de evolución. (Para obtener más información acerca de la programación predeterminada, así como la forma en que el administrador de [!DNL Workfront] puede crear una programación específica del equipo, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

El gráfico de evolución no tiene en cuenta los días parciales. Por ejemplo, si su equipo trabaja 4 horas cada viernes, se representa como un día completo en el gráfico de evolución.

Para obtener más información sobre el uso del gráfico de evolución, consulte la [descripción general del gráfico de evolución Agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar un horario de equipo alternativo para los gráficos de evolución

1. Asegúrese de que el administrador de [!DNL Workfront] ya ha creado la programación alternativa, tal como se describe en [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo de Agile que desee gestionar.
1. Haga clic en el menú **[!UICONTROL Más]** y, a continuación, seleccione **[!UICONTROL Editar]**.

1. En la sección **[!UICONTROL Agile]**, en el área **[!UICONTROL Schedule]**, seleccione la nueva programación en el menú desplegable.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
