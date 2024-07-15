---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con medidas de seguridad actualizadas
description: Google ha introducido recientemente restricciones sobre cómo los usuarios pueden utilizar su API. Este artículo describe cómo conectar [!DNL Adobe Workfront Fusion] a Google, teniendo en cuenta estas medidas de seguridad de actualización.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con medidas de seguridad actualizadas

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

## [!DNL Google Services] restricciones

[!DNL Google] introdujo restricciones sobre cómo los usuarios pueden usar su API a partir del 1 de junio de 2020. Estas medidas de seguridad protegen a los usuarios de [!DNL Google] de la filtración o el uso indebido de sus datos personales en [!DNL Google]. Las restricciones están relacionadas con las aplicaciones [!DNL Gmail] y [!DNL Google Drive]. Para obtener más información sobre estas restricciones, consulte &quot;Requisitos adicionales para ámbitos de API específicos&quot; en la [[!DNL Google] Directiva de datos de usuario de servicios de API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Para tener acceso a los ámbitos restringidos, el servicio conectado ([!DNL Adobe Workfront Fusion] o cualquier otro servicio que desee tener acceso a los datos del usuario a través de la API) debe verificarse y debe tener una carta de evaluación para probar que el servicio es seguro y transparente en cuanto a cómo utilizan los datos. [!DNL Workfront Fusion] cumple con todos los requisitos de [!DNL Google] para tener acceso a los ámbitos restringidos. Sin embargo, la mayoría de los servicios conectados de terceros en [!DNL Workfront Fusion] no tienen la carta de evaluación y, por lo tanto, no cumplen los términos de [!DNL Google]. Debido a esto, [!DNL Workfront Fusion] no tiene permiso para enviar datos a estos servicios.

## Excepciones a [!DNL Google Services] restricciones

Hay algunas excepciones que permiten enviar datos a un servicio de terceros no aprobado que no tiene la carta de evaluación sin violar ninguna de las nuevas restricciones. Difieren según [!DNL Google Workspace] con el cliente OAuth [!DNL Workfront Fusion], [!DNL Google Workspace] con otro cliente OAuth o [!DNL @gmail.com] y [!DNL @google.mail.com].

* [[!DNL Google Workspace] con  [!DNL Workfront Fusion] cliente OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] con otro cliente OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] y  [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] con [!DNL Workfront Fusion] cliente de OAuth

[!DNL Workfront Fusion] utiliza la excepción [!UICONTROL Instalación en todo el dominio]. La instalación en todo el dominio es adecuada para [!DNL Google Workspace] usuarios y permite a los usuarios integrar servicios no aprobados sin ninguna limitación. Si usa Google Workspace, no tiene que realizar ningún paso adicional y puede conectarse directamente a servicios no aprobados.

### [!DNL Google Workspace] con otro cliente OAuth

Los usuarios de [!DNL Google Workspace] que prefieran usar su propio cliente OAuth en lugar de usar el cliente OAuth de [!DNL Workfront Fusion] pueden conectarse a [!DNL Google Services] mediante el método de uso [!UICONTROL interno]. Esta opción está destinada a usuarios avanzados. Para obtener instrucciones, consulta [Conectar [!DNL Adobe Workfront Fusion] con [!DNL Google Services] mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] y [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

El usuario que tiene acceso a [!DNL Google Services] a través de [!DNL @gmail.com] o [!DNL @googlemail.com] puede conectarse a [!DNL Google Services] a través del método de uso personal. Esta opción está destinada a usuarios avanzados. Para obtener instrucciones, consulta [Conectar [!DNL Adobe Workfront Fusion] con [!DNL Google Services] mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [¿Qué aplicaciones de  [!DNL Adobe Workfront Fusion]  se ven afectadas?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [¿Tengo una cuenta de  [!DNL Google Workspace] ?](#do-i-have-a-g-suite-account)
* [¿Qué debo hacer si soy  [!DNL @gmail.com] o [!DNL @googlemail.com] usuario?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [¿Qué debo hacer si soy un usuario de  [!DNL Google Workspace] ?](#what-should-i-do-if-im-a-g-suite-user)

### ¿Qué aplicaciones de [!DNL Adobe Workfront Fusion] se ven afectadas? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] y correo electrónico (conectado a la cuenta de [!DNL Gmail]).

### ¿Tengo una cuenta de [!DNL Google Workspace]? {#do-i-have-a-g-suite-account}

Si su dirección de correo electrónico termina con [!DNL @gmail.com] o [!DNL @googlemail.com], su cuenta no es una cuenta de [!DNL Google Workspace]. Si su cuenta de [!DNL Google] termina con un dominio personalizado como @my-company.com, entonces es una cuenta de [!DNL Google Workspace].

### ¿Qué debo hacer si soy [!DNL @gmail.com] o [!DNL @googlemail.com] usuario? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Estas nuevas restricciones solo se aplican si está integrando [!DNL Google Drive] o [!DNL Gmail]. Si desea conectarse a [!DNL Google Drive] o [!DNL Gmail], puede

* Cambiar a [!DNL Google Workspace]

  o

* Cree un cliente de OAuth personalizado. Esta opción está destinada a usuarios avanzados.

  Para obtener instrucciones, consulta [Conectar [!DNL Adobe Workfront Fusion] con [!DNL Google Services] mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Si desea integrar cualquier otro servicio que no sea [!DNL Google Drive] o [!DNL Gmail], estas restricciones no se aplican.

Para obtener instrucciones sobre cómo conectar otros [!DNL Google Services] a [!DNL Workfront Fusion], consulte [Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### ¿Qué debo hacer si soy un usuario de [!DNL Google Workspace]? {#what-should-i-do-if-im-a-g-suite-user}

No se requiere ninguna acción.
