---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analizador de texto
description: Puede utilizar la herramienta Analizador de texto para analizar texto y utilizarlo en otros [!DNL Adobe Workfront Fusion] módulos de escenario. El analizador de texto no requiere una conexión.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL Analizador de texto]

Puede usar la variable [!UICONTROL Herramienta analizador de texto] para analizar texto y utilizarlo en otros [!DNL Adobe Workfront Fusion] módulos de escenario. La variable [!UICONTROL Analizador de texto] no requiere conexión.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analizador de texto] módulos y sus campos

Al configurar [!UICONTROL Analizador de texto] módulos, [!DNL Adobe Workfront Fusion] muestra los campos que se enumeran a continuación. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformadores

* [[!UICONTROL Obtención de elementos del HTML]](#get-elements-from-html)
* [[!UICONTROL Obtener elementos del texto]](#get-elements-from-text)
* [[!UICONTROL HTML a texto]](#html-to-text)
* [[!UICONTROL Patrón de coincidencia]](#match-pattern)
* [[!UICONTROL Reemplazar]](#replace)

#### [!UICONTROL Obtención de elementos del HTML]

Recupera los elementos deseados del código del HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continúe con la ejecución de la ruta aunque el módulo no encuentre coincidencias]</td> 
   <td> <p>Active esta opción para asegurarse de que el módulo no detenga el escenario si no devuelve resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de elemento]</td> 
   <td> <p> Seleccione el tipo de elemento que desea recuperar del código del HTML. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL Elemento(s) iFrame]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Introduzca o asigne el código de HTML desde el que desea recuperar los tipos de elemento especificados.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener elementos del texto]

Analiza los elementos del texto según el patrón dado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Texto de entrada]</td> 
   <td> <p>Introduzca o asigne el texto que desea analizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Seleccione el patrón que refleja los elementos que desea analizar del texto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Omitir ocurrencias duplicadas]</td> 
   <td> <p>Marque esta casilla para ignorar las ocurrencias duplicadas de un elemento de texto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML a texto]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Introduzca el código de HTML que desea convertir en texto sin formato.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line break] </td> 
   <td> <p>Seleccione el tipo de línea nueva (salto de línea).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Encabezados en mayúsculas]</p> </td> 
   <td> <p>Active esta opción para convertir el texto incluido en las etiquetas de encabezado (por ejemplo, &lt;h2&gt; &lt;/h2&gt;) en texto en mayúsculas.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Patrón de coincidencia]

La variable [!UICONTROL Patrón de coincidencia] permite buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda de un texto determinado. Este módulo utiliza expresiones regulares (también conocidas como regex o regexp).

Una expresión regular es una secuencia de caracteres en la que cada carácter es un metacaractero, tiene un significado especial, o un carácter normal que tiene un significado literal. Estos caracteres y metacaracteres identifican un patrón que se puede usar para buscar texto. Por ejemplo, si desea buscar nombres, puede configurar una expresión regular para buscar un patrón que consista en dos palabras consecutivas que empiecen por mayúsculas. Las expresiones regulares son una potente herramienta para buscar y manipular texto.

El debate sobre las expresiones regulares está fuera del alcance de este artículo. Recomendamos los siguientes recursos:

* La lista completa de metacaracteres puede consultarse en [Expresiones regulares](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) en documentos web de MDN.
* Para ver un tutorial sobre cómo crear expresiones regulares, se recomienda [RegexOne](https://regexone.com/).
* Para experimentar con expresiones regulares, se recomienda usar la variable [Expresiones regulares 101](https://regex101.com/) sitio web. Seleccione el FLAVOR de ECMAScript (JavaScript) en el panel izquierdo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Introduzca el patrón de expresión regular. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrae todos los números del texto proporcionado.</p> <p>Nota:  <p>El patrón debe contener al menos un grupo de captura entre paréntesis <code>()</code>. Si el patrón no contiene ningún grupo de captura, el paquete de salida está vacío.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Active esta opción para recuperar todas las coincidencias del texto. Cada coincidencia se genera en un paquete separado. Si esta opción está desactivada, el módulo recupera solo la primera entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Distinción entre mayúsculas y minúsculas]</td> 
   <td> <p> Active esta opción para que el texto de este módulo distinga entre mayúsculas y minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Active esta opción para garantizar que los metacaracteres de inicio y fin (<code>^</code> y <code>$</code>) coincide con el principio o el final de cada línea, no solo con el principio o el final de toda la cadena de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Línea única]</td> 
   <td>Active esta opción para asegurarse de que el punto (.) coincide con los caracteres de nueva línea (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continúe con la ejecución de la ruta aunque el módulo no devuelva ningún resultado]</td> 
   <td> <p>Active esta opción para asegurarse de que el módulo no detenga el escenario si no devuelve resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Introduzca o asigne el texto que desea que coincida con el patrón.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Reemplazar]

Busca en el texto introducido un valor especificado o una expresión regular y reemplaza el resultado por el nuevo valor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Introduzca el término de búsqueda. También puede utilizar una expresión regular. Para obtener más información sobre la expresión regular, consulte la <a href="#match-pattern" class="MCXref xref">[!UICONTROL Patrón de coincidencia]</a> módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuevo valor]</td> 
   <td> <p> Introduzca un valor que sustituya el término de búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Active esta opción para recuperar todas las coincidencias del texto. Cada coincidencia se genera en un paquete separado. Si esta opción está desactivada, el módulo recupera solo la primera entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Distinción entre mayúsculas y minúsculas]</td> 
   <td> <p> Active esta opción para que el texto de este módulo distinga entre mayúsculas y minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Active esta opción para garantizar que los metacaracteres de inicio y fin (<code>^</code> y <code>$</code>) coincide con el principio o el final de cada línea, no solo con el principio o el final de toda la cadena de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Línea única]</td> 
   <td>Active esta opción para asegurarse de que el punto (.) coincide con los caracteres de nueva línea (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto] </td> 
   <td> <p>Introduzca el texto que desea buscar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Creación de datos

El raspado de datos, a veces denominado raspado web, extracción de datos o recolección web, es el proceso de recopilación de datos de sitios web y almacenamiento en la base de datos u hojas de cálculo locales. Si desea crear secuencias de comandos de datos de un sitio web y no está familiarizado con las expresiones regulares, puede utilizar una herramienta de secuencias de comandos de datos:

* [Apify](https://apify.com/)
* [Mejores herramientas de eliminación de datos para 2019](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

Si la herramienta de extracción de datos proporciona una API de REST, puede conectarse a ella a través de nuestra API universal [[!UICONTROL HTTP] módulos](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) y [Enlaces web](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) módulos.
