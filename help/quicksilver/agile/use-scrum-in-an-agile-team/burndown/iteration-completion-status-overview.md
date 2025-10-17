---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Resumen del estado de finalización de iteración
description: La información de finalización descrita en este artículo se muestra encima del gráfico de evolución.
author: Jenny
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 87%

---

# Información general del estado de finalización de la iteración

La información de finalización descrita en este artículo se muestra encima del gráfico de evolución.

Porcentaje de finalización en una iteración:

![panel de detalles de iteración](assets/burndown-percentcomplete-350x47.png)

Esta información indica el estado de finalización de la iteración del día seleccionado actualmente en el gráfico de evolución. De forma predeterminada, el estado de finalización se muestra en función de la fecha del día actual.

La información disponible es la siguiente:

* **[!UICONTROL Porcentaje completado]:** progreso general de la iteración

  [!UICONTROL Porcentaje completado] se ajusta en función del porcentaje completado de cada historia o tarea dentro de la iteración, incluidas las historias o las tareas que solo se han completado parcialmente.

  El color de la barra de estado [!UICONTROL Porcentaje completado] se muestra en rojo o verde para que coincida con el color de la tasa de evolución real. Se muestra en rojo cuando la tasa de evolución es inferior a la ideal (quedan más puntos u horas por día que el cálculo de evolución ideal) y en verde cuando la tasa de evolución es igual o mejor que la ideal (quedan igual o menos puntos por día que el cálculo de evolución ideal).

* **[!UICONTROL Historias completadas]:** (disponible solo en iteraciones) El número de historias marcadas como [!UICONTROL Completadas]. Esto se muestra en relación con el número total de historias en la iteración. Por ejemplo, &quot;3 de 6&quot; indica que 3 de las 6 historias de la iteración se han marcado como [!UICONTROL Completar].
* **[!UICONTROL Puntos/Horas completados]:** (disponible solo en iteraciones) el número de puntos o horas marcadas [!UICONTROL Completar]. Se muestra en relación con el número total de puntos u horas de la iteración. Por ejemplo, &quot;5 de 11&quot; indica que 5 de las 11 historias de la iteración se han marcado como [!UICONTROL Completar]. Este número está directamente relacionado con el cálculo [!UICONTROL Porcentaje completado] y se actualiza al mismo tiempo que el [!UICONTROL Porcentaje completado].

  Los puntos y las horas están asociados a las historias. Cuando un caso se marca como [!UICONTROL Completar], los puntos o las horas asociados con dicho caso se marcan como Completar.

  De forma predeterminada, se utilizan puntos. Puede cambiar esto modificando la configuración de su equipo, tal como se describe en [Crear un equipo Agile](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Puntos / Horas por día]:** (disponible solo en iteraciones) El número promedio de puntos u horas marcados [!UICONTROL Completar] cada día desde el comienzo de la iteración hasta el día actual.

  Se calcula mediante el total de puntos u horas completadas, dividido por el número total de días hasta el día actual. (Los días parciales se registran como un día entero).

  Esta información puede resultar útil a la hora de planificar una iteración futura.

* **[!UICONTROL Finalización estimada]:** la fecha estimada en la que se completará la iteración, basada en la tasa actual en Puntos/Horas por día (para iteraciones).

  Cuando la fecha de [!UICONTROL Finalización estimada] es posterior a la fecha de finalización definida para la iteración, el número de días laborables restantes se muestra en rojo entre paréntesis junto a la fecha de [!UICONTROL Finalización estimada].

  Cuando la fecha de [!UICONTROL Finalización estimada] es anterior a la fecha de finalización planificada de la iteración, el número de días laborables restantes se muestra en verde. La fecha de finalización de la iteración se especifica cuando se planifica la iteración, tal como se describe en [Crear una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); la fecha de finalización del proyecto es la [!UICONTROL Fecha planificada de finalización], o bien es la fecha actual si la [!UICONTROL Fecha planificada de finalización] es anterior. La [!UICONTROL fecha planificada de finalización] del proyecto se calcula en función de la duración de las tareas del proyecto.) Al planificar la iteración, si establece la fecha de finalización de la iteración para un día no laborable y la iteración está realizando un seguimiento para finalizar a tiempo, la fecha de finalización estimada se establece para el último día laborable anterior a la fecha de finalización de la iteración establecida (porque el trabajo no está programado para quemarse en días no laborables).

  Por ejemplo, &quot;(+9 días)&quot; indica que la fecha de finalización estimada es 9 días hábiles después de la fecha de finalización planificada de la iteración.

  Para obtener más información, consulte [Información general del estado de finalización de la iteración](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
