---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Elegir dónde se inicia un módulo de activador en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 82%

---

# Elegir dónde se inicia un módulo de activador en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Elija dónde se inicia un módulo de déclencheur](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/choose-where-trigger-module-starts.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Algunos módulos de activación le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.

También puede especificar si desea recuperar todos los paquetes o solo los paquetes después de una fecha específica.

Para obtener más información acerca de los módulos de activadores, consulte la sección [Módulos de activador](../../workfront-fusion/modules/module-types.md#triggers) en el artículo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Elegir dónde se inicia un módulo de activador

1. Guarde un módulo de activador.

   O

   Cambie la configuración del módulo de activador tal como se describe en [Configuración de un módulo en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   O

   Haga clic con el botón secundario del mouse (ratón) en el módulo de activador en el [!UICONTROL Editor de escenarios], tal como se describe en [Crear un escenario en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Seleccione una opción en el cuadro **[!UICONTROL Elegir por dónde empezar]** que aparece.

   ![](assets/choose-where-to-start-350x346.jpg)

   Las opciones mostradas dependen de las posibilidades de un servicio determinado. Pueden incluir lo siguiente:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on] (valor predeterminado)</td>
            <td>Recupera todos los paquetes añadidos o actualizados (según la configuración) a partir de ahora</td>
        </tr>
        <tr>
            <td>[!UICONTROL From after a specific date]</td>
            <td>Recupera todos los paquetes añadidos o actualizados (según la configuración) después de una fecha u hora especificadas</td>
        </tr>
        <tr>
            <td>[!UICONTROL With ID greater than or equal to a specific value]</td>
            <td>Recupera todos los paquetes con un ID mayor o igual que un ID especificado</td> 
        </tr>
        <tr>
            <td>[!UICONTROL All bundles]</td>
            <td>Recupera todos los paquetes disponibles</td>
        </tr>
        <tr>
            <td>[!UICONTROL Select the first bundle]</td>
            <td>Permite seleccionar el primer paquete desde el que se va a iniciar la recuperación de paquetes</td>
        </tr>
   </table>
