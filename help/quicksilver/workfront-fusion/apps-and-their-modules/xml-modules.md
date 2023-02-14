---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: La aplicación XML permite analizar un texto con formato XML mediante XML &gt; Analice el módulo XML y conviértelo en un paquete para que los datos estén disponibles para otros módulos. También puede convertir un paquete en un texto con formato XML mediante XML &gt; Crear módulo XML
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 1%

---

# XML

La variable [!UICONTROL XML] permite analizar un texto con formato XML mediante la variable [!UICONTROL XML] > [!UICONTROL Analizar XML] y conviértala en un paquete para que los datos estén disponibles para otros módulos. También puede convertir un paquete en un texto con formato XML mediante la variable [!UICONTROL XML] > [!UICONTROL Crear XML] módulo

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analizar XML]

La variable [!UICONTROL XML] > [!UICONTROL Analizar XML] analiza un texto con formato XML y genera un paquete único que contiene toda la información extraída del XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>La estructura de datos describe la estructura del XML para que la salida del módulo esté disponible en el panel de asignación para los siguientes módulos.</p> <p>Si tiene un ejemplo del XML que desea analizar, puede utilizarlo para generar la estructura de datos:</p> 
    <ol> 
     <li value="1">Haga clic en el <strong>[!UICONTROL Agregar]</strong> botón.</li> 
     <li value="2">Haga clic en el <strong>[!UICONTROL Generator]</strong> botón.</li> 
     <li value="3">Copie y pegue el ejemplo XML en el <strong>[!UICONTROL Datos de muestra]</strong> campo .</li> 
     <li value="4">Haga clic en <strong>[!UICONTROL Guardar]</strong>.</li> 
     <li value="5">Compruebe que la estructura de datos se haya generado correctamente.</li> 
     <li value="6"> <p>Haga clic en el <strong>[!UICONTROL Guardar]</strong> para guardar la estructura de datos.</p> <p>Puede omitir los pasos 2-5 para proporcionar una estructura de datos vacía. Si la estructura de datos está vacía, la salida del módulo no está disponible en el panel de asignación hasta que el módulo se haya ejecutado al menos una vez.</p> </li> 
    </ol> <p>Para obtener más información, consulte <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Estructuras de datos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conservar números como texto]</td> 
   <td>Active esta opción para garantizar que los números se mantengan como valores de texto (cadena). De lo contrario, los números se convierten en valores numéricos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Introduzca o asigne el texto con formato XML que desee analizar.</p> <p>Si utiliza una fórmula, asegúrese de que su tipo de valor de resultado sea (o se pueda forzar automáticamente a) el tipo de datos [!UICONTROL Text]. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Si el tipo de valor de resultado es [!UICONTROL Buffer] (datos binarios), utilice la variable <code>toString()</code> para convertirla al tipo de datos Text . Para obtener más información, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a> y <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Para descargar un archivo XML desde una URL y analizar su contenido:
>
>1. Cree un nuevo escenario.
>1. Insertar [!UICONTROL HTTP] > [!UICONTROL Obtener un archivo] módulo
>1. Abra la configuración del módulo y configúrela de la siguiente manera:

