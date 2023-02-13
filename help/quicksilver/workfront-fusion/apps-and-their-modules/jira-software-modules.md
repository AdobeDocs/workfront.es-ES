---
title: Módulos de software Jira
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Jira] Software, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2039'
ht-degree: 1%

---

# [!DNL Jira Software] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Jira Software], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL Workfront Fusion para automatización e integración del trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Requisitos previos

Para usar [!DNL Jira] Los módulos deben tener un [!DNL Jira] cuenta.

## Connect [!DNL Jira Software] a [!DNL Workfront Fusion]

El método de conexión se basa en si está utilizando [!DNL Jira Cloud] o [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] a Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] a [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Para conectar [!DNL Jira Software] a [!DNL Workfront Fusion], debe crear un token de API e insertarlo junto con la URL del servicio y el nombre de usuario en la variable [!UICONTROL Crear una conexión] en [!DNL Workfront Fusion].

#### Cree un token de API en [!DNL Jira]

1. Vaya a [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e inicie sesión.
1. Haga clic en **[!UICONTROL Crear token de API]**.
1. Escriba un nombre para el token, como *Workfront Fusion*.
1. Copie el token utilizando la variable **[!UICONTROL Copiar al portapapeles]** botón.

   >[!IMPORTANT]
   >
   >No puede volver a ver el token después de cerrar este cuadro de diálogo.
1. Almacene el token generado en un lugar seguro.
1. Continuar con [Configure las variables [!DNL Jira] Token de API en [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configure las variables [!DNL Jira] Token de API en [!DNL Workfront Fusion]

1. En [!DNL Workfront Fusion], agregue un [!DNL Jira] a un escenario para abrir el **[!UICONTROL Crear una conexión]** en la ventana
1. Especifique la siguiente información:

   * **[!UICONTROL URL del servicio]**
   * **[!UICONTROL Nombre de usuario]**
   * **[!UICONTROL Token de API]:** Este es el token de API que creó en la variable [Cree un token de API en [!DNL Jira]](#create-an-api-token-in-jira) de este artículo.

1. Haga clic en [!UICONTROL Continuar] para crear la conexión y volver al módulo.

### Connect [!DNL Jira Server] a [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Para autorizar una conexión entre [!DNL Workfront Fusion] y [!DNL Jira Server], necesita la clave de consumidor, la clave privada y la URL del servicio. Es posible que deba ponerse en contacto con su [!DNL Jira] administrador para esta información.

* [Genere claves públicas y privadas para su [!DNL Jira] connection](#generate-public-and-private-keys-for-your-jira-connection)
* [Configure la aplicación cliente como consumidor en [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Crear una conexión con [!DNL Jira] Servidor o centro de datos Jira en [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Genere claves públicas y privadas para su [!DNL Jira] connection

Para adquirir una clave privada para su [!DNL Workfront Fusion Jira] conexión, debe generar claves públicas y privadas.

1. En su terminal, ejecute lo siguiente `openssl` comandos.

   * `openssl genrsa -out jira_privatekey.pem 1024`

      Este comando genera una clave privada de 1024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

      Este comando crea un certificado X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

      Este comando extrae la clave privada (formato PKCS8) en la variable `jira_privatekey.pcks8`
archivo.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

      Este comando extrae la clave pública del certificado en la variable `jira_publickey.pem` archivo.

      >[!NOTE]
      >
      >Si utiliza Windows, es posible que deba guardar la clave pública en la variable `jira_publickey.pem` manualmente:
      >
      >1. En el terminal, ejecute el siguiente comando:
      >   
      >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
      >   
      >1. Copie la salida de terminal (incluyendo `-------BEGIN PUBLIC KEY--------` y `-------END PUBLIC KEY--------`
      >   
      >1. Pegar la salida de terminal en un archivo llamado `jira_publickey.pem`.



1. Continúe con [Configure la aplicación cliente como consumidor en [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configure la aplicación cliente como consumidor en [!DNL Jira]

1. Inicie sesión en su [!DNL Jira] instancia.
1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL [!DNL Jira]Configuración]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Aplicaciones]**> **[!UICONTROL Vínculos de aplicación]**.
1. En el **[!UICONTROL Introduzca la URL de la aplicación que desea vincular]** , introduzca

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Haga clic en **[!UICONTROL Crear nuevo vínculo]**. Ignore el mensaje de error &quot;No se recibió ninguna respuesta de la URL que ingresó&quot;.
1. En el **[!UICONTROL Vincular aplicaciones]** , introduzca valores en la **[!UICONTROL Clave del consumidor]** y **[!UICONTROL Secreto compartido]** campos.

   Puede elegir los valores de estos campos.

1. Copie los valores de la variable **[!UICONTROL Clave del consumidor]** y **[!UICONTROL Secreto compartido]** a una ubicación segura.

   Necesitará estos valores más adelante en el proceso de configuración.

1. Rellene los campos URL como se indica a continuación:

   | Campo | Descripción |
   |---|---|
   | [!UICONTROL URL del token de solicitud] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL de autorización] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL Dirección URL del token de acceso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Seleccione el **[!UICONTROL Crear vínculo entrante]** casilla de verificación.
1. Haga clic en **[!UICONTROL Continuar]**.
1. En el **[!UICONTROL Vincular aplicaciones]** , rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Pegue en la clave de consumidor que ha copiado en una ubicación segura.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre del consumidor]</td> 
      <td>Escriba el nombre que desee. Este nombre es para su propia referencia.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clave pública]</td> 
      <td>Pegue en la clave pública de su <code>[!DNL jira_publickey.pem]</code> archivo.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]**.
1. Continúe con [Crear una conexión con [!DNL Jira Server] o [!DNL Jira Data Center] en [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Crear una conexión con [!DNL Jira Server] o [!DNL Jira Data Center] en [!DNL Workfront Fusion]

>[!NOTE]
>
>Utilice la variable [!DNL Jira Server] aplicación a la que conectarse [!DNL Jira Server] o [!DNL Jira Data Center].
1. En cualquier [!DNL Jira Server] módulo en [!DNL Workfront Fusion], haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL connection] campo .
1. En el [!UICONTROL Crear una conexión] , rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Escriba un nombre para la conexión</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Pegue en la clave de consumidor que ha copiado en una ubicación segura en <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configure la aplicación cliente como consumidor en [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Pegue en la clave privada desde la <code>[!DNL jira_privatekey.pcks8]</code> archivo creado en <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Genere claves públicas y privadas para su [!DNL Jira] connection</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Escriba la [!DNL Jira] URL de instancia. </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo .

## [!DNL Jira Software] módulos y sus campos

Al configurar [!DNL Jira Software] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Jira Software] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Ver registros]

Este módulo de déclencheur inicia un escenario cuando se agrega, actualiza o elimina un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td> <p>Seleccione el vínculo web que desee usar para buscar registros. </p> <p>Para agregar un nuevo vínculo web:</p> 
    <ol> 
     <li value="1">Haga clic en <strong>[!UICONTROL Agregar]</strong></li> 
     <li value="2">Escriba un nombre para el vínculo web.</li> 
     <li value="3"> <p>Seleccione la conexión que desee utilizar para el weblink. </p> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </li> 
     <li value="4"> <p>Seleccione el tipo de registro que desea que observe el software:</p> 
      <ul> 
       <li>[!UICONTROL Comentario] </li> 
       <li>[!UICONTROL Problema]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Agregar un problema a sprint]](#add-issue-to-sprint)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Eliminar un registro]](#delete-a-record)
* [[!UICONTROL Descargar un archivo adjunto]](#download-an-attachment)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Actualizar un registro]](#update-a-record)

#### [!UICONTROL Agregar un problema a sprint]

Este módulo de acción agrega uno o más problemas a un sprint.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Introduzca o asigne el ID de Sprint del sprint al que desea agregar un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de problema o claves]</td> 
   <td>Agregue un ID de problema o una clave para cada problema que desee agregar al sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo registro en Jira.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que cree el módulo. Al seleccionar un tipo de registro, en el módulo aparecerán otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Jira Software] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Jira Software] módulos.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Especifique una ruta relativa a<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro en particular.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que elimine el módulo. </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o clave]</td> 
   <td>Introduzca o asigne el ID o la clave del registro que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo adjunto]

Este módulo de acción descarga un archivo adjunto concreto.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del archivo adjunto que desea descargar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee datos de un registro único de [!DNL Jira Software].

Especifique el ID del registro.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Jira] registro que desea que lea el módulo.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Usuario]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los resultados que desee recibir. Las opciones de salida están disponibles en función del tipo de registro seleccionado en el campo "[!UICONTROL Record Type]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Introduzca o asigne la variable única [!DNL Jira Software] ID del registro que desea que lea el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro existente, como un problema o un proyecto.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que actualice el módulo. Al seleccionar un tipo de registro, en el módulo aparecerán otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
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

* [[!UICONTROL Registros de lista]](#list-records)
* [[!UICONTROL Buscar registros]](#search-for-records)

#### [!UICONTROL Registros de lista]

Este módulo de búsqueda recupera todos los elementos de un tipo específico que coinciden con la consulta de búsqueda

Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que muestre el módulo. Al seleccionar un tipo de registro, en el módulo aparecerán otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Comentario]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Problema con Sprint]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo recupere durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Buscar registros]

Este módulo de búsqueda busca registros en un objeto de [!DNL Jira Software] que coinciden con la consulta de búsqueda especificada.

Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Jira Software] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea que busque el módulo. Al seleccionar un tipo de registro, en el módulo aparecerán otros campos específicos de dicho tipo de registro.</p> 
    <ul> 
     <li>[!UICONTROL Problemas]</li> 
     <li> <p>[!UICONTROL Problemas de JQL (lenguaje de consulta Jira)] </p> <p>Para obtener más información sobre JQL, consulte <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> en el sitio de ayuda de Atlassian. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Proyecto por problema]</li> 
     <li>[!UICONTROL Usuario]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
