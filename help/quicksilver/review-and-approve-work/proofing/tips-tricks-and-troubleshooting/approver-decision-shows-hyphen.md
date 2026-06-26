---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: La decisión del aprobador muestra un guion en el informe de aprobación de la prueba
description: Un guion en el campo Decisión del aprobador del informe Aprobación de la prueba indica que un destinatario ya no está en la función de toma de decisiones de la prueba.
author: Courtney
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: f465ac03e0ff91216d1ef934a1696127796645ba
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# La decisión del aprobador muestra un guion en el informe de aprobación de la prueba

## Problema

En el informe de aprobación de pruebas, el campo Decisión del aprobador de un destinatario muestra un guion (-) aunque el campo Fecha de decisión muestre una fecha y Esperando decisión sea Falso.

![La decisión del aprobador muestra un guion en el informe de aprobación de pruebas](assets/approver-decision-hyphen.png)

## Causa

Un guion en el campo Decisión del aprobador significa que el destinatario ya no está en una función de toma de decisiones en la prueba. Esto puede suceder cuando:

* El destinatario se añadió a la prueba, tomó una decisión y se eliminó más tarde del flujo de trabajo. Si el destinatario vuelve a visitar la prueba, el sistema de prueba registra la visita como un cambio en la decisión. Dado que el destinatario ya no es un aprobador, el sistema registra la nueva decisión como un guion.
* La función de prueba del destinatario se cambió a una que no incluye derechos de aprobación, como Revisor. Para obtener información acerca de las acciones que cada rol puede realizar en una prueba, consulte [Resumen de roles de prueba](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).
* El perfil de permiso de prueba del destinatario se bajó de categoría después de tomar su decisión.

## Qué significa esto en los informes

El guión es intencional. Indica que el sistema no está esperando a que el destinatario apruebe la prueba y que el destinatario ya no tiene una función de toma de decisiones en la prueba.

El campo Fecha de decisión aún muestra la fecha de la actividad de decisión más reciente del destinatario, pero su decisión ya no se cuenta en el informe.

Para obtener información sobre cómo crear y usar el informe de aprobación de pruebas, consulte [Usar el informe de aprobación de pruebas](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md).



