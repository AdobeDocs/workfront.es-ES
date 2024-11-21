---
title: Módulos de software de Jira
description: En un escenario  [!DNL Adobe Workfront Fusion] puede automatizar los flujos de trabajo que usan [!DNL Jira] Software, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2112'
ht-degree: 1%

---

# [!DNL Jira Software] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Jira Software], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Requisitos previos

Para usar módulos de [!DNL Jira], debe tener una cuenta de [!DNL Jira].

## Información de API de Jira

El conector Jira utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"></td> 
   <td> Jira Cloud</td> 
   <td> Servidor Jira</td> 
  </tr> 
  <tr> 
   <td role="rowheader">apiVersion</td> 
   <td> 2</td> 
   <td> 2</td> 
  </tr> 
  <tr> 
   <td role="rowheader">apiVersionAgile</td> 
   <td> 1,0 </td> 
   <td> 1,0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>1.7.29</td> 
   <td>1.0.19</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]

El método de conexión se basa en si está usando [!DNL Jira Cloud] o [!DNL Jira Server].

* [Conectar [!DNL Jira Cloud] a Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Conectar [!DNL Jira Server] a [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Conectar [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Conectar [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Para conectar [!DNL Jira Software] a [!DNL Workfront Fusion], debe crear un token de API e insertarlo junto con la URL de servicio y el nombre de usuario en el campo [!UICONTROL Crear una conexión] en [!DNL Workfront Fusion].

#### Crear un token de API en [!DNL Jira]

1. Vaya a [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e inicie sesión.
1. Haga clic en **[!UICONTROL Crear token de API]**.
1. Escriba un nombre para el token, como *Workfront Fusion*.
1. Copie el token con el botón **[!UICONTROL Copiar al portapapeles]**.

   >[!IMPORTANT]
   >
   >No puede volver a ver el token después de cerrar este cuadro de diálogo.
1. Almacene el token generado en un lugar seguro.
1. Continuar con [Configurar el token de API [!DNL Jira] en [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configurar el token de la API [!DNL Jira] en [!DNL Workfront Fusion]

1. En [!DNL Workfront Fusion], agregue un módulo [!DNL Jira] a un escenario para abrir el cuadro **[!UICONTROL Crear una conexión]**.
1. Especifique la siguiente información:

   * **[!UICONTROL URL de servicio]:** Esta es la URL base que usas para acceder a tu cuenta Jira. Ejemplo: `yourorganization.atlassian.net`
   * **[!UICONTROL Nombre de usuario]**
   * **[!UICONTROL Token de API]:** Este es el token de API que creó en la sección [Crear un token de API en [!DNL Jira]](#create-an-api-token-in-jira) de este artículo.

1. Haga clic en [!UICONTROL Continuar] para crear la conexión y volver al módulo.

### Conectar [!DNL Jira Server] a [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Para autorizar una conexión entre [!DNL Workfront Fusion] y [!DNL Jira Server], necesita su clave de consumidor, clave privada y dirección URL del servicio. Es posible que deba ponerse en contacto con el administrador de [!DNL Jira] para obtener esta información.

* [Genere las claves pública y privada de su conexión  [!DNL Jira] s](#generate-public-and-private-keys-for-your-jira-connection)
* [Configurar la aplicación cliente como consumidor en  [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Crear una conexión con  [!DNL Jira] Server o el centro de datos Jira en [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Generar claves públicas y privadas para la conexión [!DNL Jira]

Para adquirir una clave privada para la conexión de [!DNL Workfront Fusion Jira], debe generar claves públicas y privadas.

1. En su terminal, ejecute los siguientes `openssl` comandos.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Este comando genera una clave privada de 1024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Este comando crea un certificado X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Este comando extrae la clave privada (formato PKCS8) en `jira_privatekey.pcks8`
archivo.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Este comando extrae la clave pública del certificado al archivo `jira_publickey.pem`.

     >[!NOTE]
     >
     >Si utiliza Windows, es posible que tenga que guardar manualmente la clave pública del archivo `jira_publickey.pem`:
     >
     >1. En el terminal, ejecute el siguiente comando:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copie la salida de terminal (incluidos `-------BEGIN PUBLIC KEY--------` y `-------END PUBLIC KEY--------`
     >   
     >1. Pegue la salida de terminal en un archivo de nombre `jira_publickey.pem`.


1. Continúe con [Configurar la aplicación cliente como consumidor en [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configurar la aplicación cliente como consumidor en [!DNL Jira]

1. Inicie sesión en su instancia de [!DNL Jira].
1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL [!DNL Jira]Configuración]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Aplicaciones]**> **[!UICONTROL Vínculos de aplicación]**.
1. En el campo **[!UICONTROL Escriba la dirección URL de la aplicación que desea vincular]**, escriba

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Haga clic en **[!UICONTROL Crear nuevo vínculo]**. Ignore el mensaje de error &quot;No se recibió respuesta de la dirección URL que ha introducido&quot;.
1. En la ventana **[!UICONTROL Vincular aplicaciones]**, introduzca valores en los campos **[!UICONTROL Clave de consumidor]** y **[!UICONTROL Secreto compartido]**.

   Puede elegir los valores de estos campos.

1. Copie los valores de los campos **[!UICONTROL Consumer key]** y **[!UICONTROL Shared secret]** en una ubicación segura.

   Necesitará estos valores más adelante en el proceso de configuración.

1. Rellene los campos de la dirección URL como se indica a continuación:

   | Campo | Descripción |
   |---|---|
   | [!UICONTROL URL de token de solicitud] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL de autorización] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL de token de acceso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Seleccione la casilla **[!UICONTROL Crear vínculo entrante]**.
1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana **[!UICONTROL Vincular aplicaciones]**, rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Clave de consumidor de [!UICONTROL]</p> </td> 
      <td> Pegue la clave de consumidor que ha copiado en una ubicación segura.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de consumidor]</td> 
      <td>Escriba un nombre de su elección. Este nombre es para su propia referencia.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clave pública]</td> 
      <td>Pegue la clave pública desde el archivo <code>[!DNL jira_publickey.pem]</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]**.
1. Continuar a [Crear una conexión con [!DNL Jira Server] o [!DNL Jira Data Center] en [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Crear una conexión con [!DNL Jira Server] o [!DNL Jira Data Center] en [!DNL Workfront Fusion]

>[!NOTE]
>
>Use la aplicación [!DNL Jira Server] para conectarse a [!DNL Jira Server] o [!DNL Jira Data Center].

1. En cualquier módulo de [!DNL Jira Server] de [!DNL Workfront Fusion], haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL conexión].
1. En el panel [!UICONTROL Crear una conexión], rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de conexión]</p> </td> 
      <td> <p>Escriba un nombre para la conexión</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave de consumidor de [!UICONTROL]</td> 
      <td>Pegue la clave de consumidor que ha copiado en una ubicación segura de <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure la aplicación cliente como consumidor en [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Pegue la clave privada del archivo <code>[!DNL jira_privatekey.pcks8]</code> que creó en <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Generar claves públicas y privadas para la conexión [!DNL Jira]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Escriba la URL de instancia [!DNL Jira]. Ejemplo: <code>yourorganization.atlassian.net</code></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Jira Software] módulos y sus campos

Al configurar [!DNL Jira Software] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Jira Software] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Observar registros]

Este módulo de déclencheur inicia un escenario cuando se agrega, actualiza o elimina un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione el webhook que desee utilizar para buscar registros. </p> <p>Para agregar un nuevo webhook:</p> 
    <ol> 
     <li value="1">Haga clic en <strong>[!UICONTROL Agregar]</strong></li> 
     <li value="2">Escriba un nombre para el webhook.</li> 
     <li value="3"> <p>Seleccione la conexión que desea utilizar para su webhook. </p> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </li> 
     <li value="4"> <p>Seleccione el tipo de registro que desea que vea el software:</p> 
      <ul> 
       <li>[!UICONTROL Comentario] </li> 
       <li>[!UICONTROL Problema]</li> 
       <li>[!UICONTROL Proyecto] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Agregar problema al sprint]](#add-issue-to-sprint)
* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Eliminar un registro]](#delete-a-record)
* [[!UICONTROL Descargar datos adjuntos]](#download-an-attachment)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Actualizar un registro]](#update-a-record)

#### [!UICONTROL Agregar problema al sprint]

Este módulo de acción añade uno o más problemas a un sprint.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Introduzca o asigne el ID de sprint del sprint al que desea agregar un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de problema o claves]</td> 
   <td>Agregue un ID o una clave de problema para cada problema que desee agregar al sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo registro en Jira.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que cree el módulo. Al seleccionar un tipo de registro, en el módulo aparecen otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Datos adjuntos]</li> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Registro de trabajo]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Jira Software]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros [!DNL Jira Software] módulos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca una ruta relativa a<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <img src="assets/quotes-in-json-350x120.png">  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro en particular.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que elimine el módulo. </p> 
    <ul> 
     <li>[!UICONTROL Datos adjuntos]</li> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o clave]</td> 
   <td>Introduzca o asigne el ID o la clave del registro que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar datos adjuntos]

