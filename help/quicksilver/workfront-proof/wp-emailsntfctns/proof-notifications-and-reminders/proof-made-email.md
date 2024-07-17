---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Correo electrónico de la prueba realizada
description: Solo se envía un correo electrónico al creador de la prueba cuando este ha creado una prueba. Si una persona ha creado una prueba y ha hecho que otra persona sea el Propietario, solo el nuevo Propietario recibe también el correo electrónico de Prueba realizada. El Creador y/o Propietario no recibirá uno; solo recibirá el correo electrónico de la Prueba realizada. Para obtener más información sobre el correo electrónico de nueva prueba, consulte Nuevo correo electrónico de prueba.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# El correo electrónico [!UICONTROL Revisión realizada]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Se enviará un correo electrónico con [!UICONTROL Prueba realizada] al creador de la prueba solamente cuando este haya creado la prueba. Si una persona ha creado una prueba y ha hecho que otra persona sea el Propietario, solo el nuevo Propietario también recibirá el correo electrónico [!UICONTROL Prueba realizada]. El creador o el propietario no recibirán uno; solo recibirán el correo electrónico [!UICONTROL Prueba realizada]. Para obtener más información sobre el correo electrónico [!UICONTROL Nueva revisión], consulte [[!UICONTROL Nuevo mensaje de revisión]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

Los usuarios pueden deshabilitar [!UICONTROL Pruebas realizadas] correos electrónicos en la configuración de su perfil, como se explica a continuación.

>[!NOTE]
>
> Si el creador o propietario de la prueba tiene [!UICONTROL Pruebas realizadas] correos electrónicos desactivados de forma predeterminada en su configuración personal, no recibirá [!UICONTROL Pruebas realizadas] ni [!UICONTROL Nuevas pruebas], aunque la casilla [!UICONTROL Notificar a las personas por correo electrónico] esté marcada en la página [!UICONTROL Nuevas pruebas].

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

Un correo electrónico [!UICONTROL Comprobaciones realizadas] incluye su mensaje personal (si lo incluye) y los siguientes detalles de la revisión:

* Nombre de revisión
* Vínculo personal a la prueba
* Número de versión
* Miniatura de la prueba
* Progreso de revisión
* Un vínculo para compartir la prueba con otra persona
* Esto le permite compartir la URL de prueba o el vínculo de descarga del archivo original.

>[!NOTE]
>
> El uso compartido de vínculos de prueba no permite agregar explícitamente revisores a la prueba, solo se comparte la URL de prueba pública y el destinatario recibe acceso de solo lectura a la prueba.

Consulte [Compartir una revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obtener más información.

Si no deseas que este enlace aparezca en el correo electrónico de tu destinatario, debes deshabilitar la configuración de [!UICONTROL Uso compartido público] en la revisión ([!UICONTROL Descargar archivo original] y [!UICONTROL URL pública]).

## Deshabilitando el correo electrónico [!UICONTROL Prueba realizada]

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**, abra la pestaña **[!UICONTROL Valores predeterminados de revisión]** y haga clic en **[!UICONTROL Deshabilitar]** junto a **[!UICONTROL Confirmación por correo electrónico cuando las pruebas estén listas]**.

1. ![Proof_Made_-_proofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. Consulte [Configuración de notificaciones por correo electrónico en Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obtener instrucciones más detalladas.
1. Si las notificaciones por correo electrónico están deshabilitadas como predeterminadas en [!UICONTROL Configuración de la cuenta], el creador o el propietario de la prueba no recibirán ningún correo electrónico de [!UICONTROL Prueba realizada] o [!UICONTROL Nueva prueba], aunque esté habilitado en su configuración personal y la casilla de verificación [!UICONTROL Notificar a las personas por correo electrónico] esté marcada en la página [!UICONTROL Nueva prueba].
