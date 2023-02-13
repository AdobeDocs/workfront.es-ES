---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones de cadena en Adobe Workfront Fusion
description: Las siguientes funciones de cadena están disponibles en el panel de asignación de Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# Funciones de cadena en [!DNL Adobe Workfront Fusion]

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii (texto; [eliminar diacríticos])]

Quita todos los caracteres que no sean ascii de una cadena de texto.

>[!INFO]
>
>**Ejemplos:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   Devuelve: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   Devuelve: [!UICONTROL escrz]


## [!UICONTROL base64 (texto)]

Transforma el texto a base64.

>[!INFO]
>
>**Ejemplo:**
>
>`base64( workfront )`
>
>Devuelve: d29ya2Zyb250==

## [!UICONTROL mayúsculas (texto)]

Convierte el primer carácter de una cadena de texto en mayúsculas.

>[!INFO]
>
>**Ejemplo:**
>
>`capitalize( workfront )`
>
>Devuelve: [!DNL Workfront]

## contiene (texto; cadena de búsqueda)

Comprueba si el texto contiene la cadena de búsqueda.

>[!INFO]
>
>**Ejemplos:**
>
>* `contains( Hello World ; Hello )`
   >
   >   Devuelve: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   Devuelve: [!UICONTROL false]


## [!UICONTROL decodeURL (texto)]

Descodifica los caracteres especiales de una dirección URL para texto.

>[!INFO]
>
>**Ejemplo:**
>`decodeURL( Automate%20your%20workflow )`
>
>Devuelve: [!UICONTROL Automatice el flujo de trabajo]

## [!UICONTROL encodeURL (texto)]

Codifica caracteres especiales en algún texto a una dirección URL válida.

## [!UICONTROL escapeHTML (texto)]

Omite todas las etiquetas HTML del texto.

>[!INFO]
>
>**Ejemplo:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Devuelve: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Omite todas las etiquetas de Markdown del texto.

>[!INFO]
>
>**Ejemplo:**
>
>`escapeMarkdown( # Header )`
>
>Devuelve: `&#35; Header`

## [!DNL indexOf (string; value; [start])]

Devuelve la posición de la primera incidencia de un valor especificado en una cadena. Este método devuelve &#39;-1&#39; si el valor que se busca no está presente. El valor inicial indica dónde en la cadena debe comenzar la búsqueda.

>[!INFO]
>
>**Ejemplos:**
>
>* `indexOf( Workfront ; o )`
   >
   >   Devuelve: 1
>
>* `indexOf( Workfront ; x )`
   >
   >   Devuelve: -1
>
>* `indexOf( Workfront ; o ; 3 )`
   >
   >   Devuelve: 6


## [!UICONTROL length (text o buffer)]

Devuelve la longitud de la cadena de texto (número de caracteres) o el búfer binario (tamaño del búfer en bytes).

>[!INFO]
>
>**Ejemplo:**
>
>`length( hello )`
>
>Devuelve: 5

## [!UICONTROL lower (texto)]

Convierte todos los caracteres alfabéticos de una cadena de texto en minúsculas.

>[!INFO]
>
>**Ejemplo:**
>
>`lower( Hello )`
>
>Devuelve: hello

## [!UICONTROL md5 (texto)]

Calcula el hash md5 de una cadena.

>[!INFO]
>
>**Ejemplo:**
>
>`md5( Workfront )`
>
>Devuelve: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL reemplazar (texto;cadena de búsqueda; cadena de reemplazo)]

Reemplaza la cadena de búsqueda por la nueva cadena.

>[!INFO]
>
>**Ejemplo:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Devuelve: [!UICONTROL Hola, mundo]

Expresiones regulares (incluidas en `/.../`) se puede usar como cadena de búsqueda con una combinación de indicadores (como `g`, `i`, `m`) anexado:

>[!INFO]
>
>**Ejemplo:**
>
>![](assets/replace---1-350x31.png)
>
>Todos estos números X X X X se sustituyen por X

La cadena de reemplazo puede incluir los siguientes patrones de reemplazo especiales:

