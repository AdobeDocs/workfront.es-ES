---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Error de procesamiento en [!DNL Adobe Workfront Fusion]
description: A veces se puede producir un error durante la ejecución de un escenario. Esto suele ocurrir si un servicio no está disponible debido a un error en la conexión a un servicio o si falla una validación. Este artículo analiza los errores comunes que puede encontrar.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# Error de procesamiento en [!DNL Adobe Workfront Fusion]

A veces se puede producir un error durante la ejecución de un escenario. Esto suele ocurrir si un servicio no está disponible debido a un error en la conexión a un servicio o si falla una validación. Este artículo analiza los errores comunes que puede encontrar.

[!DNL Adobe Workfront Fusion] distingue entre varios tipos de error básicos. Reaccionará de forma diferente según el tipo de error que se haya producido.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Error de conexión

`ConnectionError`

El error de conexión es uno de los errores más comunes causados por la falta de disponibilidad del servicio de terceros por varios motivos (sobrecarga, mantenimiento, interrupción, etc.). La gestión predeterminada de este error depende del módulo en el que se ha encontrado:

* Si el error se produce en el primer módulo, la ejecución del escenario finaliza con un mensaje de advertencia. [!DNL Workfront Fusion] a continuación, intenta volver a ejecutar el escenario en intervalos de tiempo crecientes (estos se explican a continuación). Si todos los intentos fallan, [!DNL Workfront Fusion] desactiva el escenario.
* Si el error de conexión se produce en otro módulo que no sea el primero, los pasos siguientes dependen de la variable [Permitir el almacenamiento de ejecuciones incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) en la configuración avanzada del escenario:

   * Si esta opción está habilitada, la ejecución del escenario se mueve a la variable [!UICONTROL Ejecuciones incompletas] carpeta donde [!DNL Workfront Fusion] intenta volver a ejecutar el escenario repetidamente a intervalos de tiempo crecientes. Si todos los intentos fallan, la ejecución permanecerá en la variable [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) en espera de la resolución manual del usuario.
   * Si la opción está desactivada, la ejecución del escenario termina con un error seguido de una fase de reversión. [!DNL Workfront Fusion] a continuación, intenta volver a ejecutar el escenario en intervalos de tiempo crecientes. Si todos los intentos fallan, [!DNL Workfront Fusion] desactiva el escenario.

### Aumento de intervalos de tiempo

El algoritmo de intervalos de tiempo multiplicativamente crecientes entre los intentos cuando se produce un error se conoce como retroceso exponencial. Los intervalos de tiempo crecientes se establecen de la siguiente manera:

1. 10 minutos
1. 1 hora
1. 3 horas
1. 12 horas
1. 24 horas

La razón principal para utilizar los intervalos de tiempo crecientes en [!DNL Workfront Fusion] es evitar que los escenarios ejecutados con frecuencia consuman operaciones en intentos fallidos repetidos.

>[!INFO]
>
>**Ejemplo:**
>
>Un escenario contiene el [!DNL Google Sheets] déclencheur [!UICONTROL Filas de observación]. [!DNL Google Sheets] no está disponible durante 30 minutos debido al mantenimiento cuando [!DNL Workfront Fusion] inicia el escenario, por lo que no puede recuperar filas nuevas. El escenario se detiene y vuelve a intentarlo en 10 minutos. Como el servicio sigue no disponible en este periodo de tiempo, [!DNL Workfront Fusion] sigue sin poder obtener información sobre filas nuevas. La siguiente ejecución del escenario está programada en 1 hora. [!DNL Google Sheets] está disponible de nuevo en este plazo y el escenario se ejecuta correctamente.

## Error de datos

`DataError`

Se genera un error de datos cuando un elemento está asignado incorrectamente y no pasa la validación realizada en la variable [!DNL Workfront Fusion] o del lado del servicio de terceros que se está utilizando. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Si se produce este error, el escenario, hasta donde se produjo un error en el módulo, se mueve a la carpeta de ejecuciones incompletas, donde puede solucionar el problema. Sin embargo, el escenario no se detiene y continúa ejecutándose según su programación. Para detener la ejecución del escenario cuando aparece el error de datos, active la opción de procesamiento secuencial en el panel de configuración del escenario.

