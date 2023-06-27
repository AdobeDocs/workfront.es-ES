---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Preguntas frecuentes sobre Adobe Workfront Fusion
description: Este artículo aborda preguntas comunes relacionadas con [!DNL Adobe Workfront Fusion], incluida información sobre los objetos que se utilizan normalmente en flujos de trabajo de Fusion
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: tm+mt
source-wordcount: '668'
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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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

## ¿Qué es un escenario?

### Respuesta

Un escenario define una secuencia de pasos que se van a ejecutar en [!DNL Adobe Workfront Fusion]. Para cada escenario, se especifica la fuente de datos, cómo se van a procesar los datos, qué datos se van a utilizar y qué se van a ignorar. [!DNL Workfront Fusion] permite crear escenarios tan complejos como sea necesario; incluso los más sofisticados son posibles.

Para obtener más información, consulte [Cree un escenario de integración de prácticas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## ¿Puedo utilizar más de un módulo en un escenario? ¿O sólo un déclencheur y acción?

### Respuesta

Puede utilizar tantos módulos como desee en un escenario concreto. Puede crear rutas independientes y especificar qué datos deben fluir a través de ellas. También puede utilizar los resultados devueltos por acciones individuales y luego pasarlos a la siguiente acción.

## Puede [!DNL Workfront Fusion] ¿trabajar con archivos?

### Respuesta

Sí. Uso de [!DNL Workfront Fusion], los archivos se pueden recibir, guardar, transformar, convertir, cifrar, etc. Además, [!DNL Workfront Fusion] proporciona una amplia gama de funciones integradas diseñadas para permitir a los usuarios trabajar de forma eficaz y creativa con los datos contenidos en los archivos.

Para obtener más información, consulte [Asignación de archivos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## ¿Qué pasa si dejo que [!DNL Workfront Fusion] ¿desea procesar un correo electrónico que contenga más de un archivo adjunto?

### Respuesta

Si usa el [!UICONTROL Correo electrónico] módulo [!UICONTROL Recuperar archivos adjuntos], cada archivo adjunto se envía individualmente a través del resto de los módulos del escenario. Módulos similares también están disponibles en otras aplicaciones que reciben varios archivos a la vez.

Para obtener más información, consulte [[!UICONTROL Correo electrónico] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Algunos déclencheur permiten que los escenarios se ejecuten instantáneamente. ¿Qué significa &quot;instantáneamente&quot;?

### Respuesta

Los escenarios comunes se ejecutan a intervalos según la programación especificada (por ejemplo, cada hora, cada 5 minutos, una vez al mes, etc.). Existen déclencheur especiales, llamados déclencheur instantáneos (webhooks), que pueden iniciar su escenario inmediatamente después de recibir datos de un servicio determinado. Los déclencheur instantáneos pueden ser extremadamente útiles. Se recomienda utilizarlos siempre que sea posible. Ayudan a reducir el número de operaciones. Los datos recibidos se procesan inmediatamente sin esperar a la siguiente ejecución programada. Por ejemplo, la variable [!DNL Google Sheets] módulo [!UICONTROL Ver cambios] inicia un escenario inmediatamente después de actualizar una celda.

## ¿Qué son los acumuladores?

### Respuesta

Un [!UICONTROL Agregador] combina datos en una sola colección. Un ejemplo de esto son los archivos que se comprimen en un archivo zip y se envían como datos adjuntos de correo electrónico.

Para obtener más información, consulte [[!UICONTROL Agregador] módulo en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## ¿Qué es una operación?

### Respuesta

Una operación es cualquier tarea realizada por un módulo. Por ejemplo, se produce una operación cada vez que se ejecuta un déclencheur y cada vez que una acción realiza una tarea.

## ¿Qué es la transferencia de datos?

### Respuesta

La transferencia de datos se refiere a la cantidad de datos transferidos a través de su escenario. Por ejemplo, supongamos que tiene un escenario que recupera una imagen de 100 KB de FTP, reduce su tamaño a 50 KB y guarda ambas imágenes en [!DNL Dropbox]. La cantidad de datos utilizados en esta situación es de 250 KB.

## ¿Qué es una conexión?

### Respuesta

Una conexión es el vínculo entre sus [!DNL Workfront Fusion] y el servicio de terceros que desee utilizar. La conexión se puede crear fácilmente al editar un escenario. Para añadir una conexión, haga clic en **[!UICONTROL Añadir]** en la configuración del módulo y siga las instrucciones paso a paso.

Para obtener más información, consulte [Acerca de conectar [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
