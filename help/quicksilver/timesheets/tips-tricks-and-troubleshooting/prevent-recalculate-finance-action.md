---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Evitar que la acción Recalcular finanzas afecte a las horas históricas cuando cambian las tarifas
description: Debe actualizar el coste por hora de un usuario o rol (debido a un aumento u otra circunstancia), pero no desea que este cambio afecte a las horas que se han registrado anteriormente en los proyectos o desea que afecte solo a una parte de las horas históricas.
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Evitar que la acción Recalcular finanzas afecte a las horas históricas cuando cambian las tarifas

## Problema

Debe actualizar el coste por hora de un usuario o rol (debido a un aumento u otra circunstancia), pero no desea que este cambio afecte a las horas que se han registrado anteriormente en los proyectos o desea que afecte solo a una parte de las horas históricas.

## Solución

Agregue las horas que no desee cambiar a un Registro de facturación en el proyecto y establezca el estado del registro de facturación a Facturado.  Esto bloquea la tarifa antigua y la acción Recalcular finanzas la ignorará.  Las horas que no pertenecen a un registro de facturación Facturado se calculan con la nueva tarifa. Para obtener más información, consulte [Recalcular las finanzas del proyecto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
