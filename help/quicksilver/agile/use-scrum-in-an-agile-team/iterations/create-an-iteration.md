---
product-area: agile-and-teams
navigation-topic: iterations
title: Crear una iteración
description: Las iteraciones son un componente clave para los equipos ágiles de Scrum a la hora de planificar la capacidad de trabajo. [!DNL Adobe Workfront]  permite que los equipos ágiles de Scrum administren su trabajo creando múltiples iteraciones para satisfacer las necesidades del equipo.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: e24c97e78b210fc385052b573fe69d092b521a90
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 80%

---

# Crear una iteración

Las iteraciones son un componente clave para los equipos ágiles de Scrum a la hora de planificar la capacidad de trabajo. [!DNL Adobe Workfront] permite que los equipos ágiles de Scrum administren su trabajo creando múltiples iteraciones para satisfacer las necesidades del equipo.

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
   <td> <p>Nuevo: [!UICONTROL Light] o superior</p> 
   o
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una iteración

Puede agregar una iteración en la lista para crear rápidamente una iteración y agregarle tareas y problemas más adelante.

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En la ficha **[!UICONTROL Iteraciones]**, haga clic en **[!UICONTROL Agregar iteración]**.

   ![Haga clic en Agregar iteración](assets/click-add-iteration.png)

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Introduzca el nombre de la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>Añada las metas que tenga para la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td>Introduzca la fecha de inicio de la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong></td> 
      <td><p>Introduzca la fecha en la que debe finalizar la iteración. [!DNL Workfront] recomienda establecer una fecha de finalización que no sea superior a 4 semanas desde la fecha de inicio.</p><p>Sugerencia: asegúrese de elegir un día laborable como fecha de finalización. El gráfico de evolución solo utiliza días laborables en sus cálculos.<br>De manera predeterminada, el gráfico de evolución utiliza el horario predeterminado para definir los días laborables (tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear programación</a>). O bien, para incorporar días no laborables específicos del equipo, los equipos ágiles pueden elegir utilizar un horario alternativo (tal como se describe en “Definición de un horario de equipo alternativo para los gráficos de evolución” en <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo ágil</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Especifique la capacidad de la iteración. Es el número de puntos u horas que su equipo puede lograr en la iteración. El número que introduzca debe ser igual o mayor que el número de puntos u horas de la suma de todos las historias de la iteración.<br>[!DNL Workfront] rellena previamente este campo con 50 de capacidad de forma predeterminada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Especifique el porcentaje de enfoque del equipo. Si todos los integrantes del equipo se centran completamente en esta iteración, el enfoque sería del 100 %.<br>[!DNL Workfront] rellena previamente este campo con el 100 % de forma predeterminada. </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Agregar iteración]**. Ahora que ha creado una iteración, debe añadir historias. Para obtener más información, consulte [Añadir historias a una iteración existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planificar una iteración en la pestaña [!UICONTROL Registro de asuntos pendientes]

Utilice la función [!UICONTROL Planificar iteración] para crear una iteración con tareas en el registro de asuntos pendientes.

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione **[!UICONTROL Registro de pendientes]** en el panel izquierdo.

1. En la ficha **Historias** o **Problemas**, seleccione los elementos de trabajo que desee agregar a la iteración y, a continuación, haga clic en **[!UICONTROL Planificar iteración]**.

>[!NOTE]
>
> No puede cambiar entre la ficha Historias o Problemas ni agregar tareas adicionales al planificar una iteración en la ficha Registro de pendientes. Puede agregar historias o problemas existentes una vez que se haya creado la iteración. Para obtener más información, consulte [Agregar tareas o problemas a una iteración existente en la ficha Registro de pendientes](#add-tasks-or-issues-to-an-existing-iteration-on-the-backlog-tab) a continuación.


1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Especifique un nombre para la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td> Especifique la fecha de inicio de la iteración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong> </td> 
      <td><p>Especifique la fecha de finalización de la iteración. [!DNL Workfront] recomienda establecer una fecha de finalización no superior a 4 semanas desde la fecha de inicio.</p><p>Sugerencia: asegúrese de elegir un día laborable como fecha de finalización. El gráfico de evolución solo utiliza días laborables en sus cálculos.<br>De manera predeterminada, el gráfico de evolución utiliza el horario predeterminado para definir los días laborables (tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear programación</a>). O bien, para incorporar días no laborables específicos del equipo, los equipos Agile pueden elegir usar un horario alternativo (como se describe en <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Usar un horario de equipo alternativo para los gráficos de evolución</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Especifique el porcentaje de enfoque del equipo. Si todos los integrantes del equipo se centran completamente en esta iteración, el enfoque sería del 100 %.<br>[!DNL Workfront] rellena previamente este campo con el valor de promedio de las iteraciones anteriores del equipo. Si esta es la primera iteración del equipo, este valor de campo es 0 de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Especifique la capacidad de la iteración. Es el número de puntos u horas que su equipo puede lograr en la iteración. El número que introduzca debe ser igual o mayor que el número de puntos u horas de la suma de todos las historias de la iteración.<br>[!DNL Workfront] rellena previamente este campo con el valor de promedio de las iteraciones anteriores del equipo. Si esta es la primera iteración del equipo, este valor de campo es 0 de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Especifique una meta para la iteración. Este campo es obligatorio.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar].**: se crea la iteración.

## Agregar tareas o problemas a una iteración existente en la ficha Registro de pendientes

1. En la ficha **Registro de pendientes**, haga clic en la ficha **Historias** o **Problemas**.

1. Seleccione las historias o los problemas que desee añadir a la iteración. Las historias en la parte superior del registro de pendientes son de mayor prioridad.

   ![mover un elemento de trabajo](assets/move-to-iteration.png)

   >[!NOTE]
   >
   >  Cuando añade tareas a una iteración, la fecha de inicio de la tarea se calcula tal como se describe en [[!UICONTROL Comprender] cómo se calculan las fechas de inicio de las tareas cuando se añaden a una iteración](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).


## Comprender cómo se calculan las fechas de inicio de las tareas cuando se añaden a una iteración {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Cuando añade una tarea como una historia a una iteración, se usa la restricción [!UICONTROL Debe finalizar en la tarea] para cada historia. En la mayoría de los casos, la fecha planificada de inicio de la tarea se calcula según la siguiente fórmula:

[!UICONTROL Fecha de finalización de la iteración] menos (-) [!UICONTROL Duración de la tarea] es igual a (=) [!UICONTROL Fecha planificada de inicio de la tarea]

Se utiliza [!UICONTROL Fecha de finalización del proyecto] en lugar de la Fecha de finalización de la iteración si la fecha de inicio del proyecto es posterior a la fecha de inicio de la iteración y la fecha de finalización del proyecto es posterior a la fecha de finalización de la iteración.

Puede configurar equipos de Scrum individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
