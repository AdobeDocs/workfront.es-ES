---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 91%

---

# Activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se puede encontrar en los artículos:
>
>* [déclencheur instantáneos (webhooks)](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/webhooks-reference.html)
>* [Ver la cola de un gancho web](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-webhook-queue.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Muchos servicios proporcionan webhooks para entregar notificaciones instantáneas cada vez que se produce un determinado cambio en el servicio. Para procesar estas notificaciones, le recomendamos que utilice activadores instantáneos. Puede reconocerlos fácilmente en [!DNL Adobe Workfront Fusion] gracias a su etiqueta:

![](assets/instant-350x256.png)

Si el servicio no proporciona webhooks, es necesario utilizar activadores de sondeo para sondear periódicamente el servicio.

Para ver un vídeo introductorio a los webhooks en Workfront Fusion, consulte lo siguiente:

* [Introducción a Webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Webhooks intermedios](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ver la cola del webhook

Todos los mensajes de los webhooks entrantes se almacenan en la cola del webhook.

1. Haga clic en **[!UICONTROL webhooks]** en el menú de la izquierda.
1. Busque el webhook en el que desea ver la cola.
1. Haga clic en el botón con el icono de un camión y el número de webhooks recibidos.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Los datos de webhook entrantes siempre se almacenan en la cola, independientemente de cómo haya configurado la opción [!UICONTROL Datos], que es confidencial (se describe en [El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Tan pronto como los datos se procesan en un escenario, se eliminan del sistema de forma permanente.

## Programar activadores instantáneos

Si el escenario contiene un activador instantáneo, puede programar su ejecución inmediata:

![](assets/schedule-setting-350x185.png)

En este caso, su escenario se ejecutará inmediatamente cuando [!DNL Workfront Fusion] reciba nuevos datos del servicio. Una vez que se ejecuta el escenario, se cuenta la cantidad total de webhooks pendientes que esperan en la cola y el escenario realiza tantos ciclos como webhooks pendientes, procesando un webhook por ciclo. Para obtener más información, consulte [Ejecución de escenarios, ciclos y fases en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Un ciclo no es lo mismo que una ejecución de escenario. Puede haber varios ciclos en un escenario ejecutado.
>* Cuando se ejecuta un escenario con un activador instantáneo programado para ser inmediato, se aplican las siguientes excepciones:
>
>     * El intervalo entre dos ejecuciones no está sujeto al intervalo mínimo según el plan de precios.
>
>       Por ejemplo, una vez que el escenario termina de ejecutarse, la cola del webhook se vuelve a comprobar. Si hay algún webhook pendiente, el escenario se ejecuta inmediatamente de nuevo, procesando todos los webhooks pendientes una vez más.
>   
>     * La configuración del escenario Número máximo de ciclos se ignora y se establece en 100, lo que significa que no se procesarán más de 100 webhooks pendientes durante una sola ejecución de escenario (a razón de un evento por cada ciclo).
>


Si usa cualquier otra configuración de programación distinta de [!UICONTROL Inmediatamente], el escenario se ejecutará a los intervalos especificados. Como se pueden reunir varios webhooks en la cola durante el intervalo, se recomienda establecer el [[!UICONTROL Número máximo de ciclos]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) en un valor mayor que el predeterminado 1 para procesar más webhooks en una ejecución de escenario:

1. Haga clic en el icono [!UICONTROL Configuración del escenario] ![](assets/gear-icon-settings.png) en la parte inferior del escenario.
1. En el cuadro **[!UICONTROL Configuración de escenario]** que aparece, escriba un número en el cuadro **[!UICONTROL Número máximo de ciclos]** para indicar el número de webhooks de la cola que desea ejecutar cada vez que ejecute el escenario.

## Límites de velocidad

El límite de velocidad actual es de 5 webhooks por segundo. Si se supera el límite, se devuelve un código de estado 429.

## Caducidad de webhooks inactivos

Se eliminará un webhook que no se haya asignado a ningún escenario durante más de 120 horas.

## Cargas útiles de webhook

[!DNL Workfront Fusion] almacena cargas útiles de webhook durante 30 días. Acceder a una carga útil de webhook más de 30 días después de crearla genera el error ‘’[!UICONTROL No se pudo leer el archivo desde el almacenamiento]”.

## Gestión de errores

Cuando hay un error en su escenario con un activador instantáneo, el escenario:

* Se detiene inmediatamente cuando el escenario está configurado para ejecutarse [!UICONTROL Inmediatamente].
* Se detiene después de tres intentos fallidos (tres errores): cuando el escenario está configurado para ejecutarse según lo programado.

Si se produce un error durante la ejecución del escenario, el webhook se vuelve a poner en la cola durante la fase de reversión del activador instantáneo. En tal situación, tiene la posibilidad de corregir el escenario y volver a ejecutarlo. Para obtener más información, consulte [Reversión](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) en el artículo [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si hay un módulo de respuesta de webhook en su escenario, el error se envía ahí. El módulo de respuesta webhook siempre se ejecuta en último lugar (en caso de que la opción [!UICONTROL Confirmación automática] en la configuración del escenario no esté habilitada). Para obtener más información, consulte [Respuesta a los webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) en el artículo [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhooks personalizados

Puede crear sus propios webhooks. Para obtener más información, consulte [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Desactivación de un webhook

Los webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

* El webhook no ha estado conectado a ningún escenario durante más de 5 días
* El webhook solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

Los webhooks desactivados se borran y no se registran automáticamente si no están conectados a ningún escenario y han permanecido en estado desactivado durante más de 30 días.


