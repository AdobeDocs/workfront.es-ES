---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurar la información de usuario mediante  [!DNL Workfront Proof]
description: Configurar la información de usuario mediante  [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Configurar información de usuario mediante [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

1. Comience a crear o editar un usuario como se describe en [Crear usuarios con [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Especifique la siguiente información:

   * En la sección **[!UICONTROL Datos personales]**:

      * **Dirección de correo electrónico:** La dirección de correo electrónico del usuario.
      * **Nombre:** El nombre del usuario.
      * **Apellido:** El apellido del usuario.
      * **Posición:** La posición del usuario en la compañía.
      * **Perfil de permiso:** Los permisos del usuario en la cuenta de revisión.
      * **Idioma:** El idioma principal del usuario.
      * **Zona horaria:** Seleccione la zona horaria del usuario.
      * **Formato de fecha:** Seleccione el formato de fecha preferido del usuario.
      * **Inclusión - Correos electrónicos de marketing y productos:** Seleccione si desea que el usuario se incluya en los correos electrónicos de marketing y productos.
      * **Solo API:** Permite que el usuario inicie sesión solamente a través de la API.

   * En la sección **[!UICONTROL Detalles del usuario]**, escriba la información de contacto del usuario, como la dirección y el número de teléfono.
   * En la sección **[!UICONTROL Configuración de prueba predeterminada]**, configure las opciones que afectan la forma en que el usuario crea o trabaja en las pruebas.

      * **Función de prueba predeterminada:** Seleccione una función de prueba predeterminada para el usuario. Las opciones de rol son **[!UICONTROL Sólo lectura]**, **[!UICONTROL Revisor]**, **[!UICONTROL Aprobador]**, **[!UICONTROL Revisor y aprobador]**, **[!UICONTROL Autor]** o **[!UICONTROL Moderador]**.

        Para obtener más información sobre los roles de prueba, consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Bloquear la revisión cuando se tomen todas las decisiones:** Bloquea automáticamente la revisión de los cambios posteriores una vez que se hayan tomado todas las decisiones sobre la revisión.
      * **Se requiere inicio de sesión. La revisión solo se puede compartir con otros usuarios:** Hace que la revisión solo esté disponible para los usuarios con [!DNL Workfront Proof] credenciales de inicio de sesión.
      * **Solo se requiere una decisión:** Requiere solo una decisión en una prueba.
      * **Descarga del archivo original:** Permite al usuario descargar el archivo original para una revisión. Esta opción está habilitada de forma predeterminada.

        Para obtener más información sobre cómo descargar archivos originales, consulte [Descargar archivos almacenados en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Suscripción. Las personas pueden registrarse para obtener la revisión a través de la dirección URL pública o el código incrustado:** Permite que los revisores externos a la organización se registren para obtener la revisión a través de la dirección URL pública o el código incrustado.

        Cuando se selecciona esta opción, **el suscriptor debe hacer clic en un vínculo de un mensaje de correo electrónico para acceder a una revisión** que también está disponible. Seleccione esta opción para solicitar al revisor externo que haga clic en un vínculo del correo electrónico para acceder a la prueba.
Esta opción está habilitada de manera predeterminada si se selecciona la opción **Uso compartido público**.

      * **Función predeterminada para los nuevos revisores invitados:** Seleccione una función de prueba predeterminada para los revisores invitados. Las opciones son las mismas que las de **Función de prueba predeterminada**, excepto Moderador y Autor.

   * En la sección **[!UICONTROL Configuración predeterminada de alertas de correo electrónico]**:

      * **Alerta de correo electrónico predeterminada:** Seleccione la frecuencia con la que el usuario recibe actualizaciones por correo electrónico. Seleccione **Toda la actividad, Respuestas a mis comentarios, Decisiones, Decisión final, Resumen por hora, Resumen diario,** o **Deshabilitado**.

        Para obtener más información sobre las opciones predeterminadas de alertas por correo electrónico, consulte [Configurar la configuración de notificaciones por correo electrónico en [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Alerta de correo electrónico predeterminada para nuevos revisores invitados:** Seleccione la frecuencia con la que los revisores invitados recibirán actualizaciones de correo electrónico. Las opciones son las mismas que para la **alerta de correo electrónico predeterminada.**

      * **Enviar un mensaje de correo electrónico de confirmación cuando las pruebas estén listas:** Seleccione esta opción para enviar automáticamente un mensaje de correo electrónico de confirmación al usuario cuando las pruebas estén listas.
      * **Formato de los mensajes de correo electrónico enviados a este usuario:** Seleccione **[!UICONTROL HTML]** o **[!UICONTROL Texto sin formato]** como formato predeterminado para los mensajes de correo electrónico enviados al usuario.

   * En la sección **[!UICONTROL Configuración de mensaje personalizada]**: cree la configuración para las plantillas de prueba.

     Para obtener más información sobre las plantillas, consulte:

      * **Plantilla de asunto de prueba:** Cree una plantilla para un asunto de prueba.
      * **Plantilla de mensaje de prueba:** Cree una plantilla para un mensaje de prueba y su formato.
