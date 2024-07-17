---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Lightroom
description: Con los módulos de Adobe Lightroom, puede iniciar un escenario de Adobe Workfront Fusion basado en los eventos de su cuenta de Adobe Lightroom.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: e48bdf18-49f0-436e-9182-16c9da2b3169
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# [!DNL Adobe Lightroom] módulos

<!--Add Connection info-->

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Lightroom], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
      <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para usar la funcionalidad descrita en este artículo.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Requisitos previos

Antes de poder usar el conector [!DNL Adobe Lightroom], debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener una cuenta de [!DNL Adobe Lightroom] activa.

## Creación de una conexión con Adobe Lightroom



## Módulos Adobe Lightroom y sus campos

Al configurar [!DNL Adobe Lightroom] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Adobe Lightroom] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Otro](#other)
* [Recursos](#assets)
* [Álbumes](#albums)

### Otro

* [Comprobación de estado](#health-check)
* [Recuperar metadatos del catálogo de usuarios](#retrieve-user-catalog-metadata)

#### Comprobación de estado

Este módulo de acción recupera un ID de versión de servidor de Lightroom, que prueba si el servicio de Lightroom se está ejecutando actualmente.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credenciales]</td>
      <td>
        <p>Si desea proporcionar credenciales específicas para asegurarse de que se está ejecutando un servidor específico, haga clic en Agregar elemento e introduzca las credenciales.</p><p>Los encabezados de autorización se añaden automáticamente.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Recuperar metadatos del catálogo de usuarios

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credenciales]</td>
      <td>
        <p>Si desea proporcionar credenciales específicas para asegurarse de que puede acceder a la cuenta de usuario correcta, haga clic en Agregar elemento e introduzca las credenciales.</p><p>Los encabezados de autorización se añaden automáticamente.</p>
      </td>
    </tr>
  </tbody>
</table>

### Recursos

* [Crear un archivo original de recurso](#create-an-asset-external-xmp-develop-setting-file)
* [Crear un recurso](#create-an-asset)
* [XMP Creación de un recurso externo que desarrolle un archivo de configuración](#create-an-asset-external-xmp-develop-setting-file)
* [Generar representaciones para un archivo original](#generate-renditions-for-an-original-file)
* [Obtener un recurso de catálogo](#get-a-catalog-asset)
* [XMP Obtenga la configuración de desarrollo de recursos externos más reciente](#get-the-latest-asset-external-xmp-develop-setting-file)
* [Obtener la última representación de recursos](#get-the-latest-asset-rendition)
* [Recuperar recursos](#retrieve-assets)

#### Crear un archivo original de recurso

Este módulo de acción crea y carga un archivo original para un recurso.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>Introduzca o asigne el ID del recurso para el que desea crear y cargar un archivo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Longitud del contenido en bytes]</td>
      <td>
        <p>Introduzca o asigne la longitud del contenido en bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rango de bytes]</td>
      <td>
        <p>Introduzca o asigne el rango de bytes para la solicitud, incluidos los bytes primero y último y la longitud de entidad definida en RFC 2616. Solo debe incluirse cuando los datos sean demasiado grandes para cargarse en una sola llamada.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de contenido]</td>
      <td>
        <p>Seleccione el tipo de contenido del nuevo archivo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Crear un recurso

Este módulo de acción crea un nuevo recurso con metadatos iniciales e información de importación.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo en el que se creará el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>Introduzca o asigne el ID del nuevo recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de recurso]</td>
      <td>
        <p>Seleccione si el recurso es una imagen o un vídeo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha y hora de creación del usuario]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha y hora de actualización del usuario]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de captura]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### XMP Creación de un recurso externo que desarrolle un archivo de configuración

Este módulo de acción admite dos flujos de trabajo. XMP El primer flujo de trabajo consiste en cargar el archivo de configuración de desarrollo de recursos externo del recurso. XMP El segundo flujo de trabajo es crear un archivo de configuración de desarrollo de XMP externo de otro recurso copiándolo del archivo de configuración de desarrollo de XMP externo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Longitud del contenido en bytes]</td>
      <td>
        <p>Introduzca o asigne la longitud del contenido en bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">XMP [!UICONTROL Cargar nuevo o copiar/desarrollar archivo]</td>
      <td>
        <p>Seleccione si desea cargar un archivo nuevo o copiar un archivo de un recurso existente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>Introduzca o asigne el ID del recurso en el que desea cargar o copiar un archivo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">XMP [!UICONTROL Vínculo para crear/desarrollar archivo]</td>
      <td>
        <p>Introduzca o asigne un vínculo al archivo que desee cargar o copiar.</p><p>Este archivo debe ser JSON si copia un archivo, o XML si carga un archivo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Generar representaciones para un archivo original

Este módulo de acción genera de forma asíncrona representaciones para un archivo original.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo(s) de representación (separados por punto y coma)]</td>
      <td>
        <p>Introduzca el tipo de representación para la representación que desea crear. Si introduce más de un tipo, sepárelos con punto y coma (;). <p>Tipos posibles:</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Longitud del contenido en bytes]</td>
      <td>
        <p>Introduzca o asigne la longitud del contenido en bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>Introduzca o asigne el ID del recurso para el que desea crear una representación de un archivo.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Obtener un recurso de catálogo

Este módulo de acción recupera información sobre un único recurso de un catálogo. El catálogo debe ser propiedad del usuario cuyas credenciales se representen en la conexión utilizada en este módulo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>Introduzca o asigne el ID del recurso para el que desea recuperar información.</p>
      </td>
    </tr>
  </tbody>
</table>


#### XMP Obtenga el recurso más reciente externo para desarrollar el archivo de configuración

XMP Este módulo de acción recupera el archivo de configuración de recursos externos más reciente de la.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>XMP Introduzca o asigne el ID del recurso asociado con el archivo de configuración de desarrollo de.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Obtener la última representación de recursos

Este módulo de acción recupera la última representación de recursos del tipo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>XMP Introduzca o asigne el ID del recurso asociado con el archivo de configuración de desarrollo de.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de representación]</td>
      <td>
        <p>Seleccione el tipo de representación que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Recuperar recursos

