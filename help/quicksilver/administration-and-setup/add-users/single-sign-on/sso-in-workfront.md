---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Información general sobre el inicio de sesión único en Adobe Workfront
description: Workfront proporciona una configuración de inicio de sesión único (SSO) administrada centralmente que integra fácilmente Workfront con su solución SSO corporativa existente. Esta configuración es fácil de configurar y administrar y está disponible para los clientes OnDemand y OnPremise Enterprise.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Información general sobre el inicio de sesión único en Adobe Workfront

{{important-admin-console-onboard}}


Workfront proporciona una configuración de inicio de sesión único (SSO) administrada centralmente que integra fácilmente Workfront con su solución SSO corporativa existente. Esta configuración es fácil de configurar y administrar y está disponible para los clientes OnDemand y OnPremise Enterprise.

Para utilizar la funcionalidad SSO en Workfront, su organización debe configurar una aplicación SSO. A continuación, puede configurar Workfront para que se pueda comunicar con su solución SSO.

Las soluciones federadas permiten a los usuarios iniciar sesión en todas sus aplicaciones introduciendo su nombre de usuario y contraseña en un portal de inicio de sesión centralizado.

![](assets/overview-sso-wf.png)


## Configurar el cortafuegos

Cuando se utiliza una solución SSO, Workfront inicia una conexión con el servidor en el puerto especificado.

Si se suscribe a Workfront bajo demanda y ha configurado el firewall o el servidor de correo para permitir el acceso solo a proveedores específicos, debe agregar ciertas direcciones IP de Workfront a la lista de permitidos del cortafuegos. Para obtener más información, consulte [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configuración del inicio de sesión único

Workfront se integra con las siguientes soluciones de SSO:

* Soluciones federadas compatibles con SAML 2.0

   Para obtener información sobre la integración de Workfront con SAML 2.0, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Soluciones federadas que admiten SAML 2.0 usando ADFS

   Para obtener información sobre la integración de Workfront con SAML 2.0 mediante ADFS, consulte [Configuración de Adobe Workfront con SAML 2.0 mediante ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
