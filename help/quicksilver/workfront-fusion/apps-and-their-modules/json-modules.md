---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos JSON
description: La aplicación JSON de Adobe Workfront Fusion proporciona módulos para procesar datos en formato JSON de modo que Adobe Workfront Fusion pueda trabajar más con el contenido de datos o crear nuevo contenido JSON.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] módulos

La variable [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] la aplicación proporciona módulos para procesar datos en formato JSON de modo que [!DNL Adobe Workfront Fusion] puede trabajar más con el contenido de datos o crear nuevo contenido JSON.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Analizar JSON

* [Estructura de datos](#data-structure)
* [Colección frente a matriz](#collection-vs-array)

### Estructura de datos

La estructura de datos describe cómo se organizan los datos JSON y permite la asignación de elementos JSON individuales a otros módulos en el escenario. Si no proporciona la estructura Data , puede ejecutar manualmente el módulo y [!DNL Workfront Fusion] compilará la estructura a partir del JSON proporcionado:

1. Agregue la variable [!UICONTROL Analizar JSON] a un escenario.
1. En el **[!UICONTROL Cadena JSON]** , introduzca el JSON desde el que desea crear una estructura de datos.
1. No conecte otros módulos al [!UICONTROL Analizar JSON] todavía. Porque [!DNL Workfront Fusion] aún no conoce la estructura de los datos JSON, no es posible asignar datos del [!UICONTROL Analizar JSON] a otros módulos en su situación.
1. Ejecute el escenario manualmente. Esto permite que la variable [!UICONTROL Analizar JSON] para identificar la estructura JSON del JSON que ha proporcionado.
1. Ahora puede conectar los siguientes módulos. Los elementos del módulo Parse JSON ya están disponibles para su asignación.

Para obtener más información, consulte [Estructuras de datos en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Colección frente a matriz

Si el campo de cadena JSON contiene una colección `{ ... }`, El resultado es un paquete único que contiene los elementos de la colección.

>[!INFO]
>
>**Ejemplo:**
>
>
```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Si el campo de cadena JSON contiene una matriz `[ ... ]`, el resultado es una serie de paquetes. cada paquete contiene un elemento de la matriz.

>[!INFO]
>
>**Ejemplo:**
>
>
```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] módulos y sus campos

Al configurar [!DNL JSON] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Junto con estos, podrían mostrarse campos JSON adicionales, según factores como su nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Agregar a JSON](#aggregate-to-json)
* [Convertir JSON a XML](#convert-json-to-xml)
* [Analizar JSON](#parse-json)
* [Crear JSON](#create-json)
* [Transformar JSON](#transform-json)

### [!UICONTROL Agregar a JSON]

Este módulo de agregador agrega el resultado de un módulo anterior a JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source module] </td> 
   <td> <p>Seleccione el módulo que genera los datos que desea agregar a JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Seleccione la estructura de datos que desea utilizar para crear JSON. La estructura de datos determina qué otros campos están disponibles en este módulo. Para obtener más información, consulte <a href="#data-structure" class="MCXref xref">Estructura de datos</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sangría]</td> 
   <td> <p> Seleccione si desea aplicar sangría al JSON mediante pestañas, dos espacios o cuatro espacios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>Defina una expresión por la que desee agrupar la salida agregada. Esta expresión puede contener uno o más elementos asignados. Los datos agregados se separan en grupos utilizando el valor de esta expresión. Cada grupo genera un paquete independiente con una clave (la expresión evaluada) y un valor (el texto agregado). Puede utilizar la clave como filtro en los módulos siguientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Detenga el procesamiento después de una agregación vacía]</td> 
   <td>Active esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir JSON a XML]

Este módulo de acción convierte una cadena JSON a XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena JSON] </td> 
   <td> <p>Introduzca o asigne el JSON que desea convertir en XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analizar JSON]

Este módulo de acción analiza una cadena JSON en una estructura de datos, lo que le permite acceder a los datos dentro de la cadena JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Seleccione la estructura de datos que desea utilizar para crear JSON. Para obtener más información, consulte <a href="#data-structure" class="MCXref xref">Estructura de datos</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena JSON] </td> 
   <td> <p>Introduzca o asigne el JSON que desea analizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Crear JSON]

