---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]
description: Muchos servicios proporcionan webhooks para entregar notificaciones instantáneas cuando se produce un cambio determinado en el servicio. Para procesar estas notificaciones, le recomendamos que utilice déclencheur instantáneos. Este artículo describe el uso y la funcionalidad de los déclencheur instantáneos en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 04191419ab6079cc34576b5a7532cd1596e4b91d
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]

Muchos servicios proporcionan webhooks para entregar notificaciones instantáneas cuando se produce un cambio determinado en el servicio. Para procesar estas notificaciones, le recomendamos que utilice déclencheur instantáneos. Puede reconocerlos fácilmente en [!DNL Adobe Workfront Fusion] debido a su etiqueta :

![](assets/instant-350x256.png)

Si el servicio no proporciona enlaces web, debe utilizar déclencheur de sondeo para sondear periódicamente el servicio.

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

## Ver la cola de un enlace web

Todos los mensajes de los webhooks entrantes se almacenan en la cola del weblock.

1. Haga clic en **[!UICONTROL Enlaces web]** en el menú de la izquierda.
1. Busque el Weblock para el que desea ver la cola.
1. Haga clic en el botón con un icono de camión y el número de webhooks recibidos.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Los datos entrantes de los ganchos web siempre se almacenan en la cola, independientemente de cómo haya configurado la opción [!UICONTROL Datos] es confidencial (descrito en [El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Tan pronto como los datos se procesan en un escenario, se eliminan de forma permanente del sistema.

## Programar déclencheur instantáneos

Si el escenario contiene un déclencheur instantáneo, puede programar el escenario para que se ejecute inmediatamente:

![](assets/schedule-setting-350x185.png)

En este caso, el escenario se ejecutará inmediatamente cuando [!DNL Workfront Fusion] recibe nuevos datos del servicio. Una vez que se ejecuta el escenario, se cuenta la cantidad total de webhooks pendientes esperando en la cola y el escenario realiza tantos ciclos como hay webhooks pendientes, procesando un weblock por ciclo. Para obtener más información, consulte [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Un ciclo no es lo mismo que una ejecución de escenario. Puede haber múltiples ciclos dentro de un escenario ejecutado.
>* Cuando ejecuta un escenario con un déclencheur instantáneo programado para ser inmediato, se aplican las siguientes excepciones:
   >
   >     * El intervalo entre dos ejecuciones no está sujeto al intervalo mínimo según el plan de precios.

      >
      >       Por ejemplo, una vez que el escenario termina su ejecución, la cola del enlace web se vuelve a comprobar. Si hay algún enlace web pendiente, el escenario se ejecuta inmediatamente de nuevo, procesando de nuevo todos los enlaces web pendientes.
   >   
   >     * La configuración del escenario Número máximo de ciclos se ignora y se establece en 100, lo que significa que no se procesarán más de 100 enlaces web pendientes durante una sola ejecución del escenario (a la velocidad de 1 evento por ciclo).
>



Si utiliza cualquier otra configuración de programación que no sea [!UICONTROL Inmediatamente], el escenario se ejecuta a los intervalos especificados. Como se pueden reunir varios vínculos web en la cola durante el intervalo, se recomienda configurar la variable [[!UICONTROL Número máximo de ciclos]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) a un valor mayor que el 1 predeterminado para procesar más vínculos web en una ejecución de escenario:

1. Haga clic en el [!UICONTROL Configuración del escenario] icono ![](assets/gear-icon-settings.png) en la parte inferior de su escenario.
1. En el **[!UICONTROL Configuración del escenario]** que aparece, escriba un número en la **[!UICONTROL Número máximo de ciclos]** para indicar el número de webhooks de la cola que desea ejecutar cada vez que ejecute el escenario.

## Límites de tasa

El límite de tasa actual es de 5 enlaces web por segundo. Si se supera el límite, se devuelve un código de estado 429.

## Caducidad de webhooks inactivos

Se elimina un vínculo web que no se haya asignado a ningún escenario durante más de 120 horas.

## Carga útil de Weblock

[!DNL Workfront Fusion] almacena cargas útiles de weblock durante 30 días. El acceso a una carga útil de weblock más de 30 días después de su creación da como resultado el error &quot;[!UICONTROL No se pudo leer el archivo desde el almacenamiento.]&quot;

## Gestión de errores

Cuando hay un error en su escenario con un déclencheur instantáneo, el escenario:

* Se detiene inmediatamente: cuando el escenario está configurado para ejecutarse [!UICONTROL Inmediatamente].
* Se detiene después de 3 intentos fallidos (3 errores), cuando el escenario está configurado para ejecutarse como está programado.

Si se produce un error durante la ejecución del escenario, el enlace web se vuelve a colocar en la cola durante la fase de reversión del déclencheur instantáneo. En tal situación, tiene la posibilidad de corregir el escenario y volver a ejecutarlo. Para obtener más información, consulte [Reversión](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) en el artículo [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si hay un módulo de respuesta de Weblock en su escenario, el error se envía a la respuesta de Weblock. El módulo de respuesta Weblock siempre se ejecuta en último lugar (en el caso de que la variable [!UICONTROL Compromiso automático] en la configuración del escenario (no está activada). Para obtener más información, consulte [Respuesta a los enlaces web](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) en el artículo [Enlaces web](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Enlaces web personalizados

Puede crear sus propios enlaces web. Para obtener más información, consulte [Enlaces web](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Desactivación de Weblock

Los Webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

* El enlace web no ha estado conectado a ningún escenario durante más de 5 días
* El enlace web solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

Los enlaces web desactivados se eliminan y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.


