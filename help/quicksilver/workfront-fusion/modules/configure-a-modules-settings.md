---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configure las opciones de un módulo en [!DNL Adobe Workfront Fusion]
description: Debe configurar la configuración de cada módulo que cree.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# Configure las opciones de un módulo en [!DNL Adobe Workfront Fusion]

Debe configurar la configuración de cada módulo que cree.

Por ejemplo, la variable [[!DNL Dropbox] módulos](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) Los módulos requieren que especifique la carpeta de destino en la que desea cargar los archivos. Para la variable [[!UICONTROL Correo electrónico] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md) , debe introducir la dirección de correo electrónico a la que se deben enviar los correos electrónicos.

>[!NOTE]
>
>Además de la configuración del módulo, también puede ajustar la configuración de un escenario. Puede cambiar el nombre del escenario, cambiar su programación y especificar ajustes adicionales, entre otras acciones.

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

## Configurar las opciones de un módulo

1. Agregue un nuevo módulo a un escenario.

   O

   Haga clic en el icono del módulo en el editor de escenarios, tal como se describe en [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Si es necesario para el módulo, cree un **[!UICONTROL Conexión]** a su cuenta de usuario registrada para ese servicio determinado, tal como se describe en [Acerca de la conexión [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. En cada campo, escriba el texto adecuado.

   O

   Haga clic en **[!UICONTROL Mapa]** si aparece a la derecha del campo , asigne un elemento de otro módulo en el escenario.

   Se requieren parámetros vinculados.

   Para obtener información sobre los distintos tipos de datos de elementos [!DNL Workfront Fusion] puede reconocer (como fecha, número y texto), consulte [Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Si el módulo tiene opciones avanzadas que desea visualizar y utilizar, seleccione **[!UICONTROL Mostrar configuración avanzada]**.
