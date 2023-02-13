---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]
description: La variable [!UICONTROL Ejecuciones incompletas] carpeta almacena ejecuciones de escenario que no se completaron correctamente debido a un error. Cada ejecución incompleta almacenada se puede resolver de forma manual o automática.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]

La variable [!UICONTROL Ejecuciones incompletas] carpeta almacena ejecuciones de escenario que no se completaron correctamente debido a un error. Cada ejecución incompleta almacenada se puede resolver de forma manual o automática.

>[!NOTE]
>
>De forma predeterminada, el almacenamiento de ejecuciones incompletas está deshabilitado. Para habilitarlo, habilite la variable [!UICONTROL Permitir el almacenamiento de ejecuciones incompletas] en la configuración avanzada del escenario.
>
>Para obtener más información sobre la configuración de escenarios, consulte [El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## Ver ejecuciones incompletas

Si un módulo encuentra un error durante su operación, se agrega una nueva ejecución incompleta a la carpeta de ejecuciones incompletas. Cada ejecución incompleta contiene el modelo del escenario y todos los paquetes que se pueden asignar al módulo fallido. La lista de ejecuciones incompletas se puede abrir haciendo clic en el [!UICONTROL Ejecuciones incompletas] en la página de detalles del escenario:

![](assets/incomplete-executions-tab-350x102.png)

Para obtener más información, consulte [Errores que resultan en ejecuciones incompletas](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>El límite de tamaño actual de la carpeta de ejecuciones incompletas sin resolver por organización es de 500 MB. Si su organización supera este límite, es posible que vea el siguiente error:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Para obtener más información, consulte [Habilitar la pérdida de datos](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) en [El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Resolución de ejecuciones incompletas

Cuando se almacena una nueva ejecución incompleta, se puede resolver de la siguiente manera:

1. Haga clic en el **[!UICONTROL Ejecuciones incompletas]** pestaña .
1. Busque la ejecución incompleta que desee resolver y haga clic en **[!UICONTROL Detalle]**.


   Si desea ver el registro de todas las operaciones del módulo antes de intentar resolver la ejecución incompleta, puede resolver la ejecución incompleta desde la [!UICONTROL Historial] carpeta:

1. Haga clic en el **[!UICONTROL Historial]** pestaña .
1. Busque el registro de ejecución fallido del escenario y haga clic en **[!UICONTROL Detalles]**.
1. Abra el registro del módulo donde se muestran todas las operaciones del módulo.
1. Busque la operación fallida y haga clic en **[!UICONTROL Resolver]**:

   ![](assets/resolve-btn-350x188.png)

## Opciones relacionadas con ejecuciones incompletas

Las siguientes opciones de la sección [!UICONTROL Configuración del escenario] determine si se almacenan las ejecuciones incompletas y cómo se almacenan:

* Permitir el almacenamiento de ejecuciones incompletas
* Procesamiento secuencial
* Habilitar la pérdida de datos

Para obtener más información sobre estas opciones, consulte [El panel de configuración de escenario de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Errores que resultan en ejecuciones incompletas

Existen varias categorías de errores que resultan en el almacenamiento de ejecuciones incompletas. Entre ellas cabe mencionar:

* Errores de validación derivados de datos incompletos o erróneos, principalmente debido a la falta de un elemento que se espera para procesar correctamente todos los datos que pasan por un módulo.
* Errores que se producen cuando el destino final no está disponible debido a un error de conexión temporal o a largo plazo (por ejemplo, durante la conexión con un servidor FTP remoto o de correo electrónico).

Si se produce un error en el primer módulo del escenario, la ejecución se detiene inmediatamente y no se almacena ninguna ejecución incompleta.

Si se produce un error en cualquier otro módulo y no hay ninguna ruta de controlador de error adjunta, se produce una de las siguientes situaciones:

* Si el tipo de error es `ConnectionError`, `RateLimitError`, `OutOfSpaceError` o `ModuleTimeoutError`, se almacena un registro de ejecución incompleto con reintento automático.
* Si el tipo de error es `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`o `MaxResultsExceededError`, se almacena un registro de ejecución incompleto sin reintento automático.
* Si el tipo de error es cualquier cosa que no sea lo anterior, la ejecución falla.
