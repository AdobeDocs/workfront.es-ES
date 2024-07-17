---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Reintentar la administración de errores en  [!DNL Adobe Workfront Fusion]
description: En algunos casos, es útil volver a ejecutar un módulo fallido un par de veces si existe la posibilidad de que el motivo del error pueda pasar con el tiempo.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Reintentar la administración de errores en [!DNL Adobe Workfront Fusion]

En algunos casos, es útil volver a ejecutar un módulo que falla si existe la posibilidad de que el motivo del error pueda pasar con el tiempo.

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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Soluciones a la directiva de gestión de errores [!UICONTROL Retry]

[!UICONTROL Adobe Workfront Fusion] no ofrece actualmente la directiva de gestión de errores [!UICONTROL Retry], aunque se pueden emplear dos soluciones para imitar su funcionalidad. Para obtener más información, consulte [Directivas para la gestión de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Usar la directiva [!UICONTROL Break]

1. En el panel de configuración de escenarios, habilite la opción **[!UICONTROL Permitir el almacenamiento de ejecuciones incompletas]**.

   Para obtener más información, consulte [El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Adjunte una ruta de controlador de error al módulo, tal como se describe en [Control de errores en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Vincule la directiva [!UICONTROL Break] a la ruta del controlador de error y configúrela.

   Para obtener más información, consulte [Directivas para la gestión de errores en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Inconvenientes

* El intervalo mínimo de reintento es de un minuto.
* Si el módulo procesa varios paquetes y falla el procesamiento de un paquete, la ejecución parcial (solo el paquete que provocó el error) se mueve a la carpeta de ejecuciones incompletas y se programa para reintentos según la configuración de la directiva [!UICONTROL Break]. Sin embargo, la ejecución actual continúa y el módulo continúa procesando los paquetes posteriores. Puede habilitar la opción &quot;[!UICONTROL Procesamiento secuencial]&quot; en [!UICONTROL Configuración de escenario] para evitar que el escenario se vuelva a ejecutar hasta que la ejecución almacenada en la carpeta Ejecuciones incompletas se haya resuelto correctamente.

  Para obtener más información sobre las ejecuciones incompletas, vea [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Usar el módulo [!UICONTROL Repeater]

1. Use el módulo **[!UICONTROL Repeater]** y establezca su campo **[!UICONTROL Repeticiones]** en el número máximo de intentos.
1. Vincule el módulo que podría dar error al módulo **[!UICONTROL Repeater]**.
1. Adjuntar una ruta de controlador de error a este módulo (consulte [Control de errores en [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Vincule el módulo **[!UICONTROL Tools] > [!UICONTROL Sleep]** a la ruta del controlador de errores y establezca su campo **[!UICONTROL Delay]** en el número de segundos entre los intentos.

1. Vincule la directiva **[!UICONTROL Ignore]** después del módulo **[!UICONTROL Tools] > [!UICONTROL Sleep]** (consulte [Directivas para la gestión de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Vincule el módulo **[!UICONTROL Tools] > [!UICONTROL Set variable]** después del módulo que podría dar error y configúrelo para almacenar el resultado del módulo en una variable denominada, por ejemplo, `Result`.

1. Vincule el módulo **[!UICONTROL Array aggregator]** después de **[!UICONTROL Tools] > [!UICONTROL Set variable]** y elija el módulo **[!DNL Repeater]** en el campo Source Module.

1. Vincule el módulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** al módulo **[!UICONTROL Array aggregator]** y configúrelo para obtener el valor de la variable `Result`.

1. Inserte el módulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** entre el módulo **[!UICONTROL Repeater]** y el módulo que podría fallar y configúrelo para obtener el valor de la variable `Result`.

1. Inserte un filtro entre este módulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** y el módulo que podría dar error para continuar solo si la variable `Result` no existe.

>[!INFO]
>
>**Ejemplo:** Este es un escenario de ejemplo en el que el módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] representa el módulo que podría fallar:
>
>![](assets/http-make-request-350x116.png)
>
>Si el resultado del módulo que puede dar error es demasiado complejo para almacenarlo en una variable simple, puede utilizar un almacén de datos para almacenar o recuperar el resultado. El almacén de datos contendría un solo registro. La clave del registro puede ser, por ejemplo, `Result`.
>
>Para obtener más información sobre los almacenes de datos, vea [Almacenes de datos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Inconveniente

Esta solución puede parecer un poco compleja y también más exigente en términos de operaciones.
