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
source-git-commit: cfd13f8eb422401644f7a1abf54e909218b2e8bf
workflow-type: tm+mt
source-wordcount: '4308'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Photoshop], así como conectarlo a varias aplicaciones y servicios de terceros.


Si necesita instrucciones para crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

+++**Amplíe para ver los requisitos de acceso para la funcionalidad de este artículo.**

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

+++

## Requisitos previos

Antes de poder usar el conector [!DNL Adobe Photoshop], debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener una cuenta de [!DNL Adobe Photoshop] activa.

## Crear una conexión con [!DNL Adobe Photoshop]

Para crear una conexión para los módulos de [!DNL Adobe Photoshop]:

1. Haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

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
        <td>Escriba su [!UICONTROL Secreto de cliente] [!DNL Adobe]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
        <td>Escriba su [!DNL Adobe] [!UICONTROL ID de cuenta técnica]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de organización]</td>
        <td>Escriba su [!UICONTROL Organization ID] de [!DNL Adobe]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Clave privada]</td>
        <td>
          <p>Escriba la clave privada que se generó cuando se crearon las credenciales en [!DNL Adobe Developer Console]. </p>
          <p>Para extraer la clave privada o el certificado:</p>
          <ol>
            <li value="1">
              <p>Haga clic en <b>[!UICONTROL Extract]</b>.</p>
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
              <p>Haga clic en <b>Guardar</b> para extraer el archivo y volver a la configuración de la conexión[!UICONTROL ]e.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Photoshop] módulos y sus campos

Al configurar [!DNL Adobe Photoshop] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Adobe Photoshop] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aplicar ediciones de PSD](#apply-psd-edits)
* [Corrección automática de color de una imagen](#auto-color-correct-an-image)
* [Convertir formato de imagen](#convert-image-format)
* [Crear una máscara](#create-a-mask)
* [Creación de un nuevo PSD](#create-a-new-psd)
* [Editar capas de texto](#edit-text-layers)
* [Ejecutar desenfoque de profundidad](#execute-depth-blur)
* [Ejecutar acciones de Photoshop](#execute-photoshop-actions)
* [Ejecutar acciones de Photoshop (JSON)](#execute-photoshop-actions-json)
* [Ejecutar recorte de productos](#execute-product-crop)
* [Obtener información de capa](#get-layer-info)
* [Realizar una llamada de API personalizada](#make-a-custom-api-call)
* [Quitar fondo](#remove-background)
* [Reemplazar un objeto inteligente](#replace-a-smart-object)
* [Cambiar el tamaño de una imagen](#resize-an-image)
* [Marca de agua de una imagen](#watermark-an-image)

### Aplicar ediciones de PSD

Este módulo de acción aplica una variedad de ediciones de nivel de documento y capa.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea editar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento &gt; Tamaño de imagen) Altura]</p>
      </td>
      <td> Introduzca o asigne la altura de la imagen en píxeles. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento &gt; Tamaño de imagen) Anchura]</p>
      </td>
      <td> Introduzca o asigne el ancho de la imagen en píxeles. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento &gt; Tamaño del lienzo) Superior]</p>
      </td>
   <td> Escriba o asigne, en píxeles, la coordenada y de la esquina superior izquierda del documento. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento &gt; Tamaño del lienzo) Inferior]</p>
      </td>
   <td> Escriba o asigne, en píxeles, la coordenada y de la esquina inferior derecha del documento. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento &gt; Tamaño del lienzo) Izquierda]</p>
      </td>
   <td> Escriba o asigne, en píxeles, la coordenada x de la esquina superior izquierda del documento. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento &gt; Tamaño del lienzo) Derecha]</p>
      </td>
   <td> Escriba o asigne, en píxeles, la coordenada x de la esquina inferior derecha del documento. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones &gt; Documento) Recortar]</p>
      </td>
   <td> Seleccione Píxeles transparentes para basar el recorte en píxeles transparentes de la imagen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones) Fuente predeterminada]</p>
      </td>
   <td> Introduzca el nombre completo de la fuente postscript que se utilizará como valor predeterminado global para el documento. Esta fuente se utilizará para cualquier capa de texto a la que le falte una fuente y no se haya proporcionado específicamente ninguna otra fuente para esa capa. Si falta esta fuente, la opción especificada en Administrar fuentes que faltan surtirá efecto. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones) Fuentes]</p>
      </td>
   <td> Para cada fuente que necesite el documento, haga clic en Agregar elemento e introduzca la ubicación de almacenamiento y la ubicación de archivo de la fuente. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones) Administrar fuentes que faltan]</p>
      </td>
   <td> Seleccione la acción que debe realizarse si faltan una o más fuentes en el documento. <ul><li><code>fail</code>: el trabajo no se realizará correctamente y el estado se establecerá en fallido, con los detalles del error proporcionados en la sección de detalles en el estado.</li><li><code>useDefault</code>: El trabajo se realizará correctamente, sin embargo, de forma predeterminada, todas las fuentes que faltan se reemplazarán con ArialMT.</li></ul></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Opciones) Capas]</p>
      </td>
   <td> Para cada capa que desee añadir, haga clic en Add item and y rellene los detalles de la capa. <p>Para obtener más información sobre las opciones de capa, consulte <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_applyPsdEdits/">Aplicar ediciones de PSD</a> en la documentación de Adobe Photoshop.  </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Salidas]</td>
      <td>
        <p>Para cada archivo convertido que desee crear, haga clic en Agregar elemento e introduzca el almacenamiento, la ubicación y el tipo como se indica en esta tabla.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el nuevo archivo.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o ruta de acceso donde se almacenará el nuevo archivo. Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Tipo de salida)]</p>
      </td>
   <td>Seleccione el tipo de archivo al que desea convertir el archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>



