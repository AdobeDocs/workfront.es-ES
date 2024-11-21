---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Datadog
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que utilizan Datadog, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 1%

---

# [!DNL Datadog] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Datadog], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar módulos de [!DNL Datadog], debe tener una cuenta de [!DNL Datadog].

## Información de API de Datadog

El conector Datadog utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>1.0.11</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Datadog] a [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Recupere la clave de API y la clave de aplicación {#retrieve-your-api-key-and-application-key}

Para conectar tu cuenta de [!DNL Datadog] a [!DNL Workfront Fusion], debes recuperar una clave de API y una clave de aplicación de tu cuenta de [!DNL Datadog].

1. Inicie sesión en su cuenta de [!DNL Datadog].
1. En el panel de navegación de la izquierda, haga clic en **[!UICONTROL Integraciones]** y luego en **[!UICONTROL API]**.
1. En la pantalla principal, haga clic en **[!UICONTROL Claves de API]**.
1. Pase el ratón sobre la barra morada para mostrar la clave de API.
1. Copie la clave de API en una ubicación segura.
1. En la pantalla principal, haga clic en **[!UICONTROL Claves de aplicación]**.
1. Pase el ratón sobre la barra morada para ver la clave de la aplicación.
1. Copie la clave de la aplicación en una ubicación segura.

### Crear una conexión con [!DNL Datadog] en [!DNL Workfront Fusion]

Puede crear una conexión con su cuenta de [!DNL Datadog] directamente desde un módulo de [!UICONTROL Datadog].

1. En cualquier módulo de [!UICONTROL Datadog], haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL Conexión].
1. Rellene los campos del módulo de la siguiente manera:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de conexión]</td> 
      <td> <p> Seleccione la opción [!UICONTROL [!DNL Datadog] Application] para obtener acceso completo a la API [!DNL Datadog].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de conexión]</td> 
      <td> <p> Introduzca un nombre para la conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dominio] </td> 
      <td> <p>Seleccione el dominio al que desea conectarse (EE.UU. o UE).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave de API [!UICONTROL]</td> 
      <td> <p> Escriba su clave de API [!DNL Datadog]. </p> <p>Para obtener instrucciones sobre cómo recuperar la clave de API, consulte <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperar la clave de API y la clave de aplicación</a> en este artículo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave de aplicación [!UICONTROL]</td> 
      <td> <p> Escriba la clave de aplicación [!DNL Datadog]. </p> <p>Para obtener instrucciones sobre cómo recuperar la clave de aplicación, consulte <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperar la clave de API y la clave de aplicación</a> en este artículo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Datadog] módulos y sus campos

Al configurar [!DNL Datadog] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Datadog] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Acciones

* [[!UICONTROL Puntos de la serie horaria posterior]](#post-timeseries-points)
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)

#### [!UICONTROL Puntos de la serie horaria posterior]

El módulo le permite publicar datos de series temporales que se pueden representar gráficamente en los paneles de [!DNL Datadog].

El límite para las cargas útiles comprimidas es de 3,2 megabytes (3200000) y de 62 megabytes (62914560) para las cargas útiles descomprimidas.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Datadog] a [!DNL Workfront Fusion], vea <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Datadog] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Agregue la serie temporal que desee enviar a [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!Métrica UICONTROL]</strong> </p> <p>Introduzca el nombre de la serie temporal.</p> </li> 
     <li> <p><strong>[!UICONTROL Tipo]</strong> </p> <p>Seleccione el tipo de métrica.</p> </li> 
     <li> <p><strong>[!INTERVALO UICONTROL]</strong> </p> <p> Si el tipo de métrica es tasa o recuento, defina el intervalo correspondiente.</p> </li> 
     <li> <p><strong>[!UICONTROL Puntos]</strong> </p> <p>Añada puntos relacionados con una métrica.</p> <p>Esta es una matriz de puntos JSON. Cada punto tiene el formato: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Nota:  <p>La marca de tiempo debe estar en segundos.</p> <p>La marca de tiempo debe ser actual. Actual se define como no más de 10 minutos en el futuro o más de 1 hora en el pasado.</p> <p> El formato de valor numérico debe ser un valor flotante.</p> </p> <p>Este campo debe contener al menos 1 elemento.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Introduzca el nombre del host que produjo la métrica.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API]

Este módulo de acción le permite realizar una llamada de API personalizada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Datadog] a [!DNL Workfront Fusion], vea <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Datadog] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Escriba una ruta relativa a <code>https://api.datadoghq.com/api/</code>. Ejemplo:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** La siguiente llamada de API devuelve todos los paneles de su cuenta de [!DNL Datadog]:

URL: `/v1/dashboard`

Método: `GET`

![](assets/datadog-api-example.png)

El resultado se puede encontrar en Salida del módulo, en Paquete > Cuerpo > Paneles.

En nuestro ejemplo, se devolvieron 3 paneles:

![](assets/datadog-api-response-example.png)
