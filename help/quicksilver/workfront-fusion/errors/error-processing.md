---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Error al procesar en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 94%

---

# Error al procesar en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Tipos de error](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/error-processing.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

A veces, se puede producir un error durante la ejecución de un escenario. Esto suele ocurrir si un servicio no está disponible debido a un error al conectarse a un servicio o si falla una validación. En este artículo se analizan los errores comunes que pueden producirse.

[!DNL Adobe Workfront Fusion] distingue entre varios tipos de error básicos. Reaccionará de forma diferente en función del tipo de error que se haya producido.

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Error de conexión

`ConnectionError`

El error de conexión es uno de los errores más comunes que suelen deberse a la falta de disponibilidad del servicio de terceros por varios motivos (sobrecarga, mantenimiento, interrupción, etc.). La gestión predeterminada de este error depende del módulo en el que se encuentre:

* Si el error se produce en el primer módulo, la ejecución del escenario finaliza con un mensaje de advertencia. [!DNL Workfront Fusion] intenta reiteradamente volver a ejecutar el escenario en intervalos de tiempo crecientes (se explican a continuación). Si todos los intentos fallan, [!DNL Workfront Fusion] desactiva el escenario.
* Si el error de conexión se produce en otro módulo distinto del primero, los pasos siguientes dependen de la opción [Permitir almacenar ejecuciones incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) en la configuración avanzada del escenario:

   * Si esta opción está activada, la ejecución del escenario se mueve a la carpeta [!UICONTROL Ejecuciones incompletas], donde [!DNL Workfront Fusion] intenta repetidamente volver a ejecutar el escenario en intervalos de tiempo cada vez mayores. Si todos los intentos fallan, la ejecución permanecerá en la carpeta de ejecuciones incompletas a la espera de la resolución manual por parte del usuario.

     Para obtener más información sobre las ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Si esta opción está desactivada, la ejecución del escenario finaliza con un error seguido de una fase de reversión. [!DNL Workfront Fusion] intenta reiteradamente volver a ejecutar el escenario a intervalos de tiempo cada vez mayores. Si todos los intentos fallan, [!DNL Workfront Fusion] desactiva el escenario.

### Incremento de los intervalos de tiempo

El algoritmo de incrementar multiplicativamente los intervalos de tiempo entre intentos cuando se produce un error se conoce como retroceso exponencial. Los intervalos de tiempo crecientes se establecen de la siguiente manera:

1. 10 minutos
1. 1 hora
1. 3 horas
1. 12 horas
1. 24 horas

La razón principal para utilizar los intervalos de tiempo cada vez mayores en [!DNL Workfront Fusion] es evitar que los escenarios que se ejecutan con frecuencia consuman operaciones en intentos reiteradamente fallidos.

>[!INFO]
>
>**Ejemplo**
>
>Un escenario contiene el [!DNL Google Sheets] activador [!UICONTROL Watch Rows]. [!DNL Google Sheets] no está disponible durante 30 minutos debido a tareas de mantenimiento cuando [!DNL Workfront Fusion] inicia el escenario, por lo que no puede recuperar nuevas filas. El escenario se detiene y vuelve a intentarlo en 10 minutos. Debido a que [!DNL Google Sheets] sigue sin estar disponible, [!DNL Workfront Fusion] sigue sin poder obtener información sobre las filas nuevas. La siguiente ejecución del escenario está programada en 1 hora. [!DNL Google Sheets] vuelve a estar disponible en este momento y el escenario se ejecuta correctamente.

## Error de datos

`DataError`

Se genera un error de datos cuando un elemento está asignado incorrectamente y no pasa la validación realizada en el lado [!DNL Workfront Fusion] o en el lado del servicio de terceros que se está utilizando.

Si se produce este error, el escenario, hasta donde falló el módulo, se mueve a la carpeta de ejecuciones incompletas, donde puede solucionar el problema. Sin embargo, el escenario no se detiene y continúa ejecutándose según su programación. Para detener la ejecución del escenario cuando aparezca el error Datos, active la opción Procesamiento secuencial en el panel Configuración de escenario.

