---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Resumen del gráfico de evolución de Agile
description: El gráfico de evolución proporciona una representación visual de cómo las historias progresan a través de la iteración o el proyecto La tasa de evolución real se mide comparándola con la tasa de evolución ideal para la iteración o la cronología del proyecto.
author: Jenny
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Resumen del gráfico de evolución Agile

El gráfico de evolución proporciona una representación visual de cómo las historias progresan a través de la iteración. La tasa de evolución real se mide comparándola con la tasa de evolución ideal para la cronología de la iteración.

El gráfico de evolución se ajusta en función del día seleccionado. El día actual es el predeterminado. Cuando se selecciona un día anterior, todos los datos del gráfico de evolución y todos los valores de la sección [!UICONTROL estado de finalización] por encima del gráfico de evolución se vuelven a calcular para representar los datos tal como estaban al final del día seleccionado. (Puede seleccionar días pasados o el día actual; no puede seleccionar días en el futuro).

![](assets/agile-iteration-burndown-350x88.png)

## Indicadores visuales

El gráfico de evolución contiene los siguientes indicadores visuales:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt="Inicio de velocidad de evolución ideal"> </td> 
   <td> <p>Tasa de evolución ideal basada en el momento en que comenzó la iteración.</p> <p>Esta línea no se muestra si el ámbito de la iteración nunca cambia (las horas o los puntos nunca se agregan ni eliminan).</p> <p>Esta línea se muestra plana cuando se trabaja en un día libre. Para obtener más información, consulte <a title="Uso del gráfico de evolución de Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Cómo afectan los días libres al gráfico de evolución</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt="Tasa de evolución ideal en historias o tareas"> </td> 
   <td> <p>Tasa de evolución ideal en función de las historias o tareas actuales.</p> <p>La tasa de evolución ideal actual (línea azul sólida) difiere de la tasa de evolución ideal original (línea azul punteada) cuando se añaden horas o puntos a la iteración o se eliminan de ella después de que comience la iteración.</p> <p>Esta línea se muestra plana cuando se trabaja en un día libre.</p> <p>Para obtener más información, consulte <a title="Uso del gráfico de evolución de Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Cómo afectan los días libres al gráfico de evolución</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt="Tasa de evolución real en rojo"> </td> 
   <td> <p>La tasa de evolución real se muestra en rojo cuando la tasa de evolución es inferior a la ideal (quedan más puntos o horas por día que el cálculo de evolución ideal).</p> <p>La fórmula siguiente se utiliza para calcular la tasa de evolución real:</p> <p>[SUMA(Valor de punto u hora del trabajo en curso * Porcentaje completado) + Valor de punto u hora del trabajo completado]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt="Tasa de evolución real en verde"> </td> 
   <td> <p>La tasa de evolución real se muestra en verde cuando la tasa de evolución es igual o mejor que la ideal (quedan menos puntos por día o iguales que el cálculo de evolución ideal).</p> <p>La fórmula siguiente se utiliza para calcular la tasa de evolución real:</p> <p>[SUMA(Valor de punto u hora del trabajo en curso * Porcentaje completado) + Valor de punto u hora del trabajo completado]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Cambio en el ámbito"> </td> 
   <td> <p>Cambio en el ámbito (se añaden horas o puntos o se eliminan de la iteración).</p> <p>Los cambios de ámbito siempre se muestran como una línea vertical en medio del día. Además, se muestra un punto azul en medio de cualquier día en el que se haya producido un cambio de ámbito.</p> <p>El eje vertical del gráfico de evolución muestra los puntos o las horas del artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Cambio en el intervalo de fechas"> </td> 
   <td> <p>Cambio en el intervalo de fechas (la duración de la iteración aumenta o disminuye).</p> <p>Se muestra un punto azul en medio de cualquier día en el que se haya cambiado la duración de la iteración.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Quemado el punto verde del trabajo"> </td> 
   <td> <p>Se muestra un punto verde o rojo en la tasa de evolución real cada vez que se quema el trabajo. (Cuando la tasa de evolución real de ese día es de color rojo, el punto es de color rojo; cuando la tasa de evolución real de ese día es de color verde, el punto es de color verde).</p> <p>El trabajo se incendia cuando se produce cualquiera de las siguientes situaciones:</p> 
    <ul> 
     <li> El [!UICONTROL Percent Complete] aumenta en la historia.<br>[!UICONTROL Percent Complete] aumenta cuando: 
      <ul> 
       <li> <p>Cambiado manualmente</p> </li> 
       <li> <p>La cantidad de puntos u horas se actualiza en la historia</p> </li> 
      </ul></li>  
     <li>El estado de la historia cambia a [!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo afectan los días libres al gráfico de evolución {#how-days-off-affect-the-burndown-chart}

La programación predeterminada definida en [!DNL Workfront] afecta el gráfico de evolución al excluir los días libres (fines de semana y festivos) de la evolución. El gráfico de evolución utiliza el horario predeterminado para definir los días laborables (tal y como se describe en  [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

Los equipos de Agile pueden incorporar días no laborables específicos del equipo definiendo un horario alternativo (como se describe en el artículo [Usar un horario de equipo alternativo para los gráficos de evolución](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)). Esta programación alternativa se refleja en el gráfico de evolución de cualquier iteración asignada al equipo. La programación alternativa solo afecta al gráfico de evolución.

Los días libres solo se reflejan en el gráfico de evolución si:

* Anteriormente, el trabajo se registraba con un día libre. (Se muestra el día en que se registró el trabajo.)

  Cuando se inicia una sesión de trabajo con un día libre:

   * No se incluye ningún trabajo registrado al calcular la evolución ideal porque el equipo no tiene programado realizar ningún trabajo.
   * Las líneas de evolución ideales (la línea azul sólida y la línea azul discontinua) se muestran como planas en el gráfico de evolución para cualquier día en el que se haya realizado el trabajo o en el día en el que se visualice el gráfico de evolución (si está visualizando en un día libre).
   * El trabajo registrado se incluye al calcular otras estadísticas de evolución, como la finalización estimada y el promedio de puntos o horas por día.

* Está viendo el gráfico de evolución en un día libre. (El día que está viendo se muestra en el gráfico de evolución).
* El trabajo total restante de la iteración se completa en un día libre.

  Cuando un usuario completa el trabajo total restante para la iteración en un día libre, el campo [!UICONTROL Finalización estimada] muestra la fecha en la que se completó la iteración.

  Al planificar la iteración, si establece la fecha de finalización de la iteración para un día no laborable y la iteración está realizando un seguimiento para finalizar a tiempo, la [!UICONTROL fecha estimada de finalización] se establece para el último día laborable anterior a la fecha de finalización de la iteración establecida (porque el trabajo no está programado para ser quemado en días no laborables).

  La fecha de finalización de la iteración se especifica cuando se planea la iteración, tal como se describe en el artículo [Crear una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
