---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 93%

---

# XML

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [XML](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/xml-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

La aplicación [!UICONTROL XML] permite analizar un texto con formato XML mediante el módulo [!UICONTROL XML] > [!UICONTROL Parse XML] y convertirlo en un paquete para que los datos estén disponibles para otros módulos. También puede convertir un paquete en texto con formato XML a través del módulo [!UICONTROL XML] > [!UICONTROL Create XML]

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analizar XML]

El módulo [!UICONTROL XML] > [!UICONTROL Analizar XML] analiza un texto con formato XML y genera un solo paquete que contiene toda la información extraída del XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>La estructura de datos describe la estructura del XML para que la salida del módulo esté disponible en el panel de asignación para los siguientes módulos.</p> <p>Si tiene una muestra del XML que desea analizar, puede utilizarla para generar la estructura de datos:</p> 
    <ol> 
     <li value="1">Haga clic en el botón <strong>[!UICONTROL Add]</strong>.</li> 
     <li value="2">Haga clic en el botón <strong>[!UICONTROL Generator]</strong>.</li> 
     <li value="3">Copie y pegue la muestra de XML en el campo <strong>[!UICONTROL Sample data]</strong>.</li> 
     <li value="4">Haga clic en <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Compruebe que la estructura de datos se haya generado correctamente.</li> 
     <li value="6"> <p>Haga clic en el botón <strong>[!UICONTROL Save]</strong> para guardar la estructura de datos.</p> <p>Puede omitir los pasos 2-5 para proporcionar una estructura de datos vacía. Si la estructura de datos está vacía, la salida del módulo no estará disponible en el panel de asignación hasta que el módulo se haya ejecutado al menos una vez.</p> </li> 
    </ol> <p>Para obtener más información, consulte <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Estructuras de datos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve numbers as text]</td> 
   <td>Habilite esta opción para garantizar que los números permanezcan como valores de texto (cadena). De lo contrario, los números se convertirán en valores numéricos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Introduzca o asigne el texto con formato XML que desee analizar.</p> <p>Si usa una fórmula, asegúrese de que su tipo de valor resultante sea el tipo de datos [!UICONTROL Text] (o se pueda forzar automáticamente a dicho tipo de datos). </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Si el tipo de valor resultante es [!UICONTROL Buffer] (datos binarios), use la función <code>toString()</code> para convertirlo al tipo de datos de texto. Para obtener más información, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a> y <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** para descargar un archivo XML desde una URL y analizar su contenido:
