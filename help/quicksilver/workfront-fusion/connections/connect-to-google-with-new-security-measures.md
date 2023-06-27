---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] con medidas de seguridad actualizadas
description: Google ha introducido recientemente restricciones sobre cómo los usuarios pueden utilizar su API. Este artículo describe cómo conectar [!DNL Adobe Workfront Fusion] a Google, teniendo en cuenta estas medidas de seguridad de actualización.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] con medidas de seguridad actualizadas

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

## [!DNL Google Services] restricciones

[!DNL Google] introdujo restricciones sobre cómo los usuarios pueden utilizar su API a partir del 1 de junio de 2020. Estas medidas de seguridad protegen [!DNL Google] que los usuarios pierdan o utilicen indebidamente sus datos personales en [!DNL Google]. Las restricciones están relacionadas con [!DNL Gmail] y [!DNL Google Drive] aplicaciones. Para obtener más información sobre estas restricciones, consulte &quot;Requisitos adicionales para ámbitos de API específicos&quot; en la [[!DNL Google] Directiva de datos de usuario de servicios API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Para acceder a ámbitos restringidos, el servicio conectado ([!DNL Adobe Workfront Fusion] (o cualquier otro servicio que desee acceder a los datos del usuario a través de la API) debe verificarse y debe tener una carta de evaluación para probar que el servicio es seguro y transparente sobre cómo utilizan los datos. [!DNL Workfront Fusion] cumple con todos los [!DNL Google]Requisitos de para el acceso a ámbitos restringidos. Sin embargo, la mayoría de los servicios conectados de terceros en [!DNL Workfront Fusion] no tiene la carta de evaluación y, por lo tanto, no cumple con [!DNL Google] condiciones. Debido a eso, [!DNL Workfront Fusion] no tiene permiso para enviar datos a estos servicios.

## Excepciones a [!DNL Google Services] restricciones

Hay algunas excepciones que permiten enviar datos a un servicio de terceros no aprobado que no tiene la carta de evaluación sin violar ninguna de las nuevas restricciones. Difieren según el [!DNL G Suite] con el [!DNL Workfront Fusion] cliente de OAuth, [!DNL G Suite] con otro cliente OAuth, o [!DNL @gmail.com] y [!DNL @google.mail.com].

* [[!DNL G suite] con [!DNL Workfront Fusion] cliente de OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] con otro cliente OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] y [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] con [!DNL Workfront Fusion] cliente de OAuth

[!DNL Workfront Fusion] utiliza el [!UICONTROL Instalación en todo el dominio] excepción. La instalación en todo el dominio es adecuada para [!DNL G Suite] y permite a los usuarios integrar servicios no aprobados sin ninguna limitación. Si es usuario de G Suite, no tiene que realizar ningún paso adicional y puede conectarse directamente a servicios no aprobados.

### [!DNL G suite] con otro cliente OAuth

[!DNL G Suite] Los usuarios de que prefieren utilizar su propio cliente de OAuth en lugar de utilizar el [!DNL Workfront Fusion] El cliente de OAuth puede conectarse a [!DNL Google Services] a través de [!UICONTROL Interno] Use el método. Esta opción está destinada a usuarios avanzados. Para obtener instrucciones, consulte [Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] y [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Usuario que accede a [!DNL Google Services] mediante [!DNL @gmail.com] o [!DNL @googlemail.com] puede conectarse a [!DNL Google Services] mediante el enfoque de uso personal. Esta opción está destinada a usuarios avanzados. Para obtener instrucciones, consulte [Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [Qué aplicaciones hay en [!DNL Adobe Workfront Fusion] se ven afectados?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [¿Tengo una cuenta de [!DNL G Suite]?](#do-i-have-a-g-suite-account)
* [¿Qué debo hacer si estoy [!DNL @gmail.com] o [!DNL @googlemail.com] ¿usuario?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [¿Qué debo hacer si soy usuario de [!DNL G Suite]?](#what-should-i-do-if-im-a-g-suite-user)

### Qué aplicaciones hay en [!DNL Adobe Workfront Fusion] se ven afectados? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]y Correo electrónico (conectado a [!DNL Gmail] account).

### ¿Tengo un [!DNL G Suite] ¿Cuenta? {#do-i-have-a-g-suite-account}

Si su dirección de correo electrónico termina con [!DNL @gmail.com] o [!DNL @googlemail.com] su cuenta no es una [!DNL G Suite] cuenta. Si su [!DNL Google] La cuenta de termina con un dominio personalizado como @my-company.com y luego es un [!DNL G Suite] cuenta.

### ¿Qué debo hacer si estoy [!DNL @gmail.com] o [!DNL @googlemail.com] ¿usuario? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Estas nuevas restricciones solo se aplican si realiza la integración [!DNL Google Drive] o [!DNL Gmail]. Si desea conectarse a [!DNL Google Drive] o [!DNL Gmail], puede

* Cambiar a [!DNL G Suite]

  o

* Cree un cliente de OAuth personalizado. Esta opción está destinada a usuarios avanzados.

  Para obtener instrucciones, consulte [Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Si desea integrar cualquier otro servicio que no sea [!DNL Google Drive] o [!DNL Gmail]Sin embargo, estas restricciones no se aplican.

Para obtener instrucciones acerca de cómo conectar otros [!DNL Google Services] hasta [!DNL Workfront Fusion], consulte [Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### ¿Qué debo hacer si soy un [!DNL G Suite] ¿usuario? {#what-should-i-do-if-im-a-g-suite-user}

No se requiere ninguna acción.