Este módulo de acción crea JSON a partir de una estructura de datos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Estructura de datos</td> 
   <td> <p>Seleccione la estructura de datos que desea utilizar para crear JSON. Para obtener más información, consulte <a href="#data-structure" class="MCXref xref">Estructura de datos</a> en este artículo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Transformar JSON]

Este módulo de acción transforma un objeto en una cadena json.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL (objeto)</td> 
   <td> <p>Introduzca o asigne el objeto que desea transformar en JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Transformación de registros de datos a JSON

>[!INFO]
>
>**Ejemplo:** El siguiente ejemplo muestra cómo transformar registros de datos de [!DNL Google Sheets] al formato JSON:
>
>1. Coloque el [!DNL Google Sheets] > [!UICONTROL Seleccionar filas] en su escenario para recuperar los datos. Configure el módulo para recuperar filas de su [!DNL Google] hoja de cálculo. Configure el &#x200B;**[!UICONTROL Número máximo de filas devueltas]** a un número pequeño, pero mayor que uno con fines de prueba (por ejemplo, tres). Ejecute el [!DNL Google Sheets] , haga clic con el botón derecho del ratón y elija &quot;**[!UICONTROL Ejecutar solo este módulo]**.&quot; Compruebe la salida del módulo.
1. Conecte el [!UICONTROL Agregador de matrices] después del [!DNL Google Sheets] módulo. En la configuración del módulo, elija la opción [!DNL Google Sheets] en el **[!UICONTROL Nodo de origen]** campo . Deje los otros campos tal como están por el momento.
1. Connect [!UICONTROL JSON] > [!UICONTROL Crear JSON] después del [!UICONTROL Agregador de matrices] módulo. La configuración del módulo requiere una estructura de datos que describa el formato JSON. Haga clic en **[!UICONTROL Agregar]** para abrir la configuración de la estructura de datos. La forma más sencilla de crear esta estructura de datos es generarla automáticamente a partir de una muestra de JSON. Haga clic en **[!UICONTROL Generador]** y pegue su muestra de JSON en el **[!UICONTROL Datos de muestra]** campo:

   **Ejemplo:**
   ```
   {
   
   "books": [
   
   {
   
   "id": "ID",
   
   "title": "Title",
   
   "author": "Author"
   
   }
   
   ]
   
   }
   ```
1. Haga clic en **[!UICONTROL Guardar]**. La variable [!UICONTROL Especificación] del campo Data structure ahora contiene la estructura generada.
1. Cambie el nombre de la estructura de datos por otro más específico y haga clic en **[!UICONTROL Guardar]**. Un campo correspondiente al atributo de matriz raíz aparece como un campo asignable en la configuración del módulo JSON.
1. Haga clic en el **[!UICONTROL Mapa]** situado junto al campo y asigne la variable `Array[]` elemento de la salida Array agregator a él.
1. Haga clic en **[!UICONTROL OK]** para cerrar el [!UICONTROL JSON] configuración del módulo.
1. Abra la configuración del [!UICONTROL Agregador de matrices] módulo. Cambie el **[!UICONTROL Estructura de destino]** from [!UICONTROL Personalizado] a [!UICONTROL JSON] campo del módulo correspondiente al atributo de matriz raíz. Asigne elementos desde [!DNL Google Sheets] a los campos correspondientes.
1. Haga clic en **[!UICONTROL OK]** para cerrar el [!UICONTROL Agregador de matrices] configuración del módulo.
1. Ejecute el escenario.
   La variable [!UICONTROL JSON] genera el formato JSON correcto.
1. Abra la configuración del [!DNL Google Sheets] y aumente el [!UICONTROL Número máximo de filas devueltas] para que sea mayor que el número de filas de la hoja de cálculo para procesar todos los datos.


## Resolución de problemas

### No se pueden asignar datos desde la variable [!UICONTROL Analizar JSON] módulo

Asegúrese de que el contenido JSON esté correctamente asignado a la variable [!UICONTROL Analizar JSON] y que la estructura de datos está correctamente definida. Para obtener más información, consulte [Transformación de registros de datos a JSON](#transforming-data-records-to-json) en este artículo.

### El módulo falla al usar afirmaciones condicionales en JSON

Al utilizar afirmaciones condicionales como `if` en su JSON, ponga las comillas fuera de la afirmación condicional.

>[!INFO]
**Ejemplo:**
![](assets/quotes-in-json-350x120.png)
