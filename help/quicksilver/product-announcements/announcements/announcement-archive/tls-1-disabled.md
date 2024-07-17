---
content-type: reference
navigation-topic: announcements
title: Se requiere TLS 1.2 en Adobe Workfront
description: Para proporcionar una seguridad óptima, Adobe Workfront requiere que todas las conexiones del explorador e integraciones de API que dependen de TLS 1.0 o anteriores se actualicen para utilizar TLS 1.2. En el entorno de vista previa, TLS 1.0 ya está deshabilitado.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Se requiere TLS 1.2 en Adobe Workfront

Para proporcionar una seguridad óptima, Adobe Workfront requiere que todas las conexiones del explorador e integraciones de API que dependen de TLS 1.0 o anteriores se actualicen para utilizar TLS 1.2. En el entorno de vista previa, TLS 1.0 ya está deshabilitado.

Workfront dejó de ser compatible oficialmente con TLS 1.0 en marzo de 2018. Todas las integraciones que aprovechan TLS 1.0 dejaron de funcionar el 9 de enero de 2019.  TLS 1.1 se desactivará en el cuarto trimestre de 2019.

Las secciones siguientes proporcionan más detalles acerca de estos hitos importantes, así como la forma de prepararse para esta actualización en su organización:

## Workfront finaliza la compatibilidad oficial con TLS 1.0 (5 de marzo de 2018)

Workfront dejó de ser compatible oficialmente con TLS 1.0 en marzo de 2018.

Las conexiones del navegador y las integraciones de la API que aprovechan TLS 1.0 siguen en funcionamiento, pero Workfront no solucionará los problemas de la aplicación Workfront relacionados con TLS 1.0.

## Integraciones de Workfront con TLS 1.0 deshabilitado (9 de enero de 2019)

A partir del 9 de enero de 2019, todas las conexiones del explorador Workfront y las integraciones de la API que utilicen TLS 1.0 deben actualizarse para utilizar TLS 1.1 o posterior. Las conexiones del explorador y las integraciones de la API que siguen aprovechando TLS 1.0 (conexiones entrantes o salientes) ya no podrán comunicarse con la aplicación de Workfront después de este tiempo. 

## TLS 1.1 se desactivará en el cuarto trimestre de 2019

En el entorno de producción, TLS 1.1 se desactivó el 21 de octubre de 2019. Después de este tiempo, todas las integraciones que utilicen TLS 1.1 dejarán de funcionar.

Este cambio entrará en vigor en los entornos de Vista previa y Zona protegida el 7 de agosto para ayudar a las organizaciones a prepararse para el cierre.

## Preparación para la actualización de TLS

* [Al acceder a Workfront a través del explorador](#when-accessing-workfront-via-the-browser)
* [Al conectarse a Workfront mediante la API](#when-connecting-to-workfront-via-the-api)

### Al acceder a Workfront a través del explorador {#when-accessing-workfront-via-the-browser}

Asegúrese de que los usuarios de su organización acceden a Workfront a través de un explorador compatible. (Para obtener información acerca de los exploradores compatibles, consulte [Requisitos del explorador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Todos los exploradores compatibles con Workfront son compatibles con TLS 1.2.

### Al conectarse a Workfront mediante la API {#when-connecting-to-workfront-via-the-api}

Si integra aplicaciones de terceros en Workfront mediante la API (de entrada o de salida), compruebe que TLS 1.2 (y los protocolos de codificación TLS 1.2) estén habilitados en las integraciones.