Este módulo de acción recupera recursos propiedad del usuario cuyas credenciales se representan en la conexión utilizada en este módulo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Marca de tiempo de inicio]</td>
      <td>
        <p>Introduzca o asigne una marca de tiempo. El módulo devuelve los registros que se han actualizado después de esta marca de tiempo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Devolver recursos capturados antes]</td>
      <td>
        <p>Escriba una fecha con el formato <code>YYYY-MM-DDT00:00:00</code>. El módulo devuelve los resultados capturados antes de esta fecha.</p><p> Este campo no se puede usar con el campo <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Número máximo de recursos devueltos]</td>
      <td>
        <p>Establezca el número máximo de recursos que [!DNL Workfront Fusion] devolverá durante un ciclo de ejecución. Este número debe ser inferior o igual a 100.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 Valor hash del archivo original]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ¿Ocultar recursos que están dentro de pilas?"]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Valores de subtipo de recurso]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recursos]</td>
      <td>
        <p>Introduzca o asigne hasta 100 ID de recurso, separados por comas.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipos de recursos que se excluirán]</td>
      <td>
        <p>Seleccione si desea excluir los recursos completos o incompletos. Para incluir todos los recursos, deje este campo en blanco.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Valores de grupo]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name values]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado favorito]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### Álbumes