>
>   **URL**: URL del archivo XML (p. ej. `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Haga clic en **[!UICONTROL OK]**&#x200B; guardar y cerrar la configuración del módulo.
>1. Agregar [!UICONTROL XML] > [!UICONTROL Analizar XML] , conéctelo después de [!UICONTROL HTTP] > [!UICONTROL Obtener un archivo] y configúrelo de la siguiente manera:
><table style="table-layout:auto"> 
>    <col> 
>    <col> 
>    <tbody> 
>     <tr> 
>      <td role="rowheader">[!UICONTROL Data structure]</td> 
>      <td> 
>       <ol> 
>       <li value="1">Haga clic en el <strong>[!UICONTROL Agregar]</strong> botón.</li> 
>        <li value="2">Haga clic en el <strong>[!UICONTROL Generator]</strong> botón.</li> 
>        <li value="3">En el explorador web, abra una nueva pestaña o ventana.</li> 
>        <li value="4">Coloque la dirección URL utilizada en el tercer paso de la barra de direcciones y busque el archivo XML.</li> 
>        <li value="5">Seleccione todo el texto XML y cópielo en el portapapeles.</li> 
>        <li value="6">Cierre la pestaña o la ventana y vuelva al escenario.</li> 
>        <li value="7">Pegue el texto XML copiado en el campo Sample data .</li> 
>        <li value="8">Haga clic en <strong>[!UICONTROL Guardar]</strong>.</li> 
>        <li value="9">Compruebe que la estructura de datos se haya generado correctamente.</li> 
>        <li value="10">Haga clic en <strong>[!UICONTROL Guardar]</strong> para guardar la estructura de datos.</li> 
>       </ol> <p>Puede omitir los pasos del 2 al 9 para proporcionar una estructura de datos vacía. Si la estructura de datos está vacía, la salida del módulo no está disponible en el panel de asignación hasta que el módulo se haya ejecutado al menos una vez.</p> </td> 
>     </tr> 
>     <tr> 
>      <td role="rowheader">[!UICONTROL XML]</td> 
>      <td> <p>Asigne la variable <code>Data </code>elemento de la salida del módulo [!UICONTROL HTTP] &gt; [!UICONTROL Get a file] en el campo . Utilice la variable <code>toString()</code> para convertir su valor del tipo de datos [!UICONTROL Buffer] (datos binarios) al tipo de datos [!UICONTROL Text].</p> <p>Puede copiar y pegar el código de la fórmula en el campo : <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Para obtener más información sobre los tipos de datos Buffer y Text , consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
>     </tr> 
>    </tbody> 
>   </table>


## [!UICONTROL Análisis de atributos XML]

De forma predeterminada, la variable [!UICONTROL XML] > [!UICONTROL Analizar XML] el módulo coloca los atributos en una colección especial `_attributes` como elemento secundario del nodo que tiene estos atributos. Si el nodo es un nodo de texto y tiene atributos, se añaden dos propiedades especiales: `_attributes` para atributos y `_value` para el contenido de texto del nodo .

>[!INFO]
>**Ejemplo:** Este XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

se convierte en este paquete:

![](assets/xml-converted-to-bundle.png)

## Crear XML

La variable [!UICONTROL XML] > [!UICONTROL Crear XML] convierte un paquete en un texto con formato XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>La estructura Data describe la estructura del XML resultante. Si tiene un ejemplo del XML que desea crear, puede utilizarlo para generar la estructura de datos:</p> 
    <ol> 
     <li value="1">Haga clic en el <strong>[!UICONTROL Agregar]</strong> botón.</li> 
     <li value="2">Haga clic en el <strong>[!UICONTROL Generator]</strong> botón.</li> 
     <li value="3">Copie y pegue el ejemplo XML en el campo Sample data .</li> 
     <li value="4">Haga clic en el <strong>[!UICONTROL Guardar]</strong> botón.</li> 
     <li value="5">Compruebe que la estructura de datos se haya generado correctamente.</li> 
     <li value="6">Haga clic en <strong>[!UICONTROL Guardar]</strong> para guardar la estructura de datos.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre del elemento raíz]</td> 
   <td>Introduzca el nombre del elemento raíz del XML. El valor predeterminado es <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Escriba el nombre de archivo que se va a usar en la variable<code> !DOCTYPE SYSTEM</code> declaración</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Escriba el nombre de archivo que se va a usar en la variable<code> !DOCTYPE PUBLIC</code> declaración</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml declaration]</td> 
   <td>Active esta opción para eliminar la declaración XML <code>&lt;?xml ... ?&gt;</code> y <code>&lt;!DOCTYPE ... &gt;</code>y deje solo el elemento raíz XML y su contenido.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>**Ejemplo:**
>Un caso de uso típico es transformar datos de una [!DNL Google] >hoja de cálculo en XML.
>1. Coloque el [!DNL Google Sheets] > [!UICONTROL Seleccionar filas] en su escenario para recuperar los datos. Configure el módulo para recuperar filas de su [!DNL Google] hoja de cálculo. Configure el &#x200B;**[!UICONTROL Número máximo de filas devueltas]** a un número pequeño, pero mayor que uno con fines de prueba (por ejemplo, tres). Ejecute el [!DNL Google Sheets] , haga clic con el botón derecho del ratón y elija &quot;**[!UICONTROL Ejecutar solo este módulo]**.&quot; Compruebe la salida del módulo.
>1. Conecte el [!UICONTROL Agregador de matrices] después del [!DNL Google Sheets] módulo. En la configuración del módulo, elija la opción [!DNL Google Sheets] en el **[!UICONTROL Nodo de origen]** campo . Deje los otros campos tal como están por el momento.
>1. Conecte el [!UICONTROL XML] > [!UICONTROL Crear XML] después del [!UICONTROL Agregador de matrices] módulo.
>   La configuración del módulo requiere una estructura de datos que describa la estructura de la salida XML. Haga clic en el **[!UICONTROL Agregar]** para abrir la configuración de la estructura de datos. La forma más sencilla de crear esta estructura de datos es generarla automáticamente a partir de un ejemplo XML.
>1. Haga clic en el **[!UICONTROL Generador]** y pegue el ejemplo XML en el [!UICONTROL Datos de muestra] campo:
>
>   ![](assets/sample-data-field-350x146.png)
>
>1. Haga clic en **[!UICONTROL Guardar]**. El campo Specification de la estructura Data ahora contiene la estructura generada.
>1. Cambie el nombre de la estructura de datos por otro más específico y haga clic en **[!UICONTROL Guardar]**. Un campo correspondiente al atributo de matriz raíz aparece como un campo asignable en la configuración del módulo JSON.
>1. Haga clic en el **[!UICONTROL Mapa]** situado junto al campo y asigne la variable `Array[]` del [!UICONTROL Agrupador de matrices] salida:
>1. Haga clic en **[!UICONTROL OK]** para cerrar la configuración del módulo XML.
>1. Abra la configuración del [!UICONTROL Agregador de matrices] módulo. Cambie el **[!UICONTROL Estructura de destino]** de Personalizado a un campo del módulo XML correspondiente al elemento XML principal.Asigne elementos del [!DNL Google Sheets] a los campos correspondientes.
>1. Haga clic en **[!UICONTROL OK]** para cerrar la configuración del módulo Array Aggregator.
>1. Ejecute el escenario.
>
>   El módulo XML genera el archivo XML correcto.
>1. Abra la configuración del [!DNL Google Sheets] y aumente el [!UICONTROL Número máximo de filas devueltas] para que sea mayor que el número de filas de la hoja de cálculo para procesar todos los datos.
>   El XML resultante se puede guardar en [!DNL Dropbox], se envían como datos adjuntos por correo electrónico, se cargan mediante FTP en un servidor, etc.


## Adición de atributos XML

Si desea agregar atributos a un nodo complejo (un nodo que contendrá otros nodos), debe agregar una colección con el nombre `_attributes` para la nota compleja en la estructura de datos personalizada. Esta colección se asignará a atributos de nodo. Si desea agregar atributos a un nodo de texto (por ejemplo: `<node attr="1">abc</node>`), debe agregar una colección `_attributes` para atributos y una propiedad text `_value` para el valor node de este nodo en su estructura de datos personalizada.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Solución de problemas: No se pueden asignar datos desde la variable [!UICONTROL Analizar XML] módulo

Asegúrese de que la estructura de datos esté definida correctamente. Como alternativa, puede utilizar una estructura de datos vacía y ejecutar el módulo al menos una vez para procesar una entrada XML.
