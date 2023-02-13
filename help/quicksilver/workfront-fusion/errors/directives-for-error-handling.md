---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]
description: Este artículo describe las directivas que puede utilizar para la gestión de errores en su [!DNL Adobe Workfront Fusion] escenarios.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 50b43cd4bafdfc3379eb1d73c12e15c791e28dbe
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Directivas para la gestión de errores

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Reversión</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>La ejecución del escenario se detiene inmediatamente y <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Reversión</a> se inicia en todos los módulos en un intento de revertirlos a su estado inicial. Los módulos siguientes no se procesan.</p> <p>A excepción de algunos tipos de error, el escenario se desactiva después del número de errores consecutivos especificados en Configuración del escenario. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Número de errores consecutivos</a>.</p> <p>El estado de ejecución del escenario está marcado como "error".</p> <p>Nota: Este es el comportamiento predeterminado si no se adjunta ninguna ruta de controlador de error al módulo y al <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Permitir almacenar ejecuciones incompletas]</a> la configuración en [!UICONTROL Scenario settings] no está marcada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Confirmar</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>La ejecución del escenario se detiene inmediatamente y se inicia una fase de confirmación en todos los módulos. Los módulos siguientes no se procesan.</p> <p>Todos los paquetes sin procesar se ignoran.</p> <p>El estado de ejecución del escenario se marca como "success". Para obtener información sobre las fases de confirmación, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Confirmar</a> en el artículo <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Ejecución de escenarios, ciclos y fases en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reanudar</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Se especifica una salida sustitutiva que se suministra al módulo que encuentra un error.</p> <p>Se procesan los módulos siguientes.</p> <p>El estado de ejecución del escenario se marca como "success".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorar</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>El error se ignora y los módulos posteriores no se procesan.</p> <p>Si hay paquetes sin procesar, la ejecución del escenario continúa normalmente.</p> <p>El estado de ejecución del escenario se marca como "success".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Salto</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>El estado de la ejecución del escenario se almacena en la cola de ejecuciones incompletas, donde el error se puede resolver manualmente. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion</a>. </p> <p>Sin embargo, hay algunas excepciones. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Permitir el almacenamiento de ejecuciones incompletas</a> en el artículo <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">El panel de configuración de escenario en Adobe Workfront Fusion</a>.</p> <p>Los módulos siguientes no se procesan.</p> <p>Si hay paquetes sin procesar, la ejecución del escenario continúa normalmente.</p> <p>El estado de ejecución del escenario se marca como "advertencia" cuando la opción [!UICONTROL Automatically complete execution] está desactivada.</p> <p>Consulte la <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> para obtener más información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reintentar</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>En algunos casos podría ser útil volver a ejecutar un módulo que falla durante un par de veces cuando hay una posibilidad de que el motivo del error pase con el tiempo.</p> <p>Actualmente, Workfront Fusion no ofrece la directiva Retry , aunque se pueden usar varias soluciones para imitar su funcionalidad. Para obtener más información, consulte <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Gestión de errores de reintento en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Actualmente, las directivas de gestión de errores no pueden utilizarse fuera del ámbito de una ruta de gestión de errores y [!DNL Workfront Fusion] actualmente no ofrece un módulo Throw que le permita generar (lanzar) errores fácilmente y condicionalmente, aunque se puede utilizar una solución para imitar su funcionalidad. Para obtener más información, consulte [Ruta del controlador de errores](../../workfront-fusion/errors/error-handling.md#error) en el artículo [Gestión de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md). Consulte también [Solución para el lanzamiento](../../workfront-fusion/errors/throw.md#workarou) en el artículo [Gestión de errores de emisión en Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Salto {#break}

Cuando el [!DNL Break] , se crea un registro en la variable [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) carpeta que almacena el estado de la ejecución del escenario junto con los datos de los módulos anteriores. Para cada paquete de datos que causa el error, se crea un registro independiente.

El registro hace referencia al módulo en el que se originó el error y contiene información sobre qué datos recibió el módulo como entrada. Para obtener más información, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

En este caso, puede resolver el error manualmente actualizando el escenario (si es necesario) y ejecutándolo una vez.

Por otro lado, al habilitar la variable [!UICONTROL Finalización de la ejecución automática] en la configuración de directiva Break , se puede configurar para procesar automáticamente una ejecución incompleta ejecutando de nuevo el escenario después del número especificado de minutos.

Con esta opción habilitada, cuando se produce un error, se recupera la ejecución incompleta (después del tiempo especificado en la variable [!UICONTROL Intervalo entre intentos] ) y se ejecuta con los datos de entrada originales. Esto se repetirá hasta que la ejecución del módulo se complete sin error o hasta que se alcance el número de intentos especificado.

>[!NOTE]
>
>Si falla el intento de reintento inicial, el intervalo entre reintentos aumenta exponencialmente cada otro intento.

Cuando se activa &quot;Completar ejecución automáticamente&quot;, la ejecución del escenario se marca como &quot;Correcto&quot; porque el reintento automático del controlador de error Break está gestionando el problema automáticamente. En este caso, los usuarios no reciben un correo electrónico sobre la ejecución fallida.

Cuando se desactiva &quot;Ejecutar automáticamente&quot;, la ejecución se marca como &quot;Advertencia&quot;.

![](assets/break-directive-350x241.png)

Sin embargo, hay algunas excepciones a que las ejecuciones se almacenen en Ejecuciones incompletas y, con algunos tipos de error, el reintento automático de una ejecución de escenario no es posible. Para obtener más información, consulte [Permitir el almacenamiento de ejecuciones incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) en el artículo [El panel de configuración de escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obtener más información, consulte [Gestión de errores avanzada en Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
