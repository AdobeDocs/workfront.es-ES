---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de bibliotecas de Adobe Creative Cloud
description: Con la variable [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Módulos de bibliotecas , puede iniciar un escenario cuando se cree o actualice un elemento o biblioteca. También puede cargar, recuperar, archivar o enumerar elementos, o realizar una llamada a la función [!DNL Adobe Creative Cloud Libraries] API.
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Módulos de bibliotecas de Adobe Creative Cloud

Con la variable [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] , puede iniciar un escenario cuando se cree o actualice un elemento o biblioteca. También puede cargar, recuperar, archivar o enumerar elementos, o realizar una llamada a la función [!DNL Adobe Creative Cloud Libraries] API.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] o superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo]</p>
      </td>
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

Para usar [!DNL Adobe Creative Cloud Libraries] módulos, debe tener un [!UICONTROL Adobe Creative Cloud] cuenta.

## [!UICONTROL Bibliotecas de Adobe Creative Cloud] módulos y sus campos

Al configurar [!UICONTROL Bibliotecas de Adobe Creative Cloud] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Adobe Creative Cloud Libraries] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elementos](#elements)

* [Bibliotecas](#libraries)

* [Otro](#other)


### Elementos

* [[!UICONTROL Archivar un elemento]](#archive-an-element)

* [[!UICONTROL Obtener un elemento]](#get-an-element)

* [[!UICONTROL Elementos de lista]](#list-elements)

* [[!UICONTROL Cargar un elemento]](#upload-an-element)

* [!UICONTROL [Ver nuevo elemento en la biblioteca]](#watch-new-element-in-library)

* [[!UICONTROL Ver elementos actualizados]](#watch-updated-elements)


#### [!UICONTROL Archivar un elemento]

Este módulo de acción archiva un elemento de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca que contiene el elemento que desea archivar.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Seleccione el elemento que desea archivar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un elemento]

Este módulo de acción devuelve un solo elemento de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca que contiene el elemento que desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>Introduzca o asigne el ID del elemento que desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Seleccione el tipo de información que devuelve el módulo. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Predeterminado]</b>
            </p>
            <p>Datos básicos</p>
          </li>
          <li>
            <p><b>[!UICONTROL Detalles]</b>
            </p>
            <p>Todos los datos disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representaciones]</b>
            </p>
            <p>Una lista plana de recursos asociados al elemento de biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elementos de lista]

Este módulo de acción recupera una lista de elementos de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca desde la que desea enumerar los elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>Seleccione si desea ordenar los resultados por nombre o por la última fecha de modificación del elemento.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >Introduzca un tipo MIME para limitar los resultados a los elementos identificados con el tipo MIME especificado. Ejemplo: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Seleccione el tipo de información que devuelve el módulo. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Predeterminado]</b>
            </p>
            <p>Datos básicos</p>
          </li>
          <li>
            <p><b>[!UICONTROL Detalles]</b>
            </p>
            <p>Todos los datos disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representaciones]</b>
            </p>
            <p>Una lista plana de recursos asociados al elemento de biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Cargar un elemento]

Este módulo de acción carga un pequeño recurso de archivo en una biblioteca existente. El tamaño máximo del archivo es de 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca desde la que desea enumerar los elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modo de invocación]</td>
      <td>
        <p>Seleccione el modo de procesamiento con el que invocar este proceso de solicitud.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>La llamada de API se procesa sincrónicamente. La respuesta se envía cuando se completa el procesamiento (a menos que se agote el tiempo de espera de la llamada).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>La respuesta del monitor asíncrono se devuelve inmediatamente y el procesamiento de la solicitud se produce de forma asíncrona. La llamada es responsable de sondear el extremo hasta la finalización.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Predeterminado)</p>
            <p>Se intenta procesar la solicitud de forma sincrónica. Cuando el procesamiento supera los 5000 ms, se devuelve la respuesta del monitor asíncrono. La dirección URL del monitor debe sondearse hasta que se complete la solicitud.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo File]</td>
      <td >Introduzca o asigne el tipo MIME del archivo cargado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Archivo de origen]</td>
      <td>
        <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ver nuevo elemento en la biblioteca]

Este módulo de déclencheur inicia un escenario cuando se agrega un elemento a una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca que desea ver para los elementos actualizados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Ver elementos actualizados]

Este módulo de déclencheur inicia un escenario cuando se actualiza un elemento de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca que desea ver para los elementos nuevos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>

### Bibliotecas

* [[!UICONTROL Ver nuevas bibliotecas]](#watch-new-libraries)

* [[!UICONTROL Ver bibliotecas actualizadas]](#watch-updated-libraries)


#### [!UICONTROL Ver nuevas bibliotecas]

Este módulo de déclencheur inicia un escenario cuando se crea una biblioteca nueva.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ver bibliotecas actualizadas]

Este módulo de déclencheur inicia un escenario cuando se actualiza una biblioteca existente.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre cómo conectar su [!DNL Adobe Creative Cloud] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo realiza una llamada API personalizada a la variable [!DNL Adobe Creative Cloud Libraries] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Adobe Creative Cloud a Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con Adobe Workfront Fusion: instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Especifique una ruta relativa a <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Por ejemplo <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>Seleccione la versión del [!DNL Adobe Analytics] API a la que desea conectarse.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Método]</td>
      <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion añade los encabezados de autorización por usted.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]</td>
      <td>
        <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p>
        <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Cargar un documento transitorio]</td>
      <td>
      <p>Si desea cargar un documento transitorio, introduzca el archivo de origen del documento que desea cargar.</p>
      <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p>
    </td>
    </tr>

</tbody>
</table>
