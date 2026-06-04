---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: personal-settings
title: Designando propietarios de revisión temporales en  [!DNL Workfront Proof]
description: Si va a estar fuera de la oficina durante un período de tiempo prolongado, puede delegar la propiedad de las pruebas a otro usuario de la cuenta.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d00636d7-1eb1-4aac-9663-6335e7675836
TQID: https://experienceleague.adobe.com/C5CDLekqdsrG3LBy6c5szAFFTTinNySLgh8IyEsnMuc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 402
ht-degree: 100%

---

# Designando propietarios de revisión temporales en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si va a estar fuera de la oficina durante un período de tiempo prolongado, puede delegar la propiedad de las pruebas a otro usuario de la cuenta.

>[!NOTE]
>
>Esta función solo está disponible en [!DNL Workfront Proof].

Para designar la propiedad temporal de las pruebas:

1. En [!DNL Workfront Proof], vaya a **[!UICONTROL Configuración personal]**.\
   ![personal-settings.png](assets/personal-settings-350x83.png)

1. Haga clic en la ficha **[!UICONTROL Fuera de la oficina]**. Las configuraciones disponibles son las siguientes:

   * **[!UICONTROL Delegue sus pruebas a]** otro usuario en su cuenta.
   * Habilite y deshabilite la función **[!UICONTROL Fuera de la oficina]** marcando o desmarcando la casilla de verificación.
   * Seleccione la **[!UICONTROL Fecha de inicio]**.

     Si se elige la opción **[!UICONTROL Iniciar inmediatamente]**, la propiedad de las pruebas se delegará al usuario seleccionado inmediatamente después de activar la característica.

     Si se establecen una fecha y hora de inicio específicas, la función se activará en el día y la hora seleccionados.

   * Seleccione la **[!UICONTROL Fecha de finalización]**.

     Si no se elige una fecha de finalización, la propiedad de las pruebas se delega hasta que la función se deshabilite manualmente.

     Si se establece una fecha y hora de finalización específicas, la función se desactivará en el día y la hora seleccionados.

     ![out-of-office-options.png](assets/out-of-office-options-350x234.png)

1. Cuando se delegan las pruebas, se muestra el propietario delegado en la sección **[!UICONTROL Detalles]** de la página de detalles de la prueba. La nota de delegación de propiedad aparece en la sección **[!UICONTROL Actividad]** de la página de detalles de la prueba.

   ![activity-section-delegated.png](assets/activity-section-delegated-350x318.png)

   También se muestra una notificación [!UICONTROL Fuera de la oficina] en la cuenta del propietario de la revisión original durante el tiempo en que la característica está habilitada. Esto sirve como recordatorio para el propietario original y también le permite finalizar la delegación inmediatamente o ir a [!UICONTROL Configuración personal] para ajustarla.

   ![notification-on-account.png](assets/notification-on-account-350x15.png)

   Cuando el propietario original recupera la propiedad de las pruebas, el propietario delegado desaparece de la sección [!UICONTROL Detalles] de la página de detalles de prueba y la notificación [!UICONTROL Fuera de la oficina] ya no se muestra en la cuenta del propietario de la prueba original. Aparece una nota que muestra que la propiedad de la prueba se ha revertido en la sección [!UICONTROL Actividad] de la página de detalles de la prueba.

   >[!NOTE]
   >
   >El propietario delegado permanece en el flujo de trabajo de prueba a menos que se elimine manualmente.

   ![[!UICONTROL activity-section-taken-back].png](assets/activity-section-taken-back-350x99.png)
