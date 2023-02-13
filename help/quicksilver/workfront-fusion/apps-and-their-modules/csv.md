---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Los módulos CSV de Adobe Workfront Fusion permiten crear archivos CSV y analizar el texto CSV a partir de un valor de texto recibido o un archivo.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

La variable [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] los módulos permiten crear archivos CSV y analizar el texto CSV a partir de un valor de texto recibido o un archivo.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Crear CSV]

La variable [!UICONTROL Crear CSV] Aggregator permite crear un texto csv a partir de valores de texto recibidos.

Para obtener más información sobre los agregadores, consulte [Módulo de agregador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleccione el módulo que está utilizando para agregar los campos que necesita.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Campos agregados]</td>
        <td>Seleccione los campos que desea acumular de la lista de campos disponibles.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Incluir encabezados en la primera fila]</td>
        <td>Seleccione esta opción para incluir los encabezados en el resultado.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>Introduzca el filtro para agrupar los resultados. Por ejemplo, introduzca una fecha.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Detenga el procesamiento después de una agregación vacía]</td>
        <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td>
    </tr>
</table>

## [!UICONTROL Crear CSV (avanzado)]

La variable [!UICONTROL Crear CSV (avanzado)] Aggregator permite crear un texto CSV a partir de valores de texto recibidos. Utiliza una estructura de datos que define las columnas CSV en el archivo CSV resultante. Una vez definidas, las columnas aparecen como campos en la configuración del módulo CSV y se pueden asignar a un módulo posterior en el escenario.

Para obtener más información sobre los agregadores, consulte [Módulo de agregador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Seleccione el módulo de aplicación que utiliza para acumular los campos que necesita.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>Seleccione la estructura de datos para agregar los campos de la forma que desee. Después de definir la estructura de datos, puede asignar los elementos a los campos correspondientes.</p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Estructuras de datos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir encabezados en la primera fila] </td> 
   <td>Seleccione esta opción para incluir los encabezados en el resultado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>Introduzca el filtro para agrupar los resultados. Por ejemplo, introduzca una fecha. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Detenga el procesamiento después de una agregación vacía] </td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados. </td> 
  </tr> 
 </tbody> 
</table>


<p>Supongamos que desea exportar sus contactos de Google a un archivo CSV con dos columnas "Nombre completo" y "Correo electrónico". El paquete de salida del módulo [!UICONTROL Google Contacts] &gt;[!UICONTROL Get contacts from a group] tiene la siguiente estructura. Las direcciones de correo electrónico se almacenan dentro de la variable <code>[!UICONTROL Emails[]]</code> elemento, que es una matriz de colecciones, cada colección contiene dos elementos: <code>Label</code> y <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Si utiliza el [!DNL Create CSV] , se le ofrece una lista de casillas de verificación correspondientes a los elementos de nivel superior de un paquete. Si intenta marcar <code>Full name</code> y <code>Emails</code> , el módulo [!UICONTROL Crear CSV] produce la siguiente salida, que probablemente no es la que desea:</p>
<p>"correos electrónicos","fullName"</p>
<p>"[objeto]","Shon Winer"</p>
<p>"[objeto]","Lizeth Fulmore"</p>
<p>"[objeto]","Hilario Gullatt"</p>
<p>"[objeto]","Abby Eisenbarth"</p>
<p>Desde el elemento <code>Full Name</code> es de tipo simple Texto, se exporta perfectamente. Pero el artículo <code>Emails</code>, que es de un tipo complejo Array of Collections, se exporta como [object Object], de modo que las colecciones y matrices se transforman en texto de forma predeterminada. Para obtener más información, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en Adobe Workfront Fusion</a>.</p>
<p>Para exportar contenido de la variable <code>Email </code>elemento de la primera colección de la <code>Emails[]</code> en su lugar, es necesario emplear el módulo [!UICONTROL Crear CSV (avanzado)]. El módulo le permite definir columnas individuales del archivo CSV y asignar elementos a ellas, incluidas las anidadas.</p>
<ol>
<li value="1">Inserte el módulo [!UICONTROL Crear CSV (avanzado)] en un escenario y abra su configuración.</li>
<li value="2">Haga clic en el <strong>[!UICONTROL Agregar]</strong> situado junto al campo [!UICONTROL Data structure] para crear una nueva estructura de datos.</li>
<li value="3"> <p>Escriba un nombre para la estructura de datos y haga clic en el botón <strong>[!UICONTROL Agregar elemento]</strong> para añadir las columnas individuales. Si desea exportar dos columnas: "Nombre completo" y "Correo electrónico", la estructura de datos resultante tendría este aspecto:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Una vez que haya definido correctamente la estructura de datos, los campos correspondientes a cada columna individual deben aparecer en la configuración del módulo [!UICONTROL Crear CSV (avanzado)] para que pueda asignar los elementos. Tome el primer artículo de la <code>[!UICONTROL Emails[]]</code> matriz y asignación de elementos <code>Email </code>al campo o columna Correo electrónico:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Ejecute el escenario. Desde el elemento <code>Emails[1]: Email</code> asignado a la columna "Correo electrónico" es de tipo simple Texto, ahora exporta correctamente:</p> <p>"Nombre completo", "Correo electrónico"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Analizar CSV]

La variable [!UICONTROL Analizar CSV] transformer permite analizar texto CSV desde un valor de texto recibido o un archivo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de columnas]</td> 
   <td>Especifique el número de columnas del archivo CSV.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contiene encabezados]</td> 
   <td> <p>Seleccione esta opción si la primera fila del texto CSV contiene encabezados.</p> <p>Nota: El módulo no utiliza estos encabezados para etiquetar las columnas de la salida. En su lugar, este campo garantiza que los encabezados no se incluyan en los datos de salida.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Seleccione el delimitador para el archivo CSV. El delimitador es el carácter de texto que indica el límite entre valores o campos independientes.</p> 
    <ul> 
     <li>[!UICONTROL Coma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Otros]</p> <p>Si selecciona [!UICONTROL Otros], introduzca el carácter delimitador que utiliza el archivo CSV para separar valores. Debe introducir exactamente un carácter.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conservar comillas dentro de un campo sin comillas]</td> 
   <td>Active esta opción para conservar las comillas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Introduzca o asigne el archivo CSV que desea analizar.<p>Nota: <p>Si los datos se presentan en formato binario (normalmente de un archivo), se debe utilizar la función "toString()" para convertir los datos binarios a [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
