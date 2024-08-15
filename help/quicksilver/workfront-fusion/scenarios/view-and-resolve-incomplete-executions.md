---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ver y resolver ejecuciones incompletas en  [!DNL Adobe Workfront Fusion]
description: La carpeta [!UICONTROL Ejecuciones incompletas] almacena ejecuciones de escenarios que no se finalizaron correctamente debido a un error. Cada ejecución incompleta almacenada se puede resolver manualmente o automáticamente.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 53582d36ef2256f6073705ce3eabe8cd61c9b2cc
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 5%

---

# Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]

La carpeta [!UICONTROL Ejecuciones incompletas] almacena ejecuciones de escenarios que no se finalizaron correctamente debido a un error. Cada ejecución incompleta almacenada se puede resolver manualmente o automáticamente.

>[!NOTE]
>
>De forma predeterminada, el almacenamiento de ejecuciones incompletas está deshabilitado. Para habilitarlo, habilite la opción [!UICONTROL Permitir el almacenamiento de ejecuciones incompletas] en la configuración avanzada del escenario.
>
>Para obtener más información acerca de la configuración de escenarios, vea [El panel de configuración de escenarios en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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

## Ver ejecuciones incompletas

Si un módulo encuentra un error durante su operación, se agrega una nueva ejecución incompleta a la carpeta Ejecuciones incompletas. Cada ejecución incompleta contiene el modelo del escenario y todos los paquetes que se pueden asignar al módulo fallido. Para abrir la lista de ejecuciones incompletas, haga clic en la ficha [!UICONTROL Ejecuciones incompletas] de la página de detalles del escenario.

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

Para obtener más información, consulte [Errores que resultan en ejecuciones incompletas](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>El límite de tamaño actual de la carpeta de ejecuciones incompletas sin resolver por organización es de 500 MB. Si su organización supera este límite, es posible que vea el siguiente error:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Para obtener más información, consulte [Habilitar la pérdida de datos](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) en [El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Resolver ejecuciones incompletas

Cuando se almacena una nueva ejecución incompleta, puede resolverla de la siguiente manera:

1. Haga clic en la ficha **[!UICONTROL Ejecuciones incompletas]**.
1. Busque la ejecución incompleta que desea resolver y haga clic en **[!UICONTROL Detalle]**.


   Si desea ver el registro de todas las operaciones del módulo antes de intentar resolver la ejecución incompleta, puede resolver la ejecución incompleta desde la carpeta [!UICONTROL History]:

1. Haga clic en la ficha **[!UICONTROL Historial]**.
1. Busque el registro de ejecución con errores del escenario y haga clic en **[!UICONTROL Detalles]**.
1. Abra el registro del módulo donde se muestran todas las operaciones del módulo.
1. Busque la operación con error y haga clic en **[!UICONTROL Resolver]**:

   ![](assets/resolve-btn-350x188.png)

## Opciones relacionadas con ejecuciones incompletas

Las siguientes opciones del panel [!UICONTROL Configuración de escenarios] determinan si se almacenan las ejecuciones incompletas y cómo se almacenan:

* Permitir almacenar ejecuciones incompletas
* Procesamiento secuencial
* Habilitar la pérdida de datos

Para obtener más información acerca de estas opciones, vea [El panel de configuración del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Errores que resultan en ejecuciones incompletas

Existen varias categorías de errores que resultan en el almacenamiento de ejecuciones incompletas. Estos pueden incluir:

* Errores de validación derivados de datos incompletos o erróneos, principalmente debido a la falta de un elemento que se espera para procesar correctamente todos los datos que pasan a través de un módulo.
* Errores que se producen por la no disponibilidad del destino final debido a un error de conexión temporal o a largo plazo (por ejemplo, durante la conexión al correo electrónico o al servidor FTP remoto).

Si se produce un error en el primer módulo del escenario, la ejecución se detiene inmediatamente y no se almacena ninguna ejecución incompleta.

Si se produce un error en cualquier otro módulo y no hay ninguna ruta de tratamiento de errores asociada, se producirá una de las siguientes situaciones:

* Si el tipo de error es `ConnectionError`, `RateLimitError`, `OutOfSpaceError` o `ModuleTimeoutError`, se almacena un registro de ejecución incompleto con reintento automático.
* Si el tipo de error es `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError` o `MaxResultsExceededError`, se almacenará un registro de ejecución incompleto sin reintento automático.
* Si el tipo de error es cualquier cosa que no sea lo anterior, la ejecución falla.
