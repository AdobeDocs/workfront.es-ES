---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipos de módulos
description: '''Adobe Workfront Fusion distingue cinco tipos de módulos: módulos de acción, módulos de búsqueda, módulos de déclencheur, agregadores e iteradores. Los acumuladores y los iteradores son para escenarios avanzados."'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# Tipos de módulos

A[!UICONTROL Adobe Workfront Fusion] distingue cinco tipos de módulos: módulos de acción, módulos de búsqueda, módulos de déclencheur, agregadores e iteradores. Los acumuladores y los iteradores son para escenarios avanzados.

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
   <td>Su organización debe adquirir Adobe Workfront Fusion y Adobe Workfront para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Módulos de acción

Los módulos de acción son el tipo más común de módulo. Un módulo de acción típico devuelve un solo paquete, que luego pasa al siguiente módulo para su procesamiento.

A diferencia de los módulos de déclencheur, los módulos de acción se pueden colocar al principio, al medio o al final de un escenario. Los escenarios pueden contener un número ilimitado de módulos de acción.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Cargar un archivo]** envía un archivo a [!DNL Workfront] y devuelve su identificador.
>* **[!UICONTROL Imagen] > [!UICONTROL Cambiar tamaño]** recibe una imagen, la cambia a dimensiones especificadas y la transfiere a la siguiente acción.


El tipo de acción tiene cuatro subtipos: Crear, leer, actualizar y eliminar. El subtipo Update habilita las tres operaciones siguientes:

* **Borrar el contenido de un campo**. Esta operación se realiza cuando se evalúa el contenido del campo para borrar una palabra clave (no confundir con *empty*).

   ![](assets/erase-content-of-field.png)

* **No modificar el contenido de un campo**. Esta operación se realiza cuando el campo se deja vacío o el contenido del campo se evalúa como vacío (representado mediante nulo en JSON).

   ![](assets/leave-content-field-unchanged-350x231.png)

* **Reemplazar el contenido de un campo**. Esta operación se lleva a cabo en todos los demás casos que no sean los descritos anteriormente.

>[!NOTE]
>
>* Si no ve la variable `erase` palabra clave en el panel de asignación, el módulo no es un módulo de actualización o no se ha actualizado con las especificaciones más recientes para la aplicación.
>* &quot;[!UICONTROL Vacío]&quot; no cambia el contenido del campo. Si es necesario borrar el campo, puede utilizar la siguiente fórmula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>No es posible mantener un campo sin modificar cuando su contenido se evalúa como vacío en este momento.

## Módulos de búsqueda

Una búsqueda típica devuelve cero, uno o más paquetes, que luego pasan al siguiente módulo para su procesamiento.

Puede colocar Búsquedas al principio, al medio o al final de un escenario.

Los escenarios pueden contener un número ilimitado de búsquedas.

>[!INFO]
>
>**Ejemplo:**
>
>**[!DNL Workfront]> [!UICONTROL Leer registros relacionados]**  lee registros que coinciden con la consulta de búsqueda especificada, en un objeto principal concreto

## módulos de déclencheur

Los déclencheur generan paquetes cuando ha habido un cambio en un servicio determinado. El cambio puede ser una creación de registros nuevos, la eliminación de registros, la actualización de registros, etc.

Cada Déclencheur puede devolver cero, uno o más paquetes que luego pasan al siguiente módulo para su procesamiento.

Los déclencheur solo se pueden colocar al principio de un escenario.

Cada escenario puede contener un solo Déclencheur.

[!DNL Workfront Fusion] distingue entre dos tipos de déclencheur: Déclencheur electorales y déclencheur instantáneos.

### Déclencheur de sondeo

Los déclencheur de encuestas suelen sondear un servicio determinado aunque no haya habido ningún cambio desde su ejecución anterior. Se recomienda programar un escenario que contenga un déclencheur de sondeo para que se ejecute a intervalos regulares. Si hay un *change*, el déclencheur devuelve paquetes que contienen información sobre el cambio. Si no hay *change*, el déclencheur no genera paquetes. Para obtener instrucciones sobre cómo programar un escenario, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Los déclencheur de sondeo le permiten seleccionar el primer paquete que deben generar a través del panel de epoch. El panel se muestra automáticamente después de guardar un déclencheur o cambiar la configuración del déclencheur. Para obtener más información, consulte [Elija dónde comienza un módulo de déclencheur en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>La configuración realizada en el panel de época solo afecta a la primera ejecución del módulo. Una vez ejecutado el módulo, recuerda el último paquete de salida y anula la configuración realizada a través del panel de epoch.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Registros de Watch]** devuelve archivos que se agregaron recientemente desde la última vez que se ejecutó el escenario
>
>* **[!DNL Google Sheets]> [!UICONTROL Filas de observación]** devuelve nuevas filas agregadas por el usuario desde la última vez que se ejecutó el escenario


### Déclencheur instantáneos

Los déclencheur instantáneos permiten que el servicio notifique [!DNL Workfront Fusion] acerca de un *change* inmediatamente. Se recomienda programar un escenario que contenga un déclencheur instantáneo para que se ejecute inmediatamente. Para obtener instrucciones, consulte [Programar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Consulte también [Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) para obtener más información sobre cómo se gestionan los datos entrantes.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Eventos de Watch]** devuelve información cuando se produce un determinado tipo de evento en Workfront, como la creación de una tarea.
>* **[!DNL Google Sheets]> [!UICONTROL Ver cambios]** devuelve información cada vez que se actualiza una celda.


## Acumuladores

Un agregador es un tipo de módulo que acumula varios paquetes en un solo paquete.

Cada agregador devuelve solo un paquete, que luego pasa al siguiente módulo para su procesamiento posterior.

Solo se pueden colocar acumuladores en medio de un escenario.

Los escenarios pueden contener un número ilimitado de agregadores.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!UICONTROL Archivo] > [!UICONTROL Crear un archivo]** comprime los archivos recibidos en un archivo zip
>* **[!UICONTROL CSV] > [!UICONTROL Agregar a CSV]** combina varias cadenas de un archivo CSV en una sola fila
>* **[!UICONTROL Herramientas] > [!UICONTROL Acumulador de texto]** combina varias cadenas juntas en una sola cadena


Para obtener más información, consulte [Módulo de agregador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteradores

Un iterador es un tipo de módulo que divide las matrices en varios paquetes separados.

Cada iterador devuelve uno o más paquetes, que luego pasan al siguiente módulo para su procesamiento.

Solo puede colocar los iteradores en medio de un escenario.

Los escenarios pueden contener un número ilimitado de iteradores.

>[!INFO]
>
>**Ejemplo:**
>
>**[!UICONTROL Correo electrónico] > [!UICONTROL Recuperar archivos adjuntos]** rompe una matriz de archivos adjuntos en paquetes separados

Para obtener más información, consulte [Módulo de iteración en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) y [Asignación de una matriz en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
