---
product-area: agile-and-teams
navigation-topic: burndown
title: Usar un horario de equipo alternativo para los gráficos de evolución
description: Los horarios definidos en  [!DNL Adobe Workfront]  afectan al gráfico de evolución al excluir los días libres (fines de semana y festivos) de la evolución.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Usar un horario de equipo alternativo para los gráficos de evolución

Los horarios definidos en [!DNL Adobe Workfront] afectan el gráfico de evolución al excluir los días libres (fines de semana y festivos) de la evolución.

De forma predeterminada, el gráfico de evolución utiliza la programación predeterminada. Además del horario predeterminado, los equipos de Agile pueden elegir utilizar también un horario alternativo para incorporar días no laborables específicos del equipo. Esta programación alternativa se refleja en el gráfico de evolución de cualquier iteración asignada al equipo. La programación alternativa solo afecta al gráfico de evolución. (Para obtener más información acerca de la programación predeterminada, así como la forma en que el administrador de [!DNL Workfront] puede crear una programación específica del equipo, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

El gráfico de evolución no tiene en cuenta los días parciales. Por ejemplo, si su equipo trabaja 4 horas cada viernes, se representa como un día completo en el gráfico de evolución.

Para obtener más información sobre el uso del gráfico de evolución, consulte la [descripción general del gráfico de evolución Agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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

## Usar un horario de equipo alternativo para los gráficos de evolución

1. Asegúrese de que el administrador de [!DNL Workfront] ya ha creado la programación alternativa, tal como se describe en [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo Agile que desee administrar.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.

1. En la sección **[!UICONTROL Agile]**, en el área **[!UICONTROL Schedule]**, seleccione la nueva programación en el menú desplegable.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
