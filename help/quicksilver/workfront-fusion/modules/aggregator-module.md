---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo del agregador en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 89%

---

# Módulo [!UICONTROL Agregador] en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulo de agregado](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/aggregator-module.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Un módulo agregador es un tipo de módulo diseñado para combinar varios paquetes de datos en un único paquete.

Para obtener más información sobre los tipos de módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Información general sobre el módulo [!UICONTROL Agregador]

Cuando se ejecuta un módulo [!UICONTROL Agregador], hace lo siguiente:

* Acumula todos los paquetes que recibe durante el funcionamiento de un único módulo de origen.
* Genera un solo paquete con una matriz que contiene un elemento por cada paquete acumulado. El contenido de los elementos de la matriz depende del módulo [!UICONTROL Agregador] en particular y de su configuración.

La siguiente imagen muestra una configuración típica del módulo [!UICONTROL Agregador]:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>Módulo en el que se inicia la agregación del paquete. El módulo de origen suele ser un iterador o un módulo de búsqueda que genera una serie de paquetes.</p><p>Al configurar el módulo de origen del agregador (y cerrar la configuración del agregador), la ruta entre el módulo de origen y el módulo del agregador se ajusta en una zona gris para que pueda ver claramente el inicio y el final de la agregación. 
   </p> <p>Para obtener más información sobre los iteradores, consulte el módulo <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]</a></p> <p>Para obtener más información sobre los módulos de búsqueda, consulte módulos de búsqueda en <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>(Aplicable únicamente para el módulo [!UICONTROL Array aggregator]). La estructura de destino donde se agregan los datos. La opción predeterminada, [!UICONTROL Custom], le permite elegir elementos que deberín agregarse al <code>Array </code>elemento del paquete de salida del [!UICONTROL Array aggregator]:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Una vez que conecte más módulos después del módulo [!UICONTROL Array aggregator] y vuelva a la configuración del módulo, el menú desplegable del tipo de estructura de [!UICONTROL Target] contendrá todos los módulos siguientes y sus campos del tipo “Matriz de colecciones”, tal como se muestra en el campo [!UICONTROL Attachments] del módulo [!DNL Slack] &gt;[!UICONTROL Create a Message]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>Campos que desea incluir en la salida del módulo del agregador.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>La salida del agregador se puede dividir en varios grupos con la ayuda del campo [!UICONTROL Group by]. El campo [!UICONTROL Group by] puede contener una fórmula que se evalúa para cada paquete de entrada del agregador. A continuación, el agregador genera un paquete por cada valor de fórmula distinto. Cada paquete contiene dos elementos:</p> 
    <ul> 
     <li><code>Key </code>contiene el valor distinto.</li> 
     <li><code>Array </code>contiene los datos agregados de los paquetes para los que la fórmula se evaluó en el valor <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Detener procesamiento después de una agregación vacía</p> </td> 
   <td> <p>De forma predeterminada, el módulo [!UICONTROL Aggregator] genera el resultado de la agregación incluso si no se han alcanzado paquetes en el módulo [!UICONTROL Aggregator] (por ejemplo, porque todos se han filtrado en su camino). Si la opción [!UICONTROL Stop processing after an empty aggregation] está habilitada, el módulo [!UICONTROL Aggregator] no producirá ningún paquete de salida en este caso y el flujo se detendrá.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Los paquetes generados por los módulos entre el módulo de origen y el [!UICONTROL Agregador] no se generan en el [!UICONTROL Agregador], por lo que los módulos del flujo no pueden obtener acceso a ellos después del [!UICONTROL Agregador]. Si necesita datos de un paquete generado por un módulo entre el módulo de origen y el [!UICONTROL Agregador], asegúrese de incluir el elemento proporcionado en la configuración del [!UICONTROL Agregador] (como en el campo [!UICONTROL Campos agregados] de la configuración del módulo [!UICONTROL Agregador de matrices]).


## Escenario de ejemplo de cómo funcionan los agregadores

Este escenario de ejemplo muestra cómo comprimir todos los archivos adjuntos de correo electrónico y cargar el ZIP en [!DNL Dropbox].

![](assets/dropbox-archive-350x87.png)

El siguiente escenario muestra cómo:

* El primer módulo controla un buzón de correo electrónico entrante: [!UICONTROL Correo electrónico] >[!UICONTROL Ver correos electrónicos] el activador generará un paquete con el elemento `Attachments[]`, que es una matriz que contiene todos los archivos adjuntos del correo electrónico.

* El segundo modelo itera los archivos adjuntos del correo electrónico: [!UICONTROL Correo electrónico] >[!UICONTROL Iterar archivos adjuntos] el iterador toma los elementos de la matriz `Attachments[]` uno por uno y los envía más como paquetes separados.

* El tercer módulo agrega los paquetes generados por el módulo [!UICONTROL Correo electrónico] >[!UICONTROL Iterar archivos adjuntos]: [!UICONTROL Archivo] >[!UICONTROL Crear un agregador de archivos] acumula todos los paquetes que recibe y genera un solo paquete que contiene el archivo ZIP.

* El último módulo carga el archivo ZIP resultante en [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Cargar un archivo] obtiene el archivo ZIP del módulo [!UICONTROL Archivo] > [!UICONTROL Crear un archivo] y lo carga en [!DNL Dropbox].



A continuación, se muestra una configuración de ejemplo del agregador [!UICONTROL Archivo] > [!UICONTROL Crear un archivo]:

![](assets/archive-create-an-archive-350x484.png)