* [Añadir recursos a un álbum](#add-assets-to-an-album)
* [Crear un álbum](#create-an-album)
* [Eliminar un álbum](#delete-an-album)
* [Consigue un álbum](#get-an-album)
* [Enumerar los recursos de un álbum](#list-assets-of-an-album)
* [Recuperar álbumes](#retrieve-albums)
* [Actualizar un álbum](#update-album)

#### Añadir recursos a un álbum

Este módulo de acción añade uno o más recursos al álbum especificado. Puede añadir hasta 50 recursos en un ciclo de ejecución.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el álbum al que desea agregar recursos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de álbum]</td>
      <td>
        <p>Introduzca o asigne el ID del álbum al que desea agregar recursos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>Para cada recurso que desee agregar al álbum, haga clic en <b>Agregar elemento</b> e introduzca los campos siguientes.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID de recurso]</td>
      <td>
        <p>Introduzca o asigne el ID del recurso que desea agregar al álbum</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ¿Es este recurso una portada de álbum?]</td>
      <td>
        <p>Seleccione si desea que este recurso se muestre como la imagen que representa el álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Pedido]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Metadatos]</td>
      <td>
        <p>Introduzca o asigne cualquier metadato que desee incluir en el recurso. Debe ser una sola cadena de texto con una longitud máxima de 1 a 24 caracteres.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID remoto]</td>
      <td>
        <p>Introduzca un identificador para el recurso.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Crear un álbum

Este módulo de acción crea un nuevo álbum en Lightroom.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo en el que desea crear un álbum.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de álbum]</td>
      <td>
        <p>Introduzca o asigne un ID para el nuevo álbum.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtipo]</td>
      <td>
        <p>Seleccione el subtipo del álbum.</p>
      </td>
    <tr>
      <td role="rowheader">Clave de API [!UICONTROL]</td>
      <td>
        <p>Introduzca la clave API del servicio que está creando el álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha y hora de creación del usuario]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha y hora de actualización del usuario]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre del álbum]</td>
      <td>
        <p>Introduzca o asigne un nombre para el nuevo álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID de portada]</td>
      <td>
        <p>Introduzca o asigne el ID de un recurso para utilizarlo como portada de este álbum.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID remoto]</td>
      <td>
        <p>Introduzca un identificador para el recurso.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de creación]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Fecha de actualización]</td>
      <td>
        <p>Escriba o asigne una fecha con el formato <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ¿Se ha eliminado el álbum?]</td>
      <td>
        <p>Active esta opción si se ha eliminado el contenido afiliado externo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL de la ubicación para editar contenido afiliado]</td>
      <td>
        <p>Si hay una URL donde los usuarios pueden editar el contenido de este álbum, ingrese la URL aquí.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL de la ubicación para ver el contenido afiliado]</td>
      <td>
        <p>Si hay una URL donde los usuarios pueden ver el contenido de este álbum, ingrese la URL aquí.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Eliminar un álbum

Este módulo de acción elimina un álbum.

El álbum eliminado debe haber sido creado por la misma aplicación cliente que ahora lo está eliminando, y debe ser del subtipo `project` o `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el álbum que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de álbum]</td>
      <td>
        <p>Introduzca o asigne el ID del álbum que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ¿Desea eliminar los álbumes secundarios?]</td>
      <td>
        <p>Seleccione si desea eliminar los álbumes secundarios del álbum eliminado.</p>
      </td>
    </tr>
  </tbody>
</table>

### Consigue un álbum

Este módulo de acción recupera el álbum especificado

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el álbum que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de álbum]</td>
      <td>
        <p>Introduzca o asigne el ID del álbum que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Enumerar los recursos de un álbum

Este módulo de acción recupera una lista de recursos en el álbum especificado.



#### Recuperar álbumes

Este módulo de acción recupera una lista de álbumes en el catálogo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene los álbumes que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtipos]</td>
      <td>
        <p>Introduzca o asigne el ID del álbum que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre del álbum que precederá a los resultados actuales]</td>
      <td>
        <p>Si está paginando los resultados, escriba o asigne el nombre del último álbum de la página anterior.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Número máximo de álbumes devueltos]</td>
      <td>
        <p>Establezca el número máximo de recursos que [!DNL Workfront Fusion] devolverá durante un ciclo de ejecución. El valor predeterminado de este campo es 100. Este módulo puede devolver más álbumes que este límite si varios álbumes en el límite del límite tienen el mismo valor <code>name_after</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Actualizar álbum

Este módulo de acción actualiza el álbum especificado.

El álbum actualizado debe haber sido creado por la misma aplicación cliente que ahora lo está actualizando y debe ser del subtipo `project` o `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Lightroom], vea <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Crear una conexión con [!DNL Adobe Lightroom]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catálogo]</td>
      <td>
        <p>Introduzca o asigne el ID del catálogo que contiene el álbum que desea actualizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de álbum]</td>
      <td>
        <p>Introduzca o asigne el ID del álbum que desea actualizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Otros campos</td>
      <td>
      <td>Para obtener descripciones de otros campos de este módulo, consulte <a href="#create-an-album" class="MCXref xref" >Crear un álbum</a> en este artículo.</td>
      </td>
    </tr>
  </tbody>
</table>
