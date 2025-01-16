---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de Bibliotecas de Adobe Creative Cloud
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 91%

---

# Módulos de Bibliotecas de Adobe Creative Cloud

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de bibliotecas Adobe Creative Cloud](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/creative-cloud-libraries-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Con los módulos [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries], puede iniciar un escenario cuando se cree o actualice un elemento o biblioteca. También puede cargar, recuperar, archivar o enumerar elementos, o bien realizar una llamada a la API [!DNL Adobe Creative Cloud Libraries].

Si necesita instrucciones sobre cómo crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!IMPORTANT]
>
>Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
      <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Para usar módulos de [!DNL Adobe Creative Cloud Libraries], debe tener una cuenta de [!UICONTROL Adobe Creative Cloud].

## Información de API de bibliotecas Adobe Creative Cloud

El conector Bibliotecas Adobe Creative Cloud utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td>https://cc-libraries.adobe.io/api/v1</td> 
  </tr>
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.1.7</td> 
  </tr>
 </tbody> 
 </table>

## Módulos de las [!UICONTROL Bibliotecas de Adobe Creative Cloud] y sus campos

Al configurar los módulos de [!UICONTROL Bibliotecas de Adobe Creative Cloud], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse campos de [!DNL Adobe Creative Cloud Libraries] adicionales, en función de factores como el nivel de acceso del que disponga en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elementos](#elements)

* [Bibliotecas](#libraries)

* [Otro](#other)


### Elementos

* [[!UICONTROL Archivar un elemento]](#archive-an-element)

* [[!UICONTROL Obtener un elemento]](#get-an-element)

* [[!UICONTROL Enumerar elementos]](#list-elements)

* [[!UICONTROL Cargar un elemento]](#upload-an-element)

* [!UICONTROL [Watch New Element in Library]](#watch-new-element-in-library)

* [[!UICONTROL Ver elementos actualizados]](#watch-updated-elements)


#### [!UICONTROL Archivar un elemento]

Este módulo de acción archiva un elemento de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
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
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
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
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Datos base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Todos los datos disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>Una lista aplanada de recursos asociados al elemento de biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar elementos]

Este módulo de acción recupera una lista de elementos de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca de la que desee enumerar los elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>Seleccione si desea ordenar los resultados por el nombre o por la última fecha de modificación del elemento.</td>
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
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Datos base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Todos los datos disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>Una lista aplanada de recursos asociados al elemento de biblioteca</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Cargar un elemento]

Este módulo de acción carga un recurso de archivo pequeño en una biblioteca existente. El tamaño máximo de archivo es de 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca de la que desee enumerar los elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Invocation Mode]</td>
      <td>
        <p>Seleccione el modo de procesamiento con el que invocar este proceso de solicitud.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>La llamada de la API se procesa de forma síncrona. La respuesta se envía cuando se completa el procesamiento (salvo que se agote el tiempo de espera de la llamada).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>La respuesta asíncrona del monitor se devuelve inmediatamente y el procesamiento de la solicitud se produce de forma asíncrona. La llamada es responsable del sondeo del punto final hasta la finalización.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (predeterminado)</p>
            <p>Se intenta el procesamiento síncrono de la solicitud. Cuando el procesamiento se extiende más allá de 5000 ms, se devuelve la respuesta asíncrona del monitor. Se debe sondear la URL del monitor hasta que se complete la solicitud.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >Introduzca o asigne el tipo MIME del archivo cargado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source File]</td>
      <td>
        <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ver nuevo elemento en la biblioteca]

Este módulo de activador inicia un escenario cuando se añade un elemento a una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca en la que desea ver los elementos actualizados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Ver elementos actualizados]

Este módulo de activador inicia un escenario cuando se actualiza un elemento de una biblioteca.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Seleccione la biblioteca en la que desea ver los nuevos elementos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td>
    </tr>
  </tbody>
</table>

### Bibliotecas

* [[!UICONTROL Ver bibliotecas nuevas]](#watch-new-libraries)

* [[!UICONTROL Ver bibliotecas actualizadas]](#watch-updated-libraries)


#### [!UICONTROL Ver bibliotecas nuevas]

Este módulo de activador inicia un escenario cuando se crea una biblioteca nueva.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ver bibliotecas actualizadas]

Este módulo de activador inicia un escenario cuando se actualiza una biblioteca existente.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Seleccionar una conexión de Bibliotecas de Creative Cloud existente. Actualmente, la creación de conexiones no está disponible en el conector de Bibliotecas de Creative Cloud. Las conexiones existentes funcionan según lo esperado.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</td>
    </tr>
  </tbody>
</table>

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo realiza una llamada de API personalizada a la API de [!DNL Adobe Creative Cloud Libraries].

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
        <p>Escriba una ruta relativa a <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Por ejemplo, <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>Seleccione la versión de la API [!DNL Adobe Analytics] a la que desea conectarse.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion añade los encabezados de autorización para usted.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p>
        <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice instrucciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la instrucción condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Upload a transient document]</td>
      <td>
      <p>Si desea cargar un documento transitorio, introduzca el archivo de origen del documento que desea cargar.</p>
      <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p>
    </td>
    </tr>

</tbody>
</table>
