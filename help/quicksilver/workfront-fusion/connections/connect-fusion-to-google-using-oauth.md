---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado
description: Puede utilizar [!DNL Adobe Workfront Fusion] para conectarse a [!DNL Google Services] mediante un cliente de OAuth personalizado. Este procedimiento requiere un [!DNL Google] cuenta.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Necesita un existente [!DNL Google] cuenta para realizar esta conexión.

## Creación de un proyecto en [!DNL Google Cloud Platform]

El siguiente procedimiento está destinado a:

* Uso personal ([!DNL @gmail.com] y [!DNL @googlemail.com] users)
* Uso interno ([!DNL G Suite] usuarios que prefieren utilizar un cliente de OAuth personalizado)

Para crear un proyecto en [!DNL Google Cloud] Plataforma:

1. Iniciar sesión en [[!DNL Google Cloud] Plataforma](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) uso de su [!DNL Google] credenciales.
1. En el panel izquierdo, haga clic en **[!UICONTROL Tablero]**.
1. Clic **[!UICONTROL Crear proyecto]** en la esquina superior derecha de la pantalla.
1. Introduzca el **[!UICONTROL Nombre del proyecto]**, luego haga clic en **[!UICONTROL Crear]**.

1. Haga clic en **[!UICONTROL Habilitar API y servicios]** cerca de la parte superior de la pantalla.
1. En el **[!UICONTROL Buscar API y servicios]** en la parte superior de la pantalla, escriba el nombre del servicio que desea utilizar (por ejemplo, [!DNL Gmail] API o [!DNL Google Drive] API).
1. Cuando aparezca, haga clic en la API o el servicio al que desee conectarse [!DNL Workfront Fusion].
1. Clic **[!UICONTROL Activar]** para habilitar la API seleccionada.
1. Repita los pasos del 6 al 8 para cada API que desee habilitar.

   >[!NOTE]
   >
   >Debe activar [!DNL Google Drive] API, así como la API de todos los [!DNL Google] aplicaciones que desea utilizar (como [!DNL Google Sheets] API).

1. En la pantalla que aparece, haga clic en **[!UICONTROL Crear credenciales]** en la esquina superior derecha.
1. Continúe con la sección [Configuración del consentimiento de OAuth](#configure-oauth-consent-settings) en este artículo.

## Configurar [!UICONTROL Consentimiento de OAuth] configuración

1. En el panel izquierdo, haga clic en **[!UICONTROL Pantalla de consentimiento de OAuth]**.
1. Seleccionar **[!UICONTROL Externo]**, luego haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >No se le cobrará al seleccionar esta opción. Para obtener más información, consulte [!DNL Google]La información de acerca de las excepciones a los requisitos de verificación.

1. Rellene los campos obligatorios como se indica a continuación:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de aplicación]</p> </td> 
      <td> <p>Introduzca el nombre de la aplicación que solicita consentimiento.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Correo electrónico de asistencia al usuario]</td> 
      <td>Introduzca una dirección de correo electrónico para que los usuarios se pongan en contacto con usted si tienen preguntas sobre su consentimiento al conectarse a esta aplicación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Direcciones de correo electrónico]</td> 
      <td>Escriba una o más direcciones de correo electrónico que Google pueda usar para notificarle sobre cualquier cambio en su proyecto.</td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL Dominios autorizados], haga clic en **[!UICONTROL Añadir dominio]** y escriba `workfrontfusion.com`.

1. Clic **[!UICONTROL Guardar y continuar]**.
1. Clic **[!UICONTROL Agregar o quitar ámbitos]**.
1. En el panel derecho, habilite los siguientes ámbitos:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Servicio/API</th> 
      <th>Ámbitos requeridos</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Es posible que tenga que expandir la lista o ir a la siguiente página de la lista para verlos todos.

1. Clic **[!UICONTROL Actualizar]**.
1. Clic **[!UICONTROL Guardar y continuar]**.
1. (Opcional) Añada al proyecto cualquier usuario de prueba.
1. Clic **[!UICONTROL Guardar y continuar]**.
1. Examine la información para comprobar su precisión y haga clic en **[!UICONTROL Volver al tablero]**.

   >[!NOTE]
   >
   >No es necesario que envíe la pantalla de consentimiento y la solicitud de verificación de [!DNL Google].

