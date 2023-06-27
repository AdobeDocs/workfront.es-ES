---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: La aplicación XML permite analizar un texto con formato XML mediante el módulo XML &get; Parse XML y convertirlo en un paquete para que los datos estén disponibles para otros módulos. También puede convertir un paquete en texto con formato XML mediante el módulo XML &get; Create XML
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 2%

---

# XML

El [!UICONTROL XML] La aplicación permite analizar un texto con formato XML a través de [!UICONTROL XML] > [!UICONTROL Analizar XML] y convertirlo en un paquete para que los datos estén disponibles para otros módulos. También puede convertir un paquete en texto con formato XML mediante el [!UICONTROL XML] > [!UICONTROL Crear XML] módulo

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analizar XML]

El [!UICONTROL XML] > [!UICONTROL Analizar XML] El módulo analiza un texto con formato XML y genera un único paquete que contiene toda la información extraída del XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estructura de datos]</p> </td> 
   <td> <p>La estructura de datos describe la estructura del XML para que la salida del módulo esté disponible en el panel de asignación para los siguientes módulos.</p> <p>Si tiene un ejemplo del XML que desea analizar, puede utilizarlo para generar la estructura de datos:</p> 
    <ol> 
     <li value="1">Haga clic en <strong>[!UICONTROL Agregar]</strong> botón.</li> 
     <li value="2">Haga clic en <strong>[!UICONTROL Generator]</strong> botón.</li> 
     <li value="3">Copiar y pegar el ejemplo XML en <strong>[!UICONTROL Datos de ejemplo]</strong> field.</li> 
     <li value="4">Clic <strong>[!UICONTROL Guardar]</strong>.</li> 
     <li value="5">Compruebe que la estructura de datos se ha generado correctamente.</li> 
     <li value="6"> <p>Haga clic en <strong>[!UICONTROL Guardar]</strong> para guardar la estructura de datos.</p> <p>Puede omitir los pasos 2-5 para proporcionar una estructura de datos vacía. Si la estructura de datos está vacía, la salida del módulo no estará disponible en el panel de asignación hasta que el módulo se haya ejecutado al menos una vez.</p> </li> 
    </ol> <p>Para obtener más información, consulte <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Estructuras de datos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conservar números como texto]</td> 
   <td>Active esta opción para asegurarse de que los números permanecen como valores de texto (cadena). De lo contrario, los números se convierten en valores numéricos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Introduzca o asigne el texto con formato XML que desee analizar.</p> <p>Si usa una fórmula, asegúrese de que su tipo de valor de resultado es (o se puede forzar automáticamente) el tipo de datos [!UICONTROL Text]. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Si el tipo de valor de resultado es [!UICONTROL Buffer] (datos binarios), utilice el <code>toString()</code> para convertirla al tipo de datos Text. Para obtener más información, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a> y <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Para descargar un archivo XML desde una dirección URL y analizar su contenido:
