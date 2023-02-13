---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado
description: Puede usar [!DNL Adobe Workfront Fusion] para conectarse a [!DNL Google Services] uso de un cliente OAuth personalizado. Este procedimiento requiere una [!DNL Google] cuenta.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Necesita una [!DNL Google] para realizar esta conexión.

## Crear un proyecto en [!DNL Google Cloud Platform]

El siguiente procedimiento está destinado a:

* Uso personal ([!DNL @gmail.com] y [!DNL @googlemail.com] usuarios)
* Uso interno ([!DNL G Suite] usuarios que prefieran utilizar un cliente OAuth personalizado)

Para crear un proyecto en [!DNL Google Cloud] Plataforma:

1. Iniciar sesión en [[!DNL Google Cloud] Plataforma](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) usando el [!DNL Google] credenciales.
1. En el panel izquierdo, haga clic en **[!UICONTROL Panel]**.
1. Haga clic en **[!UICONTROL Crear proyecto]** en la esquina superior derecha de la pantalla.
1. Introduzca la variable **[!UICONTROL Nombre del proyecto]** y haga clic en **[!UICONTROL Crear]**.

1. Haga clic en el **[!UICONTROL Habilitar API y servicios]** cerca de la parte superior de la pantalla.
1. En el **[!UICONTROL Buscar API y servicios]** en la parte superior de la pantalla, escriba el nombre del servicio que desee utilizar (por ejemplo, [!DNL Gmail] API o [!DNL Google Drive] API).
1. Cuando aparezca, haga clic en la API o el servicio al que desee conectarse [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Habilitar]** para habilitar la API seleccionada.
1. Repita los pasos 6-8 para cada API que desee habilitar.

   >[!NOTE]
   >
   >Debe habilitar [!DNL Google Drive] API, así como la API de todas las [!DNL Google] aplicaciones que desee usar (como [!DNL Google Sheets] API).

1. En la pantalla que aparece, haga clic en **[!UICONTROL Crear credenciales]** en la esquina superior derecha.
1. Continúe con la sección [Configuración del consentimiento de OAuth](#configure-oauth-consent-settings) en este artículo.

## Configurar [!UICONTROL Consentimiento de OAuth] configuración

1. En el panel izquierdo, haga clic en **[!UICONTROL Pantalla de consentimiento de OAuth]**.
1. Select **[!UICONTROL Externo]** y haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >Al seleccionar esta opción, no se le cargará. Para obtener más información, consulte [!DNL Google]Información de sobre excepciones a los requisitos de verificación.

1. Rellene los campos obligatorios de la siguiente manera:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Introduzca el nombre de la aplicación que solicita el consentimiento.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Correo electrónico de asistencia al usuario]</td> 
      <td>Introduzca una dirección de correo electrónico para que los usuarios se pongan en contacto con usted con preguntas sobre su consentimiento al conectarse a esta aplicación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Direcciones de correo electrónico]</td> 
      <td>Introduzca una o varias direcciones de correo electrónico que Google pueda utilizar para notificarle de los cambios realizados en el proyecto.</td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL Dominios autorizados], haga clic en **[!UICONTROL Añadir dominio]** y escriba `workfrontfusion.com`.

1. Haga clic en **[!UICONTROL Guardar y continuar]**.
1. Haga clic en **[!UICONTROL Agregar o quitar ámbitos]**.
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

Es posible que tenga que ampliar la lista o ir a la siguiente página de la lista para verlas todas.

1. Haga clic en **[!UICONTROL Actualizar]**.
1. Haga clic en **[!UICONTROL Guardar y continuar]**.
1. (Opcional) Agregue cualquier usuario de prueba al proyecto.
1. Haga clic en **[!UICONTROL Guardar y continuar]**.
1. Examine la información para comprobar su precisión y haga clic en **[!UICONTROL Volver al tablero]**.

   >[!NOTE]
   >
   >No es necesario que envíe la pantalla de consentimiento y la solicitud de verificación mediante [!DNL Google].

1. Continúe con [Crear credenciales de OAuth](#create-oauth-credentials).

## Crear credenciales de OAuth

1. En el panel izquierdo, haga clic en **[!UICONTROL Credenciales]**.

   >[!NOTE]
   >
   >Si esta no es la primera API o servicio ([!DNL Gmail] o [!DNL Google Drive]) que ha habilitado, no tiene que crear nuevas credenciales.

1. Haga clic en **[!UICONTROL Crear credenciales]** cerca de la parte superior de la pantalla y, a continuación, seleccione **[!UICONTROL ID de cliente de OAuth]** en el menú desplegable.

1. Rellene los campos obligatorios de la siguiente manera:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL URI de redireccionamiento autorizado], haga clic en **[!UICONTROL Añadir URI]** y escriba **one** de lo siguiente:

   * Para [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para otros [!DNL Google] aplicaciones: `https://app.workfrontfusion.com/oauth/cb/google`

1. Haga clic en **[!UICONTROL Crear]**.

   La variable [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente] visualización.

1. Copie el [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente] a una ubicación segura. Los usará para establecer una conexión en [!DNL Workfront Fusion].
1. Continúe con [Conectar a [!DNL Google] en [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Conectar a [!DNL Google] en [!DNL Workfront Fusion]

Proceso de creación de una conexión con [!DNL Google] difiere en función de si está usando un módulo de un [!DNL Google] servicio(como [!DNL Google Sheets] o [!DNL Google Docs]), o si se está conectando a [!DNL Google] a través de la variable [!UICONTROL HTTP] >[!UICONTROL Crear un OAuth2.0] módulo de solicitud.

* [Conectar a [!DNL Google] en un [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Conectar a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth2.0] módulo](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Conectar a [!DNL Google] en un [!DNL Google] service

1. En [!DNL Workfront Fusion], ubique la variable [!DNL Google] para el que debe crear una conexión.
1. Haga clic en **[!UICONTROL Crear una conexión]** y haga clic en **[!UICONTROL Mostrar configuración avanzada]**.

1. Introduzca la variable [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente] recuperó en [[!UICONTROL Crear credenciales de OAuth]](#create-oauth-credentials) en los campos respectivos, haga clic en **[!UICONTROL Continuar]**.

1. Inicie sesión con su [!DNL Google] cuenta.

   La variable **[!UICONTROL Esta aplicación no está verificada]** se muestra. Tenga en cuenta que la &quot;aplicación&quot; mencionada en el título de la ventana es el cliente OAuth que ha creado anteriormente.

1. Haga clic en **[!UICONTROL Avanzadas]** y haga clic en **[!UICONTROL Vaya a [!DNL Workfront Fusion] (no seguro)]** para permitir el acceso mediante su cliente OAuth personalizado.

1. Haga clic en **[!UICONTROL Permitir]** a conceder [!DNL Workfront Fusion] permiso.
1. En la ventana que aparece, haga clic en **[!UICONTROL Permitir]** para confirmar las opciones.

   La conexión con el [!DNL Google] se establece mediante un cliente OAuth personalizado.

### Conectar a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth2.0] módulo {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para instrucciones sobre la conexión a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth2.0] módulo, consulte [Instrucciones para crear una conexión a [!DNL Google] en el [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) en [[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Posible mensaje de error:[!UICONTROL [403] Acceso no configurado]

Si la variable [!UICONTROL [403] Acceso no configurado] aparece un mensaje de error y debe habilitar la API correspondiente en su Google Cloud Platform. Para habilitar la API, siga los pasos de la sección [Crear un proyecto en [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) en este artículo.
