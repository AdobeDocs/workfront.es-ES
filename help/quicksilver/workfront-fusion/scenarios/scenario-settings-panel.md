---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: El panel de configuración de escenario en Adobe Workfront Fusion
description: Este artículo describe la configuración disponible en la [!UICONTROL configuración de escenario] del panel [!DNL Adobe Workfront Fusion] escenarios.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Abrir la configuración de escenario

1. Abra el editor de escenarios, tal como se explica en [El editor de escenarios de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Haga clic en el icono de engranaje cerca de la esquina inferior izquierda de la página.

   ![](assets/scenario-settings-350x221.png)

   En el [!UICONTROL Configuración del escenario] que se muestra, puede configurar varias opciones de configuración avanzadas para el escenario.

## [!UICONTROL Permitir el almacenamiento de ejecuciones incompletas]

Esta opción determina cómo [!DNL Adobe Workfront Fusion] se ejecuta si se produce un error durante la ejecución de un escenario. Con esta opción habilitada, el escenario se pone en pausa y se mueve a [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Esto le ofrece la posibilidad de solucionar el problema y continuar ejecutándose desde donde se detuvo el escenario. Si esta opción está desactivada, la ejecución del escenario se detiene y se inicia una fase de reversión.

## [!UICONTROL Procesamiento secuencial]

Esta opción determina cómo [!DNL Workfront Fusion] se ejecuta si se produce un error y la ejecución de un escenario se mueve al [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Si la variable [!UICONTROL Procesamiento secuencial] está activada, Workfront Fusion deja de procesar la secuencia de tareas por completo hasta que se resuelven todas las ejecuciones incompletas. Si la variable [!UICONTROL Procesamiento secuencial] está desactivada, el escenario sigue ejecutándose según su programación, acompañado de repetidos intentos de volver a ejecutar las ejecuciones incompletas.

Para obtener más información sobre la programación, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Los datos son confidenciales

Una vez ejecutado un escenario, puede mostrar de forma predeterminada información sobre qué datos fueron procesados por módulos en el escenario. Si no desea que se almacene esta información, habilite la variable [!UICONTROL Los datos son confidenciales] .

Para obtener más información sobre la visualización de información, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Si activa esta opción, puede resultar difícil resolver los errores que puedan producirse durante la ejecución de un escenario.

## Habilitar la pérdida de datos

Esta opción tiene que ver con habilitar la pérdida de datos si [!DNL Workfront Fusion] no se puede guardar un paquete en la cola de [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (por ejemplo, debido a la falta de espacio libre). Con esta opción habilitada, los datos se pierden para evitar interrupciones en la ejecución general del escenario. Esto resulta útil en escenarios en los que la prioridad más alta es la ejecución continua y los datos erróneos entrantes no son tan importantes.

Aparte de esto, al ejecutar un escenario, un módulo puede encontrar a veces un archivo que supera el tamaño máximo permitido. En este caso, [!DNL Workfront Fusion] el producto de conformidad con la definición de [!UICONTROL Habilitar la pérdida de datos] y se muestra un mensaje de advertencia.

Para obtener más información sobre el tamaño máximo del archivo, consulte [Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Para obtener más información sobre las advertencias, consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Compromiso automático]

La variable [!UICONTROL Compromiso automático] la configuración se aplica a las transacciones y define la forma de procesar un escenario. Si la opción de confirmación automática está activada, la fase de confirmación de cada módulo se inicia inmediatamente después de completar la fase de operación. Con la opción de confirmación automática desactivada, no se realiza ninguna confirmación hasta que se ejecutan las operaciones para todos los módulos (este es el modo predeterminado).

Para obtener más información sobre las transacciones, consulte [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Número máximo de ciclos

La configuración de más ciclos puede resultar útil cuando desea evitar la interrupción de la conexión a un servicio de terceros y garantizar que todos los registros se procesen dentro de la ejecución de un escenario.

* Si el escenario comienza con un déclencheur de sondeo, la configuración define el número máximo de ciclos permitidos durante la ejecución del escenario.

   Para obtener más información sobre los déclencheur de sondeo, consulte [Déclencheur de sondeo](../../workfront-fusion/modules/module-types.md#polling) en [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Si el escenario comienza con un déclencheur instantáneo, el ajuste se ignora y todos los eventos pendientes se procesan durante una sola ejecución del escenario, un evento por ciclo.

   Para obtener más información sobre los déclencheur instantáneos, consulte [Déclencheur instantáneos](../../workfront-fusion/modules/module-types.md#instant) en [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Si el escenario no comienza con un déclencheur (instantáneo/sondeo), siempre se realiza el número máximo especificado de ciclos.

>[!INFO]
>
>**Ejemplos:**  [!DNL Workfront] > [!UICONTROL Registro de Watch] observa los nuevos problemas que surgen y [!DNL Workfront] >[!UICONTROL Convertir objeto] convierte la nueva solicitud en un proyecto y la asigna a la plantilla adecuada.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL más ciclos] solo se aplica cuando se programa la ejecución del escenario. Al usar la variable [!UICONTROL Ejecutar una vez] , se tiene en cuenta la configuración del ciclo.
>
>### El número máximo de ciclos se establece en 1 (predeterminado)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>La variable [!UICONTROL Número máximo de archivos devueltos] en el [!UICONTROL Dropbox] >[!UICONTROL Archivos de Watch] módulo está configurado en `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Si se envían 100 solicitudes a [!DNL Workfront]y [!UICONTROL Límite] se establece en 10 y, después de ejecutar un escenario, se dejan sin procesar 90 archivos. Los siguientes 10 archivos se procesan en la siguiente ejecución del escenario programado.
>
>### El número máximo de ciclos se establece en 10
>
>La variable [!UICONTROL Número máximo de archivos devueltos] en el [!UICONTROL Dropbox] >[!UICONTROL Archivos de Watch] módulo está configurado en `10`.
>
>Si se añaden 100 archivos a la carpeta del Dropbox y a la [!UICONTROL Número máximo de archivos devueltos] se establece en 10, luego se procesan 10 archivos durante el primer ciclo, los siguientes 10 archivos en el segundo ciclo, los siguientes 10 archivos en el tercer ciclo y así sucesivamente, hasta que se procesen todos los archivos.
>
>Todos los archivos se procesan dentro de un escenario ejecutado.
>
>Puede ver los ciclos ya ejecutados en los detalles del escenario:
>
>![](assets/scenario-detail-350x207.png)
>
>Para obtener más información sobre esta página, consulte [Detalles del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Número de errores consecutivos

Define el número máximo de intentos de ejecución consecutivos antes de desactivar la ejecución de un escenario (excluyendo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] y [!UICONTROL ConnectionError]).

Para obtener más información sobre los errores, consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Si un escenario comienza con un déclencheur instantáneo, el ajuste se ignora y el escenario se desactiva inmediatamente una vez que se ha producido el primer error.