* `$&` Inserta la subcadena coincidente.
* `$n` Cuando n es un entero positivo menor que 100, inserta la cadena de subcoincidencia enésima entre paréntesis. Esto está indexado en 1.

>[!INFO]
>
>**Ejemplos:**
>
>![](assets/variable-value-350x63.png)
>
>Devuelve: Número de teléfono `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>Devuelve: Número de teléfono: `+420777111222`

>[!CAUTION]
No utilice grupos de captura con nombres como `/ is (?<number>\d+)/` en el argumento de cadena de reemplazo. Al hacerlo, se produce un error.

Para obtener más información sobre las expresiones regulares, consulte [Analizador de texto](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (texto; [encoding]; [key])]

Calcula el hash sha1 de una cadena. Si se especifica el argumento clave, se devuelve hash sha1 HMAC en su lugar. Codificaciones compatibles: &quot;hex&quot; (predeterminado), &quot;base64&quot; o &quot;latin1&quot;.

>[!INFO]
**Ejemplo:**
`sha1( workfront )`
Devuelve: b2b30b8ae1f9e5b40fbb0696eabdbfd8d0c087f

## [!UICONTROL sha256 (texto; [encoding]; [key])]

Calcula el hash sha256 de una cadena. Si se especifica el argumento clave, se devuelve hash sha256 HMAC en su lugar. Codificaciones compatibles: &quot;hex&quot; (predeterminado), &quot;base64&quot; o &quot;latin1&quot;.>

>[!INFO]
**Ejemplo:**
`sha256( workfront )`
Devuelve: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bc

## [!UICONTROL sha512 (texto; [codificación de salida]; [key]; [codificación de claves])]

Calcula el hash sha512 de una cadena. Si se especifica el argumento clave, se devuelve hash sha512 HMAC en su lugar.

Codificaciones compatibles:

* &quot;[!UICONTROL hex]&quot; (predeterminado)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codificaciones de claves compatibles:

* &quot;[!UICONTROL text]&quot; (predeterminado)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot; o &quot;[!UICONTROL binario]&quot;

Al usar &quot;[!UICONTROL binario]&quot; clave, una clave debe ser un búfer, no una cadena.

>[!INFO]
**Ejemplo:**
`sha512(workfront)`
Devuelve: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b 85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL dividido (texto; separador)]

Divide una cadena en una matriz de cadenas separándola en subcadenas.

>[!INFO]
**Ejemplo:**
`split( John, George, Paul ; , )`

## [!UICONTROL inicial (texto)]

Capitaliza la primera letra de cada palabra y baja mayúsculas de todas las demás letras.

>[!INFO]
**Ejemplo:**
`startcase( hello WORLD )`
Devuelve: [!UICONTROL Hello World]

## [!UICONTROL StripHTML (texto)]

Quita todas las etiquetas de HTML del texto.

>[!INFO]
**Ejemplo:**
`stripHTML( <b>Hello</b> )`
Devuelve: Hello

## [!UICONTROL subcadena (texto; start;end)]

Devuelve una parte de una cadena de texto entre la posición &quot;inicio&quot; y la posición &quot;final&quot;.

>[!INFO]
**Ejemplos:**
* `substring( Hello ; 0 ; 3)`

   Devuelve: Talón
* `substring( Hello ; 1 ; 3 )`

   Devuelve: el


## [!UICONTROL toBinary (valor)]

Convierte cualquier valor en datos binarios.

También se puede especificar la codificación como segundo argumento para aplicar conversiones binarias de hex o base64 a datos binarios.

>[!INFO]
**Ejemplos:**
* `toBinary( Workfront )`

   Devuelve: 67 6f 72 6b 66 72 6f 6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   Devuelve: 67 6f 72 6b 66 72 6f 6e 74


## [!UICONTROL toString (valor)]

Convierte cualquier valor en una cadena.

## [!UICONTROL trim (texto)]

Elimina los caracteres de espacio al principio o al final del texto.

## [!UICONTROL upper (texto)]

Convierte todos los caracteres alfabéticos de una cadena de texto en mayúsculas.

>[!INFO]
**Ejemplo:**
`upper( Hello )`
Devuelve: [!UICONTROL HOLA]