Este módulo de acción descarga un archivo adjunto concreto.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del archivo adjunto que desea descargar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee datos de un único registro de [!DNL Jira Software].

Especifique el ID del registro.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro [!DNL Jira] que desea que lea el módulo.</p> 
    <ul> 
     <li>[!UICONTROL Datos adjuntos]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Usuario]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione las salidas que desee recibir. Las opciones de salida están disponibles en función del tipo de registro seleccionado en el campo "[!UICONTROL Record Type]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Escriba o asigne el identificador único [!DNL Jira Software] del registro que desea que lea el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro existente, como un problema o un proyecto,.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que actualice el módulo. Al seleccionar un tipo de registro, en el módulo aparecen otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Problema de transición]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o clave]</td> 
   <td>Introduzca o asigne el ID o la clave del registro que desea actualizar.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Enumerar registros]](#list-records)
* [[!UICONTROL Buscar registros]](#search-for-records)

#### [!UICONTROL Enumerar registros]

Este módulo de búsqueda recupera todos los elementos de un tipo específico que coinciden con la consulta de búsqueda

Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que enumere el módulo. Al seleccionar un tipo de registro, en el módulo aparecen otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Sprint issue]</li> 
     <li>[!UICONTROL Registro de trabajo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Resultados máximos]</p> </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo recupere durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Buscar registros]

Este módulo de búsqueda busca registros en un objeto de [!DNL Jira Software] que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Jira Software] a [!DNL Workfront Fusion], vea <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Conectar [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que busque el módulo. Al seleccionar un tipo de registro, en el módulo aparecen otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Problemas]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Language)] </p> <p>Para obtener más información sobre JQL, consulte <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> en el sitio de ayuda de Atlassian. </p> </li> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Proyecto por problema]</li> 
     <li>[!UICONTROL Usuario]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
