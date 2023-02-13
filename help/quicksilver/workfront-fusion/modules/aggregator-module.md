---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo de agregación en Adobe Workfront Fusion
description: Un módulo de agregador es un tipo de módulo diseñado para combinar varios paquetes de datos en un único paquete.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL Acumulador] módulo en [!DNL Adobe Workfront Fusion]

Un módulo de agregador es un tipo de módulo diseñado para combinar varios paquetes de datos en un único paquete.

Para obtener más información sobre los tipos de módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

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

## [!UICONTROL Acumulador] módulo

Cuando una [!UICONTROL Acumulador] se ejecuta, hace lo siguiente:

* Acumula todos los paquetes que recibe durante la operación de un solo módulo de origen.
* Genera un solo paquete con una matriz que contiene un elemento por cada paquete acumulado. El contenido de los elementos de la matriz depende de [!UICONTROL Acumulador] y su configuración.

La siguiente imagen muestra una configuración típica de la variable [!UICONTROL Acumulador] módulo :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>Módulo desde el que se iniciará la agregación de paquetes. El módulo de origen suele ser un iterador o un módulo de búsqueda que genera una serie de paquetes. Al configurar el módulo de origen del agregador (y cerrar la configuración del agregador), la ruta entre el módulo de origen y el módulo del agregador se envuelve en un área gris para que pueda ver claramente el inicio y el final de la agregación. 
   </p> <p>Para obtener más información sobre los iteradores, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Módulo [!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]</a></p> <p>Para obtener más información sobre los módulos de búsqueda, consulte los módulos de búsqueda en <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de estructura de destino]</p> </td> 
   <td> <p>(Aplicable únicamente para el módulo [!UICONTROL Array agregator]). Estructura objetivo en la que se agregarán los datos. La opción predeterminada, [!UICONTROL Personalizado], permite elegir elementos que deben agregarse al paquete de salida de A[!UICONTROL rray agregator] <code>Array </code>elemento:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Una vez que conecte más módulos después del módulo [!UICONTROL Array agregator] y vuelva a la configuración del módulo, la lista desplegable de tipo de estructura [!UICONTROL Target] contendrá todos los módulos siguientes y sus campos que sean del tipo Array of Collections, como se muestra en el campo [!UICONTROL Attachments] del tipo [!DNL Slack] &gt; Módulo[!UICONTROL Crear un mensaje]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos agregados]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo de agregación.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>La salida del agregador se puede dividir en varios grupos con la ayuda del campo [!UICONTROL Group by]. El campo [!UICONTROL Group by] puede contener una fórmula que se evalúa para cada paquete de entrada del agregador. A continuación, el agregador genera un paquete por cada valor de fórmula distinta. Cada paquete contiene dos elementos:</p> 
    <ul> 
     <li><code>Key </code>contiene el valor distinto.</li> 
     <li><code>Array </code>contiene los datos agregados de los paquetes para los que la fórmula evaluada en la variable <code>Key </code>valor.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Detener procesamiento después de una agregación vacía</p> </td> 
   <td> <p>De forma predeterminada, el módulo [!UICONTROL Aggregator] genera el resultado de la agregación incluso en caso de que no se hayan alcanzado paquetes en el módulo [!UICONTROL Aggregator] (por ejemplo, porque todos se han filtrado en su camino). Si la opción [!UICONTROL Detenga el procesamiento después de una agregación vacía] está habilitada, el módulo [!UICONTROL Aggregator] no producirá ningún paquete de salida en este caso y el flujo se detendrá.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Paquetes generados por módulos entre el módulo de origen y el [!UICONTROL Acumulador] no son resultado de la [!UICONTROL Acumulador] , por lo que los módulos del flujo después del [!UICONTROL Acumulador]. Si necesita datos de un paquete generado por un módulo entre el módulo de origen y el [!UICONTROL Acumulador] , asegúrese de incluir el elemento dado en la variable [!UICONTROL Acumulador] configuración del módulo (como en la [!UICONTROL Campos agregados] en la configuración del [!UICONTROL Agrupador de matrices] ).


>[!INFO]
>
>**Ejemplo:** Caso de uso: Comprimir todos los archivos adjuntos de correo electrónico y cargar el ZIP en [!DNL Dropbox]
>
>El siguiente escenario muestra cómo:
>
>* Vea un buzón para correos electrónicos entrantes: [!UICONTROL Correo electrónico] >[!UICONTROL Ver correos electrónicos] El déclencheur mostrará un paquete con el elemento `Attachments[]`, que es una matriz que contiene todos los archivos adjuntos del correo electrónico.
>
>* Iterar los archivos adjuntos del correo electrónico: [!UICONTROL Correo electrónico] >[!UICONTROL Iteración de archivos adjuntos] El iterador toma los elementos del `Attachments[]` array uno por uno y los envía como paquetes separados.
>
>* Agregue los paquetes que genera el [!UICONTROL Correo electrónico] >[!UICONTROL Iteración de archivos adjuntos] módulo: [!UICONTROL Archivo] >[!UICONTROL Creación de un agregador de archivos] acumula todos los paquetes que recibe y genera un solo paquete que contiene el archivo ZIP.
>
>* Cargue el archivo ZIP resultante a [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Cargar un archivo] obtiene el archivo ZIP del [!UICONTROL Archivo] > [!UICONTROL Crear un archivo] y lo carga en [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>A continuación se muestra una configuración de muestra de la variable [!UICONTROL Archivo] > [!UICONTROL Crear un archivo] agregador:
>
>![](assets/archive-create-an-archive-350x484.png)
