---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestión de errores de reintento en [!DNL Adobe Workfront Fusion]
description: En algunos casos, es útil volver a ejecutar un módulo que falla un par de veces si existe la posibilidad de que el motivo del error pase con el tiempo.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Gestión de errores de reintento en [!DNL Adobe Workfront Fusion]

En algunos casos, es útil volver a ejecutar un módulo fallido si existe la posibilidad de que el motivo del error pase con el tiempo.

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

## Soluciones a [!UICONTROL Reintentar] directiva de gestión de errores

[!UICONTROL Adobe Workfront Fusion] actualmente no ofrece el [!UICONTROL Reintentar] directiva de gestión de errores, aunque se pueden usar dos soluciones para imitar su funcionalidad. Para obtener más información, consulte [Directivas para la gestión de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utilice la variable [!UICONTROL Salto] directiva

1. En el panel de configuración de escenario, habilite la variable **[!UICONTROL Permitir el almacenamiento de ejecuciones incompletas]** .

   Para obtener más información, consulte [El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Adjunte una ruta de controlador de errores al módulo, tal como se describe en [Gestión de errores en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Vincule el [!UICONTROL Salto] a la ruta del controlador de errores y configúrela.

   Para obtener más información, consulte [Directivas para la gestión de errores en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Inconvenientes

* El intervalo mínimo de reintentos es de un minuto.
* Si el módulo está procesando varios paquetes y falla el procesamiento de un paquete, la ejecución parcial (solo el paquete que causó el error) se mueve a la carpeta de ejecuciones incompletas y está programada para reintentos según la variable [!UICONTROL Salto] configuración de directiva. Sin embargo, la ejecución actual continúa y el módulo continúa procesando los paquetes posteriores. Puede habilitar el &quot;[!UICONTROL Procesamiento secuencial]&quot; en la [!UICONTROL Configuración del escenario] para evitar que el escenario se ejecute de nuevo hasta que la ejecución almacenada en la carpeta de ejecuciones incompletas se haya resuelto correctamente.

Para obtener más información sobre las ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utilice la variable [!UICONTROL Repetidor] módulo

1. Emplee el **[!UICONTROL Repetidor]** y establezca su [!UICONTROL Repetidas] al número máximo de intentos.
1. Vincule el módulo que potencialmente falla al **[!UICONTROL Repetidor]** módulo.
1. Adjuntar una ruta del controlador de errores a este módulo (consulte [Gestión de errores en [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Vincule el **[!UICONTROL Herramientas] > [!UICONTROL Sueño]** a la ruta del controlador de errores y establezca su **[!UICONTROL Retraso]** al número de segundos entre los intentos.

1. Vincule el **[!UICONTROL Ignorar]** después de **[!UICONTROL Herramientas] > [!UICONTROL Sueño]** módulo (consulte [Directivas para la gestión de errores en Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Vincule el **[!UICONTROL Herramientas] > [!UICONTROL Establecer variable]** módulo después del módulo que potencialmente falla y configúrelo para almacenar el resultado del módulo en una variable denominada, por ejemplo, `Result`.

1. Vincule el **[!UICONTROL Agrupador de matrices]** después del **[!UICONTROL Herramientas] > [!UICONTROL Establecer variable]** y seleccione **[!DNL Repeater]** en su campo Módulo de origen.

1. Vincule el **[!UICONTROL Herramientas] > [!UICONTROL Obtener variable]** al **[!UICONTROL Agrupador de matrices]** y configúrelo para obtener el valor de la variable `Result` variable.

1. Inserte el **[!UICONTROL Herramientas] > [!UICONTROL Obtener variable]** entre **[!UICONTROL Repetidor]** y el módulo potencialmente defectuoso y configúrelo obtenga el valor de la variable `Result` variable.

1. Inserte un filtro entre **[!UICONTROL Herramientas] > [!UICONTROL Obtener variable]** y el módulo potencialmente defectuoso continuará solo si la variable `Result` no existe.

>[!INFO]
>
>**Ejemplo:** Este es un escenario de ejemplo en el que la variable [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] representa el módulo potencialmente defectuoso:
>
>![](assets/http-make-request-350x116.png)
>
>Si el resultado del módulo potencialmente defectuoso es demasiado complejo para almacenarlo en una variable simple, puede emplear un almacén de datos para almacenar/recuperar el resultado. El almacén de datos solo contendría un registro. La clave del registro puede ser, por ejemplo, `Result`.
>
>Para obtener más información sobre los almacenes de datos, consulte [Almacenes de datos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Retorno

Esta solución puede parecer demasiado compleja y también es más exigente en términos de operaciones.
