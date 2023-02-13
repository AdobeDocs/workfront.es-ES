---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: El correo electrónico de prueba realizada
description: Un correo electrónico de prueba se envía al creador de pruebas solo cuando ha creado una prueba. Si una persona ha creado una prueba y ha hecho de otra persona el propietario, solo el nuevo propietario recibe también el correo electrónico de prueba. El Creador o el Propietario no tendrán uno; solo reciben el correo electrónico Proof Made. Para obtener más información sobre el correo electrónico de prueba nueva, consulte Correo electrónico de prueba nueva.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# La variable [!UICONTROL Prueba realizada] email

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

A [!UICONTROL Prueba realizada] el correo electrónico se envía al creador de pruebas solo cuando ha creado una prueba. Si una persona ha creado una prueba y ha hecho de otra persona el propietario, solo el nuevo propietario recibe la variable [!UICONTROL Prueba realizada] correo electrónico. El Creador o el Propietario no tendrán uno; solo reciben la variable [!UICONTROL Prueba realizada] correo electrónico. Para obtener más información sobre la variable [!UICONTROL Nueva prueba] correo electrónico, consulte [[!UICONTROL Nueva prueba] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

Los usuarios pueden desactivar [!UICONTROL Prueba realizada] correos electrónicos en la configuración de perfil, como se explica a continuación.

>[!NOTE]
>
> Si el Creador o el Propietario de la prueba tiene [!UICONTROL Prueba realizada] los correos electrónicos desactivados de forma predeterminada en su configuración personal no reciben ningún [!UICONTROL Prueba realizada] o [!UICONTROL Nueva prueba] los correos electrónicos, incluso si la variable [!UICONTROL Notificar a las personas por correo electrónico] está activada en la casilla [!UICONTROL Nueva prueba] página.

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

A [!UICONTROL Prueba realizada] El correo electrónico incluye su mensaje personal (si lo incluye) y los siguientes detalles de prueba:

* Nombre de revisión
* Enlace personal a la prueba
* Número de versión
* Miniatura de la prueba
* Progreso de revisión
* Un vínculo para compartir la prueba con otra persona
* Esto le permite compartir la URL de prueba o el vínculo de descarga del archivo original.

>[!NOTE]
>
> El uso compartido de vínculos de prueba no permite añadir explícitamente revisores a la prueba, solo se comparte la URL de prueba pública y el destinatario recibe acceso de solo lectura a la prueba.

Consulte [Compartir una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obtener más información.

Si no desea que este vínculo aparezca en el correo electrónico del destinatario, deshabilite el [!UICONTROL Uso compartido público] configuración de la prueba ([!UICONTROL Descargar archivo original] y [!UICONTROL URL pública]).

## Desactivación de la función [!UICONTROL Prueba realizada] Correo electrónico

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes personales]**, abra el **[!UICONTROL Valores predeterminados de prueba]** a continuación, haga clic en **[!UICONTROL Deshabilitar]** junto a **[!UICONTROL Confirmación por correo electrónico cuando las pruebas están listas]**.

1. ![Proof_Made_-_proofing_default.png](assets/proof-made---proofing-defaults-350x103.png)

1. Consulte [Configuración de las notificaciones por correo electrónico en Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obtener instrucciones más detalladas.
1. Si las notificaciones por correo electrónico están deshabilitadas de forma predeterminada en la variable [!UICONTROL Configuración de la cuenta], el creador o el propietario de la prueba no recibirán ninguna [!UICONTROL Prueba realizada] o [!UICONTROL Nueva prueba] los correos electrónicos, incluso si están activados en su Configuración personal y en el [!UICONTROL Notificar a las personas por correo electrónico] está activada en la casilla [!UICONTROL Nueva prueba] página.