>
>1. Cree un nuevo escenario. 
>1. Inserte el módulo [!UICONTROL HTTP] > [!UICONTROL Obtener un archivo]
>1. Abra la configuración del módulo y configúrelo de la siguiente manera:
>
>   **URL**: URL del archivo XML (p. ej., `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Haga clic en **[!UICONTROL Aceptar]** para guardar y cerrar la configuración del módulo.
1. Añada el módulo [!UICONTROL XML] > [!UICONTROL Analizar XML], conéctelo después del módulo [!UICONTROL HTTP] > [!UICONTROL Obtenga un archivo] y configúrelo de la siguiente manera:
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Data structure]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Haga clic en el botón <strong>[!UICONTROL Add]</strong>.</li> 
&gt;        <li value="2">Haga clic en el botón <strong>[!UICONTROL Generator]</strong>.</li> 
&gt;        <li value="3">En el explorador web, abra una nueva pestaña o ventana.</li> 
&gt;        <li value="4">Coloque la dirección URL que utilizó en el tercer paso en la barra de direcciones y recupere el archivo XML.</li> 
&gt;        <li value="5">Seleccione todo el texto XML y cópielo en el portapapeles.</li> 
&gt;        <li value="6">Cierre la pestaña o la ventana y vuelva a su escenario.</li> 
&gt;        <li value="7">Pegue el texto XML copiado en el campo Datos de muestra.</li> 
&gt;        <li value="8">Haga clic en <strong>[!UICONTROL Save]</strong>.</li> 
&gt;        <li value="9">Compruebe que la estructura de datos se haya generado correctamente.</li> 
&gt;        <li value="10">Haga clic en <strong>[!UICONTROL Save]</strong> para guardar la estructura de datos.</li> 
&gt;       </ol> <p>Puede omitir los pasos del 2 al 9 para proporcionar una estructura de datos vacía. Si la estructura de datos está vacía, la salida del módulo no estará disponible en el panel de asignación hasta que el módulo se haya ejecutado al menos una vez.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Asigne el elemento <code>Data </code> de la salida del módulo [!UICONTROL HTTP] &gt; [!UICONTROL Get a file] al campo. Utilice la función <code>toString()</code> para convertir su valor del tipo [!UICONTROL Buffer] (datos binarios) al tipo de datos [!UICONTROL Text].</p> <p>Puede copiar y pegar el código de la fórmula en el campo: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Para obtener más información sobre los tipos de datos de texto y búfer, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL Análisis de atributos XML]

De manera predeterminada, el módulo [!UICONTROL XML] > [!UICONTROL Analizar XML] coloca los atributos en una colección especial `_attributes` como elemento secundario del nodo que tiene estos atributos. Si el nodo es un nodo de texto y tiene atributos, se añaden dos propiedades especiales: `_attributes` para los atributos y `_value` para el contenido de texto del nodo.

>[!INFO]
>
**Ejemplo:** este XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

se convierte en este paquete:

![](assets/xml-converted-to-bundle.png)

## Crear XML

El módulo [!UICONTROL XML] > [!UICONTROL Crear XML] convierte un paquete en texto con formato XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>La estructura de datos describe la estructura del XML resultante. Si tiene un ejemplo del XML que desea crear, puede utilizarlo para generar la estructura de datos:</p> 
    <ol> 
     <li value="1">Haga clic en el botón <strong>[!UICONTROL Add]</strong>.</li> 
     <li value="2">Haga clic en el botón <strong>[!UICONTROL Generator]</strong>.</li> 
     <li value="3">Copie y pegue el XML de ejemplo en el campo Datos de ejemplo.</li> 
     <li value="4">Haga clic en el botón <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Compruebe que la estructura de datos se haya generado correctamente.</li> 
     <li value="6">Haga clic en <strong>[!UICONTROL Save]</strong> para guardar la estructura de datos.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Root element name]</td> 
   <td>Introduzca el nombre del elemento raíz del XML. El valor predeterminado es <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Escriba el nombre de archivo que se usará en la declaración <code> !DOCTYPE SYSTEM</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Escriba el nombre de archivo que se usará en la declaración <code> !DOCTYPE PUBLIC</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml Declaration]</td> 
   <td>Active esta opción para quitar la declaración XML <code>&lt;?xml ... ?&gt;</code> y <code>&lt;!DOCTYPE ... &gt;</code> y dejar solamente el elemento raíz XML y su contenido.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**Ejemplo:**
>
Un caso de uso típico es transformar datos de una hoja de cálculo de [!DNL Google] > en XML.
>
1. Coloque el módulo [!DNL Google Sheets] > [!UICONTROL Seleccionar filas] en su escenario para recuperar los datos. Configure el módulo para recuperar filas de la hoja de cálculo de [!DNL Google]. Establezca el **[!UICONTROL Número máximo de filas devueltas]** en un número pequeño, pero mayor que uno para realizar pruebas (por ejemplo, tres). Ejecute el módulo de [!DNL Google Sheets] haciendo clic con el botón secundario en él y eligiendo &quot;**[!UICONTROL Ejecutar este módulo solamente]**&quot;. Compruebe la salida del módulo.
1. Conecte el módulo [!UICONTROL Agregador de matrices] después del módulo [!DNL Google Sheets]. En la configuración del módulo, elija el módulo de [!DNL Google Sheets] en el campo **[!UICONTROL Nodo de origen]**. Deje los demás campos tal como están por el momento.
1. Conecte el módulo [!UICONTROL XML] > [!UICONTROL Crear XML] después del módulo [!UICONTROL Agregador de matrices].
>
La configuración del módulo requiere una estructura de datos que describa la estructura de la salida XML. Haga clic en el botón **[!UICONTROL Añadir]** para abrir la configuración de la estructura de datos. La forma más sencilla de crear esta estructura de datos es generarla automáticamente a partir de un ejemplo XML.
>
1. Haga clic en el botón **[!UICONTROL Generador]** y pegue el XML de ejemplo en el campo [!UICONTROL Datos de muestra]:
>
![](assets/sample-data-field-350x146.png)
>
1. Haga clic en **[!UICONTROL Guardar]**. El campo Especificación de la estructura de datos contiene ahora la estructura generada.
1. Cambie el nombre de la estructura de datos por otro más específico y haga clic en **[!UICONTROL Guardar]**. Un campo correspondiente al atributo de la matriz raíz aparece como un campo asignable en la configuración del módulo JSON.
1. Haga clic en el botón **[!UICONTROL Asignar]** que está al lado del campo y asígnele el elemento `Array[]` de la salida del [!UICONTROL Agregador de matrices]:
1. Haga clic en **[!UICONTROL Aceptar]** para cerrar la configuración del módulo XML.
1. Abra la configuración del módulo [!UICONTROL Agregador de matrices]. Cambie la **[!UICONTROL estructura de destino]** del campo personalizado a un campo del módulo XML correspondiente al elemento XML principal. Asigne elementos del módulo de [!DNL Google Sheets] a los campos apropiados.
1. Haga clic en **[!UICONTROL Aceptar]** para cerrar la configuración del módulo Agregador de matrices.
1. Ejecute el escenario.
>
El módulo XML genera el archivo XML correcto.
>
1. Abra la configuración del módulo [!DNL Google Sheets] y aumente el número [!UICONTROL Máximo número de filas devueltas] para que sea mayor que el número de filas de la hoja de cálculo y procesar todos los datos.
>
El XML resultante se puede guardar en [!DNL Dropbox], enviar como archivo adjunto por correo electrónico, subir por FTP a un servidor, etc.

## Adición de atributos XML

Si desea añadir atributos a un nodo complejo (un nodo que contendrá otros nodos), debe añadir una colección con el nombre `_attributes` para la nota compleja en la estructura de datos personalizada. Esta colección se asignará a atributos de nodo. Si desea añadir atributos a un nodo de texto (por ejemplo: `<node attr="1">abc</node>`), debe añadir una colección `_attributes` para atributos y una propiedad de texto `_value` para el valor del nodo para este nodo en la estructura de datos personalizada.

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

## Solución de problemas: no se pueden asignar datos del módulo [!UICONTROL Analizar XML]

Asegúrese de que la estructura de datos está definida correctamente. También puede utilizar una estructura de datos vacía y ejecutar el módulo al menos una vez para procesar una entrada XML.
