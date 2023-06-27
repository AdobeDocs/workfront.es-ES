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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL Agregador] módulo en [!DNL Adobe Workfront Fusion]

Un módulo agregador es un tipo de módulo diseñado para combinar varios paquetes de datos en un único paquete.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## [!UICONTROL Agregador] módulo

Cuando un [!UICONTROL Agregador] se ejecuta, hace lo siguiente:

* Acumula todos los paquetes que recibe durante el funcionamiento de un solo módulo de origen.
* Genera un solo paquete con una matriz que contiene un elemento por cada paquete acumulado. El contenido de los elementos de la matriz depende de [!UICONTROL Agregador] y su configuración.

La siguiente imagen muestra una configuración típica del [!UICONTROL Agregador] módulo :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Módulo de origen]</p> </td> 
   <td> <p>Módulo desde el que se iniciará la agregación del paquete. El módulo de origen suele ser un iterador o un módulo de búsqueda que genera una serie de paquetes. Al configurar el módulo de origen del agregador (y cerrar la configuración del agregador), la ruta entre el módulo de origen y el módulo del agregador se ajusta en una zona gris para que pueda ver claramente el inicio y el final de la agregación. 
   </p> <p>Para obtener más información sobre los iteradores, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Módulo [!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]</a></p> <p>Para obtener más información sobre los módulos de búsqueda, consulte módulos de búsqueda en <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de estructura de destino]</p> </td> 
   <td> <p>(Aplicable únicamente para el módulo [!UICONTROL Array aggregator]). La estructura objetivo en la que se agregarán los datos. La opción predeterminada, [!UICONTROL Custom], permite elegir elementos que deben agregarse al paquete de salida del agregador de matrices A[!UICONTROL] <code>Array </code>elemento:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Una vez que conecte más módulos después del módulo [!UICONTROL Array aggregator] y vuelva a la configuración del módulo, la lista desplegable de tipo de estructura de [!UICONTROL Target] contendrá todos los módulos siguientes y sus campos de tipo Array of Collections, como se muestra en el campo [!UICONTROL Attachments] del [!DNL Slack] &gt;[!UICONTROL Crear un mensaje] módulo:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos agregados]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo del acumulador.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>La salida del agregador se puede dividir en varios grupos con la ayuda del campo [!UICONTROL Agrupar por]. El campo [!UICONTROL Group by] puede contener una fórmula que se evalúa para cada paquete de entrada del agregador. A continuación, el agregador genera un paquete por cada valor de fórmula distinto. Cada paquete contiene dos elementos:</p> 
    <ul> 
     <li><code>Key </code>contiene el valor distinto.</li> 
     <li><code>Array </code>contiene los datos agregados de los paquetes para los que la fórmula se evaluó en el <code>Key </code>valor.</li> 
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
>Paquetes generados por módulos entre el módulo de origen y el [!UICONTROL Agregador] Los módulos de no se generan mediante [!UICONTROL Agregador] , por lo que los módulos del flujo no pueden acceder a ellos después de la variable [!UICONTROL Agregador]. Si necesita datos de un paquete generado por un módulo entre el módulo de origen y el [!UICONTROL Agregador] , asegúrese de incluir el elemento dado en el [!UICONTROL Agregador] configuración del módulo (como en el [!UICONTROL Campos agregados] en la configuración del [!UICONTROL Agregador de matrices] módulo).


>[!INFO]
>
>**Ejemplo:** Caso de uso: Comprimir todos los archivos adjuntos del correo electrónico y cargar el ZIP en [!DNL Dropbox]
>
>El siguiente escenario muestra cómo:
>
>* Inspeccione un buzón para ver los correos electrónicos entrantes: [!UICONTROL Correo electrónico] >[!UICONTROL Ver correos electrónicos] El déclencheur generará un paquete con el elemento `Attachments[]`, que es una matriz que contiene todos los archivos adjuntos del correo electrónico.
>
>* Itere los archivos adjuntos del correo electrónico: [!UICONTROL Correo electrónico] >[!UICONTROL Repetir archivos adjuntos] El iterador toma los elementos del `Attachments[]` matriz uno por uno y los envía más como paquetes separados.
>
>* Agregar los paquetes generados por el [!UICONTROL Correo electrónico] >[!UICONTROL Repetir archivos adjuntos] módulo: [!UICONTROL Archivar] >[!UICONTROL Crear un agregador de archivos] acumula todos los paquetes que recibe y genera un solo paquete que contiene el archivo ZIP.
>
>* Cargue el archivo ZIP resultante en [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Cargar un archivo] obtiene el archivo ZIP del [!UICONTROL Archivar] > [!UICONTROL Crear un archivo] y lo sube a [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>A continuación se muestra un ejemplo de configuración del [!UICONTROL Archivar] > [!UICONTROL Crear un archivo] agregador:
>
>![](assets/archive-create-an-archive-350x484.png)
