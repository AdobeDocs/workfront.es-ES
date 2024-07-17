---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Directivas para la administración de errores en  [!DNL Adobe Workfront Fusion]
description: Este artículo describe las directivas que puede usar para la administración de errores en sus  [!DNL Adobe Workfront Fusion] escenarios.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 12%

---

# Directivas para la administración de errores en [!DNL Adobe Workfront Fusion]

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

## Directivas para la gestión de errores

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Reversión</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>La ejecución del escenario se detiene inmediatamente y se inicia una fase de <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Rollback</a> en todos los módulos en un intento de revertirlos a su estado inicial. Los módulos siguientes no se procesan.</p> <p>Salvo algunos tipos de error, el escenario se desactiva después del número de errores consecutivos especificados en Configuración de escenario. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Número de errores consecutivos</a>.</p> <p>El estado de ejecución del escenario está marcado como “error”.</p> <p>Nota: Este es el comportamiento predeterminado si no hay ninguna ruta de controlador de error adjunta al módulo y la opción <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Permitir el almacenamiento de ejecuciones incompletas]</a> en [!UICONTROL Configuración de escenario] no está activada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Confirmar</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>La ejecución del escenario se detiene inmediatamente y se inicia una fase de confirmación en todos los módulos. Los módulos siguientes no se procesan.</p> <p>Se ignorarán todos los paquetes sin procesar.</p> <p>El estado de ejecución del escenario se marca como "correcto". Para obtener información sobre las fases de confirmación, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Confirmación</a> en el artículo <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Ejecución de escenarios, ciclos y fases en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reanudar</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Se especifica una salida sustitutiva que se suministra al módulo que encuentra un error.</p> <p>Se procesan los módulos siguientes.</p> <p>El estado de ejecución del escenario se marca como “éxito”.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorar</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>El error se ignora y los módulos posteriores no se procesan.</p> <p>Si hay paquetes sin procesar, la ejecución del escenario continúa normalmente.</p> <p>El estado de ejecución del escenario se marca como “éxito”.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Salto</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>El estado de la ejecución del escenario se almacena en la cola de ejecuciones incompletas, donde el error se puede resolver manualmente. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion</a>. </p> <p>Sin embargo, hay algunas excepciones. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Permitir el almacenamiento de ejecuciones incompletas</a> en el artículo <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">El panel de configuración de escenarios en Adobe Workfront Fusion</a>.</p> <p>Los módulos siguientes no se procesan.</p> <p>Si hay paquetes sin procesar, la ejecución del escenario continúa normalmente.</p> <p>El estado de ejecución del escenario se marca como "advertencia" cuando la opción [!UICONTROL Automatic complete execution] está deshabilitada.</p> <p>Consulte la sección <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> más abajo para obtener más información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reintentar</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>En algunos casos, podría resultar útil volver a ejecutar un módulo fallido un par de veces cuando existe la posibilidad de que el motivo del error pueda pasar con el tiempo.</p> <p>Actualmente, Workfront Fusion no ofrece la directiva de reintento, aunque se pueden emplear varias soluciones para imitar su funcionalidad. Para obtener más información, consulte <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Reintentar la gestión de errores en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Actualmente, las directivas de gestión de errores no se pueden usar fuera de una ruta de gestión de errores.
>
>   Para obtener más información, consulte [Ruta del controlador de error](../../workfront-fusion/errors/error-handling.md#error) en el artículo [Control de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] actualmente no ofrece un módulo de lanzamiento que le permita generar errores (lanzamiento) de forma fácil y condicional, aunque se puede emplear una solución para imitar su funcionalidad.
>
>   Para obtener más información, consulte [Solución alternativa para el lanzamiento](../../workfront-fusion/errors/throw.md#workaround-for-throw) en el artículo [Control de errores de lanzamiento en Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Salto {#break}

Cuando la directiva [!DNL Break] gestiona un error, se crea un registro en la carpeta de ejecuciones incompletas. Este registro almacena el estado de la ejecución del escenario, junto con los datos de los módulos anteriores. El registro hace referencia al módulo en el que se originó el error y contiene información sobre qué datos recibió el módulo como entrada. Para cada paquete de datos que causa el error, se crea un registro independiente.

Para obtener más información, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Resolver errores resultantes de la directiva Break

Puede resolver el error manualmente actualizando el escenario (si es necesario) y ejecutándolo una vez.

También puede configurar el escenario para que procese automáticamente una ejecución incompleta volviendo a ejecutarlo. Para configurar el módulo para que procese ejecuciones incompletas:

1. Dentro del módulo Interrumpir, habilite la opción [!UICONTROL **Finalizar ejecución automáticamente**].
1. En el campo **Número de intentos**, indique o asigne el número máximo de intentos que desea que el módulo reintente la ejecución

   Este número debe estar entre 1 y 100.
1. En el campo **Intervalo entre intentos**, escriba o asigne el número de minutos entre cada intento de reintento.

Con esta opción habilitada, cuando se produce un error, la ejecución incompleta se recupera (después del tiempo especificado en el campo [!UICONTROL Intervalo entre intentos]) y se ejecuta con los datos de entrada originales. Esto se repetirá hasta que la ejecución del módulo se complete sin error o hasta que se alcance el Número de intentos especificado.

>[!NOTE]
>
>Si falla el intento de reintento inicial, el intervalo entre reintentos aumenta exponencialmente en cada intento.


Cuando se activa &quot;Ejecución completa automática&quot;, la ejecución del escenario se marca como &quot;Correcta&quot; porque el reintento automático del controlador de error de interrupción gestiona el problema automáticamente. En este caso, los usuarios no reciben un correo electrónico sobre la ejecución fallida.

Cuando la opción &quot;Ejecución completa automáticamente&quot; está desactivada, la ejecución se marca como &quot;Advertencia&quot;.

Hay algunas excepciones a que las ejecuciones se almacenen en Ejecuciones incompletas y, con algunos tipos de error, no es posible reintentar automáticamente la ejecución de un escenario.

Para obtener más información, consulte [Permitir el almacenamiento de ejecuciones incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) en el artículo [El panel de configuración de escenarios en Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obtener más información, consulte [Gestión avanzada de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
