---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Impedir que la acción Recalcular finanzas afecte a las horas históricas cuando cambien las tasas
description: Es necesario actualizar el coste por hora de un usuario o función de trabajo (debido a un aumento u otra circunstancia), pero no desea que este cambio afecte a las horas que ya han iniciado sesión en proyectos o que solo afecte a una parte de las horas históricas.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Impedir que la acción Recalcular finanzas afecte a las horas históricas cuando cambien las tasas

## Problema

Es necesario actualizar el coste por hora de un usuario o función de trabajo (debido a un aumento u otra circunstancia), pero no desea que este cambio afecte a las horas que ya han iniciado sesión en proyectos o que solo afecte a una parte de las horas históricas.

## Solución

Agregue las horas que no desea cambiar a un registro de facturación en el proyecto y establezca el estado del registro de facturación en Facturado.  Esto bloquea el tipo anterior y la acción Recalcular finanzas ignorará.  Cualquier hora que no pertenezca a un registro de facturación facturada se calcula a la nueva tasa. Para obtener más información, consulte [Volver a calcular las finanzas del proyecto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
