---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: módulos de Adobe Firefly
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Firefly], así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: f1821568ea69d370dc5b2e4cbaaf6b0a72f9fe7f
workflow-type: tm+mt
source-wordcount: '1274'
ht-degree: 0%

---

# [!DNL Adobe Firefly] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Firefly], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Heredado: cualquiera </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nuevo:</p> <ul><li>[!UICONTROL Seleccionar] o [!UICONTROL Prime] [!DNL Workfront] Plan: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] está incluido.</li></ul>
   <p>O</p>
   <p>Actual: Su organización debe comprar [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Antes de usar el [!DNL Adobe Firefly] Conector de, debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener un activo [!DNL Adobe Firefly] cuenta.

## Cree una conexión con [!DNL Adobe Firefly]

Para crear una conexión para su [!DNL Adobe Firefly] módulos:

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
        <td role="rowheader">[!UICONTROL Entorno]</td>
        <td>Seleccione si desea conectarse a un entorno de producción o de no producción.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tipo]</td>
        <td>Seleccione si desea conectarse a una cuenta de servicio o a una cuenta personal.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca el [!UICONTROL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Introduzca su [!DNL Adobe] [!UICONTROL Secreto de cliente]. Esto se puede encontrar en la sección de detalles de [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Firefly] módulos y sus campos

Al configurar [!DNL Adobe Firefly] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Adobe Firefly] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Realizar una llamada de API personalizada

Este módulo de acción realiza una llamada personalizada a la API del Firefly.

Para ver las API disponibles específicas, consulte [API DE ADOBE FIREFLY](https://developer.adobe.com/firefly-services/docs/firefly-api/) en la documentación de Adobe Developer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Firefly], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Cree una conexión con [!DNL Adobe Firefly]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Introduzca una ruta relativa a <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
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
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Expandir una imagen

Este módulo de acción expande una imagen, de forma opcional con contenido de una solicitud proporcionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Cree una conexión con [!DNL Adobe Firefly]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Introduzca o asigne un mensaje para el contenido con el que desea expandir la imagen. Si no se proporciona ningún mensaje, la imagen se expandirá con contenido que coincida con la imagen original.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de variaciones]</td> 
   <td>Escriba un número entre 1 y 4. El módulo generará este número de variaciones de imagen expandidas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de imagen expandido]</td> 
   <td>Seleccione el formato de archivo con el que se guardará la imagen expandida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>  <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y el archivo de imagen del archivo de origen (datos).</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tamaño]</td> 
   <td>Seleccione el tamaño que desea que tenga la imagen expandida.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Semilla]</td> 
   <td>Introduzca o asigne un entero. Puede utilizar esta misma semilla en otro módulo Expandir una imagen para generar una imagen similar con estilos diferentes. </td> 
  </tr> 
 </tbody> 
</table>

## Rellenar una imagen

Este módulo de acción rellena el área enmascarada de una imagen, opcionalmente con contenido de una solicitud proporcionada.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Cree una conexión con [!DNL Adobe Firefly]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Introduzca o asigne un mensaje para el contenido con el que desea rellenar la imagen. Si no se proporciona ningún mensaje, la imagen se rellenará con contenido que coincida con la imagen original.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de variaciones]</td> 
   <td>Escriba un número entre 1 y 4. El módulo generará este número de variaciones de imágenes rellenadas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de imagen rellena]</td> 
   <td>Seleccione el formato de archivo con el que se guardará la imagen rellenada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Imagen]</td> 
   <td>  <p> Clic <b>Añadir una imagen</b>. Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos de imagen del archivo de origen.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máscara]</td> 
   <td>  <p> Clic <b>Añadir una máscara</b>. Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de máscara del archivo de origen. El archivo Mask representa la máscara personalizada que se rellenará con el contenido generado.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tamaño]</td> 
   <td>Seleccione el tamaño que desea que tenga la imagen rellena.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Semilla]</td> 
   <td>Introduzca o asigne un entero. Puede utilizar esta misma semilla en otro módulo Expandir una imagen para generar una imagen similar con estilos diferentes. </td> 
  </tr> 
 </tbody> 
</table>

## Generar una imagen

Este módulo de acción genera una imagen basada en una solicitud proporcionada. También puede proporcionar una imagen de referencia opcional, y la imagen generada coincidirá con el estilo de la imagen de referencia.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Campaign], consulte <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Cree una conexión con [!DNL Adobe Firefly]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Introduzca o asigne un indicador para la imagen que desea crear. Más detalles en la solicitud le permitirá tener más control sobre lo que aparece en la imagen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de variaciones]</td> 
   <td>Escriba un número entre 1 y 4. El módulo generará este número de variaciones de imagen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de imagen generado]</td> 
   <td>Seleccione el formato de archivo con el que se guardará la imagen expandida. Si selecciona Por defecto (default), el formato de fichero será JPEG si no se proporciona ninguna imagen de referencia. Si se proporciona una imagen de referencia, el formato de archivo de la imagen generada será el mismo que la imagen de referencia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>  <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre del archivo de imagen de referencia del archivo de origen y el archivo de imagen de referencia (datos). La imagen generada se creará de modo que coincida con el estilo de la imagen de referencia.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ajustes preestablecidos]</td> 
   <td>Si desea utilizar un estilo preestablecido, haga clic en Agregar elemento y escriba o asigne el estilo que desea utilizar.<p>Para ver una lista de estilos preestablecidos, consulte <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >Estilos del modelo de imagen</a> en la documentación para desarrolladores de Adobe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mensaje negativo]</td> 
   <td>Introduzca o asigne las palabras que desea evitar en el contenido generado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Clase de contenido]</td> 
   <td>Seleccione si desea que la imagen generada sea más similar a una foto o más similar al arte creado. <ul><li><b>Fotografía</b><p>Introduzca valores para la apertura, la velocidad de obturación (en segundos) y el campo de visión (en milímetros).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Semilla]</td> 
   <td>Introduzca o asigne un entero. Puede utilizar esta misma semilla en otro módulo Expandir una imagen para generar una imagen similar con estilos diferentes. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tamaño]</td> 
   <td>Seleccione el tamaño que desea que tenga la imagen generada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intensidad]</td> 
   <td>Introduzca o asigne un entero que represente la intensidad con la que la imagen generada coincidirá con el estilo del estilo preestablecido o la imagen de referencia. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intensidad visual]</td> 
   <td>Escriba o asigne un entero que represente la intensidad general de las características visuales existentes de la fotografía. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuración regional]</td> 
   <td>Si se proporciona una configuración regional, el módulo genera contenido más relevante para la configuración regional especificada. <p>La configuración regional debe proporcionarse en el código de idioma ISO 639-1 y en la región ISO 3166-1.</p><p> Ejemplo: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
