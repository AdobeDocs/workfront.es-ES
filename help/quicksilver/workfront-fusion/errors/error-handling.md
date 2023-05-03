---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestión de errores en [!DNL Adobe Workfront Fusion]
description: Cuando se producen errores durante la ejecución de un escenario, normalmente se debe a que un servicio no está disponible debido a un error, un servicio responde con datos inesperados o la validación de datos de entrada falla.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: e936bbd2837e4aec67d4136b8efcccb6f8454a89
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Gestión de errores en [!DNL Adobe Workfront Fusion]

Cuando se producen errores durante la ejecución de un escenario, normalmente se debe a que un servicio no está disponible debido a un error, un servicio responde con datos inesperados o la validación de datos de entrada falla.

Si un módulo genera un error durante la ejecución del escenario y no hay ninguna ruta de gestión de errores adjunta al módulo, se ejecuta la lógica de gestión de errores predeterminada, tal como se describe en [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Al agregar una ruta de tratamiento de errores a un módulo, puede reemplazar la lógica de gestión de errores predeterminada con la suya propia. [!DNL Adobe Workfront Fusion] ofrece cinco directivas diferentes que se pueden insertar al final de las rutas del gestor de errores.

Para obtener más información, consulte [Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Ruta del controlador de errores

Para añadir una ruta de controlador de errores a un módulo:

1. Haga clic con el botón derecho del ratón en el módulo y seleccione **[!UICONTROL Agregar controlador de error]**:

   ![](assets/error-handler-route.png)

   El módulo muestra una lista de directivas, así como las aplicaciones que se utilizan en su escenario.

1. Si el módulo al que ha agregado un controlador de error es el último de la ruta, seleccione una de las directivas.

   O

   Agregue uno o más módulos a la ruta del controlador de errores.

   Si agrega más módulos a la ruta, la variable [!UICONTROL Ignorar] se aplica de forma predeterminada y, en caso de error, se procesan los módulos posteriores de esa ruta.


>[!INFO]
>
>En este ejemplo, si se produce un error al ejecutar el [!UICONTROL Crear una carpeta] módulo, la variable [!UICONTROL Ignorar] se aplicará automáticamente y el escenario pasará al siguiente módulo de la ruta del controlador de errores.
>
>Sin embargo, si no hay ningún error, el escenario pasará al [!UICONTROL Enumerar todos los archivos en un módulo de carpetas] en la ruta regular.
>
>![](assets/if-there-is-no-error-350x234.png)

Tenga en cuenta que una ruta del controlador de errores está compuesta por círculos transparentes, mientras que una ruta normal está compuesta por círculos sólidos.

## Directivas de gestión de errores

Las directivas se explican brevemente a continuación. Para obtener más información, consulte [Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Hay un total de cinco directivas que pueden agruparse en las siguientes categorías en función de si la ejecución de un escenario debe continuar o no.

Las siguientes directivas garantizan que continúe la ejecución de un escenario:

* **[!UICONTROL Reanudar]**: Permite especificar una salida sustitutiva para el módulo con el error . El estado de ejecución del escenario se marca como éxito
* **[!UICONTROL Ignorar]**: ignora el error. El estado de ejecución del escenario se marca como éxito
* **[!UICONTROL Salto]**: Almacena la entrada en la cola de ejecuciones incompletas. El estado de ejecución del escenario se marca como advertencia. Para obtener más información, consulte [Ver y resolver ejecuciones incompletas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Si la ejecución de un escenario debe detenerse cuando se produce un error, utilice una de las siguientes directivas:

* **[!UICONTROL Reversión]**: Detiene la ejecución del escenario inmediatamente y marca su estado como error
* **[!UICONTROL Confirmar]**: Detiene la ejecución del escenario inmediatamente y marca su estado como éxito

Para obtener más información sobre la gestión de errores, consulte:

* [Directivas para la gestión de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Gestión de errores avanzada en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)