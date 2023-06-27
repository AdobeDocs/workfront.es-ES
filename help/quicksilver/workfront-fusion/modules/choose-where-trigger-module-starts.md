---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Elija dónde se inicia un módulo de déclencheur en Adobe Workfront Fusion
description: Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Elija dónde comienza un módulo de déclencheur en [!DNL Adobe Workfront Fusion]

Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.

También puede especificar si desea recuperar todos los paquetes o solo los paquetes después de una fecha específica.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Elija dónde se inicia un módulo de déclencheur

1. Guarde un módulo de déclencheur.

   O

   Cambie la configuración del módulo de déclencheur como se describe en [Configuración de un módulo en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   O

   Haga clic con el botón derecho en el icono del módulo de déclencheur en la [!UICONTROL Editor de escenarios], tal como se describe en [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Seleccione una opción en la **[!UICONTROL Elija por dónde empezar]** que aparece.

   ![](assets/choose-where-to-start-350x346.jpg)

   Las opciones mostradas dependen de las posibilidades de un servicio determinado. Pueden incluir lo siguiente:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL A partir de ahora] (predeterminado)</td>
            <td>Recupera todos los paquetes añadidos o actualizados (según la configuración) a partir de ahora</td>
        </tr>
        <tr>
            <td>[!UICONTROL Desde después de una fecha específica]</td>
            <td>Recupera todos los paquetes añadidos o actualizados (según la configuración) después de una fecha u hora especificadas</td>
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
            <td>[!UICONTROL Seleccionar el primer paquete]</td>
            <td>Permite seleccionar el primer paquete desde el que se inicia la recuperación de paquetes</td>
        </tr>
   </table>