Si no ha habilitado la opción [!UICONTROL Allow storing incomplete executions] en la configuración del escenario, la ejecución del escenario finaliza con el error y se realiza una reversión.

Para obtener más información sobre la asignación, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Para obtener información sobre las ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obtener información sobre el panel de configuración de escenario, consulte [El panel Ajustes de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Error de duplicación de datos

`DuplicateDataError`

Si [!DNL Workfront Fusion] intenta insertar el mismo paquete dos veces en un servicio que no permite datos duplicados, se generará un error de datos duplicados. Si se produce este error, [!DNL Workfront Fusion] procede del mismo modo que para el error de datos.

## Error de token de acceso no válido

`InvalidAccessTokenError`

Se produce un error de token de acceso no válido cuando [!DNL Workfront Fusion] no puede obtener acceso a su cuenta registrada con un servicio de terceros. Esto suele ocurrir cuando se revocan los derechos de acceso de [!DNL Workfront Fusion] en la administración de un servicio determinado, pero los escenarios relacionados siguen ejecutándose según la programación.

Si se produce este error, la ejecución de un escenario se detiene inmediatamente. El resto del escenario que comienza desde el módulo donde se produjo el error se mueve a la carpeta de ejecuciones incompletas.

Para obtener información acerca de las ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Error de límite de velocidad

`RateLimitError`

Si se supera un límite establecido por un servicio determinado, se genera un error de límite de velocidad. Si se produce este error, [!DNL Workfront Fusion] procede del mismo modo que para el error de conexión.

Para obtener más información, consulte [Error de conexión](#connection-error).

## Error de datos incompletos

`IncompleteDataError`

Un error de datos incompleto solo se produce con los activadores. Este error se genera si un activador no puede descargar los datos necesarios de un servicio determinado.

Si un escenario termina con `IncompleteDataError`, su comportamiento posterior dependerá de su configuración de [!UICONTROL Max number of consecutive errors]

Para obtener más información, consulte [Número de errores consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) en el artículo [El panel Ajustes del escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Ejemplo**
>
>Un escenario tiene el activador [!DNL Workfront] [!UICONTROL Watch Record] configurado para inspeccionar documentos. El escenario se ejecutará mientras se carga un documento grande, como un vídeo largo. Dado que [!UICONTROL Workfront Fusion] intenta descargar el vídeo mientras se sigue cargando en Workfront, el escenario termina con `IncompleteDataError`.

## Error de tiempo de ejecución

`RuntimeError`

Si aparece algún otro error (no mencionado anteriormente) durante la ejecución del escenario, se comunica como un `RunTimeError`.

Si un escenario termina con `RuntimeError`, su comportamiento posterior dependerá de su configuración de [!UICONTROL Max number of consecutive errors]. Para obtener más información, consulte [Número de errores consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) en el artículo [El panel Ajustes de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Si un escenario comienza con un activador instantáneo, se ignora la configuración de [!UICONTROL Max number of consecutive errors] y el escenario se desactiva inmediatamente una vez que se ha producido el primer error. Para obtener más información, consulte [Activadores instantáneos](../../workfront-fusion/modules/module-types.md#instant) en el artículo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Error de incoherencia

`InconsistencyError`

Si algún error descrito anteriormente se produce durante la fase de confirmación o reversión, un escenario finalizará con un error de incoherencia. Para obtener más información, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si este error aparece en un escenario, la ejecución del escenario se detiene inmediatamente.

## Advertencia

Al ejecutar un escenario, es posible que reciba una advertencia que le informe sobre un problema. Sin embargo, esto no impide que el escenario se complete correctamente.

Por ejemplo, puede aparecer una advertencia cuando se exceda el tamaño máximo de archivo permitido y la opción [!UICONTROL Habilitar pérdida de datos] esté deshabilitada. Para obtener más información, consulte [Habilitar la pérdida de datos](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) en el artículo [El panel de configuración de escenarios en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
