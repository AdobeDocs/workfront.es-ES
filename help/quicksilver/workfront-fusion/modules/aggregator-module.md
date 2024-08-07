---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo de agregado en Adobe Workfront Fusion
description: Un módulo agregador es un tipo de módulo diseñado para combinar varios paquetes de datos en un único paquete.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# Módulo [!UICONTROL Aggregator] en [!DNL Adobe Workfront Fusion]

Un módulo agregador es un tipo de módulo diseñado para combinar varios paquetes de datos en un único paquete.

Para obtener más información acerca de los tipos de módulos, vea [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
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

+++

## Resumen del módulo [!UICONTROL Aggregator]

Cuando se ejecuta un módulo [!UICONTROL Aggregator], hace lo siguiente:

* Acumula todos los paquetes que recibe durante el funcionamiento de un solo módulo de origen.
* Genera un solo paquete con una matriz que contiene un elemento por cada paquete acumulado. El contenido de los elementos de la matriz depende del módulo [!UICONTROL Aggregator] en particular y de su configuración.

La siguiente imagen muestra una configuración típica del módulo [!UICONTROL Aggregator]:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Módulo Source]</p> </td> 
   <td> <p>Módulo en el que se inicia la agregación del paquete. El módulo de origen suele ser un iterador o un módulo de búsqueda que genera una serie de paquetes.</p><p>Al configurar el módulo de origen del agregador (y cerrar la configuración del agregador), la ruta entre el módulo de origen y el módulo del agregador se ajusta en una zona gris para que pueda ver claramente el inicio y el final de la agregación. 
   </p> <p>Para obtener más información sobre los iteradores, vea el módulo <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]</a></p> <p>Para obtener más información sobre los módulos de búsqueda, consulte módulos de búsqueda en <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de estructura de destino]</p> </td> 
   <td> <p>(Aplicable únicamente para el módulo [!UICONTROL Array aggregator]). La estructura de destino donde se agregan los datos. La opción predeterminada, [!UICONTROL Custom], permite elegir elementos que deben agregarse al <code>Array </code>elemento del paquete de salida del [!UICONTROL Array aggregator]:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Una vez que conecte más módulos después del módulo [!UICONTROL Array aggregator] y vuelva a la configuración del módulo, el menú desplegable del tipo de estructura de [!UICONTROL Target] contendrá todos los módulos siguientes y sus campos que son del tipo "Matriz de colecciones", como se muestra en el campo [!UICONTROL Attachments] del módulo [!DNL Slack] &gt;[!UICONTROL Create a Message]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos agregados]</td> 
   <td>Los campos que desea incluir en la salida del módulo del agregador.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>La salida del agregador se puede dividir en varios grupos con la ayuda del campo [!UICONTROL Agrupar por]. El campo [!UICONTROL Group by] puede contener una fórmula que se evalúa para cada paquete de entrada del agregador. A continuación, el agregador genera un paquete por cada valor de fórmula distinto. Cada paquete contiene dos elementos:</p> 
    <ul> 
     <li><code>Key </code>contiene el valor distinto.</li> 
     <li><code>Array </code>contiene los datos agregados de los paquetes para los que la fórmula se evaluó en el valor <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Detener procesamiento después de una agregación vacía</p> </td> 
   <td> <p>De forma predeterminada, el módulo [!UICONTROL Aggregator] genera el resultado de la agregación incluso en el caso de que no se hayan alcanzado paquetes en el módulo [!UICONTROL Aggregator] (por ejemplo, porque todos se han filtrado en su camino). Si la opción [!UICONTROL Detener procesamiento después de una agregación vacía] está habilitada, el módulo [!UICONTROL Aggregator] no producirá ningún paquete de salida en este caso y el flujo se detendrá.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Los paquetes generados por los módulos entre el módulo de origen y el módulo [!UICONTROL Aggregator] no se generan en el módulo [!UICONTROL Aggregator], por lo que los módulos del flujo no pueden obtener acceso a ellos después de [!UICONTROL Aggregator]. Si necesita datos de un paquete generado por un módulo entre el módulo de origen y el módulo [!UICONTROL Aggregator], asegúrese de incluir el elemento proporcionado en la configuración del módulo [!UICONTROL Aggregator] (como en el campo [!UICONTROL Campos agregados] de la configuración del módulo [!UICONTROL Array aggregator]).


## Ejemplo de cómo funcionan los agregadores

Este escenario de ejemplo muestra cómo comprimir todos los archivos adjuntos de correo electrónico y cargar el ZIP en [!DNL Dropbox].

![](assets/dropbox-archive-350x87.png)

El siguiente escenario muestra cómo:

* El primer módulo vigila un buzón de correo electrónico entrante: [!UICONTROL Correo electrónico] >[!UICONTROL Ver correos electrónicos] El déclencheur mostrará un paquete con el elemento `Attachments[]`, que es una matriz que contiene todos los archivos adjuntos del correo electrónico.

* El segundo modelo repite los archivos adjuntos del correo electrónico: [!UICONTROL Correo electrónico] >[!UICONTROL Archivos adjuntos iterados] el iterador toma los elementos de la matriz `Attachments[]` uno por uno y los envía más como paquetes separados.

* El tercer módulo agrega los paquetes generados por el módulo [!UICONTROL Correo electrónico] >[!UICONTROL Archivos adjuntos iterados]: [!UICONTROL Archivo] >[!UICONTROL Crear un agregador de archivos] acumula todos los paquetes que recibe y genera un solo paquete que contiene el archivo ZIP.

* El último módulo carga el archivo ZIP resultante en [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Cargar un archivo] obtiene el archivo ZIP del módulo [!UICONTROL Archivo] > [!UICONTROL Crear un archivo] y lo sube a [!DNL Dropbox].



A continuación se muestra una configuración de ejemplo del agregador [!UICONTROL Archivo] > [!UICONTROL Crear un archivo]:

![](assets/archive-create-an-archive-350x484.png)
