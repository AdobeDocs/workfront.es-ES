---
product-area: agile-and-teams
navigation-topic: iterations
title: Crear una iteración
description: Las iteraciones son un componente clave para los equipos de Scrum Agile en la planificación de la capacidad de trabajo. [!DNL Adobe Workfront] permite a los equipos inteligentes gestionar su trabajo creando varias iteraciones para adaptarse a las necesidades del equipo.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 0%

---

# Crear una iteración

Las iteraciones son un componente clave para los equipos de Scrum Agile en la planificación de la capacidad de trabajo. [!DNL Adobe Workfront] permite a los equipos inteligentes gestionar su trabajo creando varias iteraciones para adaptarse a las necesidades del equipo.

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
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Añadir una iteración

Utilice la variable [!UICONTROL Agregar iteración] para crear rápidamente una iteración y añadir tareas y problemas más tarde.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En el **[!UICONTROL Iteraciones]** , haga clic en **[!UICONTROL Agregar iteración]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. Especifique lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nombre de iteración]</strong></td> 
      <td>Introduzca el nombre de la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>Añada los objetivos que tenga para la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de inicio]</strong></td> 
      <td>Introduzca la fecha en la que debe comenzar la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de finalización]</strong></td> 
      <td><p>Introduzca la fecha en la que debe finalizar la iteración. [!DNL Workfront] recomienda establecer una fecha de finalización no superior a 4 semanas a partir de la fecha de inicio.</p><p>Sugerencia: Asegúrese de elegir un día laborable como fecha de finalización. El gráfico desplegable solo utiliza días laborables en sus cálculos.<br>De forma predeterminada, el gráfico desplegable utiliza la programación predeterminada para definir los días laborables (tal y como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>). O bien, para incorporar días no laborables específicos del equipo, los equipos ágiles pueden elegir utilizar una programación alternativa (como se describe en "Definición de una programación de equipo alternativa para gráficos de desglose" en <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo ágil</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Especifique la capacidad de la iteración. Este es el número de puntos o horas que su equipo puede realizar en la iteración. El número introducido debe ser igual o bueno que el número de puntos u horas desde la suma de todos los artículos de la iteración.<br>[!DNL Workfront] rellena previamente este campo con 50 capacidades de forma predeterminada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Especifique el porcentaje de enfoque del equipo. Si todos los miembros del equipo se concentraran completamente en esta iteración, el enfoque sería del 100%.<br>[!DNL Workfront] rellena previamente este campo con el 100 % de forma predeterminada. </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Submit]**. Ahora que ha creado una iteración, debe agregar artículos. Para obtener más información, consulte [Añadir artículos a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planificar una iteración en el [!UICONTROL Retraso] ficha

Utilice la variable [!UICONTROL Iteración del plan] para crear una iteración mediante tareas en el registro de trabajo pendiente.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Select **[!UICONTROL Retraso]** en el panel izquierdo. A continuación, haga clic en **[!UICONTROL Iteración del plan]**.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nombre de iteración]</strong></td> 
      <td>Especifique un nombre para la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de inicio]</strong></td> 
      <td> Especifique la fecha en la que debe comenzar la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de finalización]</strong> </td> 
      <td><p>Especifique la fecha en la que debe finalizar la iteración. [!DNL Workfront] recomienda establecer una fecha de finalización no superior a 4 semanas a partir de la fecha de inicio.</p><p>Sugerencia: Asegúrese de elegir un día laborable como fecha de finalización. El gráfico desplegable solo utiliza días laborables en sus cálculos.<br>De forma predeterminada, el gráfico desplegable utiliza la programación predeterminada para definir los días laborables (tal y como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>). O bien, para incorporar días no laborables específicos del equipo, los equipos ágiles pueden elegir utilizar una programación alternativa (como se describe en <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md" class="MCXref xref">Usar una programación de equipo alternativa para gráficos de desglose</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Especifique el porcentaje de enfoque del equipo. Si todos los miembros del equipo se concentraran completamente en esta iteración, el enfoque sería del 100%.<br>[!DNL Workfront] rellena previamente este campo con el valor promedio de las iteraciones anteriores del equipo. Si esta es la primera iteración del equipo, el valor de este campo es 0 de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Especifique la capacidad de la iteración. Este es el número de puntos o horas que su equipo puede realizar en la iteración. El número introducido debe ser igual o bueno que el número de puntos u horas desde la suma de todos los artículos de la iteración.<br>[!DNL Workfront] rellena previamente este campo con el valor promedio de las iteraciones anteriores del equipo. Si esta es la primera iteración del equipo, el valor de este campo es 0 de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Especifique un objetivo para la iteración. Este campo no es obligatorio.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Seleccione artículos para agregarlos a la iteración ahora o puede omitir este paso y agregar artículos a una iteración más adelante. Los artículos que están en la parte superior del atraso son de mayor prioridad. Las historias se resaltan en verde cuando se ajustan a su capacidad; se resaltan en rojo si no lo hacen.\
   Puede añadir tareas y problemas a una sola iteración:

   * **Para agregar tareas a la iteración:** En el **[!UICONTROL Retraso]** , asegúrese de que la **[!UICONTROL Historias]** está seleccionada (esta pestaña está seleccionada de forma predeterminada al ver el &quot;backlog&quot;). Seleccione los artículos que desee agregar a la iteración.\

      Cuando agrega tareas a una iteración, la fecha de inicio de la tarea se calcula tal como se describe en [[!UICONTROL Comprender] cómo se calculan las fechas de inicio de la tarea cuando se añaden a una iteración](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Para agregar problemas a la iteración:** En el **[!UICONTROL Retraso]** , haga clic en la pestaña **[!UICONTROL Problemas]** pestaña . Seleccione los problemas que desee añadir a la iteración.

1. Haga clic en **[!UICONTROL Guardar].**
Se crea la iteración.

1. (Opcional) Para agregar artículos a una iteración existente, consulte [Añadir artículos a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Comprender cómo se calculan las fechas de inicio de la tarea cuando se añaden a una iteración {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Cuando agrega una tarea como artículo a una iteración, la variable [!UICONTROL Debe finalizar en la tarea] para cada artículo se utiliza restricción. En la mayoría de los casos, la fecha de inicio prevista de la tarea se calcula en función de la fórmula siguiente:

[!UICONTROL Fecha de finalización de iteración] menos (-) [!UICONTROL Duración de la tarea] es igual a (=) [!UICONTROL Fecha de inicio planeada para la tarea]

La variable [!UICONTROL Fecha de finalización del proyecto] se utiliza en lugar de si la fecha de inicio del proyecto es posterior a la fecha de inicio de la iteración y la fecha de finalización del proyecto es posterior a la fecha de finalización de la iteración.

Puede configurar equipos de Anulación individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar la anulación](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
