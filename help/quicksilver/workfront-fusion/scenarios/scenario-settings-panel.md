---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: El panel de configuración de escenarios en Adobe Workfront Fusion
description: Este artículo describe la configuración disponible en la [!UICONTROL configuración de escenarios] panel en su [!DNL Adobe Workfront Fusion] escenarios.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 4d9832d0870c3fccf847c3932ad4f985a62b9672
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]

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

## Abrir la configuración del escenario

1. Abra el editor de escenarios, tal como se explica en [El editor de escenarios en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Haga clic en el icono de engranaje situado cerca de la esquina inferior izquierda de la página.

   ![](assets/scenario-settings-350x221.png)

   En el [!UICONTROL Configuración de escenarios] en el panel que se muestra, puede configurar varias opciones avanzadas para el escenario.

## [!UICONTROL Permitir almacenar ejecuciones incompletas]

Esta opción determina cómo [!DNL Adobe Workfront Fusion] procede si se produce un error durante la ejecución de un escenario. Con esta opción habilitada, el escenario se detiene y se mueve a [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Esto le ofrece la posibilidad de solucionar el problema y seguir ejecutando desde el lugar en el que se detuvo el escenario. Si esta opción está desactivada, la ejecución del escenario se detiene y se inicia una fase de reversión.

## [!UICONTROL Procesamiento secuencial]

Esta opción determina cómo [!DNL Workfront Fusion] procede si se produce un error y la ejecución de un escenario se mueve a la [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Si la variable [!UICONTROL Procesamiento secuencial] Si la opción está activada, Workfront Fusion deja de procesar la secuencia de tareas hasta que se resuelven todas las ejecuciones incompletas. Si la variable [!UICONTROL Procesamiento secuencial] está desactivada, el escenario sigue ejecutándose según su programación, acompañado de repetidos intentos de volver a ejecutar las ejecuciones incompletas.

>[!NOTE]
>
>El procesamiento secuencial puede provocar un retraso en la ejecución de un escenario. Si todavía hay ejecuciones incompletas en la cola cuando hay un déclencheur de escenario instantáneo o un escenario programado está configurado para ejecutarse, ese escenario se ejecutará después de que se hayan completado todas las ejecuciones antes de que esté en la cola.
>
>Si el caso de uso para sus escenarios no requiere procesamiento secuencial, se recomienda desactivar la opción de procesamiento secuencial.

Para obtener más información sobre la programación, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Los datos son confidenciales

Una vez ejecutado un escenario, puede mostrar de forma predeterminada información sobre los datos que han procesado los módulos en el escenario. Si no desea almacenar esta información, habilite la opción [!UICONTROL Los datos son confidenciales] opción.

Para obtener más información sobre cómo mostrar la información, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Si activa esta opción, puede resultar difícil resolver los errores que pueden producirse durante la ejecución de un escenario.

## Habilitar la pérdida de datos

Esta opción tiene que ver con la activación de la pérdida de datos si [!DNL Workfront Fusion] no se puede guardar un paquete en la cola de [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (por ejemplo, debido a la falta de espacio libre). Con esta opción habilitada, los datos se pierden para evitar interrupciones en la ejecución general del escenario. Esto resulta útil en escenarios en los que la prioridad más alta es la ejecución continua y los datos erróneos entrantes no son tan importantes.

Aparte de esto, al ejecutar un escenario, un módulo a veces puede encontrar un archivo que sea más grande que el tamaño máximo permitido. En este caso, [!DNL Workfront Fusion] procede de acuerdo con la configuración de la [!UICONTROL Habilitar la pérdida de datos] y se muestra un mensaje de advertencia.

Para obtener más información sobre el tamaño máximo de archivo, consulte [Asignación de archivos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Para obtener más información sobre las advertencias, consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Confirmación automática]

El [!UICONTROL Confirmación automática] La configuración de se aplica a las transacciones y define la forma de procesar un escenario. Si la opción de confirmación automática está activada, la fase de confirmación de cada módulo se inicia inmediatamente después de completar la fase de operación. Con la opción de confirmación automática desactivada, no se produce ninguna confirmación hasta que se ejecutan las operaciones para todos los módulos (este es el modo predeterminado).

Para obtener más información sobre las transacciones, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Número máximo de ciclos

La configuración de más ciclos puede resultar útil cuando desea evitar la interrupción de la conexión a un servicio de terceros y garantizar que todos los registros se procesen dentro de la ejecución de un escenario.

* Si el escenario comienza con un déclencheur de sondeo, la configuración define el número máximo de ciclos permitidos durante la ejecución del escenario.

  Para obtener más información sobre los déclencheur de sondeo, consulte [Déclencheur de sondeo](../../workfront-fusion/modules/module-types.md#polling) in [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Si el escenario comienza con un déclencheur instantáneo, el ajuste se ignora y todos los eventos pendientes se procesan durante una sola ejecución de escenario, un evento por ciclo.

  Para obtener más información sobre los déclencheur instantáneos, consulte [Déclencheur instantáneos](../../workfront-fusion/modules/module-types.md#instant) in [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Si el escenario no comienza con un déclencheur (instantáneo/sondeo), siempre se realiza el número máximo especificado de ciclos.

>[!INFO]
>
>**Ejemplos:**  [!DNL Workfront] > [!UICONTROL Ver registro] busca nuevos problemas que llegan, y [!DNL Workfront] >[!UICONTROL Convertir objeto] convierte la nueva solicitud en un proyecto y le asigna la plantilla adecuada.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL más ciclos] La configuración de solo se aplica cuando se programa la ejecución del escenario. Cuando se usa la variable [!UICONTROL Ejecutar una vez] botón, se tienen en cuenta los ajustes del ciclo.
>
>### El número máximo de ciclos se establece en 1 (predeterminado)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>El [!UICONTROL Número máximo de archivos devueltos] en el [!UICONTROL Dropbox] >[!UICONTROL Ver archivos] El módulo se ha definido en `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Si se envían 100 solicitudes a [!DNL Workfront], y el [!UICONTROL Límite] Si el campo se establece en 10, luego de ejecutar un escenario se dejarán 90 archivos sin procesar. Los siguientes 10 archivos se procesan en la siguiente ejecución de escenario programada.
>
>### El número máximo de ciclos se establece en 10
>
>El [!UICONTROL Número máximo de archivos devueltos] en el [!UICONTROL Dropbox] >[!UICONTROL Ver archivos] El módulo se ha definido en `10`.
>
>Si se añaden 100 archivos a la carpeta Dropbox y la variable [!UICONTROL Número máximo de archivos devueltos] opción se establece en 10, luego se procesan 10 archivos durante el primer ciclo, los siguientes 10 archivos en el segundo ciclo, los siguientes 10 archivos en el tercer ciclo y así sucesivamente, hasta que se procesen todos los archivos.
>
>Todos los archivos se procesan en 1 escenario de ejecución.
>
>Puede ver los ciclos ya ejecutados en los detalles de Escenario:
>
>![](assets/scenario-detail-350x207.png)
>
>Para obtener más información sobre esta página, consulte [Detalles del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Número de errores consecutivos

Define el número máximo de intentos de ejecución consecutivos antes de que se desactive la ejecución de un escenario (excluyendo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] y [!UICONTROL ConnectionError]).

Para obtener más información sobre los errores, consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Si un escenario comienza con un déclencheur instantáneo, la configuración se ignora y el escenario se desactiva inmediatamente después de que se haya producido el primer error.
