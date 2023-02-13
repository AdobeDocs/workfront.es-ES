---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestión de errores de emisión en Adobe Workfront Fusion
description: En algunos casos, es posible que desee detener la ejecución del escenario a la fuerza, seguida de la fase de reversión o confirmación, o detener el procesamiento de una ruta y, opcionalmente, almacenarla en la cola de Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Tratamiento de errores de lanzamiento en [!DNL Adobe Workfront Fusion]

En algunos casos, es posible que desee detener la ejecución del escenario a la fuerza, seguida de [Reversión](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) o [Confirmar](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) o para detener el procesamiento de una ruta y, opcionalmente, almacenarla en la cola de ejecuciones incompletas.

Actualmente, las directivas de gestión de errores no se pueden usar fuera del ámbito de un [Ruta del controlador de errores](../../workfront-fusion/errors/error-handling.md#error) y [!DNL Adobe Workfront Fusion] no ofrece un módulo que le permita generar (generar) errores de forma fácilmente condicional.

Para obtener información sobre ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obtener información sobre las directivas de gestión de errores, consulte [Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solución para el lanzamiento

Para generar un error condicionalmente, puede configurar un módulo para que falle de forma opcional durante su operación. Una posibilidad es emplear el [!UICONTROL JSON] > [!UICONTROL Analizar JSON] módulo (consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurado para generar opcionalmente un error (BundleValidationError en este caso):

A continuación, puede adjuntar una de las directivas de gestión de errores a la ruta de gestión de errores a:

* Forzar la ejecución del escenario para que se detenga y realice la fase de reversión: [!UICONTROL Reversión]
* Forzar la ejecución del escenario para que se detenga y realice la fase de confirmación: [!UICONTROL Confirmar]
* Detenga el procesamiento de una ruta: [!UICONTROL Ignorar]
* Detenga el procesamiento de una ruta y guárdela en la cola de la carpeta de ejecuciones incompletas: [!UICONTROL Salto]

El siguiente ejemplo muestra el uso de la variable [!DNL Rollback] directiva:

![](assets/rollback-directive-350x175.png)
