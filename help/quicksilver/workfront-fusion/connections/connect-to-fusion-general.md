---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas
description: Muchos [!DNL Adobe Workfront Fusion] Los conectores de no requieren una configuración personalizada al crear una conexión. Este artículo describe el proceso de creación de conexiones predeterminado.
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
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

## Crear una conexión

Para crear una conexión dentro de un [!DNL Workfront Fusion] módulo:

1. Clic **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] para abrir el **[!UICONTROL Crear una conexión]** panel.
1. (Opcional) Cambiar el valor predeterminado **[!UICONTROL Nombre de conexión]**.
1. (Condicional) Si la aplicación requiere una configuración de conexión avanzada, como un ID, una clave o [!UICONTROL secreto], introduzca esa información.

   Es posible que tenga que hacer clic en **[!UICONTROL Mostrar configuración avanzada]** para mostrar los campos donde puede introducir este tipo de información.

1. Clic **[!UICONTROL Continuar]**.
1. En la ventana de inicio de sesión que aparece, introduzca sus credenciales para iniciar sesión en la aplicación si aún no lo ha hecho.
1. (Condicional) Si **[!UICONTROL Permitir]** , examine las acciones que podrá realizar el conector y haga clic en el botón para conectar la aplicación [!DNL Workfront Fusion].

   >[!NOTE]
   >
   >Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
   >
   >Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.