### Corrección automática de color de una imagen

El color automático de este módulo de acción corrige la imagen especificada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo con el color correcto.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo cuyo color desea corregir. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el nuevo archivo.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o ruta de acceso donde se almacenará el nuevo archivo. Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Tipo de salida)]</p>
      </td>
   <td>Seleccione el tipo de archivo al que desea convertir el archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>


### Convertir formato de imagen

Este módulo de acción convierte un archivo en JPEG, PNG, PSD o TIFF.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que se almacena el archivo del que desea quitar el fondo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo desde el que desea quitar el fondo. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Salidas]</td>
      <td>
        <p>Para cada archivo convertido que desee crear, haga clic en Agregar elemento e introduzca el almacenamiento, la ubicación y el tipo como se indica en esta tabla.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el nuevo archivo.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o ruta de acceso donde se almacenará el nuevo archivo. Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Tipo de salida)]</p>
      </td>
   <td>Seleccione el tipo de archivo al que desea convertir el archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>



### Crear una máscara

Este módulo de acción devuelve un archivo PNG con un mástil aplicado alrededor del asunto.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos desde el que se almacena el archivo desde el que desea crear una máscara.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Escriba o asigne la dirección URL o la ruta de acceso del archivo desde el que desea crear una máscara. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el archivo de máscara.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta de acceso donde se almacenará el archivo de máscara. Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Espacio de color]</p>
      </td>
   <td>Seleccione si la imagen de salida utiliza color RGB o RGBA. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Formato de máscara]</p>
      </td>
   <td>Seleccione si la máscara debe ser suave (con calado) o binaria. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimizar]</p>
      </td>
   <td>Seleccione Rendimiento para optimizar la velocidad o Lote para permitir el tiempo de espera. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Procesamiento posterior]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Versión]</p>
      </td>
   <td>El valor predeterminado es 4.0</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>

### Creación de un nuevo PSD

Este módulo de acción crea un nuevo PSD con capas opcionales y genera representaciones o guarda como PSD.

Para ver los campos relacionados con este módulo, consulte [Crear un nuevo PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) en la documentación de Adobe Photoshop.

### Editar capas de texto

