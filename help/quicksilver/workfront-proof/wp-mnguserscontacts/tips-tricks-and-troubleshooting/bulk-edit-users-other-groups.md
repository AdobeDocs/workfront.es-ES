---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Otros grupos del usuario de edición masiva
description: Cuando realizaba ediciones masivas, intentaba añadir un solo grupo Otros a numerosos usuarios. Después de guardar los cambios, se eliminaron todos los otros grupos existentes y solo permaneció el nuevo grupo.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Otros grupos del usuario de edición masiva

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

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
