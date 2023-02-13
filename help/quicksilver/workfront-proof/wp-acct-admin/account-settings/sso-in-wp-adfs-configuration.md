---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: '"Inicio de sesión único" [!DNL Workfront Proof]: Configuración de AD FS'''
description: Si es administrador en su servidor de AD, puede instalar y configurar AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Inicio de sesión único [!DNL Workfront Proof]: Configuración de AD FS

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Si es administrador en su servidor de AD, puede instalar y configurar AD FS.

## Instalación y configuración de AD FS

1. Descargar [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) al equipo.
1. Abra el archivo AdfsSetup.exe descargado para iniciar el asistente de instalación de ADFS (Servicios de federación de Active Directory).
1. En la pantalla Función del servidor, seleccione una de las opciones (necesita como mínimo un servidor de federación).
1. Si no desea exponer IIS en su servidor de AD a Internet (puertos 80 y 443 para HTTP y HTTPS), primero puede configurar un servidor de federación detrás del firewall y, a continuación, crear un segundo proxy de servidor de federación que pase las solicitudes a través del firewall al servidor de federación.
1. Una vez que complete la configuración de AD FS, seleccione **[!UICONTROL Inicie el complemento de administración de AD FS 2.0]** y haga clic en **[!UICONTROL Finalizar]**. Una vez completado esto, la ventana de administración de AD FS 2.0 se abrirá de inmediato. Si no es así, puede abrirlo desde **[!UICONTROL Inicio]** > **[!UICONTROL Herramientas administrativas]** > **[!UICONTROL Administración de AD FS 2.0]**. Esta es la aplicación de control principal de AD FS.

1. Para empezar, haga clic en el Asistente para la configuración del servidor de federación de AD FS 2.0 .
Esto le ayudará a configurar AD FS y a conectarlo a Internet a través de IIS y a AD.
1. Si está configurando un nuevo servidor AD FS, seleccione **[!UICONTROL Crear un nuevo servicio de federación]**.
1. Select **[!UICONTROL Servidor de federación independiente]** (con fines de ensayo y evaluación).

1. Para obtener una alta disponibilidad y equilibrio de carga, haga clic en New federation server farm.
1. Especifique el nombre del Servicio de federación.
De forma predeterminada, el asistente de configuración recupera el certificado SSL enlazado al sitio web predeterminado en IIS y utiliza el nombre de asunto especificado en él. Si utiliza un certificado comodín, deberá introducir el nombre del Servicio de federación.
Si no hay ningún certificado SSL configurado en IIS, el asistente de configuración buscará certificados válidos en el almacén de certificados del equipo local. Se muestran en la lista desplegable de certificados SSL. Si no se encuentran certificados, puede usar el Generador de certificados de servidor en IIS para crear uno.

1. Continúe con la configuración y haga clic en **[!UICONTROL Cerrar]** una vez finalizada.

## Configuración [!DNL Workfront Proof] Inicio de sesión único

Si es [!DNL Workfront Proof] administrador, puede configurar el inicio de sesión único en el [!DNL Workfront Proof] lado. Para obtener más información, consulte [Inicio de sesión único [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** y, a continuación, abra el **[!UICONTROL Inicio de sesión único]** pestaña .

1. En el **URL de SSO** , pegue el identificador de entidad.
A continuación se muestra un ejemplo de un ID de entidad: http://*&lt;adfs.your-company.com>*/adfs/services/trust El identificador de entidad se encuentra en el archivo XML de metadatos de federación.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Los metadatos de federación se encuentran en la carpeta del complemento AD FS 2.0 > Service > Endpoints . En la sección Metadatos , busque el que tiene el tipo Metadatos de federación . Para ver los metadatos, pegue este punto final en el explorador. También puede ir directamente a este vínculo: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml después de reemplazar {adfs.your-company.com} por sus propios detalles.
1. En el **[!UICONTROL URL de inicio de sesión]** , pegue su inicio de sesión de SSO.
1. El siguiente es un ejemplo de inicio de sesión de SSO:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Este vínculo se encuentra en el archivo XML de metadatos de federación.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. En el **[!UICONTROL URL de cierre de sesión]** , introduzca el vínculo y guarde.
A continuación se muestra un ejemplo de una URL de cierre de sesión: https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Vaya a su administrador de AD FS > Relaciones de confianza > Fianzas de partes confiables - Propiedades de ProofHQ.
   1. En Puntos finales, haga clic en [!UICONTROL Agregar y entrada] con los siguientes detalles:

      * Tipo de extremo = cierre de sesión SAML
      * Enlace = POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * Este paso se puede completar después de configurar la confianza del fiador (consulte a continuación) en su AD FS.
   1. En el **[!UICONTROL Huella digital del certificado]** , introduzca los datos del certificado.
   1. Vaya a su complemento de ADFS 2.0 , vaya a Servicio > Certificados > Firma de tokens.
   1. Haga clic con el botón derecho en esta entrada para ver el certificado.
   1. En el [!UICONTROL Detalles del certificado] copie la huella digital y péguela en la pestaña **[!UICONTROL Inicio de sesión único de prueba de Workfront]** pestaña de configuración.

   1. Los caracteres de huella digital pueden separarse con dos puntos o espacios, pero se recomienda eliminarlos. Si tiene algún problema con la configuración de inicio de sesión único, póngase en contacto con el equipo de asistencia al cliente.


## Adición de una confianza de entidad de confianza

Una vez completada la configuración, debe trabajar en la sección Confiar en las Fianzas de Parte en su AD FS.

1. Vaya a **[!UICONTROL Relaciones de confianza]** > **[!UICONTROL Confiar en las confianzas del partido]** carpeta y, a continuación, haga clic en **[!UICONTROL Añadir una confianza de entidad de confianza]** para iniciar el asistente de configuración.

1. Seleccione la fuente de datos.
Todos los metadatos para su [!DNL ProofHQ] La cuenta se encuentra bajo un vínculo como este: https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq Esto configurará la mayor parte de Confiying Party Trust.

   >[!NOTE]
   >
   >* Si tiene problemas para establecer la conexión desde la dirección URL, guarde los metadatos como un archivo y elija importar datos de un archivo.
   >* Cuando tiene un dominio personalizado completo (por ejemplo, www.your-proofing.com) configurado en su [!DNL ProofHQ] la cuenta reemplazará toda la parte &quot;{yoursubdomain}.proofhq.com&quot; con su propio dominio para crear su [!DNL ProofHQ] vínculo de metadatos.



## Configuración de reglas de reclamación

Una vez completada la configuración de Confiar en el Fiduciario, está listo para configurar las reglas de reclamo para completar la configuración. Configurará dos reglas de reclamo para ProofHQ: Correo electrónico e ID de nombre.

1. Abra el **[!UICONTROL Editar reglas de solicitud]** para abrir el Navegador.
1. Vaya a **[!UICONTROL ProofHQ Confiando en la Parte]** y haga clic en **[!UICONTROL Editar reglas de solicitud]** (1)\
   La ventana emergente se abrirá automáticamente si ha seleccionado esta opción al final de la configuración de la confianza.

1. Haga clic en **[!UICONTROL Agregar regla]** (2) para abrir la ventana de configuración de la reclamación.

   * Correo electrónico (Enviar atributos LDAP como plantilla de regla de Reclamaciones)
   * NameID (Transformar una plantilla de regla de solicitud entrante)
