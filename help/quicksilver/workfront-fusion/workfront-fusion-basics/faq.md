---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Preguntas frecuentes sobre Adobe Workfront Fusion
description: Este artículo aborda preguntas comunes relacionadas con [!DNL Adobe Workfront Fusion], incluida información sobre los objetos que se utilizan habitualmente en flujos de trabajo de Fusion
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Preguntas frecuentes sobre Adobe Workfront Fusion

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## ¿Qué es un escenario?

### Respuesta

Un escenario define una secuencia de pasos por los que ejecutar [!DNL Adobe Workfront Fusion]. Para cada escenario, se especifica la fuente de datos, cómo se procesarán los datos, qué datos se utilizarán y qué se omitirán. [!DNL Workfront Fusion] permite crear escenarios tan complejos como sea necesario; incluso los escenarios más sofisticados son posibles.

Para obtener más información, consulte [Cree un escenario de integración de prácticas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## ¿Puedo utilizar más de un módulo en un escenario? ¿O simplemente un déclencheur y una acción?

### Respuesta

Puede utilizar tantos módulos como desee en un escenario. Puede crear rutas independientes y especificar qué datos deben fluir a través de ellas. También puede utilizar los resultados devueltos por acciones individuales y luego pasarlos a la siguiente acción.

## Can [!DNL Workfront Fusion] ¿trabajar con archivos?

### Respuesta

Sí. Uso [!DNL Workfront Fusion], los archivos se pueden recibir, guardar, transformar, convertir, encriptar, etc. Además, [!DNL Workfront Fusion] proporciona una amplia gama de funciones integradas diseñadas para permitir a los usuarios trabajar de forma eficaz y creativa con los datos contenidos en los archivos.

Para obtener más información, consulte [Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## ¿Qué sucede si dejo que [!DNL Workfront Fusion] procesar un correo electrónico que contenga más de un archivo adjunto?

### Respuesta

Si usa la variable [!UICONTROL Correo electrónico] módulo [!UICONTROL Recuperar archivos adjuntos], cada archivo adjunto se envía individualmente a través del resto de los módulos del escenario. También hay módulos similares disponibles en otras aplicaciones que reciben varios archivos a la vez.

Para obtener más información, consulte [[!UICONTROL Correo electrónico] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Algunos déclencheur permiten que los escenarios se ejecuten instantáneamente. ¿Qué significa &quot;instantáneamente&quot;?

### Respuesta

Los escenarios comunes se ejecutan a intervalos según la programación especificada (por ejemplo, cada hora, cada 5 minutos, una vez al mes, etc.). Existen déclencheur especiales, llamados déclencheur instantáneos (webhooks), que pueden iniciar su escenario inmediatamente después de recibir datos de un servicio determinado. Los déclencheur instantáneos pueden ser extremadamente útiles. Se recomienda utilizarlos siempre que sea posible. Ayudan a reducir el número de operaciones. Los datos recibidos se procesan inmediatamente sin esperar a la siguiente ejecución programada. Por ejemplo, la variable [!DNL Google Sheets] módulo [!UICONTROL Ver cambios] inicia un escenario inmediatamente después de actualizar una celda.

## ¿Qué son los agregadores?

### Respuesta

Un [!UICONTROL Acumulador] combina datos en una única colección. Un ejemplo de esto es que los archivos se comprimen en un archivo zip y se envían como datos adjuntos de correo electrónico.

Para obtener más información, consulte [[!UICONTROL Acumulador] módulo en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## ¿Qué es una operación?

### Respuesta

Una operación es cualquier tarea realizada por un módulo. Una operación se produce, por ejemplo, cada vez que se ejecuta un déclencheur y cada vez que una acción realiza una tarea.

## ¿Qué es la transferencia de datos?

### Respuesta

La transferencia de datos se refiere a la cantidad de datos transferidos a través del escenario. Por ejemplo, supongamos que tiene un escenario que recupera una imagen de 100 KB de FTP, reduce su tamaño a 50 KB y guarda ambas imágenes en [!DNL Dropbox]. La cantidad de datos utilizada en este escenario es de 150 KB.

## ¿Qué es una conexión?

### Respuesta

Una conexión es el vínculo entre su [!DNL Workfront Fusion] y el servicio de terceros que desee utilizar. La conexión se puede crear fácilmente al editar un escenario. Para añadir una conexión, haga clic en el botón **[!UICONTROL Agregar]** en la configuración del módulo y siga las instrucciones paso a paso.

Para obtener más información, consulte [Acerca de la conexión [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
