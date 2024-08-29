---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Resumen del estado de finalización de iteración
description: La información de finalización descrita en este artículo se muestra encima del gráfico de evolución.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Resumen del estado de finalización de iteraciones

La información de finalización descrita en este artículo se muestra encima del gráfico de evolución.

Porcentaje de finalización en una iteración:

![](assets/burndown-percentcomplete-350x47.png)

Esta información indica el estado de finalización de la iteración del día seleccionado actualmente en el gráfico de evolución. De forma predeterminada, el estado de finalización se muestra en función de la fecha del día actual.

La información disponible es la siguiente:

* **[!UICONTROL Porcentaje completado]:** Progreso general de la iteración

  [!UICONTROL Porcentaje completado] se ajusta en función del porcentaje completado de cada artículo o tarea dentro de la iteración, incluidos los artículos o las tareas que solo se han completado parcialmente.

  El color de la barra de estado [!UICONTROL Porcentaje completado] se muestra en rojo o verde para coincidir con el color de la tasa de evolución real. Se muestra en rojo cuando la tasa de evolución es menor que la ideal (quedan más puntos o horas por día que el cálculo de evolución ideal) y en verde cuando la tasa de evolución es igual o mejor que la ideal (quedan menos puntos por día que el cálculo de evolución ideal).

* **[!UICONTROL Historias completadas]:** (disponible solo en iteraciones) El número de historias marcadas como [!UICONTROL Completas]. Esto se muestra en relación con el número total de historias en la iteración. Por ejemplo, &quot;3 de 6&quot; indica que 3 de las 6 historias de la iteración se han marcado como [!UICONTROL Completadas].
* **[!UICONTROL Puntos/Horas completados]:** (disponible solo en iteraciones) El número de puntos o horas marcadas [!UICONTROL Completar]. Se muestra en relación con el número total de puntos u horas de la iteración. Por ejemplo, &quot;5 de 11&quot; indica que 5 de las 11 historias de la iteración se han marcado como [!UICONTROL Completas]. Este número está directamente relacionado con el cálculo [!UICONTROL Porcentaje completado] y se actualiza al mismo tiempo que el [!UICONTROL Porcentaje completado].

  Los puntos y las horas están asociados a las historias. Cuando un artículo se marca como [!UICONTROL Completo], los puntos o las horas asociados con ese artículo se marcan como Completado.

  De forma predeterminada, se utilizan puntos. Puede cambiar esto modificando la configuración de su equipo, tal como se describe en [Crear un equipo Agile](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Puntos / Horas por día]:** (Disponible solo en iteraciones) El número promedio de puntos u horas marcados [!UICONTROL Completar] cada día desde el comienzo de la iteración hasta el día actual.

  Se calcula mediante el total de puntos u horas completadas, dividido por el número total de días hasta el día actual. (Los días parciales se registran como un día entero).

  Esta información puede resultar útil al planificar una iteración futura.

* **[!UICONTROL Finalización estimada]:** La fecha estimada en que se completará la iteración, basada en la tasa actual en Puntos/Horas por día (para iteraciones).

  Cuando la [!UICONTROL fecha de finalización estimada] es posterior a la fecha de finalización definida para la iteración, el número de días laborables restantes se muestra en rojo entre paréntesis junto a la [!UICONTROL fecha de finalización estimada].

  Cuando la [!UICONTROL fecha estimada de finalización] es anterior a la fecha planificada de finalización de la iteración, el número de días laborables restantes se muestra en verde. (La fecha de finalización de la iteración se especifica cuando se planea la iteración, tal como se describe en [Crear una iteración](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); la fecha de finalización del proyecto es la [!UICONTROL Fecha planificada de finalización], o bien es la fecha actual si la [!UICONTROL Fecha planificada de finalización] es anterior. La [!UICONTROL fecha planificada de finalización] del proyecto se calcula en función de la duración de las tareas del proyecto.) Al planificar la iteración, si establece la fecha de finalización de la iteración para un día no laborable y la iteración está realizando un seguimiento para finalizar a tiempo, la fecha de finalización estimada se establece para el último día laborable anterior a la fecha de finalización de la iteración establecida (porque el trabajo no está programado para quemarse en días no laborables).

  Por ejemplo, &quot;(+9 días)&quot; indica que la fecha de finalización estimada es 9 días hábiles después de la fecha de finalización planificada de la iteración.

  Para obtener más información, vea [Información general sobre el estado de finalización de iteraciones](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
