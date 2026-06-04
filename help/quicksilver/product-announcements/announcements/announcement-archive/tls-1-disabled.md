---
content-type: reference
navigation-topic: announcements
title: Se requiere TLS 1.2 en Adobe Workfront
description: Para proporcionar una seguridad óptima, Adobe Workfront requiere que todas las conexiones del explorador e integraciones de API que dependan de TLS 1.0 o versiones anteriores se actualicen a TLS 1.2. En el entorno de vista previa, TLS 1.0 ya se deshabilitó.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
TQID: https://experienceleague.adobe.com/23UVEvZitUFvhkTkgOnubLK76Lzl8QKiyz-R4svWcc8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 93%

---

# Se requiere TLS 1.2 en Adobe Workfront

Para proporcionar una seguridad óptima, Adobe Workfront requiere que todas las conexiones del explorador e integraciones de API que dependan de TLS 1.0 o versiones anteriores se actualicen a TLS 1.2. En el entorno de vista previa, TLS 1.0 ya se deshabilitó.

Workfront dejó de ser compatible oficialmente con TLS 1.0 en marzo de 2018. Todas las integraciones que usaban TLS 1.0 dejaron de funcionar el 9 de enero de 2019.  TLS 1.1 se desactivará en el cuarto trimestre de 2019.

Las secciones siguientes proporcionan más detalles acerca de estos hitos importantes, así como la forma de prepararse para esta actualización en las organizaciones:

## Se acaba la compatibilidad oficial de Workfront con TLS 1.0 (5 de marzo de 2018)

Workfront dejó de ser compatible oficialmente con TLS 1.0 en marzo de 2018.

Las conexiones del navegador y las integraciones de API que usen TLS 1.0 seguirán en funcionamiento, pero Workfront no solucionará los problemas de la aplicación Workfront relacionados con TLS 1.0.

## Las integraciones de Workfront que usaban TLS 1.0 se deshabilitaron (9 de enero de 2019)

A partir del 9 de enero de 2019, todas las conexiones del explorador Workfront y las integraciones de la API que utilicen TLS 1.0 deben actualizarse para utilizar TLS 1.1 o posterior. Las conexiones del explorador y las integraciones de la API que siguen aprovechando TLS 1.0 (conexiones entrantes o salientes) ya no podrán comunicarse con la aplicación de Workfront después de este tiempo. 

## TLS 1.1 se desactivará en el cuarto trimestre de 2019

En el entorno de producción, TLS 1.1 se desactivó el 21 de octubre de 2019. Después de este tiempo, todas las integraciones que utilicen TLS 1.1 dejarán de funcionar.

Este cambio entrará en vigor en los entornos de vista previa y zona protegida el 7 de agosto para que las organizaciones puedan prepararse para el cierre.

## Preparación para la actualización de TLS

* [Al acceder a Workfront a través del explorador](#when-accessing-workfront-via-the-browser)
* [Al conectarse a Workfront mediante la API](#when-connecting-to-workfront-via-the-api)

### Al acceder a Workfront a través del explorador {#when-accessing-workfront-via-the-browser}

Asegúrese de que los usuarios de su organización accedan a Workfront a través de exploradores compatibles. (Para obtener información acerca de los exploradores compatibles, consulte [Requisitos de explorador de Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md)).

Todos los exploradores compatibles con Workfront son compatibles con TLS 1.2.

### Al conectarse a Workfront mediante la API {#when-connecting-to-workfront-via-the-api}

Si se integran aplicaciones de terceros en Workfront mediante la API (de entrada o de salida), es necesario comprobar que TLS 1.2 (y los protocolos de cifrado de TLS 1.2) se habiliten en las integraciones.