Este módulo de acción edita las capas de texto en un archivo Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
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
   <td> <p>Para obtener detalles sobre las opciones de capa, consulte <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Editar capa de texto</a> en la documentación de Adobe Photoshop.</p>  </td>     </tr>
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



### Ejecutar acciones de Photoshop (JSON)

Este módulo de acción ejecuta acciones de Photoshop mediante comandos JSON.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo que desea editar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea editar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Acción JSON]</td>
      <td>
        <p>Introduzca el comando JSON para la acción que desea realizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fonts / Patterns / Brushes / Additional images]</td>
      <td>
        <p>Para cada fuente, patrón, pincel o imagen adicional que desee utilizar en esta acción, haga clic en Agregar elemento e introduzca el almacenamiento y la ubicación de archivo del elemento.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Fuente / Patrón / URL del archivo de pincel]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo que desea utilizar. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Genera almacenamiento de archivos]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que desea almacenar el archivo editado.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL del archivo de salida]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta de acceso donde se almacenará el archivo editado.  Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
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
    <tr>
      <td role="rowheader">[!UICONTROL Salidas]</td>
      <td>
        <p>Para cada archivo convertido que desee crear, haga clic en Agregar elemento e introduzca el almacenamiento, la ubicación y el tipo como se indica en esta tabla.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el nuevo archivo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o ruta de acceso donde se almacenará el nuevo archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Tipo de salida)]</p>
      </td>
   <td>Seleccione el tipo de archivo al que desea convertir el archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
      </tbody>
</table>

### Ejecutar desenfoque de profundidad

Este módulo de acción ejecuta Desenfoque profundo en el archivo seleccionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
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
        <p>Para obtener más información sobre otras opciones de Desenfoque profundo, consulte <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Ejecutar Desenfoque Profundo </a> en la documentación de la API de Adobe Photoshop.</p>
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

### Ejecutar acciones de Photoshop

Este módulo de acción ejecuta una acción de Photoshop en la imagen seleccionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
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

### Ejecutar recorte de productos

Este módulo de acción ejecuta el recorte de productos en la imagen seleccionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
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

### Obtener información de capa

Este módulo de acción recupera información de capa del archivo de PSD especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
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

### Realizar una llamada de API personalizada

Este módulo de acción realiza una llamada personalizada a la API de Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Escriba una ruta relativa a <code>https://image.adobe.io/pie/psdService</code>. Ejemplo: <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Quitar fondo

Este módulo de acción identifica el asunto principal de la imagen y elimina el fondo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos en el que se almacena el archivo del que desea quitar el fondo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo desde el que desea quitar el fondo. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el nuevo archivo.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o ruta de acceso donde se almacenará el nuevo archivo.  Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Espacio de color]</p>
      </td>
   <td>Seleccione si la imagen de salida utiliza color RGB o RGBA. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Formato de máscara]</p>
      </td>
   <td>Seleccione si los bordes de la imagen deben ser suaves (calados) o binarios. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimizar]</p>
      </td>
   <td>Seleccione Rendimiento para optimizar la velocidad o Lote para permitir el tiempo de espera. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Procesamiento posterior]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Versión]</p>
      </td>
   <td>El valor predeterminado es 4.0</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>



### Reemplazar un objeto inteligente

Este módulo de acción sustituye un objeto inteligente en una capa de PSD y genera nuevas representaciones.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Entrada) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el objeto inteligente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Entrada) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del objeto inteligente. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Capas]</p>
      </td>
   <td>Para cada capa que desee añadir al objeto inteligente, haga clic en Añadir elemento e introduzca el nombre o ID del objeto, el servicio de archivos donde se almacena el objeto inteligente y la dirección URL o ruta de acceso de la capa.<p>Para obtener descripciones de la configuración de avances en esta área, consulte <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_replaceSmartObject/">Reemplazar un objeto inteligente</a> en la documentación de la API de Photoshop </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Salidas]</td>
      <td>
        <p>Para cada nueva representación que desee que produzca el módulo, haga clic en Agregar elemento y rellene los campos siguientes. Puede tener un máximo de 25 archivos de salida.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el nuevo archivo.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o ruta de acceso donde se almacenará el nuevo archivo.  Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Anchura de salida)]</p>
      </td>
   <td> Anchura, en píxeles, del archivo de salida. El módulo conservará la relación de aspecto original. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>



