---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipos de módulos
description: '"Adobe Workfront Fusion distingue cinco tipos de módulos: módulos de acción, módulos de búsqueda, módulos de déclencheur, agregadores e iteradores. Los acumuladores e iteradores son para escenarios avanzados".'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# Tipos de módulos

A[!UICONTROL Adobe Workfront Fusion] distingue cinco tipos de módulos: módulos de acción, módulos de búsqueda, módulos de déclencheur, agregadores e iteradores. Los acumuladores e iteradores son para escenarios avanzados.

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
   <td>Su organización debe adquirir Adobe Workfront Fusion y Adobe Workfront para utilizar la funcionalidad que se describe en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Módulos de acción

Los módulos de acción son el tipo más común de módulo. Un módulo de acción típico devuelve un solo paquete, que luego pasa al siguiente módulo para su procesamiento.

A diferencia de los módulos de déclencheur, los módulos de acción se pueden colocar al principio, en el centro o al final de un escenario. Los escenarios pueden contener un número ilimitado de módulos de acción.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Cargar un archivo]** envía un archivo a [!DNL Workfront] y devuelve su identificador.
>* **[!UICONTROL Imagen] > [!UICONTROL Redimensionar]** recibe una imagen, cambia su tamaño a las dimensiones especificadas y pasa la imagen cambiada a la siguiente acción.

El tipo de acción tiene cuatro subtipos: Crear, Leer, Actualizar y Eliminar. El subtipo Update habilita las tres operaciones siguientes:

* **Borrar el contenido de un campo**. Esta operación tiene lugar cuando el contenido del campo se evalúa para borrar la palabra clave (no confundirlo con *vaciar*).

  ![](assets/erase-content-of-field.png)

* **No modifique el contenido de un campo**. Esta operación se realiza cuando el campo se deja vacío o cuando el contenido del campo se evalúa como vacío (representado mediante nulo en JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Reemplazar el contenido de un campo**. Esta operación tiene lugar en todos los demás casos que no sean los dos descritos anteriormente.

>[!NOTE]
>
>* Si no ve el `erase` palabra clave en el panel asignación, el módulo no es un módulo de actualización o no se ha actualizado a las especificaciones más recientes para la aplicación.
>* &quot;[!UICONTROL Empty]&quot; no cambia el contenido del campo. Si es necesario borrar el campo, se puede utilizar la siguiente fórmula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Actualmente no es posible dejar un campo sin cambiar cuando su contenido se evalúa como vacío.

## Buscar módulos

Una búsqueda típica devuelve cero, uno o más paquetes, que luego pasan al siguiente módulo para su procesamiento.

Puede colocar Búsquedas al principio, al medio o al final de un escenario.

Los escenarios pueden contener un número ilimitado de búsquedas.

>[!INFO]
>
>**Ejemplo:**
>
>**[!DNL Workfront]> [!UICONTROL Leer registros relacionados]**  lee registros que coinciden con la consulta de búsqueda especificada, en un objeto primario concreto

## módulos de déclencheur

Los déclencheur generan paquetes cuando se ha producido un cambio en un servicio determinado. El cambio puede consistir en la creación de registros nuevos, la eliminación de registros, la actualización de registros, etc.

Cada Déclencheur puede devolver cero, uno o más paquetes que luego pasan al siguiente módulo para su procesamiento.

Los déclencheur solo se pueden colocar al principio de un escenario.

Cada escenario solo puede contener un Déclencheur.

[!DNL Workfront Fusion] distingue entre dos tipos de déclencheur: déclencheur de sondeo y déclencheur instantáneos.

### Déclencheur de sondeo

Los déclencheur encuestadores encuestan con regularidad un servicio determinado aunque no haya habido cambios desde la ejecución anterior. Le recomendamos que programe un escenario que contenga un déclencheur de sondeo para que se ejecute a intervalos regulares. Si hay un *cambiar*, el déclencheur devuelve paquetes que contienen información sobre el cambio. Si no hay *cambiar*, el déclencheur no genera ningún paquete. Para obtener instrucciones sobre cómo programar un escenario, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Los déclencheur de sondeo le permiten seleccionar el primer paquete que debe generar a través del panel epoch. El panel se muestra automáticamente después de guardar un déclencheur déclencheur o cambiar su configuración. Para obtener más información, consulte [Elija dónde comienza un módulo de déclencheur en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>La configuración realizada en el panel Epoch afecta únicamente a la primera ejecución del módulo. Una vez ejecutado el módulo, recuerda el último paquete saliente y anula la configuración realizada mediante el panel epoch.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Ver registros]** devuelve los archivos que se agregaron recientemente desde la última vez que se ejecutó el escenario
>
>* **[!DNL Google Sheets]> [!UICONTROL Observar filas]** devuelve las filas nuevas agregadas por el usuario desde la última vez que se ejecutó el escenario

### Déclencheur instantáneos

Los déclencheur instantáneos permiten que el servicio notifique [!DNL Workfront Fusion] acerca de a *cambiar* inmediatamente. Le recomendamos que programe un escenario que contenga un déclencheur instantáneo para que se ejecute de inmediato. Para obtener instrucciones, consulte [Programar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Consulte también [Déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) para obtener más información sobre cómo se gestionan los datos entrantes.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Ver eventos]** devuelve información cuando se produce un determinado tipo de evento en Workfront, como la creación de una tarea.
>* **[!DNL Google Sheets]> [!UICONTROL Ver cambios]** devuelve información cada vez que se actualiza una celda.

## Agregadores

Un Aggregator es un tipo de módulo que acumula varios paquetes en uno solo.

Cada acumulador devuelve solo un paquete, que luego pasa al siguiente módulo para un procesamiento posterior.

Puede colocar Agregadores solo en medio de un escenario.

Los escenarios pueden contener un número ilimitado de acumuladores.

>[!INFO]
>
>**Ejemplos:**
>
>* **[!UICONTROL Archivar] > [!UICONTROL Crear un archivo]** comprime los archivos recibidos en un archivo zip
>* **[!UICONTROL CSV] > [!UICONTROL Agregar a CSV]** combina varias cadenas de un archivo CSV en una sola fila
>* **[!UICONTROL Herramientas] > [!UICONTROL Agregador de texto]** combina varias cadenas en una sola

Para obtener más información, consulte [Módulo de agregado en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteradores

Un iterador es un tipo de módulo que divide las matrices en varios paquetes independientes.

Cada iterador devuelve uno o más paquetes, que luego pasan al siguiente módulo para su procesamiento.

Puede colocar Iterators solamente en medio de un escenario.

Los escenarios pueden contener un número ilimitado de iteradores.

>[!INFO]
>
>**Ejemplo:**
>
>**[!UICONTROL Correo electrónico] > [!UICONTROL Recuperar archivos adjuntos]** divide una matriz de archivos adjuntos en paquetes independientes

Para obtener más información, consulte [Módulo iterador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) y [Asignación de una matriz en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
