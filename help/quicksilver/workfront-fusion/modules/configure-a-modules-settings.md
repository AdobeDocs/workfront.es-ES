---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configuración de un módulo en [!DNL Adobe Workfront Fusion]
description: Debe configurar las opciones de cada módulo que cree.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 1%

---

# Configuración de un módulo en [!DNL Adobe Workfront Fusion]

Debe configurar las opciones de cada módulo que cree.

Por ejemplo, la variable [[!DNL Dropbox] módulos](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) Los módulos de requieren que especifique la carpeta de destino en la que desea cargar los archivos. Para el [[!UICONTROL Correo electrónico] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md) módulos, debe introducir la dirección de correo electrónico a la que se deben enviar los correos electrónicos.

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

## Configuración de la configuración de un módulo

1. Agregue un módulo nuevo a un escenario.

   O

   Haga clic en el icono del módulo en el editor de escenarios, como se describe en [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Si es necesario para el módulo, cree un **[!UICONTROL Conexión]** a su cuenta de usuario registrada para ese servicio determinado, tal como se describe en [Acerca de conectar [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. En cada campo, escriba el texto adecuado.

   O

   Clic **[!UICONTROL Mapa]** si aparece a la derecha del campo, asigne un elemento de otro módulo en su escenario.

   Se requieren parámetros en negrita.

   Para obtener información sobre los distintos tipos de datos de elementos [!DNL Workfront Fusion] puede reconocer (como fecha, número y texto), consulte [Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Si el módulo tiene opciones avanzadas que desea mostrar y utilizar, seleccione **[!UICONTROL Mostrar configuración avanzada]**.
