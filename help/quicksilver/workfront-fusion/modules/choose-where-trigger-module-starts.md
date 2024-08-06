---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Elija dónde se inicia un módulo de déclencheur en Adobe Workfront Fusion
description: Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 489ed23fe0d7945753b59810ff9da084bd3e92e4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Elija dónde comienza un módulo de déclencheur en [!DNL Adobe Workfront Fusion]

Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.

También puede especificar si desea recuperar todos los paquetes o solo los paquetes después de una fecha específica.

Para obtener más información acerca de los módulos de déclencheur, consulte la sección [Módulos de Déclencheur](../../workfront-fusion/modules/module-types.md#triggers) en el artículo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

+++

## Elija dónde se inicia un módulo de déclencheur

1. Guarde un módulo de déclencheur.

   O

   Cambie la configuración del módulo de déclencheur como se describe en [Configuración de un módulo en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   O

   Haga clic con el botón secundario del mouse (ratón) en el déclencheur del módulo en el [!UICONTROL Editor de escenarios], tal como se describe en [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Seleccione una opción en el cuadro **[!UICONTROL Elegir por dónde empezar]** que aparece.

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
            <td>[!UICONTROL Con ID mayor o igual que un valor específico]</td>
            <td>Recupera todos los paquetes con un ID mayor o igual que un ID especificado</td> 
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