### Cambiar el tamaño de una imagen

Esta acción cambia el tamaño de una imagen con la misma proporción de aspecto.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo cuyo tamaño desea cambiar.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Ubicación de archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo cuyo tamaño desea cambiar.  Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Salidas]</td>
      <td>
        <p>Para cada archivo convertido que desee crear, haga clic en Agregar elemento e introduzca las opciones de almacenamiento, ubicación y otras que se enumeran en esta tabla.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo]</p>
      </td>
   <td>Seleccione el tipo de archivo al que desea convertir el archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Anchura]</p>
      </td>
   <td>Introduzca un número que represente la anchura, en píxeles, de la imagen cuyo tamaño se ha cambiado. Se conservará la proporción de aspecto.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Anchura máxima]</p>
      </td>
   <td>Cuando la anchura es 0, se puede proporcionar el máximo de para obtener el tamaño. La anchura máxima tiene prioridad porque es más pequeña que la anchura del documento.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Recortar a lienzo]</p>
      </td>
   <td>Seleccione Sí para recortar las representaciones al tamaño Lienzo o No para convertirlas en tamaño de capa.</td> 
    </tr>
    </tbody>
</table>

### Marca de agua de una imagen

Este módulo de acción añade una marca de agua a la imagen seleccionada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Photoshop], vea <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Crear una conexión con [!DNL Adobe Photoshop]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">Almacenamiento de [!UICONTROL (base/entrada)]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena el archivo al que desea agregar una marca de agua.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Base / Input) Ubicación del archivo]</p>
      </td>
   <td> Introduzca o asigne la dirección URL o la ruta del archivo al que desea agregar una marca de agua. </td> 
    </tr>
    <tr>
      <td role="rowheader">Almacenamiento de [!UICONTROL (filigrana/entrada)]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena la marca de agua que desea agregar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Almacenamiento de [!UICONTROL (filigrana/entrada)]</td>
      <td>
        <p>Seleccione el servicio de archivos donde se almacena la marca de agua que desea agregar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Altura de marca de agua / límites)]</p>
      </td>
   <td>Introduzca o asigne la altura deseada de la marca de agua en píxeles.</td> 
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Marca de agua / Límites) Anchura]</p>
      </td>
   <td> Especifique o asigne el ancho deseado de la marca de agua en píxeles. </td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Marca de agua / Límites) Izquierda]</p>
      </td>
   <td> Especifique o asigne la distancia en píxeles desde el lado izquierdo de la imagen a la que debe estar la marca de agua.</td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Marca de agua / Límites) Superior]</p>
      </td>
   <td> Especifique o asigne la distancia en píxeles desde la parte superior de la imagen a la que debe estar la marca de agua.</td> 
    </tr>  
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Almacenamiento]</td>
      <td>
        <p>Seleccione el servicio de archivos donde desea almacenar el archivo de marca de agua.</p><p>Al seleccionar Fusion internal storage, el archivo está disponible para módulos posteriores, pero no lo hace fuera del escenario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Salida) Ubicación del archivo]</p>
      </td>
   <td> Escriba o asigne la dirección URL o ruta de acceso donde se almacenará el archivo de marca de agua. Esto solo es necesario si no ha elegido el almacenamiento interno de Fusion para el almacenamiento de salida.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Tipo de salida)]</p>
      </td>
   <td>Seleccione el tipo de archivo al que desea convertir el archivo. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Anchura de salida)]</p>
      </td>
   <td> Anchura, en píxeles, del archivo de salida. El módulo conservará la relación de aspecto original. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Salida) Sobrescribir]</td>
      <td>
        <p>Seleccione si el archivo recién editado sobrescribirá cualquier archivo de salida que ya exista. Esto solo se aplica a los archivos en el almacenamiento de Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de resultados devueltos]</p>
      </td>
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
    </tr>
    </tbody>
</table>















