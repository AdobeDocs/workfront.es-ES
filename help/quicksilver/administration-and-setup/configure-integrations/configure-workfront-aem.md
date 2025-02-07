---
title: Configurar  [!DNL Workfront] con [!DNL Adobe Experience Manager] conector heredado
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador de  [!DNL Adobe Workfront] puede integrar [!DNL Workfront] con Adobe Experience Manager (AEM) Assets y proporcionar a su organización una solución completa de administración de contenido para la creación, el uso compartido y el mantenimiento de recursos dentro de su flujo de trabajo.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1877'
ht-degree: 99%

---

# Configurar [!DNL Workfront] con el conector heredado de [!DNL Adobe Experience Manager]

Como administrador de [!DNL Adobe Workfront] puede integrar [!DNL Workfront] con [!UICONTROL Adobe Experience Manager (AEM) Assets] y proporcionar a su organización una solución completa de administración de contenido para la creación, el uso compartido y el mantenimiento de recursos dentro de su flujo de trabajo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

+++

## [!DNL Workfront for AEM Assets]

[!DNL Workfront for AEM Assets connector] permite que su organización haga lo siguiente:

* Colaborar y administrar contenido creativo vinculando recursos y carpetas de AEM a proyectos, tareas, problemas y solicitudes en [!DNL Workfront].

  Para obtener más información sobre cómo configurar las integraciones de documentación con aplicaciones de terceros, consulte [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrar con el repositorio [!DNL AEM Digital Asset Managemen]t (DAM), lo que le permite usar [!DNL Workfront] para administrar y compartir recursos digitales almacenados en DAM.

  Para obtener más información sobre la vinculación de documentos y carpetas de recursos, consulte [Enlazar documentos a partir de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combinar y aplicar metadatos de ambas aplicaciones a un recurso.
* Ver un flujo de comunicación inclusivo para un recurso. Las actualizaciones y los comentarios realizados en un recurso ya sea en [!DNL Workfront] o en [!UICONTROL AEM Assets] se sincronizan con la otra aplicación, lo que establece un historial completo de las comunicaciones realizadas en el recurso.

  Para obtener más información acerca de cómo realizar comentarios en [!DNL Workfront], consulte [Añadir una actualización a un documento](../../documents/managing-documents/add-update-documents.md).

## Requisitos previos para instalar el conector de [!DNL AEM Assets]

Antes de instalar el conector de [!DNL Workfront] para [!UICONTROL AEM Assets], asegúrese de que se cumplan los siguientes requisitos previos:

* [!UICONTROL AEM Assets] está instalado y configurado, versión 6.5 o posterior. Para obtener información sobre la instalación de [!UICONTROL AEM Assets], consulte la [[!DNL Adobe Experience Manager] documentación](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Condicional) Si las reglas del cortafuegos no permiten el tráfico tal como esperaba, añada la dirección IP o el dominio del clúster a la lista de permitidos. Para obtener más información, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Instalar el paquete del conector de [!DNL Workfront for AEM Assets] {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Las siguientes instrucciones son para un conector de [!DNL Workfront with AEM Assets] heredado que ha sido reemplazado por el conector mejorado de [[!DNL Workfront for Experience Manager] ](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Póngase en contacto con su representante de cuenta para obtener más información.

Para instalar el conector de [!DNL Workfront for AEM Assets], debe importarlo en AEM como un paquete mediante el [!UICONTROL Administrador de paquetes de CRX].

1. En una estación de trabajo en la que ya haya instalado AEM, descargue el archivo de instalación del conector de [!DNL Workfront for AEM Assets].

   Puede obtener el conector de [!DNL Workfront for AEM Assets] a través de su representante de [!DNL Workfront].

1. Inicie sesión en AEM con una cuenta de administrador.
1. Haga clic en **[!UICONTROL Herramientas]** > **[!UICONTROL Implementación]** > **[!UICONTROL Paquetes]**.

   Se abre el [!UICONTROL Administrador de paquetes de CRX].

1. Haga clic en **[!UICONTROL Cargar paquete].**

1. En el cuadro de diálogo [!UICONTROL Cargar paquete], busque y seleccione el paquete [!UICONTROL Workfront Connector] y, a continuación, haga clic en **[!UICONTROL Aceptar]**.\
   El paquete se muestra en el [!UICONTROL Administrador de paquetes de CRX].

1. Haga clic en **[!UICONTROL Instalar].**

1. En el cuadro de diálogo [!UICONTROL Paquete], ignore los ajustes avanzados y haga clic en **[!UICONTROL Instalar]**.
1. (Opcional) Para confirmar que el conector se ha instalado correctamente, asegúrese de que la siguiente instrucción se muestra en el [!UICONTROL Registro de actividades]:

   ```
   Package installed in <time>
   ```

1. Cierre el [!UICONTROL Administrador de paquetes de CRX].

   El conector está instalado y ahora puede configurar [!DNL AEM Assets] para integrarlo con [!DNL Workfront].

1. Continuar con [Configurar [!DNL AEM Assets] para integrar con [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Configurar [!DNL AEM Assets] para integrarlo con [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Después de instalar el conector, importe el paquete del conector en AEM y configure AEM para que se vincule con los documentos de [!DNL Workfront].

Para obtener información sobre la instalación del conector, consulte [Instalar el [!DNL Workfront for AEM Assets] paquete del conector](#install-the-workfront-for-aem-assets-connector-package).

* [Requisitos previos](#prerequisites)
* [Integrar AEM con [!DNL Workfront]](#integrate-aem-with-workfront)
* [Configurar el [!UICONTROL Externalizador AEM]](#configure-the-aem-externalizer)

### Requisitos previos {#prerequisites}

Antes de empezar, debe habilitar los permisos para workfront-service:

1. En AEM, vaya a **[!UICONTROL Herramientas]**> **[!UICONTROL Seguridad]**> **[!UICONTROL Permisos]**.
1. En la esquina superior izquierda, elija **[!UICONTROL Usuarios]** en el menú desplegable e indique *[!UICONTROL servicio de Workfront]* en el campo **[!UICONTROL Buscar]**. Seleccione el usuario [!UICONTROL workfront-service].
1. En el lado derecho de la pantalla, seleccione **[!UICONTROL Añadir ACE]** para crear nuevas entradas.
1. En la ventana&#x200B;**[!UICONTROL Añadir nueva entrada]**, seleccione el icono de casilla de verificación en el campo **[!UICONTROL Ruta]** y elija la carpeta: */conf*
1. En el campo Privilegios escriba: *jcr:read*
1. Seleccione **[!UICONTROL Añadir]** en la esquina superior derecha
1. (Opcional) Repita los pasos para crear más entradas.

### Integrar AEM con [!DNL Workfront] {#integrate-aem-with-workfront}

1. Inicie sesión en AEM Assets como administrador.
1. Haga clic en **[!UICONTROL Herramientas]** >**[!UICONTROL Cloud Service]**>**[!UICONTROL Configuración de integración de Workfront]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Condicional) Si aún no lo ha hecho, cree un archivo de configuración de nube de [!DNL Workfront].

   1. Haga clic en **[!UICONTROL Crear]** en la esquina superior derecha de la página de [!DNL Global-Workfront].
   1. En el cuadro **[!UICONTROL URL de Workfront]**, especifique la URL de la instancia de [!DNL Workfront].

      Por ejemplo, [!DNL https]://`<account>`.my.workfront.com, donde `<account>` es la cuenta que usa para las integraciones con AEM.

   1. En el campo&#x200B;**[!UICONTROL Carpeta base]**, seleccione el icono de casilla de verificación y, a continuación, en el menú desplegable, seleccione la ruta en la que se almacenan los documentos vinculados a objetos [!DNL Workfront].
   1. En el modal de AEM que aparece, siga la ruta hasta la carpeta con los documentos conectados a objetos [!DNL Workfront]. Elija la carpeta y presione **[!UICONTROL Seleccionar]** en la esquina superior derecha.

      Puede vincular a cualquier carpeta debajo de la raíz /content/dam/.

   1. En el cuadro **[!UICONTROL Clave de API de Workfront]**, especifique su clave de API de [!UICONTROL Workfront].

      Para recuperar su clave de API de [!DNL Workfront]:

      1. Abra una pestaña del explorador e inicie sesión en su cuenta de [!DNL Workfront] como administrador de [!DNL Workfront].

      {{step-1-to-setup}}

      1. Haga clic en **[!UICONTROL Sistema]** >**[!UICONTROL Información del cliente]**.

         Si ya ha generado una clave de API, la clave de API de [!DNL Workfront] se muestra en la etiqueta Clave de API del usuario.

      1. (Condicional) Si aún no ha generado una clave de API, debe generar una:

         1. En la sección **[!UICONTROL Configuración de clave API]**, asegúrese de que la opción **[!UICONTROL Después de la creación, las claves API caducan en]** esté establecida en Ninguno.

            Si selecciona un periodo de caducidad, el conector dejará de funcionar una vez que caduque la clave de API. Tendrá que volver a generar una clave de API y actualizar la configuración de [!DNL Workfront].

         1. En la etiqueta **[!UICONTROL Su clave API de usuario]**, haga clic en **[!UICONTROL Generar clave API]**.

            Se genera y se muestra una clave API para [!DNL Workfront].
      1. Copie la clave API en el portapapeles.
      1. Abra la pestaña del explorador correspondiente al conector AEM y, en el cuadro **[!DNL Workfront API Key]**, pegue la clave de API que ha copiado.
   1. (Condicional) Haga clic en la pestaña **[!UICONTROL Avanzado]** en la esquina superior izquierda de la página [!UICONTROL [!DNL Workfront] Configuración de integración] y seleccione las siguientes opciones si corresponde:

      **[!UICONTROL Permitir exploración de colecciones]:** seleccione esta opción si su organización permite que usuarios de [!DNL Workfront] vinculen colecciones de AEM Assets a [!DNL Workfront] objetos.

      **[!UICONTROL Federated ID de usuarios]:** seleccione esta opción si su organización utiliza Federated ID o un inicio de sesión único (SSO) al iniciar sesión en Workfront.

      **[!UICONTROL Omitir dominio de correo electrónico]:** seleccione esta opción si los usuarios de AEM no utilizan el nombre de dominio en su identificador de usuario.

      **[!UICONTROL Restringir el acceso]:** seleccione esta opción para especificar las direcciones IP de [!DNL Workfront] apropiadas que deben añadirse a la lista de permitidos. Para obtener más información acerca de la lista de permitidos, consulte [Configuración de la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Haga clic en la pestaña **[!UICONTROL Básico]** en la esquina superior izquierda de la página Configuración de integración de Workfront y, a continuación, haga clic en **[!UICONTROL Conectar]**.

      >[!NOTE]
      >
      >Los cambios pueden tardar un poco en aplicarse. El reinicio del paquete puede acelerar el proceso.



1. (Condicional) Si ya creó un archivo de configuración de nube de [!DNL Workfront], seleccione **[!UICONTROL Global-[!DNL Workfront]]** y, a continuación, en la esquina superior izquierda, haga clic en **[!UICONTROL Propiedades]**.

1. Genere la clave API de AEM haciendo clic en **[!UICONTROL Generar clave],** y, a continuación, copie la clave API de AEM en el portapapeles.

   Más adelante necesitará la clave API de AEM para configurar [!UICONTROL Workfront] y que se integre con [!UICONTROL AEM Assets]. Para obtener más información, consulte [Configurar Workfront para integrarlo con AEM Assets](#configure-workfront-to-integrate-with-aem-assets).

1. En la esquina superior derecha, haga clic en **[!UICONTROL Guardar]**.

   Se muestra la ventana [!UICONTROL Global-[!DNL Workfront]].

   ![Properties.png](assets/properties-350x117.png)

1. (Opcional) Sincronice la comunicación bidireccional entre AEM y [!DNL Workfront].

   1. Haga clic en **[!UICONTROL Global-[!DNL Workfront]].**
   1. En la esquina superior izquierda de la ventana, haga clic en **[!UICONTROL Propiedades]**.

      Se muestra la página [!UICONTROL [!DNL Workfront] Integration Configuration].

      ![Properties2.png](assets/properties2-350x444.png)

   1. (Opcional) Para habilitar la sincronización de comentarios entre [!UICONTROL AEM Assets] y [!DNL Workfront], haga clic en **[!UICONTROL Habilitar sincronización de comentarios]**.

      >[!IMPORTANT]
      >
      >Debe habilitar [!UICONTROL Sincronizar documentos] para sincronizar los recursos.

   1. (Opcional) Para desactivar la sincronización de comentarios, haga clic en **[!UICONTROL Deshabilitar sincronización de comentarios].**

      O

      Elimine la suscripción al evento [!UICONTROL NOTE CREATE] registrada en la instancia de AEM.

      Para obtener información sobre las suscripciones a eventos, consulte [API de suscripción a eventos](../../wf-api/general/event-subs-api.md).

1. Continúe con [Configure the [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Configurar el [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

El [!UICONTROL AEM Externalizer] permite que AEM pase direcciones URL en un formato que se puede usar en [!DNL Workfront]. Si no se configura correctamente, [!DNL Workfront] no puede realizar llamadas a la API de AEM y las direcciones URL que vinculan documentos de AEM en Workfront no funcionarán.

1. En AEM, haga clic en **[!UICONTROL Herramientas]** > **[!UICONTROL Operaciones]** > **[!UICONTROL Consola web]**.

1. Haga clic en **[!UICONTROL OSGI]** y, a continuación, haga clic en **[!UICONTROL Configuración]** en el menú desplegable.

1. En la lista de configuración, seleccione **[!UICONTROL Externalizador de vínculo CQ por día].**

   Se muestra la página [!UICONTROL Externalizer].

1. En la sección **[!UICONTROL Dominios]**, asegúrese de que el dominio que aparece en el campo [!UICONTROL Autor] sea el nombre de dominio al que los usuarios de AEM pueden acceder externamente.

   El nombre de dominio en el campo [!UICONTROL Autor] debe coincidir con el dominio que aparece en la línea URL de la instancia de AEM.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Condicional) Si es necesario, actualice el dominio en el campo [!UICONTROL Autor].
1. Haga clic en **[!UICONTROL Guardar]**.

   [!UICONTROL AEM Assets] ya está configurado para vincular documentos con [!DNL Workfront]

1. Continúe con [Configure [!DNL Workfront] to integrate with [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Configurar [!DNL Workfront] para integrarlo con [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Después de instalar el conector de [!UICONTROL Workfront for AEM Assets] (como se describe en [Instalar el paquete del conector [!UICONTROL Workfront for AEM Assets]](#install-the-workfront-for-aem-assets-connector-package)) y configurar [!UICONTROL AEM Assets] (como se describe en [Configurar[!UICONTROL  AEM Assets] para integrarlo con [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), debe configurar [!DNL Workfront] para vincular documentos entre [!DNL Workfront] y [!DNL AEM Assets].

1. Inicie sesión en [!DNL Workfront] como administrador de [!UICONTROL Workfront].

   >[!TIP]
   >
   >[!UICONTROL Workfront] recomienda crear un administrador de [!UICONTROL Workfront] dedicado exclusivamente a la integración de AEM. Para obtener más información sobre cómo asignar el nivel de acceso de administrador de [!UICONTROL Workfront] a un usuario, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Documentos]**> **[!UICONTROL Integración personalizada].**

1. Haga clic en **[!UICONTROL Agregar integración personalizada]**.
1. En el cuadro **[!UICONTROL Nombre]**, especifique el nombre de la integración personalizada.

   Este es el nombre que ven los usuarios cuando usan la integración en [!UICONTROL Workfront]; por ejemplo, podría escribir *&quot;[!DNL AEM Assets]&quot;* para el nombre.

1. En el cuadro **[!UICONTROL Dirección URL de API básica]**, especifique la dirección URL de la instancia de AEM.

   La dirección URL de API básica consiste en la dirección URL de la instancia de AEM seguida de la ruta: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. En el menú desplegable **[!UICONTROL Tipo de autenticación]**, seleccione **[!UICONTROL ApiKey].**

1. En el cuadro **[!UICONTROL Clave de API]**, pegue la Clave de API de AEM que copió cuando configuró [!UICONTROL AEM Assets].
1. Haga clic en **[!UICONTROL Guardar]**.
1. (Opcional) Asegúrese de que la integración esté marcada como [!UICONTROL Activa].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] ya está configurado para trabajar con [!DNL AEM Assets].

   Para tener acceso a los recursos en AEM, cada usuario de [!DNL Workfront] que necesite utilizar el conector debe estar configurado como usuario en AEM. Para obtener información sobre cómo crear usuarios, consulte [Configurar usuarios para que utilicen el conector](#set-up-users-to-use-the-connector).

## Configurar usuarios para que utilicen el conector {#set-up-users-to-use-the-connector}

Para que los usuarios puedan acceder al conector, deben tener un perfil de usuario en AEM y pertenecer a un grupo de [!DNL Workfront] con niveles de acceso que incluyan los permisos para [!UICONTROL Crear] y [!UICONTROL Eliminar].

Para obtener más información sobre los permisos de [!DNL Workfront], consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Configurar usuarios en  [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Configurar usuarios en [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Inicie sesión en [!DNL AEM Assets] como administrador de [!DNL Workfront].
1. Haga clic en **[!UICONTROL Herramientas]** >**&#x200B;**&#x200B;**[!UICONTROL Seguridad]** >**[!UICONTROL Usuarios]**.

1. (Condicional) Si el usuario no tiene un perfil de usuario en AEM, cree un un perfil de usuario de AEM.

   1. Haga clic en **[!UICONTROL Crear usuario].**
   1. Introduzca la información personal del usuario.

      ![64NewUser.png](assets/64newuser-350x524.png)

      El único campo obligatorio es el campo de ID. El identificador AEM del usuario debe coincidir con su identificador de [!DNL Workfront], que es la dirección de correo electrónico de [!DNL Workfront] del usuario.

      Si seleccionó la opción [!UICONTROL Ignorar dominio de correo electrónico] al configurar la integración de AEM con [!DNL Workfront], entonces el identificador de AEM no coincidirá con la dirección de correo electrónico de [!DNL Workfront].

1. (Condicional) Si el usuario tiene un perfil de AEM, abra el perfil de AEM del usuario.

   1. Haga clic en **[!UICONTROL Usuario].**

      Se muestra la página [!UICONTROL Administración de usuarios].

   1. Haga clic en el usuario que desee añadir y luego haga clic en **[!UICONTROL Propiedades]**.

      Se muestra la página de configuración del usuario.

1. Haga clic en la pestaña **[!UICONTROL Grupos]**.

   ![Pestaña Grupos](assets/groupstab.png)

1. Asegúrese de que el usuario pertenezca al menos a un grupo de [!DNL Workfront] con niveles de acceso que incluyan los permisos para [!UICONTROL Crear] y [!UICONTROL Eliminar].

   1. Para añadir el usuario a un grupo existente, empiece a escribir el nombre del grupo en el cuadro **[!UICONTROL Escriba el nombre del grupo]** y, a continuación, seleccione el grupo cuando aparezca en el menú desplegable.

      O

      Para seleccionar un grupo del que el usuario ya es integrante, seleccione un grupo en la sección **[!UICONTROL Grupos a los que pertenece este usuario]**.

1. Haga clic en **[!UICONTROL Guardar].**
