---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones de cadena en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 90%

---

# Funciones de cadena en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Funciones de cadena](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/string-functions.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <p>Actual: no se requiere licencia para [!DNL Workfront Fusion].</p> 
   <p>O</p> 
   <p>Heredado: cualquiera </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Producto</td>  
   <td> 
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] está incluido.</li></ul> 
   <p>O</p> 
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL longitud (texto o búfer)]

Devuelve la longitud de la cadena de texto (número de caracteres) o del búfer binario (tamaño del búfer en bytes).

>[!INFO]
>
> **Ejemplo:**
>
>`length( hello )`
>
>Devuelve: 5

## [!UICONTROL inferior (texto)]

Convierte a minúsculas todos los caracteres alfabéticos de una cadena de texto.

>[!INFO]
>
>**Ejemplo:**
>
>`lower( Hello )`
>
>Devuelve: hello

## [!UICONTROL poner en mayúsculas (texto)]

Convierte el primer carácter de una cadena de texto en mayúscula.

>[!INFO]
>
>**Ejemplo:**
>
>`capitalize( workfront )`
>
>Devuelve: [!DNL Workfront]

## [!UICONTROL mayúscula inicial (texto)]

Pone en mayúscula la primera letra de cada palabra y en minúsculas todas las demás letras.

>[!INFO]
>
>**Ejemplo:**
>`startcase( hello WORLD )`
>
>Devuelve: [!UICONTROL Hello World]

## [!UICONTROL ascii (texto; [quitar diacríticos])]

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



## [!UICONTROL reemplazar (texto; cadena de búsqueda; cadena de reemplazo)]

Reemplaza la cadena de búsqueda por la nueva cadena.

>[!INFO]
>
>**Ejemplo:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Devuelve: [!UICONTROL Hi World]

Las expresiones regulares (entre `/.../`) se pueden usar como cadena de búsqueda con una combinación de indicadores (como `g`, `i`, `m`) anexados:

>[!INFO]
>
>**Ejemplo:**
>
>![](assets/replace---1-350x31.png)
>
>Todos estos números X X X X se sustituyen por X

La cadena de reemplazo puede incluir los siguientes patrones de reemplazo especiales:

* `$&` Inserta la subcadena coincidente.
* `$n` Donde n es un entero positivo menor que 100, inserta la enésima cadena de subcoincidencias entre paréntesis. Se indexa en 1.

>[!INFO]
>
>**Ejemplos:**
>
>![](assets/variable-value-350x63.png)
>
>Devuelve: número de teléfono `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Devuelve: número de teléfono: `+420777111222`

>[!CAUTION]
>
>No utilice grupos de captura con nombre como `/ is (?<number>\d+)/` en el argumento de cadena de reemplazo. Al hacerlo, se produce un error.

Para obtener más información sobre las expresiones regulares, consulte [Analizador de texto](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL recortar (texto)]

Quita los caracteres de espacio al principio o al final del texto.

## [!UICONTROL mayúsculas (texto)]

Convierte todos los caracteres alfabéticos de una cadena de texto a mayúsculas.

>[!INFO]
>
>**Ejemplo**
>
>`upper( Hello )`
>
>Devuelve: [!UICONTROL HELLO]

## [!UICONTROL subcadena (texto; inicio;fin)]

Devuelve una parte de una cadena de texto entre la posición “inicial” y “final”.

>[!INFO]
>
>**Ejemplos:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Devuelve: Hel
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Devuelve: el

## [!DNL indexOf (string; value; [start])]

Devuelve la posición de la primera aparición de un valor especificado en una cadena. Este método devuelve &#39;-1&#39; si el valor que se busca no está allí. El valor inicial indica en qué punto de la cadena debe comenzar la búsqueda.

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

## [!UICONTROL toBinary (valor)]

Convierte cualquier valor en datos binarios.

También puede especificar la codificación como un segundo argumento para aplicar conversiones binarias de hex o base64 a datos binarios.

>[!INFO]
>
>**Ejemplos:**
>
>* `toBinary( Workfront )`
>
>   Devuelve: 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Devuelve: 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (valor)]

Convierte cualquier valor en una cadena.

## [!UICONTROL encodeURL (texto)]

Codifica los caracteres especiales de algún texto en una dirección URL válida.

## [!UICONTROL decodeURL (texto)]

Decodifica los caracteres especiales de una dirección URL en texto.

>[!INFO]
>
>**Ejemplo:**
>`decodeURL( Automate%20your%20workflow )`
>
>Devuelve: [!UICONTROL Automatizar su flujo de trabajo]

## [!UICONTROL escapeHTML (texto)]

Excluye todas las etiquetas de HTML del texto.

>[!INFO]
>
>**Ejemplo:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Devuelve: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(texto)]

Excluye todas las etiquetas Markdown del texto.

>[!INFO]
>
>**Ejemplo:**
>
>`escapeMarkdown( # Header )`
>
>Devuelve: `&#35; Header`

## [!UICONTROL stripHTML (text)]

Quita todas las etiquetas HTML del texto.

>[!INFO]
>
>**Ejemplo:**
>
>`stripHTML( <b>Hello</b> )`
>
>Devuelve: hello

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

## [!UICONTROL split (text; separator)]

Divide una cadena en una matriz de cadenas separando la cadena en subcadenas.

>[!INFO]
>
>**Ejemplo:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5 (text)]

Calcula el hash md5 de una cadena.

>[!INFO]
>
>**Ejemplo:**
>
>`md5( Workfront )`
>
>Devuelve: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1 (text; [encoding]; [key])]

Calcula el hash sha1 de una cadena. Si se especifica el argumento clave, se devuelve un hash HMAC sha1 en su lugar. Codificaciones compatibles: &quot;hex&quot; (predeterminado), &quot;base64&quot; o &quot;latin1&quot;.

>[!INFO]
>
>**Ejemplo:**
>
>`sha1( workfront )`
>
>Devuelve: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [encoding]; [key])]

Calcula el hash sha256 de una cadena. Si se especifica el argumento clave, se devuelve un hash sha256 HMAC en su lugar. Codificaciones compatibles: &quot;hex&quot; (predeterminado), &quot;base64&quot; o &quot;latin1&quot;.>

>[!INFO]
>
>**Ejemplo:**
>
>`sha256( workfront )`
>
>Devuelve: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (text; [codificación de salida]; [clave]; [codificación clave])]

Calcula el hash sha512 de una cadena. Si se especifica el argumento clave, se devuelve un hash HMAC sha512 en su lugar.

Codificaciones compatibles:

* &quot;[!UICONTROL hex]&quot; (predeterminado)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codificaciones de claves compatibles:

* &quot;[!UICONTROL text]&quot; (predeterminado)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot; o &quot;[!UICONTROL binary]&quot;

Al utilizar la codificación de claves &quot;[!UICONTROL binary]&quot;, una clave debe ser un búfer, no una cadena.

>[!INFO]
>
>**Ejemplo:**
>
>`sha512(workfront)`
>
>Devuelve: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb11 9

## [!UICONTROL base64 (text)]

Transforma el texto en base64.

>[!INFO]
>
>**Ejemplo:**
>
>`base64( workfront )`
>
>Devuelve: d29ya2Zyb250==
