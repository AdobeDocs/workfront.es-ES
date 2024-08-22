---
title: Configurar  [!DNL Workfront] con [!DNL Adobe Experience Manager] conector heredado
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador de  [!DNL Adobe Workfront] puede integrar [!DNL Workfront] con Adobe Experience Manager AEM () Assets y proporcionar a su organización una solución completa de administración de contenido para la creación, el uso compartido y el mantenimiento de recursos dentro de su flujo de trabajo.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 0%

---

# Configurar [!DNL Workfront] con [!DNL Adobe Experience Manager] conector heredado

Como administrador de [!DNL Adobe Workfront], puede integrar [!DNL Workfront] con [!UICONTROL Adobe Experience Manager AEM () Assets] y proporcionar a su organización una solución completa de administración de contenido para la creación, el uso compartido y el mantenimiento de recursos dentro de su flujo de trabajo.

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
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

+++

## [!DNL Workfront for AEM Assets]

[!DNL Workfront for AEM Assets connector] permite que su organización haga lo siguiente:

* AEM Colabore y administre contenido creativo vinculando recursos y carpetas de recursos a proyectos, tareas, problemas y solicitudes en [!DNL Workfront].

  Para obtener más información sobre cómo configurar integraciones de documentación con aplicaciones de terceros, consulte [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integre con el repositorio [!DNL AEM Digital Asset Managemen]t (DAM), lo que le permite usar [!DNL Workfront] para administrar y compartir recursos digitales almacenados en DAM.

  Para obtener más información sobre la vinculación de documentos y carpetas de recursos, consulte   [Enlazar documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combine y aplique metadatos de ambas aplicaciones a un recurso.
* Vea un flujo de comunicación inclusivo para un recurso. Las actualizaciones y los comentarios realizados en un recurso en [!DNL Workfront] o [!UICONTROL AEM Assets] se sincronizan con la otra aplicación, lo que establece un historial completo de las comunicaciones realizadas en el recurso.

  Para obtener más información acerca de cómo realizar comentarios en [!DNL Workfront], vea [Agregar una actualización a un documento](../../documents/managing-documents/add-update-documents.md).

## Requisitos previos para instalar el conector [!DNL AEM Assets]

Antes de instalar el conector [!DNL Workfront] para [!UICONTROL AEM Assets], asegúrese de que se cumplan los siguientes requisitos previos:

* [!UICONTROL AEM Assets] instalado y configurado, versión 6.5 o posterior. Para obtener información acerca de la instalación de [!UICONTROL AEM Assets], consulte la [[!DNL Adobe Experience Manager] documentación](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Condicional) Si las reglas del cortafuegos no permiten el tráfico como se espera, agregue la dirección IP o el dominio del clúster a la lista de permitidos. Para obtener más información, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Instalar el paquete del conector [!DNL Workfront for AEM Assets] {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Las siguientes instrucciones son para un conector heredado [!DNL Workfront with AEM Assets] que ha sido reemplazado por el [[!DNL Workfront for Experience Manager] conector mejorado](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Póngase en contacto con el representante de su cuenta para obtener más información.

AEM Para instalar el conector [!DNL Workfront for AEM Assets], debe importarlo a como un paquete en la interfaz de usuario de [!UICONTROL Administrador de paquetes de CRX].

1. AEM En una estación de trabajo en la que ya haya instalado la instalación, descargue el archivo de instalación del conector [!DNL Workfront for AEM Assets].

   Puede obtener el conector [!DNL Workfront for AEM Assets] de su representante de [!DNL Workfront].

1. AEM Inicie sesión en la cuenta de usuario de administrador de para iniciar sesión en el.
1. Haga clic en **[!UICONTROL Herramientas]** > **[!UICONTROL Implementación]** > **[!UICONTROL Paquetes]**.

   Se abre [!UICONTROL Administrador de paquetes CRX].

1. Haga clic en **[!UICONTROL Cargar paquete].**

1. En el cuadro de diálogo [!UICONTROL Cargar paquete], busque y seleccione el paquete de [!UICONTROL Conector de Workfront], y luego haga clic en **[!UICONTROL Aceptar]**.\
   El paquete se muestra en [!UICONTROL CRX Package Manager].

1. Haga clic en **[!UICONTROL Instalar].**

1. En el cuadro de diálogo [!UICONTROL Paquete], ignore la configuración avanzada y haga clic en **[!UICONTROL Instalar]**.
1. (Opcional) Para confirmar que el conector se instaló correctamente, asegúrese de que se muestre la siguiente instrucción en el [!UICONTROL Registro de actividades]:

   ```
   Package installed in <time>
   ```

1. Cierre el [!UICONTROL Administrador de paquetes de CRX].

   El conector está instalado y ahora puede configurar [!DNL AEM Assets] para integrarlo con [!DNL Workfront].

1. Continuar con [Configurar [!DNL AEM Assets] para integrar con [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Configurar [!DNL AEM Assets] para que se integre con [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

AEM AEM Después de instalar el conector, importe el paquete del conector para que se pueda y configurar para que se vincule con los documentos de [!DNL Workfront].

Para obtener información sobre la instalación del conector, consulte [Instalar el [!DNL Workfront for AEM Assets] paquete del conector](#install-the-workfront-for-aem-assets-connector-package).

* [Requisitos previos](#prerequisites)
* [AEM Integrar la con  [!DNL Workfront]](#integrate-aem-with-workfront)
* [AEM Configurar el [!UICONTROL Externalizador de fechas ]](#configure-the-aem-externalizer)

### Requisitos previos {#prerequisites}

Antes de empezar, debe habilitar los permisos para workfront-service:

1. AEM En la, vaya a **[!UICONTROL Herramientas]**> **[!UICONTROL Seguridad]**> **[!UICONTROL Permisos]**.
1. En la esquina superior izquierda, elija **[!UICONTROL Usuarios]** en el menú desplegable e indique *[!UICONTROL servicio de Workfront]* en el campo **[!UICONTROL Buscar]**. Seleccione al usuario [!UICONTROL workfront-service].
1. En el lado derecho de la pantalla, seleccione **[!UICONTROL Agregar ACE]** para crear nuevas entradas.
1. En la ventana&#x200B;**[!UICONTROL Agregar nueva entrada]**, seleccione el icono de casilla de verificación en el campo **[!UICONTROL Ruta]** y elija la carpeta: */conf*
1. En el campo Privilegios escriba: *jcr:read*
1. Seleccione **[!UICONTROL Agregar]** en la esquina superior derecha
1. (Opcional) Repita los pasos para crear más entradas.

### AEM Integrar el con [!DNL Workfront] {#integrate-aem-with-workfront}

1. Inicie sesión en AEM Assets como administrador.
1. Haga clic en **[!UICONTROL Herramientas]** >**[!UICONTROL Cloud Service]**>**[!UICONTROL Configuración de integración de Workfront]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Condicional) Si aún no lo ha hecho, cree un archivo de configuración de nube de [!DNL Workfront].

   1. Haga clic en **[!UICONTROL Crear]** en la esquina superior derecha de la página [!DNL Global-Workfront].
   1. En el cuadro **[!UICONTROL URL de Workfront]**, especifique la URL de la instancia [!DNL Workfront].

      AEM Por ejemplo, [!DNL https]://`<account>`.my.workfront.com, donde `<account>` es la cuenta que usa para las integraciones con el servicio de identidad de los usuarios de la red de área de nombres de la red ().

   1. En el campo&#x200B;**[!UICONTROL Carpeta base]**, seleccione el icono de casilla de verificación y, a continuación, en el menú desplegable, seleccione la ruta en la que se almacenan los documentos vinculados a [!DNL Workfront] objetos.
   1. AEM En el modal de que aparece, siga la ruta a la carpeta con los documentos conectados a [!DNL Workfront] objetos. Elija la carpeta y presione **[!UICONTROL Seleccionar]** en la esquina superior derecha.

      Puede vincular a cualquier carpeta debajo de la raíz /content/dam/.

   1. En el cuadro **[!UICONTROL Clave de API de Workfront]**, especifique su clave de API [!UICONTROL Workfront].

      Para recuperar su clave de API [!DNL Workfront]:

      1. Abra una ficha del explorador e inicie sesión en su cuenta de [!DNL Workfront] como administrador de [!DNL Workfront].

      {{step-1-to-setup}}

      1. Haga clic en **[!UICONTROL Sistema]** >**[!UICONTROL Información del cliente]**.

         Si ya ha generado una clave de API, la clave de API [!DNL Workfront] se muestra en la etiqueta Clave de API del usuario.

      1. (Condicional) Si aún no ha generado una clave de API, debe generar una:

         1. En la sección **[!UICONTROL Configuración de clave API]**, asegúrese de que la opción **[!UICONTROL Después de la creación, las claves API caducan en]** esté establecida en Ninguno.

            Si selecciona un periodo de caducidad, el conector dejará de funcionar una vez que caduque la clave de API. Necesitará volver a generar una clave de API y actualizar la configuración de [!DNL Workfront].

         1. En la etiqueta **[!UICONTROL Su clave API de usuario]**, haga clic en **[!UICONTROL Generar clave API]**.

            Se genera y muestra una clave API para [!DNL Workfront].
      1. Copie la clave API en el portapapeles.
      1. AEM Abra la pestaña del explorador correspondiente al conector de la API de y, en el cuadro **[!DNL Workfront API Key]**, pegue la clave de API que ha copiado.
   1. (Condicional) Haga clic en la ficha **[!UICONTROL Avanzado]** en la esquina superior izquierda de la página [!UICONTROL [!DNL Workfront] Configuración de integración] y seleccione las siguientes opciones si corresponde:

      **[!UICONTROL Permitir exploración de colecciones]:** Seleccione esta opción si su organización permite que [!DNL Workfront] usuarios vinculen colecciones de AEM Assets a [!DNL Workfront] objetos.

      **[!UICONTROL Federated ID de usuarios]:** Seleccione esta opción si su organización utiliza Federated ID o un inicio de sesión único (SSO) al iniciar sesión en Workfront.

      AEM **[!UICONTROL Omitir dominio de correo electrónico]:** Seleccione esta opción si los usuarios de su cuenta de correo electrónico no utilizan el nombre de dominio en su identificador de usuario.

      **[!UICONTROL Restringir el acceso]:** Seleccione esta opción para especificar las [!DNL Workfront] direcciones IP apropiadas que deben agregarse a la lista de permitidos. Para obtener más información acerca de la lista de permitidos, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Haga clic en la ficha **[!UICONTROL Básico]** en la esquina superior izquierda de la página Configuración de integración de Workfront y, a continuación, haga clic en **[!UICONTROL Conectar]**.

      >[!NOTE]
      >
      >Los cambios pueden tardar algún tiempo en aplicarse. El reinicio del paquete puede acelerar el proceso.



1. (Condicional) Si ya creó un archivo de configuración de nube de [!DNL Workfront], seleccione **[!UICONTROL Global-[!DNL Workfront]]** y, a continuación, en la esquina superior izquierda, haga clic en **[!UICONTROL Propiedades]**.

1. AEM AEM Genere la clave API de la haciendo clic en **[!UICONTROL Generar clave],** y, a continuación, copie la clave API de la en el portapapeles.

   AEM Necesitará la clave API de la más adelante al configurar [!UICONTROL Workfront] para que se integre con [!UICONTROL AEM Assets]. Para obtener más información, consulte [Configuración de Workfront AEM para la integración con recursos de la](#configure-workfront-to-integrate-with-aem-assets).

1. En la esquina superior derecha, haz clic en **[!UICONTROL Guardar]**.

   Se muestra la ventana [!UICONTROL Global-[!DNL Workfront]].

   ![Propiedades.png](assets/properties-350x117.png)

1. AEM (Opcional) Sincronice la comunicación bidireccional entre los puntos de conexión de y de [!DNL Workfront].

   1. Haga clic en **[!UICONTROL Global-[!DNL Workfront]].**
   1. En la esquina superior izquierda de la ventana, haga clic en **[!UICONTROL Propiedades]**.

      Se muestra la página Configuración de la integración [!UICONTROL [!DNL Workfront]].

      ![Propiedades2.png](assets/properties2-350x444.png)

   1. (Opcional) Para habilitar la sincronización de comentarios entre [!UICONTROL AEM Assets] y [!DNL Workfront], haga clic en **[!UICONTROL Habilitar sincronización de comentarios]**.

      >[!IMPORTANT]
      >
      >Debe habilitar [!UICONTROL Sincronización de documentos] para sincronizar los recursos.

   1. (Opcional) Para desactivar la sincronización de comentarios, haga clic en **[!UICONTROL Deshabilitar sincronización de comentarios].**

      O

      AEM Elimine la suscripción de evento [!UICONTROL NOTE CREATE] registrada en la instancia de la.

      Para obtener información sobre las suscripciones a eventos, consulte [API de suscripción a eventos](../../wf-api/general/event-subs-api.md).

1. AEM Continúe con [Configurar el externalizador ](#configure-the-aem-externalizer).

### AEM Configurar el [!UICONTROL Externalizador de fechas ] {#configure-the-aem-externalizer}

AEM AEM El externalizador  permite que los usuarios pasen direcciones URL en un formato que se puede usar en [!DNL Workfront]. AEM AEM Si no se configura correctamente, [!DNL Workfront] no puede realizar llamadas a la API de la y las direcciones URL que vinculan documentos en Workfront no funcionarán.

1. AEM En la pantalla, haga clic en **[!UICONTROL Herramientas]** > **[!UICONTROL Operaciones]** >**[!UICONTROL Consola web]**.

1. Haga clic en **[!UICONTROL OSGI]** y, a continuación, haga clic en **[!UICONTROL Configuración]** en el menú desplegable.

1. En la lista de configuración, seleccione&#x200B;**[!UICONTROL Externalizador de vínculos CQ por día].**

   Se muestra la página [!UICONTROL Externalizer].

1. AEM En la sección **[!UICONTROL Dominios]**, asegúrese de que el dominio que aparece en el campo [!UICONTROL Autor] sea el nombre de dominio al que los usuarios pueden acceder externamente a través de la interfaz de usuario de la cuenta de usuario de.

   AEM El nombre de dominio en el campo [!UICONTROL autor] debe coincidir con el dominio que aparece en la línea URL de la instancia de.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Condicional) Si es necesario, actualice el dominio en el campo [!UICONTROL Autor].
1. Haga clic en **[!UICONTROL Guardar]**.

   [!UICONTROL AEM Assets] se ha configurado para vincular documentos con [!DNL Workfront]

1. Continuar con [Configurar [!DNL Workfront] para integrar con [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Configurar [!DNL Workfront] para que se integre con [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Después de instalar el conector [!UICONTROL Workfront for AEM Assets] (como se describe en [Instalar el paquete del conector [!UICONTROL Workfront for AEM Assets]](#install-the-workfront-for-aem-assets-connector-package)) y configurar [!UICONTROL AEM Assets] (como se describe en [Configurar[!UICONTROL  AEM Assets] para integrarlo con [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), debe configurar [!DNL Workfront] para vincular documentos entre [!DNL Workfront] y [!DNL AEM Assets].

1. Inicie sesión en [!DNL Workfront] como administrador de [!UICONTROL Workfront].

   >[!TIP]
   >
   >[!UICONTROL Workfront] recomienda crear un administrador de [!UICONTROL Workfront AEM] dedicado únicamente a tu integración de la. Para obtener más información sobre cómo asignar el nivel de acceso de administrador de [!UICONTROL Workfront] a un usuario, consulte [Conceder acceso administrativo a usuarios en ciertas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Documentos]**> **[!UICONTROL Integración personalizada].**

1. Haga clic en **[!UICONTROL Agregar integración personalizada]**.
1. En el cuadro **[!UICONTROL Nombre]**, especifique el nombre de la integración personalizada.

   Este es el nombre que ven los usuarios al usar la integración en [!UICONTROL Workfront]; por ejemplo, podría escribir *&quot;[!DNL AEM Assets]&quot;* para el nombre.

1. AEM En el cuadro **[!UICONTROL Dirección URL de la API base]**, especifique la dirección URL de la instancia de la.

   AEM La dirección URL de la API base consiste en la dirección URL de la instancia de seguida de la ruta: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. En el menú desplegable **[!UICONTROL Tipo de autenticación]**, seleccione **[!UICONTROL ApiKey].**

1. AEM En el cuadro&#x200B;**[!UICONTROL Clave de API]**, pegue la Clave de API que copió cuando configuró [!UICONTROL AEM Assets].
1. Haga clic en **[!UICONTROL Guardar]**.
1. (Opcional) Asegúrese de que la integración esté marcada como [!UICONTROL Activa].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] se ha configurado para trabajar con [!DNL AEM Assets].

   AEM AEM Para tener acceso a los recursos en la, cada usuario de [!DNL Workfront] que necesite utilizar el conector debe estar configurado como usuario en la interfaz de usuario de la interfaz de usuario de. Para obtener información sobre cómo crear usuarios, consulte [Configurar usuarios para que usen el conector](#set-up-users-to-use-the-connector).

## Configuración de usuarios para que utilicen el conector {#set-up-users-to-use-the-connector}

AEM Para que los usuarios tengan acceso al conector, deben tener un perfil de usuario en la lista de usuarios y pertenecer a un grupo de [!DNL Workfront] que tenga niveles de acceso que incluyan los permisos de [!UICONTROL Crear] y [!UICONTROL Eliminar].

Para obtener más información acerca de los permisos de [!DNL Workfront], vea [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Configurar usuarios en  [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Configurar usuarios en [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Inicie sesión en [!DNL AEM Assets] como administrador de [!DNL Workfront].
1. Haga clic en **[!UICONTROL Herramientas]** >**&#x200B;**&#x200B;**[!UICONTROL Seguridad]** >**[!UICONTROL Usuarios]**.

1. AEM AEM (Condicional) Si el usuario no tiene un perfil de usuario en el que se pueda crear un perfil de usuario en el que se pueda crear un perfil de usuario en el que se pueda crear un perfil de usuario en el que se pueda crear un perfil de usuario en el que se pueda crear un.

   1. Haga clic en **[!UICONTROL Crear usuario].**
   1. Introduzca la información personal del usuario.

      ![64NuevoUsuario.png](assets/64newuser-350x524.png)

      El único campo obligatorio es el campo de ID. AEM El identificador de la cuenta de usuario debe coincidir con su identificador de [!DNL Workfront], que es la dirección de correo electrónico [!DNL Workfront] del usuario.

      AEM AEM Si seleccionó la opción [!UICONTROL Omitir dominio de correo electrónico] al configurar la integración con [!DNL Workfront], entonces el identificador de la no coincidirá con la dirección de correo electrónico [!DNL Workfront].

1. AEM AEM (Condicional) Si el usuario tiene un perfil de, abra el perfil de usuario de la cuenta de usuario de la cuenta de usuario de la cuenta de usuario de la cuenta de usuario de la cuenta de usuario de la cuenta de usuario de la cuenta de usuario de la cuenta de usuario.

   1. Haga clic&#x200B;**[!UICONTROL Usuario].**

      Se muestra la página [!UICONTROL Administración de usuarios].

   1. Haga clic en el usuario que desee agregar y luego haga clic en **[!UICONTROL Propiedades]**.

      Se muestra la página de configuración del usuario.

1. Haga clic en la ficha **[!UICONTROL Grupos]**.

   ![](assets/groupstab.png)

1. Asegúrese de que el usuario pertenezca al menos a un grupo de [!DNL Workfront] que tenga niveles de acceso que incluyan los permisos [!UICONTROL Crear] y [!UICONTROL Eliminar].

   1. Para agregar el usuario a un grupo existente, empiece a escribir el nombre del grupo en el cuadro **[!UICONTROL Escriba el nombre del grupo]** y, a continuación, seleccione el grupo cuando aparezca en el menú desplegable.

      O

      Para seleccionar un grupo al que pertenece el usuario, seleccione un grupo en la sección **[!UICONTROL Grupos a los que pertenece este usuario]**.

1. Haga clic en **[!UICONTROL Guardar].**
