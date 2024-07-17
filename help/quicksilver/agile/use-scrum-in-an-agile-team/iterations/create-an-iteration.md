---
product-area: agile-and-teams
navigation-topic: iterations
title: Creación de una iteración
description: Las iteraciones son un componente clave para los equipos de Scrum Agile a la hora de planificar la capacidad de trabajo. [!DNL Adobe Workfront] permite que los equipos de Scrum Agile administren su trabajo creando múltiples iteraciones para satisfacer las necesidades del equipo.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 0%

---

# Creación de una iteración

Las iteraciones son un componente clave para los equipos de Scrum Agile a la hora de planificar la capacidad de trabajo. [!DNL Adobe Workfront] permite que los equipos de Scrum Agile administren su trabajo creando múltiples iteraciones para satisfacer las necesidades del equipo.

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

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Añadir una iteración

Use la característica [!UICONTROL Agregar iteración] para crear rápidamente una iteración y agregar tareas y problemas más adelante.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y luego haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En la ficha **[!UICONTROL Iteraciones]**, haga clic en **[!UICONTROL Agregar iteración]**.\
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
      <td role="rowheader"><strong>[!UICONTROL Meta]</strong></td> 
      <td>Añada los objetivos que tenga para la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de inicio]</strong></td> 
      <td>Introduzca la fecha de inicio de la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de finalización]</strong></td> 
      <td><p>Introduzca la fecha en la que debe finalizar la iteración. [!DNL Workfront] recomienda establecer una fecha de finalización que no sea mayor a 4 semanas desde la fecha de inicio.</p><p>Sugerencia: Asegúrese de elegir un día laborable como fecha de finalización. El gráfico de evolución solo utiliza días laborables en sus cálculos.<br>De manera predeterminada, el gráfico de evolución utiliza la programación predeterminada para definir los días laborables (tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>). O, para incorporar días no laborables específicos del equipo, los equipos Agile pueden elegir usar un horario alternativo (como se describe en "Definición de un horario de equipo alternativo para gráficos de evolución" en <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo Agile</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Especifique la capacidad de la iteración. Es el número de puntos u horas que su equipo puede lograr en la iteración. El número que introduzca debe ser igual o mayor que el número de puntos u horas de la suma de todos los artículos de la iteración.<br>[!DNL Workfront] rellena previamente este campo con 50 de capacidad de forma predeterminada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Enfoque]</strong></td> 
      <td>Especifique el porcentaje de enfoque del equipo. Si todos los miembros del equipo se centran completamente en esta iteración, el enfoque sería del 100 %.<br>[!DNL Workfront] rellena previamente este campo con el 100% de forma predeterminada. </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Enviar]**. Ahora que ha creado una iteración, debe agregar historias. Para obtener más información, vea [Agregar historias a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planifique una iteración en la ficha [!UICONTROL Registro de pendientes]

Use la característica [!UICONTROL Planificar iteración] para crear una iteración con tareas en el registro de pendientes.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y luego haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![Cambiar de icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione **[!UICONTROL Registro de pendientes]** en el panel izquierdo. A continuación, haga clic en **[!UICONTROL Planificar iteración]**.

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
      <td><p>Especifique la fecha en la que debe finalizar la iteración. [!DNL Workfront] recomienda establecer una fecha de finalización que no sea mayor a 4 semanas desde la fecha de inicio.</p><p>Sugerencia: Asegúrese de elegir un día laborable como fecha de finalización. El gráfico de evolución solo utiliza días laborables en sus cálculos.<br>De manera predeterminada, el gráfico de evolución utiliza la programación predeterminada para definir los días laborables (tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>). O bien, para incorporar días no laborables específicos del equipo, los equipos Agile pueden elegir usar un horario alternativo (como se describe en <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Usar un horario de equipo alternativo para los gráficos de evolución</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Enfoque]</strong></td> 
      <td>Especifique el porcentaje de enfoque del equipo. Si todos los miembros del equipo se centran completamente en esta iteración, el enfoque sería del 100 %.<br>[!DNL Workfront] rellena previamente este campo con el valor promedio de las iteraciones anteriores del equipo. Si esta es la primera iteración del equipo, este valor de campo es 0 de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Especifique la capacidad de la iteración. Es el número de puntos u horas que su equipo puede lograr en la iteración. El número que introduzca debe ser igual o mayor que el número de puntos u horas de la suma de todos los artículos de la iteración.<br>[!DNL Workfront] rellena previamente este campo con el valor promedio de las iteraciones anteriores del equipo. Si esta es la primera iteración del equipo, este valor de campo es 0 de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Meta]</strong></td> 
      <td> Especifique un objetivo para la iteración. Este campo no es obligatorio.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Seleccione historias para agregarlas a la iteración ahora, o bien puede omitir este paso y agregar historias a una iteración más adelante. Las historias en la parte superior del registro de pendientes son de mayor prioridad. Las historias se resaltan en verde cuando caben en la capacidad; si no, se resaltan en rojo.\
   Puede agregar tareas y problemas a una sola iteración:

   * **Para agregar tareas a la iteración:** En la ficha **[!UICONTROL Registro de pendientes]**, asegúrese de que la ficha **[!UICONTROL Historias]** esté seleccionada (esta ficha está seleccionada de forma predeterminada al ver el registro de pendientes). Seleccione las historias que desee añadir a la iteración.\

     Cuando agrega tareas a una iteración, la fecha de inicio de la tarea se calcula tal como se describe en [[!UICONTROL Comprender] cómo se calculan las fechas de inicio de las tareas cuando se agregan a una iteración](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Para agregar problemas a la iteración:** En la ficha **[!UICONTROL Registro de pendientes]**, haga clic en la ficha **[!UICONTROL Problemas]**. Seleccione los problemas que desee añadir a la iteración.

1. Haga clic en **[!UICONTROL Guardar].**
Se crea la iteración.

1. (Opcional) Para agregar historias a una iteración existente, consulte [Agregar historias a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Comprender cómo se calculan las fechas de inicio de las tareas cuando se añaden a una iteración {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Cuando agrega una tarea como artículo a una iteración, se usa la restricción [!UICONTROL Debe finalizar la tarea] para cada artículo. En la mayoría de los casos, la fecha de inicio planificada de la tarea se calcula según la siguiente fórmula:

[!UICONTROL Fecha de finalización de iteración] menos (-) [!UICONTROL Duración de tarea] es igual a (=) [!UICONTROL Fecha de inicio planificada para la tarea]

Se usa la [!UICONTROL fecha de finalización del proyecto] en lugar del   si la fecha de inicio del proyecto es posterior a la fecha de inicio de la iteración y la fecha de finalización del proyecto es posterior a la fecha de finalización de la iteración.

Puede configurar equipos de Scrum individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
