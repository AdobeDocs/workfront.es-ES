---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configure la zona de colocación en [!DNL Workfront Proof]
description: Como [!DNL Workfront Proof] administrador, puede establecer, ver y editar la configuración de Dropzone de los usuarios. Para obtener más información sobre Dropzone, consulte The Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Configure la zona de colocación en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Como [!DNL Workfront Proof] administrador, puede establecer, ver y editar la configuración de Dropzone de los usuarios. Para obtener información sobre Dropzone, consulte [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** y, a continuación, abra el **[!UICONTROL Dropzone]** pestaña .

1. Realice cualquiera de los siguientes cambios en la **[!UICONTROL Detalles de Dropzone]** sección:

   * **[!UICONTROL Web Dropzone]**: Habilite o deshabilite Dropzone.
   * **[!UICONTROL URL de zona de Web]**: Dirección URL que debe introducir en el explorador para enviar pruebas a través de Dropzone.
   * **[!UICONTROL Zona de colocación de correo electrónico]**: Habilite o deshabilite la zona de colocación de correo electrónico.

      >[!NOTE]
      >
      >Ya no se admite el envío por correo electrónico a las zonas de colocación.

   * **[!UICONTROL Propietario de Dropzone]**: Defina o edite el propietario de Dropzone. Esta es la persona a la que se notificará de nuevos envíos a Dropzone. Para que se establezca como propietario de Dropzone, el usuario debe ser Supervisor, Administrador, Administrador de facturación o Creador de cuentas. Para obtener más información, consulte [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Función predeterminada para creadores]**: Todos los remitentes se añaden a la prueba con esta función como valor predeterminado.
   * **[!UICONTROL Notificación por correo electrónico de todos los creadores]**: Establezca aquí la preferencia de alerta de correo electrónico para los creadores de pruebas (remitentes). Consulte [Configure las opciones de notificación por correo electrónico en [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obtener información sobre los diferentes ajustes de alerta disponibles.

   * **[!UICONTROL Nueva función de versión]**: Habilite y deshabilite la función Nueva versión en Dropzone. Esto proporciona o elimina la capacidad de las personas de enviar nuevas versiones de pruebas a través de Dropzone.
   * **[!UICONTROL Eliminar pruebas de borrador después de (días)]**: Especifique el número de días después de los cuales se eliminará un borrador de prueba. Las pruebas permanecen en estado de borrador si el envío de Dropzone no se completa después de cargar el archivo en Dropzone.
   * **[!UICONTROL Ocultar función de revisor]**: Oculte el campo de función del revisor al añadir personas a la zona de colocación.
   * **[!UICONTROL Enviar mensaje de prueba al activar]**: Configurar [!DNL Workfront Proof] para enviar correos electrónicos de notificación de prueba a los revisores automáticamente cuando se activa una prueba.
   * **[!UICONTROL Activar la prueba al enviar]**: Configurar [!DNL Workfront Proof] para activar las pruebas automáticamente al enviarlas (eliminando la necesidad de activarlas manualmente).

   * Si se mueve una prueba fuera de la zona de colocación (por ejemplo, a otra carpeta de la cuenta), la configuración de zona de colocación ya no se aplicará a la prueba. Esto es especialmente importante con respecto a la configuración de alertas por correo electrónico.

1. Realice cambios en la variable **[!UICONTROL Campos de zona desplegable]** para especificar qué campos se muestran en la sección [!UICONTROL Detalles de la prueba] sección de la página de envío de Dropzone cuando se envían pruebas a través de Dropzone.
1. En el **[!UICONTROL Dominios permitidos]** , especifique los dominios a los que desea permitir utilizar Dropzone.

   * Puede hacer clic en **[!UICONTROL Añadir dominio]** para agregar un dominio. Cuando haya terminado de agregar los detalles del dominio, haga clic en **[!UICONTROL Guardar]**.

   * Puede **[!UICONTROL Editar]** y **[!UICONTROL Eliminar]** cualquier dominio existente que haya agregado anteriormente.

1. En **[!UICONTROL Personas a las que enviar una notificación]**, especifique las personas a las que desea que se le notifique junto con el propietario de Dropzone cuando se envíen nuevas pruebas a Dropzone [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Haga clic en **[!UICONTROL Agregar personas]**, introduzca los detalles del destinatario y haga clic en **[!UICONTROL Guardar]**.

   * **[!UICONTROL Eliminar]** personas que agregó anteriormente.
