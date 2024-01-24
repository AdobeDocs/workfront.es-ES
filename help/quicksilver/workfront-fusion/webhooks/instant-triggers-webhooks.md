---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]
description: Muchos servicios proporcionan webhooks para entregar notificaciones instantáneas cada vez que se produce un determinado cambio en el servicio. Para procesar estas notificaciones, le recomendamos que utilice déclencheur instantáneos. En este artículo se describe el uso y la funcionalidad de los déclencheur instantáneos en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]

Muchos servicios proporcionan webhooks para entregar notificaciones instantáneas cada vez que se produce un determinado cambio en el servicio. Para procesar estas notificaciones, le recomendamos que utilice déclencheur instantáneos. Puede reconocerlas fácilmente en [!DNL Adobe Workfront Fusion] debido a su etiqueta:

![](assets/instant-350x256.png)

Si el servicio no proporciona webhooks, usted necesita utilizar déclencheur de sondeo para sondear periódicamente el servicio.

Para ver un vídeo introductorio a los webhooks en Workfront Fusion, consulte:

* [Introducción a Webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Webhooks intermedios](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

## Ver la cola de un gancho web

Todos los mensajes de los webhooks entrantes se almacenan en la cola del webhook.

1. Clic **[!UICONTROL Webhooks]** en el menú de la izquierda.
1. Busque el webhook para el que desea ver la cola.
1. Haga clic en el botón con un icono de camión y el número de webhooks recibidos.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Los datos del gancho web entrante siempre se almacenan en la cola, independientemente de cómo haya configurado la opción [!UICONTROL Datos] es confidencial (descrito en [El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Tan pronto como los datos se procesan en un escenario, se eliminan del sistema de forma permanente.

## Programar déclencheur instantáneos

Si el escenario contiene un déclencheur instantáneo, puede programar su ejecución inmediata:

![](assets/schedule-setting-350x185.png)

En este caso, el escenario se ejecutará inmediatamente cuando [!DNL Workfront Fusion] recibe nuevos datos del servicio de. Una vez que se ejecuta el escenario, se cuenta la cantidad total de webhooks pendientes que esperan en la cola y el escenario realiza tantos ciclos como webhooks pendientes, procesando un webhook por ciclo. Para obtener más información, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Un ciclo no es lo mismo que una ejecución de escenario. Puede haber varios ciclos en 1 escenario ejecutado.
>* Cuando se ejecuta un escenario con un déclencheur instantáneo programado para ser inmediato, se aplican las siguientes excepciones:
>
>     * El intervalo entre dos ejecuciones no está sujeto al intervalo mínimo según el plan de precios.
>
>       Por ejemplo, una vez que el escenario termina de ejecutarse, la cola del gancho web se vuelve a comprobar. Si hay algún webhooks pendiente, el escenario se ejecuta inmediatamente de nuevo, procesando todos los webhooks pendientes una vez más.
>   
>     * La configuración del escenario Número máximo de ciclos se ignora y se establece en 100, lo que significa que no se procesarán más de 100 webhooks pendientes durante una sola ejecución de escenario (a razón de 1 evento por cada ciclo).
>


Si utiliza cualquier otra configuración de programación que no sea [!UICONTROL Inmediata], el escenario se ejecutará a los intervalos especificados. Dado que se pueden agrupar varios webhooks en la cola durante el intervalo, se recomienda configurar la variable [[!UICONTROL Número máximo de ciclos]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) a un valor mayor que el predeterminado 1 para procesar más webhooks en un escenario ejecute:

1. Haga clic en [!UICONTROL Configuración de escenarios] icono ![](assets/gear-icon-settings.png) en la parte inferior de su escenario.
1. En el **[!UICONTROL Configuración de escenarios]** que aparece, escriba un número en el cuadro **[!UICONTROL Número máximo de ciclos]** para indicar el número de webhooks de la cola que desea ejecutar cada vez que ejecute el escenario.

## Límites de velocidad

El límite de velocidad actual es de 5 webhooks por segundo. Si se supera el límite, se devuelve un código de estado 429.

## Caducidad de webhooks inactivos

Se elimina un webhook que no haya sido asignado a ningún escenario por más de 120 horas.

## Cargas útiles de Webhook

[!DNL Workfront Fusion] almacena cargas útiles de webhook durante 30 días. Acceder a una carga útil de gancho web más de 30 días después de crearla provoca el error &quot;[!UICONTROL Error al leer el archivo desde el almacenamiento.]&quot;

## Control de errores

Cuando hay un error en su escenario con un déclencheur instantáneo, el escenario:

* Se detiene inmediatamente: cuando el escenario está configurado para ejecutarse [!UICONTROL Inmediata].
* Se detiene después de tres intentos fallidos (tres errores): cuando el escenario está configurado para ejecutarse según lo programado.

Si se produce un error durante la ejecución del escenario, el gancho web se vuelve a colocar en la cola durante la fase de reversión del déclencheur instantáneo. En tal situación, tiene la posibilidad de corregir el escenario y volver a ejecutarlo. Para obtener más información, consulte [Reversión](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) en el artículo [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si hay un módulo de respuesta de webhook en su escenario, el error se envía a la respuesta de webhook. El módulo de respuesta Webhook siempre se ejecuta en último lugar (en caso de que la variable [!UICONTROL Confirmación automática] en la configuración del escenario (no está activada). Para obtener más información, consulte [Respuesta a los webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) en el artículo [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhooks personalizados

Puede crear sus propios webhooks. Para obtener más información, consulte [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Desactivación de webhook

Los webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

* El webhook no ha estado conectado a ningún escenario durante más de 5 días
* El webhook solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

Los webhooks desactivados se borran y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.


