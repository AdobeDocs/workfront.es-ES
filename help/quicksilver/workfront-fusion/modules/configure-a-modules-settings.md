---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configurar la configuración de un módulo en  [!DNL Adobe Workfront Fusion]
description: Debe configurar las opciones de cada módulo que cree.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---

# Configurar la configuración de un módulo en [!DNL Adobe Workfront Fusion]

Debe configurar las opciones de cada módulo que cree.

Por ejemplo, los módulos [[!DNL Dropbox] module](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) requieren que especifique la carpeta de destino en la que desea cargar los archivos. Para los módulos [[!UICONTROL Email] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md), debes ingresar la dirección de correo electrónico a la que se deben enviar los correos electrónicos.

>[!NOTE]
>
>Además de la configuración del módulo, también puede ajustar la configuración de un escenario. Puede cambiar el nombre del escenario, cambiar su programación y especificar configuraciones adicionales, entre otras acciones.

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

## Configuración de la configuración de un módulo

1. Agregue un módulo nuevo a un escenario.

   O

   Haga clic en el icono del módulo en el editor de escenarios, como se describe en [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Si es necesario para el módulo, cree una **[!UICONTROL Conexión]** a su cuenta de usuario registrada para ese servicio determinado, tal como se describe en [Información general sobre Conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. En cada campo, escriba el texto adecuado.

   O

   Haga clic en **[!UICONTROL Asignar]** si aparece a la derecha del campo y, a continuación, asigne un elemento de otro módulo en su escenario.

   Se requieren parámetros en negrita.

   Para obtener información acerca de los diferentes tipos de datos de elementos que [!DNL Workfront Fusion] puede reconocer (como fecha, número y texto), vea [Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Si el módulo tiene opciones avanzadas que desea mostrar y usar, seleccione **[!UICONTROL Mostrar configuración avanzada]**.
