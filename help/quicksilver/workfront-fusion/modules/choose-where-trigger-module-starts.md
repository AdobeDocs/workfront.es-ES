---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Elija dónde se inicia un módulo de déclencheur en Adobe Workfront Fusion
description: Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea iniciar la recuperación de paquetes.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Elija dónde comienza un módulo de déclencheur en [!DNL Adobe Workfront Fusion]

Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea iniciar la recuperación de paquetes.

También puede especificar si desea recuperar todos los paquetes o solo los paquetes de después de una fecha específica.

Para obtener más información sobre los módulos de déclencheur, consulte la sección [módulos de déclencheur](../../workfront-fusion/modules/module-types.md#triggers) en el artículo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

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

## Elegir dónde se inicia un módulo de déclencheur

1. Guarde un módulo de déclencheur.

   O

   Cambie la configuración del módulo de déclencheur como se describe en [Configure las opciones de un módulo en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   O

   Haga clic con el botón derecho en el icono del módulo de déclencheur en la [!UICONTROL Editor de escenarios], tal como se describe en [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Seleccione una opción en la **[!UICONTROL Elija dónde empezar]** que aparece.

   ![](assets/choose-where-to-start-350x346.jpg)

   Las opciones mostradas dependen de las posibilidades de un servicio determinado. Pueden incluir lo siguiente:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL A partir de ahora] (predeterminado)</td>
            <td>Recupera todos los paquetes agregados o actualizados (según la configuración) a partir de ahora</td>
        </tr>
        <tr>
            <td>[!UICONTROL A partir de una fecha específica]</td>
            <td>Recupera todos los paquetes agregados o actualizados (según la configuración) después de una fecha y hora especificadas</td>
        </tr>
        <tr>
            <td>[!UICONTROL Con ID bueno o igual a un valor específico]</td>
            <td>Recupera todos los paquetes con un ID bueno o igual a un ID especificado</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Todos los paquetes]</td>
            <td>Recupera todos los paquetes disponibles</td>
        </tr>
        <tr>
            <td>[!UICONTROL Seleccione el primer paquete]</td>
            <td>Permite seleccionar el primer paquete desde el que se inicia la recuperación de paquetes</td>
        </tr>
   </table>
