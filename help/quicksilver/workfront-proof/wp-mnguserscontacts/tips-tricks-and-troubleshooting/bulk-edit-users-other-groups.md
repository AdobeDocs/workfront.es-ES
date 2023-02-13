---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Editar masivamente otros grupos del usuario
description: Al editar masivamente intenté agregar un solo Otro Grupo a numerosos usuarios. Después de Save Changes, se eliminaron todos los otros grupos existentes y sólo quedó el nuevo otro grupo.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Editar masivamente otros grupos del usuario

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

## Problema:

Al editar masivamente intenté agregar un solo Otro Grupo a numerosos usuarios.
Después de Save Changes, se eliminaron todos los otros grupos existentes y sólo quedó el nuevo otro grupo.

## Respuesta:

El comportamiento resultante depende de la pertenencia al grupo actual de los usuarios seleccionados:

* Si todos los usuarios seleccionados, las pertenencias a Otros grupos coinciden exactamente... Después de seleccionar los usuarios y seleccionar [!UICONTROL editar], el [!UICONTROL Otros grupos] mostrará la lista completa de todos los grupos a los que pertenecen estos usuarios.

* Si los usuarios seleccionados tienen miembros de Otros grupos diferentes... Después de seleccionar los usuarios y hacer clic en [!UICONTROL Editar], el [!UICONTROL Otros grupos] se deja en blanco.

Al hacer clic en **[!UICONTROL Guardar cambios]**, se guardará lo que se muestre en el campo Otros grupos .

Se sobrescribe el contenido anterior del campo.