Si no ha habilitado la variable [!UICONTROL Permitir el almacenamiento de ejecuciones incompletas] en la configuración del escenario, la ejecución del escenario termina con el error y se realiza una reversión.

Para obtener información sobre ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obtener información sobre el panel de configuración de escenarios, consulte [El panel de configuración de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Duplicar error de datos

`DuplicateDataError`

If [!DNL Workfront Fusion] intenta insertar el mismo paquete dos veces en un servicio que no permite datos duplicados; se genera un error de datos duplicado. Si se produce este error, [!DNL Workfront Fusion] funciona del mismo modo que para el error de datos.

## Error de token de acceso no válido

`InvalidAccessTokenError`

Se produce un error de token de acceso no válido cuando [!DNL Workfront Fusion] no puede acceder a su cuenta registrada con un servicio de terceros. Esto ocurre principalmente cuando se revocan los derechos de acceso para [!DNL Workfront Fusion] en la administración de un servicio determinado pero los escenarios relacionados siguen funcionando según lo programado.

Si se produce este error, la ejecución de un escenario se detiene inmediatamente. El resto del escenario que comienza desde el módulo en el que se produjo el error se mueve a la carpeta de ejecuciones incompletas.

Para obtener información sobre ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Error de límite de tasa

`RateLimitError`

Si se supera un límite establecido por un servicio determinado, se genera un error de límite de velocidad. Si se produce este error, [!DNL Workfront Fusion] funciona del mismo modo que para el error de conexión. Para obtener más información, consulte [Error de conexión](#connection-error).

## Error de datos incompletos

`IncompleteDataError`

Un error de datos incompleto solo se produce con déclencheur. Este error se genera si un déclencheur no descarga los datos necesarios de un servicio determinado.

Si un escenario termina con la variable `IncompleteDataError`, su comportamiento futuro dependerá de su configuración de [!UICONTROL Número máximo de errores consecutivos]. Para obtener más información, consulte [Número de errores consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) en el artículo [El panel de configuración de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Ejemplo:** Un escenario tiene la variable [!DNL Workfront] déclencheur [!UICONTROL Registro de Watch] configurado para buscar documentos. El escenario se ejecuta mientras se carga un documento grande, como un vídeo largo. Porque [!UICONTROL Workfront Fusion] intenta descargar el vídeo mientras todavía se está cargando en Workfront, el escenario termina con el `IncompleteDataError`.

## Error de tiempo de ejecución

`RuntimeError`

Si aparece cualquier otro error (no mencionado anteriormente) durante la ejecución del escenario, se comunica como un `RunTimeError`.

Si un escenario termina con la variable `RuntimeError`, su comportamiento futuro dependerá de su configuración de [!UICONTROL Número máximo de errores consecutivos]. Para obtener más información, consulte [Número de errores consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) en el artículo [El panel de configuración de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Si un escenario comienza con un déclencheur instantáneo, la configuración de [!UICONTROL Número máximo de errores consecutivos] se ignora y el escenario se desactiva inmediatamente una vez que se ha producido el primer error. Para obtener más información, consulte [Déclencheur instantáneos](../../workfront-fusion/modules/module-types.md#instant) en el artículo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Error de incoherencia

`InconsistencyError`

Si se produce cualquier error descrito anteriormente durante la fase de confirmación o reversión, el escenario terminará con Error de incoherencia. Para obtener más información, consulte [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si este error aparece en un escenario, la ejecución del escenario se detiene inmediatamente.

## Advertencia

Mientras ejecuta un escenario, puede recibir una advertencia que le informe de un problema. Sin embargo, no impide que el escenario se complete correctamente.

Por ejemplo, puede aparecer una advertencia cuando se supere el tamaño máximo permitido del archivo y la variable [!UICONTROL Habilitar la pérdida de datos] está desactivada. Para obtener más información, consulte [Habilitar la pérdida de datos](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) en el artículo [El panel de configuración de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
