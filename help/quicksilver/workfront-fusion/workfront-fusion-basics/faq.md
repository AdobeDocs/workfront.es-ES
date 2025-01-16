---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Preguntas frecuentes sobre Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 89%

---

# Preguntas frecuentes sobre Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Preguntas frecuentes sobre la planificación de escenarios](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/faq.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## ¿Qué es un escenario?

### Respuesta

Un escenario define una secuencia de pasos que [!DNL Adobe Workfront Fusion] debe ejecutar. Para cada escenario, se especifica la fuente de datos, cómo se van a procesar los datos, qué datos se van a utilizar y cuáles se van a ignorar. [!DNL Workfront Fusion] le permite crear escenarios tan complejos como necesite; incluso los más sofisticados son posibles.

Para obtener más información, consulte [Crear un escenario de integración de prácticas en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## ¿Puedo utilizar más de un módulo en un escenario? ¿O solo un activador y una acción?

### Respuesta

Puede utilizar tantos módulos como desee en un escenario concreto. Puede crear rutas independientes y especificar qué datos deben fluir a través de estas. También puede utilizar los resultados devueltos por acciones individuales y luego pasarlos a la siguiente acción.

## ¿Puede [!DNL Workfront Fusion] trabajar con archivos?

### Respuesta

Sí. Con [!DNL Workfront Fusion], los archivos se pueden recibir, guardar, transformar, convertir, cifrar, etc. Además, [!DNL Workfront Fusion] proporciona una amplia gama de características integradas diseñadas para permitir que los usuarios trabajen de forma eficaz y creativa con los datos contenidos en los archivos.

Para obtener más información, consulte [Acerca de la asignación de archivos en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## ¿Qué sucede si dejo que [!DNL Workfront Fusion] procese un correo electrónico que contenga más de un archivo adjunto?

### Respuesta

Si utiliza [!UICONTROL Retrieve attachments] del módulo [!UICONTROL Email],cada archivo adjunto se enviará individualmente a través del resto de los módulos del escenario. También hay módulos similares disponibles en otras aplicaciones que reciben varios archivos a la vez.

Para obtener más información, consulte [[!UICONTROL Módulos de ]Email](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Algunos activadores permiten que los escenarios se ejecuten instantáneamente. ¿Qué significa “instantáneamente”?

### Respuesta

Los escenarios comunes se ejecutan a intervalos según la programación especificada (por ejemplo, cada hora, cada 5 minutos, una vez al mes, etc.). Existen activadores especiales, llamados activadores instantáneos (webhooks), que pueden iniciar un escenario inmediatamente después de recibir datos de un servicio determinado. Los activadores instantáneos pueden ser extremadamente útiles. Se recomienda utilizarlos siempre que sea posible. Ayudan a reducir el número de operaciones. Los datos recibidos se procesan inmediatamente sin esperar a la siguiente ejecución programada. Por ejemplo, el módulo [!DNL Google Sheets] [!UICONTROL Observar cambios] inicia un escenario inmediatamente después de actualizar una celda.

## ¿Qué son los agregadores?

### Respuesta

Un [!UICONTROL Agregador] combina datos en una sola colección. Un ejemplo de esto son los archivos que se comprimen en un archivo zip y se envían como datos adjuntos de correo electrónico.

Para obtener más información, consulte el módulo [[!UICONTROL Agregador] en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## ¿Qué es una operación?

### Respuesta

Una operación es cualquier tarea realizada por un módulo. Por ejemplo, se produce una operación cada vez que se ejecuta un activador y cada vez que una acción realiza una tarea.

## ¿Qué es la transferencia de datos?

### Respuesta

La transferencia de datos se refiere a la cantidad de datos transferidos a través de su escenario. Por ejemplo, supongamos que tiene un escenario que recupera una imagen de 100 KB del FTP, reduce su tamaño a 50 KB y guarda ambas imágenes en [!DNL Dropbox]. La cantidad de datos utilizados en esta situación es de 250 KB.

## ¿Qué es una conexión?

### Respuesta

Una conexión es el vínculo entre su cuenta de [!DNL Workfront Fusion] y el servicio de terceros que desea utilizar. La conexión se puede crear fácilmente al editar un escenario. Para añadir una conexión, haga clic en el botón **[!UICONTROL Añadir]** en la configuración del módulo y siga las instrucciones paso a paso.

Para obtener más información, consulte [Información general de las conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
