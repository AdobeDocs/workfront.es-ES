---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion]  a un servicio web que usa autorización de token de API
description: Algunos servicios no permiten soluciones de integración como  [!DNL Adobe Workfront Fusion]  para crear una aplicación que pueda usar fácilmente en su situación.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] a un servicio web que use la autorización de token de API

Algunos servicios no permiten soluciones de integración como [!DNL Adobe Workfront Fusion] para crear una aplicación que pueda usar fácilmente en su escenario.

Hay una solución alternativa para esta situación. Puede conectar el servicio (aplicación) deseado a [!DNL Workfront Fusion] mediante el módulo [!UICONTROL HTTP] de [!DNL Workfront Fusion].

Este artículo explica cómo conectar casi cualquier servicio web a [!DNL Workfront Fusion] mediante una clave de API/token de API.

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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conectarse a un servicio web que utiliza un token de API

El procedimiento para conectar el servicio a través de un token de API es similar para la mayoría de los servicios web.

1. Cree una aplicación en el sitio web del servicio web, como se explica en la sección [Cree una nueva aplicación y obtenga el token de API](#create-a-new-application-and-obtain-the-api-token) en este artículo.
1. Obtenga la clave de API o el token de API.
1. Agregue el módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud] de [!DNL Workfront Fusion] a su escenario.
1. Configure el módulo según la documentación de API del servicio web y ejecute el escenario, tal como se explica en la sección [Configurar el módulo [!UICONTROL HTTP]](#set-up-the-http-module) en este artículo.

>[!NOTE]
>
>Utilizaremos el servicio de notificación [!DNL Pushover] como ejemplo en este artículo.

## Cree una nueva aplicación y obtenga el token de API

>[!NOTE]
>
>Existen muchas maneras diferentes en que los servicios web crean y distribuyen claves API o tokens API. Para obtener instrucciones sobre la obtención de una clave de API y un token para el servicio web deseado, vaya al sitio web del servicio y busque &quot;clave de API&quot; o &quot;token de API&quot;.
>
>Solo incluimos instrucciones para obtener una clave de API de Pushover como ejemplo de lo que podría encontrar.

1. Inicie sesión en su cuenta de [!DNL Pushover].
1. Haga clic en **[!UICONTROL Crear una aplicación/token de API]** en la parte inferior de la página.
1. Rellene la información de la aplicación y haga clic en **[!UICONTROL Crear una aplicación]**.
1. Almacene el token de API proporcionado en un lugar seguro. Lo necesitará para el módulo [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] para conectarse al servicio web deseado ([!DNL Pushover], en este caso).

## Configurar el módulo [!UICONTROL HTTP]

Para conectar un servicio web al escenario [!DNL Workfront Fusion], debe usar el módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] en el escenario y configurar el módulo según la documentación de la API del servicio web.

1. Agregue el módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] a su escenario.
1. Para insertar un mensaje mediante [!DNL Workfront Fusion], configure el módulo HTTP de la siguiente manera.

   >[!NOTE]
   >
   >Esta configuración del módulo se corresponde con la documentación de la API del servicio web [!DNL Pushover]. La configuración puede ser diferente para otros servicios web. Por ejemplo, el token de API se puede insertar en el [!UICONTROL encabezado] y no en el campo [!UICONTROL Cuerpo].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>El campo URL contiene el extremo que puede encontrar en la documentación de API del servicio web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>El método utilizado depende del punto de conexión correspondiente. El punto final de Pushover para insertar mensajes utiliza el método POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Encabezados]</p> </td> 
      <td> <p>Algunos servicios web pueden utilizar encabezados para especificar la autenticación de token de API u otros parámetros. Este no es el caso en nuestro ejemplo, ya que el extremo de Pushover para insertar mensajes utiliza Body (ver a continuación) para todos los tipos de solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Cadena de consulta]</p> </td> 
      <td> <p>Algunos servicios web pueden utilizar una cadena de consulta para especificar otros parámetros. Este no es el caso en nuestro ejemplo, ya que el servicio web [!DNL Pushover] utiliza [!UICONTROL Body] (ver a continuación) para todos los tipos de solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de cuerpo]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Esta configuración le permite seleccionar el tipo de contenido JSON en el siguiente campo [!UICONTROL Tipo de contenido].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de contenido]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON es el tipo de contenido requerido por la aplicación [!UICONTROL Pushover]. Esto puede diferir de otros servicios web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Solicitar contenido]</p> </td> 
      <td> <p>Escriba el contenido de la solicitud de [!UICONTROL Body] en formato JSON. Puede usar el módulo [!UICONTROL JSON] &gt; [!UICONTROL Crear JSON] tal como se explica en <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Cuerpo de JSON asignado usando el módulo [!UICONTROL JSON] &gt; [!UICONTROL Crear JSON]</a> en este artículo. O puede introducir el contenido JSON manualmente, como se explica en <a href="#json-body-entered-manually" class="MCXref xref">Cuerpo de JSON introducido manualmente</a> en este artículo.</p> <p>Consulte la documentación de la API del servicio web para conocer los parámetros necesarios para ese servicio web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Cuerpo de JSON introducido manualmente

Especifique parámetros y valores en formato JSON.

>[!INFO]
>
>**Ejemplo:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL usuario]</p> </td> 
   <td> <p>Su USER_KEY. Esto se puede encontrar en el tablero [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Su token de API/clave de API que se generó al crear su aplicación [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL mensaje] </td> 
   <td> <p>El contenido de texto de la notificación push que se envía a los dispositivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Opcional) Título del mensaje. Si no se introduce ningún valor, se utiliza el nombre de la aplicación. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cuerpo de JSON asignado usando el módulo [!UICONTROL JSON] >[!UICONTROL Crear JSON]

El módulo [!UICONTROL Crear JSON] facilita la especificación de JSON. También le ofrece la posibilidad de definir valores de forma dinámica.

Para obtener más información sobre los módulos JSON, consulte [módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Introduzca o asigne los valores desde los que desea crear un JSON.

   ![](assets/json-values-350x288.png)

1. Conecte el módulo [!UICONTROL JSON] > [!UICONTROL Crear JSON] al módulo HTTP > Crear una solicitud.
1. Asigne la cadena JSON del módulo [!UICONTROL Crear JSON] al campo [!UICONTROL Solicitar contenido] en el módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud].

   Ahora, cuando ejecute el escenario, la notificación push se enviará al dispositivo que se haya registrado en su cuenta de [!DNL Pushover].
