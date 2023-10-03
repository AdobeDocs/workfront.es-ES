---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurar la información de usuario mediante [!DNL Workfront Proof]
description: Configurar la información de usuario mediante [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Configurar la información de usuario mediante [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

1. Comience a crear o editar un usuario como se describe en [Crear usuarios con [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Especifique la siguiente información:

   * En el **[!UICONTROL Datos personales]** sección:

      * **Correo electrónico:** La dirección de correo electrónico del usuario.
      * **Nombre:** El nombre del usuario.
      * **Apellidos:** El apellido del usuario.
      * **Posición:** La posición del usuario en la compañía.
      * **Perfil de permisos:** Los permisos del usuario en la cuenta de revisión.
      * **Idioma:** El idioma principal del usuario.
      * **Zona horaria:** Seleccione la zona horaria del usuario.
      * **Formato de fecha:** Seleccione el formato de fecha preferido del usuario.
      * **Inclusión - Correos electrónicos de producto y marketing:** Seleccione si desea que el usuario esté incluido en los correos electrónicos de marketing y productos.
      * **Solo API:** Permite al usuario iniciar sesión únicamente mediante la API.

   * En el **[!UICONTROL Detalles del usuario]** , escriba la información de contacto del usuario, como la dirección y el número de teléfono.
   * En el **[!UICONTROL Configuración de prueba predeterminada]** , configure las opciones que afectan a la forma en que el usuario crea o trabaja en las pruebas.

      * **Función de prueba predeterminada:** Seleccione una función de prueba predeterminada para el usuario. Las opciones de rol son **[!UICONTROL Solo lectura]**, **[!UICONTROL Revisor]**, **[!UICONTROL Aprobador]**, **[!UICONTROL Revisor y aprobador]**, **[!UICONTROL Autor]**, o **[!UICONTROL Moderador]**.

        Para obtener más información sobre las funciones de prueba, consulte [Administración de funciones de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Bloquear la prueba cuando se tomen todas las decisiones:** Bloquea automáticamente la prueba en caso de nuevos cambios una vez que se han tomado todas las decisiones al respecto.
      * **Debe iniciar sesión. La revisión solo se puede compartir con otros usuarios:** Hace que la prueba solo esté disponible para los usuarios con [!DNL Workfront Proof] credenciales de inicio de sesión.
      * **Solo se requiere una decisión:** Solo requiere una decisión sobre una prueba.
      * **Descargar archivo original:** Permite que el usuario descargue el archivo original para una prueba. Esta opción está habilitada de forma predeterminada.

        Para obtener más información sobre la descarga de archivos originales, consulte [Descargar archivos almacenados en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Suscripción. Se puede suscribir a la prueba mediante la URL pública o el código para insertar:** Permite a los revisores externos a la organización registrarse para la prueba mediante la URL pública o el código incrustado.

        Cuando se selecciona esta opción, **El suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba** también está disponible. Seleccione esta opción para solicitar al revisor externo que haga clic en un vínculo del correo electrónico para acceder a la prueba.
Esta opción está habilitada de forma predeterminada si la variable **Uso compartido público** La opción está seleccionada.

      * **Función predeterminada para los nuevos revisores invitados:** Seleccione una función de prueba predeterminada para los revisores invitados. Las opciones son las mismas que en **Función de prueba predeterminada**, excepto Moderador y Autor.

   * En el **[!UICONTROL Configuración predeterminada de alertas de correo electrónico]** sección:

      * **Alerta de correo electrónico predeterminada:** Seleccione la frecuencia con la que el usuario recibe actualizaciones por correo electrónico. Seleccionar **Toda la actividad, Respuestas a mis comentarios, Decisiones, Decisión final, Resumen por hora, Resumen diario,** o **Desactivado**.

        Para obtener más información sobre las opciones predeterminadas de alerta por correo electrónico, consulte [Configuración de notificaciones por correo electrónico en [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Alerta de correo electrónico predeterminada para nuevos revisores invitados:** Seleccione la frecuencia con la que los revisores invitados reciben actualizaciones de correo electrónico. Las opciones son las mismas que para **Alerta de correo electrónico predeterminada.**

      * **Envíe un correo electrónico de confirmación cuando las pruebas estén listas:** Seleccione esta opción para enviar automáticamente un correo electrónico de confirmación al usuario cuando las pruebas estén listas.
      * **Formato de los correos electrónicos enviados a este usuario:** Seleccionar **[!UICONTROL HTML]** o **[!UICONTROL Texto sin formato]** como formato predeterminado para los correos electrónicos enviados al usuario.

   * En el **[!UICONTROL Configuración de mensaje personalizada]** sección: Crear configuraciones para plantillas de prueba.

     Para obtener más información sobre las plantillas, consulte:

      * **Plantilla del asunto de la prueba:** Cree una plantilla para un asunto de prueba.
      * **Plantilla de mensaje de prueba:** Cree una plantilla para un mensaje de prueba y su formato.
