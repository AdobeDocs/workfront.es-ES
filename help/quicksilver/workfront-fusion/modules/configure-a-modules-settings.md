---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configurar la configuración de un módulo en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 81%

---

# Configurar un módulo en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Configurar un módulo](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/configure-a-modules-settings.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Debe establecer la configuración para cada módulo que crea.

Por ejemplo, los módulos de [[!DNL Dropbox] módulos](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) requieren que especifique la carpeta de destino en la que desea cargar los archivos. Para los módulos ](../../workfront-fusion/apps-and-their-modules/email-modules.md)módulos [[!UICONTROL Email], debe introducir la dirección de correo electrónico a la que se deben enviar los correos electrónicos.

>[!NOTE]
>
>Además de la configuración del módulo, también puede ajustar la configuración de un escenario. Puede cambiar el nombre del escenario y su programación, además de especificar configuraciones adicionales, entre otras acciones.

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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Configuración de los ajustes de un módulo

1. Añada un módulo nuevo a un escenario.

   O

   Haga clic en el icono del módulo en el editor de escenarios, como se describe en [Crear un escenario en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Si es necesario para el módulo, cree una **[!UICONTROL Connection]** a su cuenta de usuario registrada para ese servicio determinado, tal como se describe en [Información general sobre Conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. En cada campo, escriba el texto adecuado.

   O

   Haga clic en **[!UICONTROL Map]** si aparece a la derecha del campo y, a continuación, asigne un elemento de otro módulo en su escenario.

   Se requieren parámetros en negrita.

   Para obtener información acerca de los diferentes tipos de datos de elementos que [!DNL Workfront Fusion] puede reconocer (como fecha, número y texto), vea [Tipos de datos de elementos en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Si el módulo tiene opciones avanzadas que desea mostrar y usar, seleccione **[!UICONTROL Mostrar ajustes avanzados]**.
