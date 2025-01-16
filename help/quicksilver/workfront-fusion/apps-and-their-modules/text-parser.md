---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analizador de texto
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 87%

---

# [!UICONTROL Analizador de texto]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Analizador de texto](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Puede usar la [!UICONTROL Text parser tool] para analizar texto y utilizarlo en otros módulos de escenario de [!DNL Adobe Workfront Fusion]. El [!UICONTROL Text parser] no requiere una conexión.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Información de API del analizador de texto

El conector del analizador de texto utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 2</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Text parser] módulos y sus campos

Al configurar los módulos de [!UICONTROL Text parser], [!DNL Adobe Workfront Fusion] muestra los campos que se indican a continuación. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformadores

* [[!UICONTROL Get Elements from HTML]](#get-elements-from-html)
* [[!UICONTROL Get Elements from text]](#get-elements-from-text)
* [[!UICONTROL HTML to Text]](#html-to-text)
* [[!UICONTROL Match Pattern]](#match-pattern)
* [[!UICONTROL Replace]](#replace)

#### [!UICONTROL Get Elements from HTML]

Recupera los elementos deseados del código del HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module finds no matches]</td> 
   <td> <p>Active esta opción para asegurarse de que el módulo no detenga el escenario si no devuelve resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> Seleccione el tipo de elemento que desea recuperar del código del HTML. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame element(s)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Introduzca o asigne el código de HTML desde el que desea recuperar los tipos de elementos especificados.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Elements from text]

Analiza elementos de texto en función del patrón determinado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Input text]</td> 
   <td> <p>Introduzca o asigne el texto que desea analizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Seleccione el patrón que refleje los elementos del texto que desee analizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignore Duplicate Occurrences]</td> 
   <td> <p>Marque esta casilla para ignorar las repeticiones de un elemento de texto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL De HTML a texto]

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
   <td> <p>Seleccione el tipo de nueva línea (salto de línea).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Uppercase headings]</p> </td> 
   <td> <p>Active esta opción para convertir el texto incluido en las etiquetas de encabezado (como &lt;h2&gt; &lt;/h2&gt;) en texto en mayúsculas.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Patrón de coincidencia]

El módulo [!UICONTROL Patrón de coincidencia] le permite buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda de un texto determinado. Este módulo utiliza expresiones regulares (también conocidas como regex o regexp).

Una expresión regular es una secuencia de caracteres en la que cada carácter es un metacarácter, que tiene un significado especial, o un carácter regular que tiene un significado literal. Estos caracteres y metacaracteres identifican un patrón que se puede utilizar para buscar texto. Por ejemplo, si desea buscar nombres, puede configurar una expresión regular para buscar un patrón que consista en dos palabras consecutivas que comiencen con mayúsculas. Las expresiones regulares son una potente herramienta para buscar y manipular texto.

El análisis de las expresiones regulares excede el ámbito de este artículo. Recomendamos los siguientes recursos:

* Para obtener la lista completa de metacaracteres, consulte [Expresiones regulares](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) en los documentos web de MDN.
* Para ver un tutorial sobre cómo crear expresiones regulares, recomendamos [RegexOne](https://regexone.com/).
* Para experimentar con expresiones regulares, recomendamos el sitio web [Expresiones regulares 101](https://regex101.com/). Seleccione ECMAScript (JavaScript) FLAVOR en el panel izquierdo.

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
   <td> <p>Active esta opción para recuperar todas las coincidencias del texto. Cada coincidencia se genera en un paquete independiente. Si esta opción está desactivada, el módulo recupera únicamente la primera entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Active esta opción para que este módulo distinga entre mayúsculas y minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Habilite esta opción para asegurarse de que los metacaracteres inicial y final (<code>^</code> y <code>$</code>) coinciden con el principio o final de cada línea, no sólo con el principio o el final de toda la cadena de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Habilite esta opción para asegurarse de que el punto (.) coincida con los caracteres de línea nueva (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p>Active esta opción para asegurarse de que el módulo no detenga el escenario si no devuelve resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Introduzca o asigne el texto que desea que coincida con el patrón.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Reemplazar]

Busca un valor o una expresión regular especificados en el texto introducido y reemplaza el resultado por el nuevo valor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Introduzca el término de búsqueda. También puede utilizar una expresión regular. Para obtener más información sobre la expresión regular, consulte el módulo <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New value]</td> 
   <td> <p> Introduzca un valor que sustituya el término de búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Active esta opción para recuperar todas las coincidencias del texto. Cada coincidencia se genera en un paquete independiente. Si esta opción está desactivada, el módulo recupera únicamente la primera entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Active esta opción para que este módulo distinga entre mayúsculas y minúsculas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Habilite esta opción para asegurarse de que los metacaracteres inicial y final (<code>^</code> y <code>$</code>) coinciden con el principio o final de cada línea, no sólo con el principio o el final de toda la cadena de entrada.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Habilite esta opción para asegurarse de que el punto (.) coincida con los caracteres de línea nueva (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Introduzca el texto que desea buscar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Extracción de datos

La extracción de datos, a veces denominada extracción web o recolección web, es el proceso de recopilar datos de sitios web y almacenarlos en la base de datos u hojas de cálculo locales. Si desea obtener datos de un sitio web y no está familiarizado con las expresiones regulares, puede utilizar una herramienta de extracción de datos.

Si la herramienta de extracción de datos proporciona una API REST, puede conectarse a ella a través de nuestros módulos [[!UICONTROL HTTP] universales](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) y [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).
