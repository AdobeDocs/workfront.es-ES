---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Control de errores de lanzamiento en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 82%

---

# Control de errores de lanzamiento en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Configurar la solución de error `throw`](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En algunos casos, es posible que desee detener forzosamente la ejecución del escenario seguida de la fase [Reversión](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) o [Compromiso](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit), o bien detener el procesamiento de una ruta y, opcionalmente, almacenarla en la cola de ejecuciones incompletas.

Actualmente, las directivas de control de errores no se pueden usar fuera del ámbito de una [ruta del controlador de errores](../../workfront-fusion/errors/error-handling.md#error) y [!DNL Adobe Workfront Fusion] no ofrece un módulo que permita generar (lanzar) errores de forma fácil y condicional.

Para obtener información sobre las ejecuciones incompletas, consulte [Ver y resolver ejecuciones incompletas en Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obtener información sobre las directivas de control de errores, consulte [Directivas para el control de errores en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Para obtener información sobre licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solución alternativa al lanzamiento

Para lanzar un error de forma condicional, puede configurar un módulo con el fin de que, opcionalmente, falle de forma intencionada durante su funcionamiento. Una posibilidad es emplear el módulo [!UICONTROL JSON] > [!UICONTROL Analizar JSON] (consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurado para lanzar opcionalmente un error (BundleValidationError, en este caso):

A continuación, puede adjuntar una de las directivas de control de errores a la ruta de control de errores para lo siguiente:

* Forzar la ejecución del escenario para que se detenga y realice la fase de reversión: [!UICONTROL reversión]
* Forzar la ejecución del escenario para que se detenga y realice la fase de confirmación: [!UICONTROL Compromiso]
* Detener el procesamiento de una ruta: [!UICONTROL Ignorar]
* Detener el procesamiento de una ruta y almacenarla en la cola de la carpeta de ejecuciones incompletas: [!UICONTROL Salto]

El ejemplo siguiente muestra el uso de la directiva [!DNL Rollback]:

![](assets/rollback-directive-350x175.png)
