---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Edición en lotes de Otros grupos del usuario
description: Al realizar ediciones masivas, he intentado añadir un solo Otros grupos a numerosos usuarios. Después de guardar los cambios, se eliminaron todos los Otros grupos existentes y solo permaneció el nuevo grupo.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 170
ht-degree: 55%

---

# Edición en lotes de Otros grupos del usuario

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

## Problema:

Cuando realizaba ediciones masivas, intentaba añadir un solo grupo Otros a numerosos usuarios.
Después de guardar los cambios, se eliminaron todos los otros grupos existentes y solo permaneció el nuevo grupo.

## Respuesta:

El comportamiento resultante depende de la pertenencia al grupo actual de los usuarios seleccionados:

* Si todos los usuarios seleccionados y las suscripciones a Otros grupos coinciden exactamente...
Después de seleccionar los usuarios y seleccionar [!UICONTROL editar], el campo [!UICONTROL Otros grupos] mostrará el listado completo
de todos los grupos a los que pertenecen estos usuarios.

* Si los usuarios seleccionados tienen diferentes pertenencias de Otro grupo...
Después de seleccionar los usuarios y hacer clic en [!UICONTROL Editar], el campo [!UICONTROL Otros grupos] quedará en blanco.

Al hacer clic en **[!UICONTROL Guardar cambios]**, se guardará lo que aparezca en el campo Otros grupos.

El contenido anterior del campo se sobrescribe.
