---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con medidas de seguridad actualizadas
description: Google ha introducido recientemente restricciones sobre cómo los usuarios pueden utilizar su API. Este artículo describe cómo conectar [!DNL Adobe Workfront Fusion] a Google, teniendo en cuenta estas medidas de seguridad de actualización.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con medidas de seguridad actualizadas

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restricciones

[!DNL Google] se han introducido restricciones sobre cómo los usuarios pueden utilizar su API a partir del 1 de junio de 2020. Estas medidas de seguridad protegen [!DNL Google] usuarios de la filtración o uso indebido de sus datos personales en [!DNL Google]. Las restricciones están relacionadas con la variable [!DNL Gmail] y [!DNL Google Drive] aplicaciones. Para obtener más información sobre estas restricciones, consulte &quot;Requisitos adicionales para ámbitos de API específicos&quot; en [[!DNL Google] Política de datos del usuario de los servicios de API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Para acceder a los ámbitos restringidos, el servicio conectado ([!DNL Adobe Workfront Fusion] o cualquier otro servicio que desee acceder a los datos del usuario a través de la API) debe verificarse y tener una carta de evaluación para probar que el servicio es seguro y transparente sobre cómo utilizan los datos. [!DNL Workfront Fusion] cumple con todos [!DNL Google]Requisitos de para acceder a ámbitos restringidos. Sin embargo, la mayoría de los servicios conectados de terceros en [!DNL Workfront Fusion] no tiene la carta de evaluación y, por lo tanto, no cumple con [!DNL Google] términos. Debido a eso, [!DNL Workfront Fusion] no está permitido enviar datos a estos servicios.

## Excepciones a [!DNL Google Services] restricciones

Hay algunas excepciones que permiten enviar datos a un servicio de terceros no autorizado que no tiene la Carta de evaluación sin violar ninguna de las nuevas restricciones. Difieren en función de [!DNL G Suite] con la variable [!DNL Workfront Fusion] cliente OAuth, [!DNL G Suite] con otro cliente de OAuth, o [!DNL @gmail.com] y [!DNL @google.mail.com].

* [[!DNL G suite] con [!DNL Workfront Fusion] Cliente OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] con otro cliente OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] y [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] con [!DNL Workfront Fusion] Cliente OAuth

[!DNL Workfront Fusion] utiliza la variable [!UICONTROL Instalación en todo el dominio] excepción. La instalación en todo el dominio es adecuada para [!DNL G Suite] y permite a los usuarios integrar servicios no aprobados sin limitaciones. Si es usuario de G Suite, no tiene que realizar ningún paso adicional y puede conectarse directamente a servicios no aprobados.

### [!DNL G suite] con otro cliente de OAuth

[!DNL G Suite] usuarios que prefieran utilizar su propio cliente de OAuth en lugar de usar la variable [!DNL Workfront Fusion] El cliente de OAuth puede conectarse a [!DNL Google Services] a través de [!UICONTROL Internas] Utilice el método . Esta opción está dirigida a usuarios avanzados. Para obtener instrucciones, consulte [Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] y [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Usuario con acceso [!DNL Google Services] hasta [!DNL @gmail.com] o [!DNL @googlemail.com] puede conectarse a [!DNL Google Services] mediante el método de uso personal. Esta opción está dirigida a usuarios avanzados. Para obtener instrucciones, consulte [Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Preguntas frecuentes

* [¿Qué aplicaciones hay en [!DNL Adobe Workfront Fusion] ¿se ven afectados?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [¿Tengo una cuenta de [!DNL G Suite]?](#do-i-have-a-g-suite-account)
* [¿Qué debo hacer si soy [!DNL @gmail.com] o [!DNL @googlemail.com] usuario?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [¿Qué debo hacer si soy un usuario de [!DNL G Suite]?](#what-should-i-do-if-im-a-g-suite-user)

### ¿Qué aplicaciones hay en [!DNL Adobe Workfront Fusion] ¿se ven afectados? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]y Correo electrónico (conectado a [!DNL Gmail] cuenta).

### ¿Tengo un [!DNL G Suite] cuenta? {#do-i-have-a-g-suite-account}

Si su dirección de correo electrónico termina con [!DNL @gmail.com] o [!DNL @googlemail.com] su cuenta no es [!DNL G Suite] cuenta. Si su [!DNL Google] la cuenta termina con un dominio personalizado como @my-company.com, entonces es un [!DNL G Suite] cuenta.

### ¿Qué debo hacer si soy [!DNL @gmail.com] o [!DNL @googlemail.com] usuario? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Estas nuevas restricciones solo se aplican si está integrando [!DNL Google Drive] o [!DNL Gmail]. Si desea conectarse a [!DNL Google Drive] o [!DNL Gmail], puede

* Cambie a [!DNL G Suite]

   o

* Cree un cliente OAuth personalizado. Esta opción está dirigida a usuarios avanzados.

   Para obtener instrucciones, consulte [Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Si desea integrar cualquier otro servicio que no sea [!DNL Google Drive] o [!DNL Gmail], estas restricciones no se aplican.

Para instrucciones sobre la conexión de otros [!DNL Google Services] a [!DNL Workfront Fusion], consulte [Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### ¿Qué debo hacer si soy un [!DNL G Suite] usuario? {#what-should-i-do-if-im-a-g-suite-user}

No se requiere ninguna acción.
