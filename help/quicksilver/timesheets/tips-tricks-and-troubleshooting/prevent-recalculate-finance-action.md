---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Evitar que la acción Recalcular finanzas afecte a las horas históricas cuando cambian las tarifas
description: Debe actualizar el coste por hora de un usuario o rol (debido a un aumento u otra circunstancia), pero no desea que este cambio afecte a las horas que se han registrado anteriormente en los proyectos o desea que afecte solo a una parte de las horas históricas.
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
TQID: https://experienceleague.adobe.com/TBeLp0FaUmlRk2uk5SdCqntrUWeAAVucox6Dyx5M0Uw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 188
ht-degree: 13%

---

# Evitar que la acción Recalcular finanzas afecte a las horas históricas cuando cambian las tarifas

## Problema

Debe actualizar el coste por hora de un usuario o rol (debido a un aumento u otra circunstancia), pero no desea que este cambio afecte a las horas que se han registrado anteriormente en los proyectos o desea que afecte solo a una parte de las horas históricas.

## Solución

Agregue las horas que no desee cambiar a un Registro de facturación en el proyecto y establezca el estado del registro de facturación a Facturado.  Esto bloquea la tarifa antigua y la acción Recalcular finanzas la ignorará.  Las horas que no pertenecen a un registro de facturación Facturado se calculan con la nueva tarifa. Para obtener más información, consulte [Recalcular las finanzas del proyecto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
