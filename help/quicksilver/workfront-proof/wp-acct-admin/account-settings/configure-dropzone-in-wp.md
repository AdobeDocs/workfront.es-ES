---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configurar Dropzone en  [!DNL Workfront Proof]
description: Como administrador de  [!DNL Workfront Proof] , puede establecer, ver y editar la configuración de Dropzone de los usuarios. Para obtener información sobre Dropzone, consulte Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
TQID: https://experienceleague.adobe.com/IDL8PSxlmHC9hsENUlrbfRQK-9qhpvHYmsvKDMepVvw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 498
ht-degree: 100%

---

# Configurar Dropzone en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Como administrador de [!DNL Workfront Proof], puede establecer, ver y editar la configuración de Dropzone de los usuarios. Para obtener información sobre Dropzone, consulte [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Haga clic en **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** y, a continuación, abra la pestaña **[!UICONTROL Dropzone]**.

1. Realice cualquiera de los cambios siguientes en la sección **[!UICONTROL Dropzone details]**:

   * **[!UICONTROL Web Dropzone]**: habilite o deshabilite Dropzone.
   * **[!UICONTROL Web Dropzone URL]**: la URL que debe introducir en su navegador para enviar pruebas a través de Dropzone.
   * **[!UICONTROL Email Dropzone]**: habilite o deshabilite Dropzone de correo electrónico.

     >[!NOTE]
     >
     >Ya no se admite el envío de correos electrónicos a las Dropzones.

   * **[!UICONTROL Dropzone Owner]**: establezca o edite el propietario de Dropzone. Esta es la persona a la que se notificarán los nuevos envíos a Dropzone. Para que se establezca como propietario de Dropzone, el usuario debe ser supervisor, administrador, administrador de facturación o creador de cuentas. Para obtener más información, consulte [Perfiles de permisos de prueba en  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Default role for creators]**: todos los remitentes se añaden a la prueba con esta función como valor predeterminado.
   * **[!UICONTROL Email notification for all creators]**: establezca aquí la preferencia de alerta de correo electrónico para los creadores (remitentes) de pruebas. Consulte [Configurar las notificaciones por correo electrónico en  [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obtener información acerca de las diferentes configuraciones de alertas disponibles.

   * **[!UICONTROL New version function]**: habilite y deshabilite la función de nueva versión en Dropzone. Esto ofrece o elimina la capacidad que tienen las personas para enviar nuevas versiones de pruebas a través de Dropzone.
   * **[!UICONTROL Delete draft proofs after (days)]**: especifique el número de días después de los cuales se eliminará una prueba de borrador. Las pruebas permanecen en estado de borrador si el envío de Dropzone no se completa después de cargar el archivo en Dropzone.
   * **[!UICONTROL Hide reviewer role]**: oculte el campo de función de revisor al añadir personas a Dropzone.
   * **[!UICONTROL Send proof message on activation]**: configure [!DNL Workfront Proof] para que envíe correos electrónicos de notificación de prueba a los revisores automáticamente cuando se active una prueba.
   * **[!UICONTROL Activate proof on submission]**: configure [!DNL Workfront Proof] para que active las pruebas automáticamente al enviarlas (eliminando la necesidad de activarlas manualmente).

   * Si se mueve una prueba fuera de Dropzone (por ejemplo, a otra carpeta de su cuenta), la configuración de Dropzone ya no se aplicará a la prueba. Esto es especialmente importante con respecto a la configuración de alertas de correo electrónico.

1. Realice cualquier cambio en la sección **[!UICONTROL Dropzone fields]** para especificar qué campos se muestran en la sección [!UICONTROL Proof details] de la página de envío de Dropzone cuando se envían pruebas a través de este.
1. En la sección **[!UICONTROL Permitted domains]**, especifique los dominios a los que desea permitir el uso de Dropzone.

   * Puede hacer clic en **[!UICONTROL Add domain]** para añadir un dominio. Cuando termine de añadir los detalles del dominio, haga clic en **[!UICONTROL Save]**.

   * Puede **[!UICONTROL Edit]** y **[!UICONTROL Delete]** cualquier dominio existente que haya añadido anteriormente.

1. En **[!UICONTROL People to notify]**, especifica a las personas a las que desea que se le notifique junto con el propietario de Dropzone cuando se envíen nuevas pruebas a Dropzone [The Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Haga clic en **[!UICONTROL Add people]**, escriba los detalles del destinatario y haga clic en **[!UICONTROL Save]**.

   * **[!UICONTROL Delete]** personas que añadió anteriormente.
