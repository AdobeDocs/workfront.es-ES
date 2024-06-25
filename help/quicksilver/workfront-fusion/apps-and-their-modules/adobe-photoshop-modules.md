---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Photoshop
description: Con los módulos de Adobe Photoshop, puede iniciar un escenario de Adobe Workfront Fusion basado en los eventos de su cuenta de Adobe Photoshop, crear, leer o actualizar acuerdos y otros registros, buscar registros utilizando los criterios definidos y cargar documentos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 6bcf404432129a812b5e4d840b59e72f036ec723
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Photoshop], así como conectarlo a múltiples aplicaciones y servicios de terceros.


Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

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
        <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion para automatización e integración de trabajo]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Requisitos previos

Antes de usar el [!DNL Adobe Photoshop] Conector de, debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener un activo [!DNL Adobe Photoshop] cuenta.

## Cree una conexión con [!DNL Adobe Photoshop]

Para crear una conexión para su [!DNL Adobe Photoshop] módulos:

1. Clic **[!UICONTROL Añadir]** situado junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
        <td>
          <p>Escriba un nombre para esta conexión.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca el [!UICONTROL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Introduzca su [!DNL Adobe] [!UICONTROL Secreto de cliente]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
        <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de cuenta técnica]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de organización]</td>
        <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de organización]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Clave privada]</td>
        <td>
          <p>Introduzca la clave privada que se generó cuando se crearon las credenciales en la [!DNL Adobe Developer Console]. </p>
          <p>Para extraer la clave privada o el certificado:</p>
          <ol>
            <li value="1">
              <p>Clic <b>[!UICONTROL Extraer]</b>.</p>
            </li>
            <li value="2">
              <p>Seleccione el tipo de archivo que está extrayendo.</p>
            </li>
            <li value="3">
              <p>Seleccione el archivo que contiene la clave privada o el certificado.</p>
            </li>
            <li value="4">
              <p>Introduzca la contraseña del archivo.</p>
            </li>
            <li value="5">
              <p>Clic <b>Guardar</b> para extraer el archivo y volver a la configuración de la conexión[!UICONTROL ]e.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Photoshop] módulos y sus campos

Al configurar [!DNL Adobe Photoshop] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Adobe Photoshop] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Acciones

* [Creación de un nuevo PSD](#create-a-new-psd)
* [Editar capas de texto](#edit-text-layers)
* [Ejecutar desenfoque de profundidad](#execute-depth-blur)
* [Ejecutar acciones de Photoshop](#execute-photoshop-actions)
* [Ejecutar recorte de productos](#execute-product-crop)
* [Obtener información de capa](#get-layer-info)
* [Realizar una llamada de API personalizada](#make-a-custom-api-call)

#### Creación de un nuevo PSD

Este módulo de acción crea un nuevo PSD con capas opcionales y genera representaciones o guarda como PSD.

Para ver los campos relacionados con este módulo, consulte [Creación de un nuevo PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) en la documentación de Adobe Photoshop.

#### Editar capas de texto

Este módulo de acción edita las capas de texto en un archivo Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Cree una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento de archivo de entrada]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea editar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de entrada]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Administrar fuentes que faltan]</td>
      <td>
        <p>Seleccione la acción que debe realizarse si faltan una o más fuentes en el documento. Si no se proporciona la fuente, el módulo utilizará la fuente predeterminada.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fuente predeterminada]  </td>
      <td>
        <p>Introduzca el nombre completo de la fuente postscript que se utilizará como valor predeterminado global para el documento. Esta fuente se utilizará para cualquier capa de texto a la que le falte una fuente y no se haya proporcionado específicamente ninguna otra fuente para esa capa. Si falta esta fuente, la opción especificada en Administrar fuentes que faltan surtirá efecto.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Capas]</td>
   <td> <p>Para obtener más información sobre las opciones de capa, consulte <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Editar capa de texto</a> en la documentación de Adobe Photoshop.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento del archivo de salida]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que desea almacenar el archivo editado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de salida]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta de acceso donde se almacenará el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de archivo de salida]</p>
      </td>
   <td> Seleccione el tipo de archivo para el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compresión]</p>
      </td>
   <td> Seleccione el nivel de compresión del archivo de salida. </td> 
    </tr>
  </tbody>
</table>

#### Ejecutar desenfoque de profundidad

Este módulo de acción ejecuta Desenfoque profundo en el archivo seleccionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Cree una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento de archivo de entrada]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea editar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de entrada]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento del archivo de salida]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que desea almacenar el archivo editado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de salida]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta de acceso donde se almacenará el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de archivo de salida]</p>
      </td>
   <td> Seleccione el tipo de archivo para el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Otros campos]</td>
      <td>
        <p>Para obtener más información sobre otras opciones de Desenfoque profundo, consulte <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Ejecutar desenfoque de profundidad </a>en la documentación de la API de Adobe Photoshop.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compresión]</p>
      </td>
   <td> Seleccione el nivel de compresión del archivo de salida. </td> 
    </tr>
  </tbody>
</table>

#### Ejecutar acciones de Photoshop

Este módulo de acción ejecuta una acción de Photoshop en la imagen seleccionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Cree una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento de archivo de entrada]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea editar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de entrada]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Acciones almacenamiento de archivos]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo de acciones.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de acciones]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo de acciones. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nombre de acción]</p>
      </td>
   <td> Si sólo desea ejecutar una acción concreta, puede especificar la acción que se debe reproducir desde ActionSet. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fuente / Patrón / Pincel de almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea utilizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Fuente / Patrón / URL del archivo de pincel]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea utilizar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento del archivo de salida]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que desea almacenar el archivo editado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de salida]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta de acceso donde se almacenará el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de archivo de salida]</p>
      </td>
   <td> Seleccione el tipo de archivo para el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compresión]</p>
      </td>
   <td> Seleccione el nivel de compresión del archivo de salida. </td> 
    </tr>
  </tbody>
</table>

#### Ejecutar recorte de productos

Este módulo de acción ejecuta el recorte de productos en la imagen seleccionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Cree una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento de archivo de entrada]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea recortar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de entrada]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea recortar. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unidad]</p>
      </td>
   <td> Seleccione si desea describir el ajuste de altura y anchura en píxeles o como un porcentaje. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Anchura]</p>
      </td>
   <td> Introduzca o asigne la cantidad de relleno de anchura que desea añadir. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Altura]</p>
      </td>
   <td> Introduzca o asigne la cantidad de relleno de altura que desea añadir. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento del archivo de salida]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que desea almacenar el archivo editado.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de salida]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta de acceso donde se almacenará el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo de archivo de salida]</p>
      </td>
   <td> Seleccione el tipo de archivo para el archivo editado. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compresión]</p>
      </td>
   <td> Seleccione el nivel de compresión del archivo de salida. </td> 
    </tr>
  </tbody>
</table>

#### Obtener información de capa

Este módulo de acción recupera información de capa del archivo de PSD especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Cree una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento de archivo de entrada]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que se almacena el archivo del que desea recuperar información de capa.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de entrada]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo del que desea recuperar información de capa. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Miniaturas]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Realizar una llamada de API personalizada

Este módulo de acción realiza una llamada personalizada a la API de Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], consulte <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Cree una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Introduzca una ruta relativa a <code>https://image.adobe.io/pie/psdService</code>. Ejemplo: <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
