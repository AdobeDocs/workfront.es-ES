---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Inicio de sesión único en  [!DNL Workfront Proof]: configuración de AD FS'
description: Si es administrador del servidor de AD, puede instalar y configurar AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: 690b0817dfe4ff200982ffe8d67ad93e563e30ac
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 98%

---

# Inicio de sesión único en [!DNL Workfront Proof]: configuración de AD FS

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si es administrador del servidor de AD, puede instalar y configurar AD FS.

## Instalación y configuración de AD FS

1. Descargue Microsoft AD FS 2.0 en su equipo.
1. Abra el archivo descargado AdfsSetup.exe para iniciar el asistente para instalación de ADFS (Servicios de federación de Active Directory).
1. En la pantalla Función de servidor, seleccione una de las opciones (necesita, como mínimo, un servidor de federación).
1. Si no desea exponer IIS en el servidor de AD a Internet (puertos 80 y 443 para HTTP y HTTPS), primero puede configurar un servidor de federación detrás del cortafuegos, a continuación, crear un segundo proxy de servidor de federación que pase solicitudes a través del cortafuegos al servidor de federación.
1. Una vez completada la configuración de AD FS, seleccione **[!UICONTROL Iniciar el complemento Administración de AD FS 2.0]** y, a continuación, haga clic en **[!UICONTROL Finalizar]**. Una vez finalizado, la ventana Administración de AD FS 2.0 debería abrirse de inmediato. Si no, puede abrirlo desde **[!UICONTROL Inicio]** > **[!UICONTROL Herramientas administrativas]** > **[!UICONTROL Administración de AD FS 2.0]**. Esta es la aplicación de control principal de AD FS.

1. Para comenzar, haga clic en Asistente de configuración del servidor de federación de AD FS 2.0.
Esto le ayudará a configurar AD FS y conectarlo a Internet a través de IIS y a AD.
1. Si está configurando un nuevo servidor de AD FS, seleccione **[!UICONTROL Crear un nuevo Servicio de federación]**.
1. Seleccione **[!UICONTROL Servidor de federación independiente]** (con fines de prueba y evaluación).

1. Para obtener una alta disponibilidad y equilibrio de carga, haga clic en Nueva granja de servidores de federación.
1. Especifique el nombre del Servicio de federación.
De forma predeterminada, el asistente de configuración recupera el certificado SSL enlazado al sitio web predeterminado en IIS y utilizará el nombre de sujeto especificado allí. Si usa un certificado comodín, tendrá que introducir el nombre del Servicio de federación.
Si no hay ningún certificado SSL configurado en IIS, el asistente para configuración buscará certificados válidos en el almacén de certificados del equipo local. Estos se muestran en la lista desplegable Certificado SSL. Si no se encuentran certificados, puede utilizar el Generador de certificados de servidor en IIS para crear uno.

1. Continúe con la configuración y haga clic en **[!UICONTROL Cerrar]** una vez que se haya completado.

## Configurando [!DNL Workfront Proof] inicio de sesión único

Si es administrador de [!DNL Workfront Proof], puede configurar el inicio de sesión único en el lado [!DNL Workfront Proof]. Para obtener más información, consulte [Inicio de sesión único en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** y, a continuación, abra la pestaña **[!UICONTROL Inicio de sesión único]**.

1. En el cuadro **URL de SSO**, pegue su ID de entidad.
El siguiente es un ejemplo de ID de entidad:
http://*&lt;adfs.your-company.com>*/adfs/services/trust
Su ID de entidad se encuentra en el archivo XML de metadatos de federación.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Los metadatos de federación se encuentran en la carpeta Complemento AD FS 2.0 > Servicio > Puntos finales. En la sección Metadatos, busque el que tenga el tipo Metadatos de federación. Para ver los metadatos, pegue este punto final en el explorador. También puede ir directamente a este vínculo: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml después de reemplazar {adfs.your-company.com} por sus propios datos.
1. En el cuadro **[!UICONTROL URL de inicio de sesión]**, pegue su inicio de sesión SSO.
1. El siguiente es un ejemplo de inicio de sesión SSO:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Este vínculo se encuentra en el archivo XML de metadatos de federación.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. En el cuadro **[!UICONTROL URL de cierre de sesión]**, introduzca el vínculo y guarde.
El siguiente es un ejemplo de URL de cierre de sesión:
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Vaya a su administrador de AD FS > Relaciones de confianza > Confianza de usuarios de confianza: Propiedades de ProofHQ.
   1. En los puntos finales, haga clic en [!UICONTROL Añadir y entrada] con los siguientes detalles:

      * Tipo de punto final = Cierre de sesión de SAML
      * Enlace = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Se puede completar este paso después de configurar la confianza de usuarios de confianza (ver a continuación) en su AD FS.
   1. En el cuadro **[!UICONTROL Huella digital del certificado]**, introduzca los datos del certificado.
   1. Vaya al complemento ADFS 2.0 y vaya a Servicio > Certificados > Firma de tokens.
   1. Haga clic con el botón derecho en esta entrada para ver el certificado.
   1. Desde la pestaña [!UICONTROL Detalles del certificado], copie la huella digital y péguela en la pestaña de configuración **[!UICONTROL Inicio de sesión único de Workfront Proof]**.

   1. Los caracteres de la huella digital se pueden separar con dos puntos o espacios, pero se recomienda eliminarlos. Si tiene algún problema con la configuración del inicio de sesión único, póngase en contacto con el equipo de atención al cliente.


## Adición de una confianza de usuarios de confianza

Una vez completada la configuración, debe trabajar en la sección Confianza de usuarios de confianza en el AD FS.

1. Vaya a **[!UICONTROL Relaciones de confianza]** > **[!UICONTROL Confianza de usuarios de confianza]** y, a continuación, haga clic en **[!UICONTROL Añadir una confianza de usuarios de confianza]** para iniciar el asistente de configuración.

1. Seleccione la fuente de datos.
Todos los metadatos de su cuenta de [!DNL ProofHQ] se encuentran en un vínculo como este:
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Esto configurará la mayor parte de la confianza del usuarios de confianza.

   >[!NOTE]
   >
   >* Si tiene problemas para establecer la conexión desde la URL, guarde los metadatos como un archivo y elija importar los datos de un archivo.
   >* Cuando tenga un dominio personalizado completo (por ejemplo, www.your-proofing.com) configurado en su cuenta de [!DNL ProofHQ], reemplace toda la parte &quot;{yoursubdomain}.proofhq.com&quot; por su propio dominio para crear el vínculo de metadatos [!DNL ProofHQ].


## Configurar reglas de notificación

Una vez completada la configuración de la confianza de usuarios de confianza, puede configurar las reglas de notificación para completar la configuración. Configurará dos reglas de notificación para ProofHQ: correo electrónico e ID de nombre.

1. Abra el cuadro de diálogo **[!UICONTROL Editar reglas de notificación]**.
1. Vaya a **[!UICONTROL Confianza de usuarios de confianza de ProofHQ]** y haga clic en **[!UICONTROL Editar reglas de reclamación]** (1).\
   La ventana emergente debería abrirse automáticamente si ha seleccionado esta opción al final de la configuración de la confianza.

1. Haga clic en **[!UICONTROL Añadir regla]** (2) para abrir la ventana de configuración de notificación.

   * Correo electrónico (enviar atributos LDAP como plantilla de regla de notificaciones)
   * NameID (Transformar una plantilla de regla de notificación entrante)
