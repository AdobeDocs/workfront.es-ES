---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: El panel de ajustes de escenarios en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 81%

---

# El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Configurar opciones de escenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/configure-scenario-settings.html)
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

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Abrir la configuración del escenario

1. Abra el editor de escenarios, tal como se explica en [El editor de escenarios en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Haga clic en el icono de engranaje situado cerca de la esquina inferior izquierda de la página.

   ![](assets/scenario-settings-350x221.png)

   En el panel [!UICONTROL Configuración de escenario] que se muestra, puede configurar varias opciones avanzadas para el escenario.

## [!UICONTROL Permitir almacenar ejecuciones incompletas]

Esta opción determina cómo procede [!DNL Adobe Workfront Fusion] si se produce un error durante la ejecución de un escenario. Con esta opción habilitada, el escenario se detiene y se mueve a [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Esto le ofrece la posibilidad de solucionar el problema y seguir ejecutando desde el lugar en el que se detuvo el escenario. Si esta opción está desactivada, la ejecución del escenario se detiene y se inicia una fase de reversión.

## [!UICONTROL Procesamiento secuencial]

Esta opción fuerza que todas las ejecuciones se produzcan en orden y es principalmente relevante para los webhooks y para las ejecuciones incompletas.

Cuando se habilita el procesamiento secuencial, se desactivan las ejecuciones paralelas del escenario.

### Webhooks instantáneos

Si el déclencheur de un webhook está configurado como `instant` y &quot;Procesamiento secuencial&quot; está habilitado, todas las cargas instantáneas de los webhook se pondrán en cola y se procesarán en el orden en que lleguen. Esto puede resultar útil cuando se procesan eventos de sistemas externos en un orden exacto.

>[!NOTE]
>
>Habrá retrasos de procesamiento automático a medida que cada carga útil se procese antes de que se inicie la siguiente.

### Ejecuciones incompletas

Si también está activada la opción &quot;Ejecuciones incompletas&quot;, si se produce un error durante la ejecución de un escenario, este se detiene. A continuación, se produce una de las siguientes acciones:

* Si la opción Sequential processing está **habilitada**, Workfront Fusion deja de procesar la secuencia preexistente hasta que se resuelven todas las ejecuciones incompletas.
* Si la opción de procesamiento secuencial está **deshabilitada**, el escenario seguirá ejecutándose según su programación, acompañado de repetidos intentos de volver a ejecutar las ejecuciones incompletas.

Para obtener más información sobre las ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>El procesamiento secuencial puede provocar un retraso en la ejecución de un escenario. Si todavía hay ejecuciones incompletas en la cola cuando se activa un escenario instantáneo o uno programado está configurado para ejecutarse, este se ejecutará después de que se hayan completado todas las ejecuciones antes de que esté en la cola.
>
>Si el caso de uso para sus escenarios no requiere procesamiento secuencial, se recomienda desactivar la opción de procesamiento secuencial.

Para obtener más información sobre la programación, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Los datos son confidenciales

Una vez ejecutado un escenario, puede mostrar de forma predeterminada información sobre los datos que han procesado los módulos en el escenario. Si no desea almacenar esta información, habilite la opción [!UICONTROL Datos confidenciales].

Para obtener más información sobre cómo mostrar la información, consulte [Flujo de ejecución del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Si activa esta opción, puede resultar difícil resolver los errores que pueden producirse durante la ejecución de un escenario.

## Habilitar la pérdida de datos

Esta opción tiene que ver con la activación de la pérdida de datos si [!DNL Workfront Fusion] no puede guardar un paquete en la cola de [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (por ejemplo, debido a la falta de espacio libre). Con esta opción habilitada, los datos se pierden para evitar interrupciones en la ejecución general del escenario. Esto resulta útil en escenarios en los que la prioridad más alta es la ejecución continua y los datos erróneos entrantes no son tan importantes.

Aparte de esto, al ejecutar un escenario, un módulo a veces puede encontrar un archivo que sea más grande que el tamaño máximo permitido. En este caso, [!DNL Workfront Fusion] procede de acuerdo con la configuración de la opción [!UICONTROL Habilitar la pérdida de datos] y se muestra un mensaje de advertencia.

Para obtener más información acerca del tamaño máximo de archivo, consulte [Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Para obtener más información sobre las advertencias, consulte [Error al procesar en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Confirmación automática]

La configuración de [!UICONTROL confirmación automática] se aplica a las transacciones y define la forma de procesar un escenario. Si la opción de confirmación automática está activada, la fase de confirmación de cada módulo se inicia inmediatamente después de completar la fase de operación. Con la opción de confirmación automática desactivada, no se produce ninguna confirmación hasta que se ejecutan las operaciones para todos los módulos (este es el modo predeterminado).

Para obtener más información sobre las transacciones, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Número máximo de ciclos

La configuración de más ciclos puede resultar útil cuando desea evitar la interrupción de la conexión a un servicio de terceros y garantizar que todos los registros se procesen dentro de la ejecución de un escenario.

* Si el escenario comienza con un activador de sondeo, el ajuste define el número máximo de ciclos permitidos durante la ejecución del escenario.

  Para obtener más información sobre los activadores de sondeo, consulte [Activador de sondeo](../../workfront-fusion/modules/module-types.md#polling) en [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Si el escenario comienza con un activador instantáneo, el ajuste se ignora y todos los eventos pendientes se procesan durante una sola ejecución de escenario, un evento por ciclo.

  Para obtener más información sobre los activadores instantáneos, consulte [Activadores instantáneos](../../workfront-fusion/modules/module-types.md#instant) en [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Si el escenario no comienza con un activador (instantáneo/sondeo), siempre se realiza el número máximo de ciclos especificado.

>[!INFO]
>
>**Ejemplos:** [!DNL Workfront] > [!UICONTROL Observar registro] observa los nuevos problemas que se producen y [!DNL Workfront] >[!UICONTROL Convertir objeto] convierte la nueva solicitud en un proyecto y le asigna la plantilla adecuada.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>La configuración [!UICONTROL más ciclos] solo se aplica cuando se programa la ejecución del escenario. Al usar el botón [!UICONTROL Ejecutar una vez], se tiene en cuenta la configuración del ciclo.
>
>### El número máximo de ciclos se establece en 1 (predeterminado)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>El [!UICONTROL número máximo de archivos devueltos] en el módulo [!UICONTROL Workfront] >[!UICONTROL Observar registros] se ha establecido en `10`.
>Si se envían 100 solicitudes a [!DNL Workfront] y el campo [!UICONTROL Límite] se establece en 10, 90 archivos quedarán sin procesar tras la ejecución de un escenario. Los siguientes 10 archivos se procesan en la posterior ejecución de escenario programada.
>
>### El número máximo de ciclos se establece en 10
>
>El [!UICONTROL número máximo de archivos devueltos] en el módulo [!UICONTROL Dropbox] >[!UICONTROL Observar archivos] se ha establecido en `10`.
>
>Si se añaden 100 archivos a la carpeta Dropbox y la opción [!UICONTROL Número máximo de archivos devueltos] se establece en 10, se procesarán 10 archivos durante el primer ciclo, los siguientes 10 archivos en el segundo ciclo, los siguientes 10 archivos en el tercer ciclo, etc., hasta que se procesen todos los archivos.
>
>Todos los archivos se procesan en un escenario de ejecución.
>
>Puede ver los ciclos ya ejecutados en los detalles del escenario:
>
>![](assets/scenario-detail-350x207.png)
>
>Para obtener más información acerca de esta página, consulte [Detalles del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Número de errores consecutivos

Define el número máximo de intentos de ejecución consecutivos antes de desactivar la ejecución de un escenario (excluyendo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] y [!UICONTROL ConnectionError]).

Para obtener más información sobre los errores, consulte [Procesamiento de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Si un escenario comienza con un activador instantáneo, la configuración se ignora y el escenario se desactiva inmediatamente después de que se haya producido el primer error.