>
>1. Cree un nuevo escenario.
>1. Insertar [!UICONTROL HTTP] > [!UICONTROL Obtener un archivo] módulo
>1. Abra la configuración del módulo y configúrelo de la siguiente manera:
>
>   **URL**: URL del archivo XML (p. ej. `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Clic **[!UICONTROL OK]**&#x200B; guardar y cerrar la configuración del módulo.
1. Añadir [!UICONTROL XML] > [!UICONTROL Analizar XML] módulo, conéctelo después de que [!UICONTROL HTTP] > [!UICONTROL Obtener un archivo] y configúrelo de la siguiente manera:
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Estructura de datos]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Haga clic en <strong>[!UICONTROL Agregar]</strong> botón.</li> 
&gt;        <li value="2">Haga clic en <strong>[!UICONTROL Generator]</strong> botón.</li> 
&gt;        <li value="3">En el explorador web, abra una nueva pestaña o ventana.</li> 
&gt;        <li value="4">Coloque la dirección URL que utilizó en el tercer paso en la barra de direcciones y recupere el archivo XML.</li> 
&gt;        <li value="5">Seleccione todo el texto XML y cópielo en el portapapeles.</li> 
&gt;        <li value="6">Cierre la pestaña o la ventana y vuelva a su escenario.</li> 
&gt;        <li value="7">Pegue el texto XML copiado en el campo Datos de ejemplo.</li> 
&gt;        <li value="8">Clic <strong>[!UICONTROL Guardar]</strong>.</li> 
&gt;        <li value="9">Compruebe que la estructura de datos se ha generado correctamente.</li> 
&gt;        <li value="10">Clic <strong>[!UICONTROL Guardar]</strong> para guardar la estructura de datos.</li> 
&gt;       </ol> <p>Puede omitir los pasos del 2 al 9 para proporcionar una estructura de datos vacía. Si la estructura de datos está vacía, la salida del módulo no estará disponible en el panel de asignación hasta que el módulo se haya ejecutado al menos una vez.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Asignar el <code>Data </code>elemento de la salida del módulo [!UICONTROL HTTP] &gt; [!UICONTROL Obtener un archivo] en el campo. Utilice el <code>toString()</code> para convertir su valor del tipo [!UICONTROL Buffer] (datos binarios) al tipo de datos [!UICONTROL Text].</p> <p>Puede copiar y pegar el código de la fórmula en el campo: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Para obtener más información sobre los tipos de datos Búfer y Texto, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL Análisis de atributos XML]

De forma predeterminada, la variable [!UICONTROL XML] > [!UICONTROL Analizar XML] El módulo coloca los atributos en una colección especial `_attributes` como elemento secundario del nodo que tiene estos atributos. Si el nodo es un nodo de texto y tiene atributos, se agregan dos propiedades especiales: `_attributes` para atributos y `_value` para el contenido de texto del nodo.

>[!INFO]
>
**Ejemplo:** Este XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

se convierte en este paquete:

![](assets/xml-converted-to-bundle.png)

## Crear XML

El [!UICONTROL XML] > [!UICONTROL Crear XML] convierte un paquete en un texto con formato XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estructura de datos]</p> </td> 
   <td> <p>La estructura Data describe la estructura del XML resultante. Si tiene un ejemplo del XML que desea crear, puede utilizarlo para generar la estructura de datos:</p> 
    <ol> 
     <li value="1">Haga clic en <strong>[!UICONTROL Agregar]</strong> botón.</li> 
     <li value="2">Haga clic en <strong>[!UICONTROL Generator]</strong> botón.</li> 
     <li value="3">Copie y pegue el ejemplo XML en el campo Datos de ejemplo.</li> 
     <li value="4">Haga clic en <strong>[!UICONTROL Guardar]</strong> botón.</li> 
     <li value="5">Compruebe que la estructura de datos se ha generado correctamente.</li> 
     <li value="6">Clic <strong>[!UICONTROL Guardar]</strong> para guardar la estructura de datos.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre del elemento raíz]</td> 
   <td>Introduzca el nombre del elemento raíz del XML. El valor predeterminado es <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype ID DEL SISTEMA]</td> 
   <td>Introduzca el nombre de archivo que desea utilizar en la<code> !DOCTYPE SYSTEM</code> declaración</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Introduzca el nombre de archivo que desea utilizar en la<code> !DOCTYPE PUBLIC</code> declaración</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml Statement]</td> 
   <td>Active esta opción para quitar la declaración XML <code>&lt;?xml ... ?&gt;</code> y <code>&lt;!DOCTYPE ... &gt;</code>y deje solo el elemento raíz XML y su contenido.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**Ejemplo:**
>
Un caso de uso típico es transformar datos de una [!DNL Google] >hoja de cálculo en XML.
>
1. Coloque el [!DNL Google Sheets] > [!UICONTROL Seleccionar filas] en su escenario para recuperar los datos. Configure el módulo para recuperar filas de su [!DNL Google] hoja de cálculo. Configure las variables&#x200B;**[!UICONTROL Número máximo de filas devueltas]** a un número pequeño, pero mayor que uno para fines de prueba (por ejemplo, tres). Ejecute el [!DNL Google Sheets] haciendo clic con el botón derecho en él y seleccionando &quot;**[!UICONTROL Ejecutar solo este módulo]**.&quot; Compruebe la salida del módulo.
1. Conecte el [!UICONTROL Agregador de matrices] después del módulo [!DNL Google Sheets] módulo. En la configuración del módulo, seleccione la opción [!DNL Google Sheets] módulo en el **[!UICONTROL Nodo de origen]** field. Deje los demás campos tal como están por el momento.
1. Conecte el [!UICONTROL XML] > [!UICONTROL Crear XML] después del módulo [!UICONTROL Agregador de matrices] módulo.
>
La configuración del módulo requiere una estructura de datos que describa la estructura de la salida XML. Haga clic en **[!UICONTROL Añadir]** para abrir la configuración de la estructura de datos. La forma más sencilla de crear esta estructura de datos es generarla automáticamente a partir de un ejemplo XML.
>
1. Haga clic en **[!UICONTROL Generador]** y pegue el ejemplo XML en el [!UICONTROL Datos de muestra] campo:
>
![](assets/sample-data-field-350x146.png)
>
1. Haga clic en **[!UICONTROL Guardar]**. El campo Especificación (Specification) de la estructura de datos contiene ahora la estructura generada.
1. Cambie el nombre de la estructura de datos a algo más específico y haga clic en **[!UICONTROL Guardar]**. Un campo correspondiente al atributo de matriz raíz aparece como un campo asignable en la configuración del módulo JSON.
1. Haga clic en **[!UICONTROL Mapa]** situado junto al campo y asigne la variable `Array[]` elemento de la [!UICONTROL Agregador de matrices] salida para él:
1. Clic **[!UICONTROL OK]** para cerrar la configuración del módulo XML.
1. Abra la configuración del [!UICONTROL Agregador de matrices] módulo. Cambie el **[!UICONTROL Estructura de destino]** desde Personalizado hasta el campo de un módulo XML correspondiente a los elementos XML primarios. Asigne elementos desde el campo [!DNL Google Sheets] a los campos correspondientes.
1. Clic **[!UICONTROL OK]** para cerrar la configuración del módulo Array Aggregator.
1. Ejecute el escenario.
>
El módulo XML genera el archivo XML correcto.
>
1. Abra la configuración del [!DNL Google Sheets] y aumente el [!UICONTROL Número máximo de filas devueltas] número que será mayor que el número de filas de la hoja de cálculo para procesar todos los datos.
>
El XML resultante se puede guardar en [!DNL Dropbox], enviado como archivo adjunto por correo electrónico, cargado a través de FTP a un servidor, etc.

## Adición de atributos XML

Si desea agregar atributos a un nodo complejo (un nodo que contendrá otros nodos), debe agregar una colección con el nombre `_attributes` para la nota compleja de la estructura de datos personalizada. Esta colección se asignará a atributos de nodo. Si desea agregar atributos a un nodo de texto (por ejemplo: `<node attr="1">abc</node>`), debe agregar una colección `_attributes` para atributos y una propiedad de texto `_value` para el valor del nodo para este nodo en la estructura de datos personalizada.

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

## Solución de problemas: no se pueden asignar datos del [!UICONTROL Analizar XML] módulo

Asegúrese de que la estructura de datos está definida correctamente. También puede utilizar una estructura de datos vacía y ejecutar el módulo al menos una vez para procesar una entrada XML.
