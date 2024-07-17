---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configurar la zona de colocación en  [!DNL Workfront Proof]
description: Como administrador de  [!DNL Workfront Proof] puede establecer, ver y editar la configuración de Dropzone de los usuarios. Para obtener información sobre Dropzone, consulte Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Configurar la zona de colocación en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Como administrador de [!DNL Workfront Proof], puede establecer, ver y editar la configuración de Dropzone de los usuarios. Para obtener información sobre Dropzone, consulte [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** y, a continuación, abra la ficha **[!UICONTROL Dropzone]**.

1. Realice cualquiera de los cambios siguientes en la sección **[!UICONTROL Detalles de Dropzone]**:

   * **[!UICONTROL Dropzone web]**: habilita o deshabilita la Dropzone.
   * **[!UICONTROL URL de Dropzone web]**: La URL que debes ingresar en tu navegador para enviar pruebas a través de Dropzone.
   * **[!UICONTROL Dropzone de correo electrónico]**: habilita o deshabilita la Dropzone de correo electrónico.

     >[!NOTE]
     >
     >Ya no se admite el envío de correos electrónicos a las Dropzones.

   * **[!UICONTROL Propietario de Dropzone]**: establezca o edite el propietario de Dropzone. Esta es la persona a la que se notificarán los nuevos envíos a Dropzone. Para que se establezca como propietario de Dropzone, el usuario debe ser supervisor, administrador, administrador de facturación o creador de cuentas. Para obtener más información, consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Rol predeterminado de los creadores]**: todos los remitentes se agregan a la prueba con este rol como predeterminado.
   * **[!UICONTROL Notificación por correo electrónico para todos los creadores]**: establezca aquí la preferencia de alerta de correo electrónico para los creadores (remitentes) de pruebas. Consulte [Configurar las notificaciones por correo electrónico en [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obtener información acerca de las diferentes configuraciones de alertas disponibles.

   * **[!UICONTROL Función de nueva versión]**: habilita y deshabilita la función de nueva versión en Dropzone. Esto permite o elimina a las personas enviar nuevas versiones de pruebas a través de Dropzone.
   * **[!UICONTROL Eliminar pruebas de borrador después de (días)]**: especifique el número de días después de los cuales se eliminará una prueba de borrador. Las pruebas permanecen en estado de borrador si el envío de Dropzone no se completa después de cargar el archivo en Dropzone.
   * **[!UICONTROL Ocultar función de revisor]**: oculta el campo de función de revisor al agregar personas a Dropzone.
   * **[!UICONTROL Enviar mensaje de prueba al activarla]**: configure [!DNL Workfront Proof] para que envíe correos electrónicos de notificación de prueba a los revisores automáticamente cuando se active una prueba.
   * **[!UICONTROL Activar revisión al enviar]**: configure [!DNL Workfront Proof] para que active las revisiones automáticamente al enviar (eliminando la necesidad de activarlas manualmente).

   * Si se mueve una prueba fuera de la Dropzone (por ejemplo, a otra carpeta de su cuenta), la configuración de Dropzone ya no se aplicará a la prueba. Esto es especialmente importante con respecto a la configuración de alertas de correo electrónico.

1. Realice cualquier cambio en la sección **[!UICONTROL Campos de Dropzone]** para especificar qué campos se muestran en la sección [!UICONTROL Detalles de la prueba] de la página de envío de Dropzone cuando se envían pruebas a través de Dropzone.
1. En la sección **[!UICONTROL Dominios permitidos]**, especifique los dominios a los que desea permitir el uso de Dropzone.

   * Puede hacer clic en **[!UICONTROL Agregar dominio]** para agregar un dominio. Cuando termine de agregar los detalles del dominio, haga clic en **[!UICONTROL Guardar]**.

   * Puede **[!UICONTROL editar]** y **[!UICONTROL eliminar]** cualquier dominio existente que haya agregado anteriormente.

1. En **[!UICONTROL Personas a las que notificar]**, especifica a las personas a las que deseas que se le notifique junto con el propietario de Dropzone cuando se envíen nuevas pruebas a Dropzone [The Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Haga clic en **[!UICONTROL Agregar personas]**, escriba los detalles del destinatario y haga clic en **[!UICONTROL Guardar]**.

   * **[!UICONTROL Eliminar]** personas que agregó anteriormente.
