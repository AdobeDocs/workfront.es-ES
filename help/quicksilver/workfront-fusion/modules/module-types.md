---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipos de módulos
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 92%

---

# Tipos de módulos

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Resumen del módulo](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/module-overview.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

[!UICONTROL Adobe Workfront Fusion] distingue cinco tipos de módulos: módulos de acción, módulos de búsqueda, módulos de activación, agregadores e iteradores. Los agregadores e iteradores son para escenarios avanzados.

## Requisitos de acceso

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
   <td>Su organización debe adquirir Adobe Workfront Fusion y Adobe Workfront para utilizar la funcionalidad que se describe en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

Para obtener información sobre licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Módulos de acción

Los módulos de acción son el tipo más común de módulo. Un módulo de acción típico devuelve un solo paquete, que luego pasa al siguiente módulo para su procesamiento.

A diferencia de los módulos de activación, los módulos de acción se pueden colocar al principio, en el centro o al final de un escenario. Los escenarios pueden contener un número ilimitado de módulos de acción.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Upload a file]** envía un archivo a [!DNL Workfront] y devuelve su identificador.
>* **[!UICONTROL Image] > [!UICONTROL Resize]** recibe una imagen, la cambia a las dimensiones especificadas y pasa la imagen cambiada a la siguiente acción.

El tipo de acción tiene cuatro subtipos: Crear, Leer, Actualizar y Eliminar. El subtipo Actualizar habilita las tres operaciones siguientes:

* **Borrar el contenido de un campo**. Esta operación tiene lugar cuando el contenido del campo se evalúa para borrar la palabra clave (no confundir con *vacío*).

  ![](assets/erase-content-of-field.png)

* **No modificar el contenido de un campo**. Esta operación se realiza cuando el campo se deja vacío o cuando el contenido del campo se evalúa como vacío (representado mediante “null” en JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Reemplazar el contenido de un campo**. Esta operación tiene lugar en todos los demás casos que no sean los dos descritos anteriormente.

>[!NOTE]
>
>* Si no ve la palabra clave `erase` en el panel de asignación, el módulo no es un módulo de actualización o no se ha actualizado a las especificaciones más recientes para la aplicación.
>* &quot;[!UICONTROL Empty]&quot; no cambia el contenido del campo. Si es necesario borrar el campo, se puede utilizar la siguiente fórmula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Actualmente no es posible dejar un campo sin cambiar cuando su contenido se evalúa como vacío.

## Buscar módulos

Una búsqueda típica devuelve cero, uno o más paquetes, que luego pasan al siguiente módulo para su procesamiento.

Puede colocar búsquedas al principio, al medio o al final de un escenario.

Los escenarios pueden contener un número ilimitado de búsquedas.

>[!INFO]
>
>**Ejemplo**
>
>**[!DNL Workfront]> [!UICONTROL Read Related Records]** lee registros que coinciden con la consulta de búsqueda especificada, en un objeto principal concreto

## Módulos de activador

Los activadores generan paquetes cuando se ha producido un cambio en un servicio determinado. El cambio puede consistir en la creación de registros nuevos, la eliminación de registros, la actualización de registros, etc.

Cada activador puede devolver cero, uno o más paquetes que luego pasan al siguiente módulo para su procesamiento.

Los activadores solo se pueden colocar al principio de un escenario.

Cada escenario solo puede contener un activador.

[!DNL Workfront Fusion] distingue entre dos tipos de activadores: activadores de sondeo y activadores instantáneos.

### Activador de sondeo

Los activadores de sondeo encuestan con regularidad un servicio determinado aunque no haya habido cambios desde la ejecución anterior. Le recomendamos que programe un escenario que contenga un activador de sondeo para que se ejecute a intervalos regulares. Si hay un *cambio*, el activador devuelve paquetes que contienen información sobre el cambio. Si no se produce ningún *cambio*, el activador no genera ningún paquete. Para obtener más información sobre cómo programar un escenario, consulte [Programar un escenario en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Los activadores de sondeo le permiten seleccionar el primer paquete que debe generar a través del panel epoch. El panel se muestra automáticamente tras guardar un activador o cambiar su configuración. Para obtener más información, consulte [Elegir dónde se inicia un módulo de activador en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>La configuración realizada en el panel Epoch afecta únicamente a la primera ejecución del módulo. Una vez ejecutado el módulo, recuerda el último paquete generado y anula la configuración realizada mediante el panel epoch.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Observar registros]** devuelve archivos que se han añadido recientemente desde la última vez que se ejecutó el escenario
>
>* **[!DNL Google Sheets]> [!UICONTROL Observar filas]** devuelve nuevas filas añadidas por el usuario desde la última vez que se ejecutó el escenario

### Activadores instantáneos

Los activadores instantáneos permiten que el servicio notifique a [!DNL Workfront Fusion] un *cambio* inmediatamente. Le recomendamos que programe un escenario que contenga un activador instantáneo para que se ejecute de inmediato. Para obtener instrucciones, consulte [Programar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Consulte también [activadores instantáneos (webhooks) en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) para obtener detalles sobre cómo se gestionan los datos entrantes.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Observar eventos]** devuelve información cuando se produce un determinado tipo de evento en Workfront, como la creación de una tarea.
>* **[!DNL Google Sheets]> [!UICONTROL Observar cambios]** devuelve información cada vez que se actualiza una celda.

## Agregadores

Un agregador es un tipo de módulo que acumula varios paquetes en uno solo.

Cada agregador devuelve solo un paquete, que luego pasa al siguiente módulo para su procesamiento posterior.

Puede colocar agregadores solo en medio de un escenario.

Los escenarios pueden contener un número ilimitado de agregadores.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!UICONTROL Archivo] > [!UICONTROL Crear un archivo]** comprime los archivos recibidos en un archivo zip
>* **[!UICONTROL CSV] > [!UICONTROL Agregado a CSV]** combina varias cadenas de un archivo CSV en una sola fila
>* **[!UICONTROL Herramientas] > [!UICONTROL Agregador de texto]** combina varias cadenas en una sola

Para obtener más información, consulte [Módulo agregador en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteradores

Un iterador es un tipo de módulo que divide las matrices en varios paquetes independientes.

Cada iterador devuelve uno o más paquetes, que luego pasan al siguiente módulo para su procesamiento.

Puede colocar iteradores solamente en medio de un escenario.

Los escenarios pueden contener un número ilimitado de iteradores.

>[!INFO]
>
>**Ejemplo:**
>
>**[!UICONTROL Correo electrónico] > [!UICONTROL Recuperar archivos adjuntos]** divide una matriz de archivos adjuntos en paquetes separados

Para obtener más información, consulte [Módulo iterador en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) y [Asignar una matriz en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
