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
TQID: 'https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 67%
---
# Edición en lotes de Otros grupos del usuario

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

## Problema:

Al realizar ediciones masivas, he intentado añadir un solo Otros grupos a numerosos usuarios.
Después de guardar los cambios, se eliminaron todos los Otros grupos existentes y solo permaneció el nuevo grupo.

## Respuesta:

El comportamiento resultante depende de la pertenencia al grupo actual de los usuarios seleccionados:

* Si todos los usuarios seleccionados y las suscripciones a Otros grupos coinciden exactamente...
Después de seleccionar los usuarios y seleccionar [!UICONTROL editar], el campo [!UICONTROL Otros grupos] mostrará el listado completo
de todos los grupos a los que pertenecen estos usuarios.

* Si los usuarios seleccionados tienen diferentes pertenencias de Otro grupo...
Después de seleccionar los usuarios y hacer clic en [!UICONTROL Editar], el campo [!UICONTROL Otros grupos] quedará en blanco.

Al hacer clic en **[!UICONTROL Guardar cambios]**, se guardará lo que aparezca en el campo Otros grupos.

El contenido anterior del campo se sobrescribe.