1. Continuar a [Crear credenciales de OAuth](#create-oauth-credentials).

## Crear credenciales de OAuth

1. En el panel izquierdo, haga clic en **[!UICONTROL Credenciales]**.

   >[!NOTE]
   >
   >Si este no es el primer API o servicio ([!DNL Gmail] o [!DNL Google Drive]) Si lo ha habilitado, no es necesario que cree credenciales nuevas.

1. Clic **[!UICONTROL Crear credenciales]** cerca de la parte superior de la pantalla, seleccione **[!UICONTROL ID de cliente de OAuth]** en el menú desplegable.

1. Rellene los campos obligatorios como se indica a continuación:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de aplicación]</td> 
      <td> <p> [!UICONTROL Aplicación web]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL URI de redireccionamiento autorizados], haga clic en **[!UICONTROL Añadir URI]** y escriba **uno** de lo siguiente:

   * Para [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para otros [!DNL Google] aplicaciones: `https://app.workfrontfusion.com/oauth/cb/google`

1. Haga clic en **[!UICONTROL Crear]**.

   El [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente] mostrar.

1. Copie el [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente] a una ubicación segura. Los utilizará para establecer una conexión en [!DNL Workfront Fusion].
1. Continuar a [Conectar a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Conectar a [!DNL Google] in [!DNL Workfront Fusion]

Proceso de creación de una conexión con [!DNL Google] difiere según si utiliza un módulo de un [!DNL Google] servicio(como [!DNL Google Sheets] o [!DNL Google Docs]), o si se conecta a [!DNL Google] a través de [!UICONTROL HTTP] >[!UICONTROL Crear un OAuth2.0] módulo de solicitud.

* [Conectar a [!DNL Google] en un [!DNL Google] servicio](#connect-to-google-in-a-google-service)
* [Conectar a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realización de una solicitud OAuth2.0] módulo](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Conectar a [!DNL Google] en un [!DNL Google] servicio

1. Entrada [!DNL Workfront Fusion], busque la variable [!DNL Google] que necesita para crear una conexión.
1. Clic **[!UICONTROL Crear una conexión]**, luego haga clic en **[!UICONTROL Mostrar configuración avanzada]**.

1. Introduzca el [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente] que recuperó en [[!UICONTROL Crear credenciales de OAuth]](#create-oauth-credentials) en los campos respectivos, haga clic en **[!UICONTROL Continuar]**.

1. Inicie sesión con su [!DNL Google] cuenta.

   El **[!UICONTROL Esta aplicación no está verificada]** se muestra la ventana. Tenga en cuenta que la &quot;aplicación&quot; mencionada en el título de la ventana es el cliente de OAuth que ha creado anteriormente.

1. Clic **[!UICONTROL Avanzadas]**, luego haga clic en **[!UICONTROL Ir a [!DNL Workfront Fusion] (inseguro)]** para permitir el acceso con su cliente de OAuth personalizado.

1. Clic **[!UICONTROL Permitir]** para conceder [!DNL Workfront Fusion] permiso.
1. En la ventana que aparece, haga clic en **[!UICONTROL Permitir]** de nuevo para confirmar sus opciones.

   La conexión con el deseado [!DNL Google] se establece un servicio de con un cliente de OAuth personalizado.

### Conectar a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realización de una solicitud OAuth2.0] módulo {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para obtener instrucciones sobre cómo conectarse a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realización de una solicitud OAuth2.0] módulo, consulte [Instrucciones para crear una conexión con [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Posible mensaje de error:[!UICONTROL [403] Acceso no configurado]

Si la variable [!UICONTROL [403] Acceso no configurado] Se muestra un mensaje de error. Debe habilitar la API correspondiente en Google Cloud Platform. Para habilitar la API, siga los pasos de la sección [Creación de un proyecto en [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) en este artículo.
