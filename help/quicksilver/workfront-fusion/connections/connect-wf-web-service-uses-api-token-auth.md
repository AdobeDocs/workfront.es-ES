---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] a un servicio web que utiliza la autorización de tokens de API
description: Algunos servicios no permiten soluciones de integración como [!DNL Adobe Workfront Fusion] para crear una aplicación que pueda utilizar fácilmente en su situación.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] a un servicio web que utiliza la autorización de tokens de API

Algunos servicios no permiten soluciones de integración como [!DNL Adobe Workfront Fusion] para crear una aplicación que pueda utilizar fácilmente en su situación.

Hay una solución alternativa a esta situación. Puede conectar el servicio (aplicación) deseado a [!DNL Workfront Fusion] using [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] módulo.

Este artículo explica cómo conectar casi cualquier servicio web a [!DNL Workfront Fusion] uso de una clave de API/token de API.

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

## Conectarse a un servicio web que utiliza un token de API

El procedimiento para conectar el servicio mediante un token de API es similar en la mayoría de los servicios web.

1. Cree una aplicación en el sitio web del servicio web, tal como se explica en la sección [Cree una nueva aplicación y obtenga el token de API](#create-a-new-application-and-obtain-the-api-token) en este artículo.
1. Obtenga la clave de API o el token de API.
1. Agregar [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud] al escenario.
1. Configure el módulo según la documentación de API del servicio web y ejecute el escenario, tal como se explica en la sección [Configure el [!UICONTROL HTTP] módulo](#set-up-the-http-module) en este artículo.

>[!NOTE]
>
>Usaremos el [!DNL Pushover] servicio de notificación como ejemplo en este artículo.

## Cree una nueva aplicación y obtenga el token de API

>[!NOTE]
>
>Los servicios web crean y distribuyen claves de API o tokens de API de muchas formas diferentes. Para obtener instrucciones sobre la obtención de una clave de API y un token para el servicio web deseado, vaya al sitio web del servicio y busque &quot;clave de API&quot; o &quot;token de API&quot;.
>
>Se incluyen instrucciones para obtener una clave de API de Pushover solo como ejemplo de lo que podría encontrar.

1. Inicie sesión en su [!DNL Pushover] cuenta.
1. Haga clic en **[!UICONTROL Creación de un token de aplicación/API]** en la parte inferior de la página.
1. Rellene la Información de la aplicación y haga clic en **[!UICONTROL Crear una aplicación]**.
1. Almacene el token de API proporcionado en un lugar seguro. Lo necesitará para el [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] para conectarse al servicio web deseado ([!DNL Pushover], en este caso).

## Configure el [!UICONTROL HTTP] módulo

Para conectar un servicio web a su [!DNL Workfront Fusion] , debe utilizar el [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] en el escenario y configure el módulo según la documentación de API del servicio web.

1. Agregue la variable [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] al escenario.
1. Para insertar un mensaje mediante [!DNL Workfront Fusion], configure el módulo HTTP de la siguiente manera.

   >[!NOTE]
   >
   >Esta configuración de módulo corresponde a la variable [!DNL Pushover] documentación de la API del servicio web. La configuración puede ser diferente para otros servicios web. Por ejemplo, el token de API se puede insertar en la variable [!UICONTROL Encabezado] y no a [!UICONTROL Cuerpo] campo .

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>El campo URL contiene el punto final que puede encontrar en la documentación de la API del servicio web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>El método utilizado depende del punto final correspondiente. El punto final de Pushover para insertar mensajes utiliza el método POST .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Encabezados]</p> </td> 
      <td> <p>Algunos servicios web pueden utilizar encabezados para especificar la autenticación de token de API u otros parámetros. Este no es el caso en nuestro ejemplo, ya que el punto final de Pushover para insertar mensajes utiliza Body (ver abajo) para todos los tipos de solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Cadena de consulta]</p> </td> 
      <td> <p>Algunos servicios web pueden utilizar una cadena de consulta para especificar otros parámetros. Este no es el caso en nuestro ejemplo, ya que la variable [!DNL Pushover] el servicio web utiliza [!UICONTROL Body] (consulte a continuación) para todos los tipos de solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de cuerpo]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Esta configuración le permite seleccionar el tipo de contenido JSON en el campo [!UICONTROL Content Type] que aparece a continuación.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de contenido]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON es el tipo de contenido requerido por la aplicación [!UICONTROL Pushover]. Esto puede diferir de otros servicios web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Solicitar contenido]</p> </td> 
      <td> <p>Introduzca el contenido de solicitud de [!UICONTROL Body] en el formato JSON. Puede utilizar el módulo [!UICONTROL JSON] &gt; [!UICONTROL Crear JSON] como se explica en <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Cuerpo JSON asignado utilizando el módulo [!UICONTROL JSON] &gt; [!UICONTROL Crear JSON]</a> en este artículo. O puede introducir el contenido JSON manualmente, tal como se explica en <a href="#json-body-entered-manually" class="MCXref xref">Cuerpo de JSON introducido manualmente</a> en este artículo.</p> <p>Consulte la documentación de la API del servicio web para conocer los parámetros necesarios para ese servicio web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Cuerpo de JSON introducido manualmente

Especifique parámetros y valores en el formato JSON.

>[!INFO]
>
>**Ejemplo:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>
"token":"123459evz8aepwtxydndydgyumbfx",
>
>
"message":"Hello World!",
>
>
"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL usuario]</p> </td> 
   <td> <p>Su USER_KEY. Esto se puede encontrar en su [!DNL Pushover] tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>El token de API/clave de API que se generó creó al crear su [!DNL Pushover] aplicación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>El contenido de texto de la notificación push que se envía a los dispositivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Opcional) Título del mensaje. Si no se introduce ningún valor, se utiliza el nombre de la aplicación. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cuerpo de JSON asignado usando la variable [!UICONTROL JSON] >[!UICONTROL Crear JSON] módulo

La variable [!UICONTROL Crear JSON] facilita la especificación de JSON. También le ofrece la posibilidad de definir valores de forma dinámica.

Para obtener más información sobre los módulos JSON, consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Introduzca o asigne los valores desde los que desea crear JSON.

   ![](assets/json-values-350x288.png)

1. Conecte el [!UICONTROL JSON] > [!UICONTROL Crear JSON] a HTTP > Crear un módulo de solicitud.
1. Asigne la cadena JSON desde la variable [!UICONTROL Crear JSON] al [!UICONTROL Solicitar contenido] en el campo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] módulo.

   Ahora, cuando ejecute el escenario, la notificación push se enviará al dispositivo registrado en su [!DNL Pushover] cuenta.
