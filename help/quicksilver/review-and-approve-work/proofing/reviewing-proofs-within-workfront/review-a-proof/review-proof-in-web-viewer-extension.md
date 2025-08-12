---
product-area: documents
navigation-topic: proofing-overview
title: Revisar el contenido interactivo en la extensión del visor de revisión web
description: La herramienta de revisión de Adobe Workfront es una extensión del explorador que le permite probar el contenido interactivo en un archivo ZIP o con una dirección URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 7bff0a8c43355472453403fcd404388a3d95d471
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# Revisión del contenido interactivo con la herramienta de revisión de Adobe Workfront


>[!IMPORTANT]
>
> Se recomienda utilizar el visualizador de revisión de escritorio para el contenido interactivo que está alojado en un sitio web que requiere autenticación SSO o que impide abrir su sitio en iFrames, como Figma.

La herramienta de revisión de Adobe Workfront es una extensión de explorador basada en web que permite marcar el contenido interactivo en un archivo ZIP o con una dirección URL. La herramienta de revisión de Adobe Workfront está disponible en los siguientes exploradores:

* Firefox
* Chrome
* Edge
* Safari

## Instalación de la extensión

### Requisitos previos

* Debe quitar la extensión heredada de Web Viewer para utilizar la herramienta de revisión de Adobe Workfront.

### Instalación de la extensión

Los revisores y aprobadores deben instalar la herramienta de revisión de Adobe Workfront. en uno de los siguientes exploradores:

* [Extensión de Firefox](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Extensión de Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)


Para que las pruebas interactivas se abran automáticamente en la herramienta de revisión de Adobe Workfront, un administrador de Workfront debe actualizar la configuración de revisión en Workfront como se describe en las secciones a continuación.

## Uso de la herramienta de revisión de Adobe Workfront en GenStudio for Performance Marketing y Creative Cloud Express

Esta extensión es necesaria para revisar el contenido en GenStudio for Performance Marketing y Creative Cloud Express. Assets se abrirá automáticamente en el visor web. No es necesario que actualice ninguna configuración de la cuenta.


## Actualizar valores predeterminados de revisión de Workfront

Para utilizar la herramienta de revisión de Workfront como el visor predeterminado para el contenido interactivo, debe actualizar los valores predeterminados de revisión en Workfront.

>[!IMPORTANT]
>
>Se recomienda utilizar el Visor de corrección de escritorio si el contenido que necesita revisar está en un sitio web que
>
>* Requiere autenticación SSO
>* Impide abrir el sitio en iFrames, como Figma

### Hacer que la herramienta de revisión de Adobe Workfront sea el visor predeterminado para las pruebas de URL y ZIP

Para utilizar la herramienta de revisión web para pruebas de URL y ZIP, un administrador de Workfront debe ajustar la configuración predeterminada para las pruebas interactivas.

1. En el menú principal de Workfront, haga clic en **Revisión**.
1. Haga clic en **Configuración de la cuenta** y luego haga clic en la ficha **Configuración**.
1. En la sección **Valores predeterminados de prueba**, busque **Visor de pruebas de escritorio para la revisión interactiva** y haga clic en **Configurar**.
1. En el menú desplegable, elija **Deshabilitado**. Las pruebas interactivas creadas a partir de una URL o un archivo ZIP ahora se abren automáticamente en la herramienta Adobe Workfront Review, que es un explorador basado en web.
1. Haga clic en **Guardar**.

>[!NOTE]
>
>Este cambio se aplica a todas las pruebas interactivas de la instancia de Workfront. Se recomienda probar la nueva experiencia en el entorno de vista previa antes de habilitarla en producción. Puede volver fácilmente al Visor de escritorio cambiando la configuración de la cuenta de **Visor de corrección de escritorio para pruebas interactivas** a **Habilitado para todas las pruebas interactivas**.

### Hacer que la herramienta de revisión de Adobe Workfront sea el visor predeterminado solo para pruebas ZIP

Para utilizar la herramienta de revisión web solo para pruebas ZIP, un administrador de Workfront debe ajustar la configuración predeterminada para las pruebas interactivas.

1. En el menú principal de Workfront, haga clic en **Revisión**.
1. Haga clic en **Configuración de la cuenta** y luego haga clic en la ficha **Configuración**.
1. En la sección **Valores predeterminados de prueba**, busque **Visor de pruebas de escritorio para la revisión interactiva** y haga clic en **Configurar**.
1. En el menú desplegable, elija **Habilitado solo para pruebas interactivas creadas a partir de una dirección URL**. Las pruebas interactivas creadas a partir de un archivo ZIP ahora se abren automáticamente en la herramienta Adobe Workfront Review, que es un explorador basado en web. Las pruebas interactivas creadas a partir de una URL siguen abiertas en el Visor de pruebas de escritorio.
1. Haga clic en **Guardar**.

>[!NOTE]
>
>Este cambio se aplica a todas las pruebas de ZIP de la instancia de Workfront. Se recomienda probar la nueva experiencia en el entorno de vista previa antes de habilitarla en producción. Puede volver fácilmente al Visor de escritorio cambiando la configuración de la cuenta de **Visor de corrección de escritorio para pruebas interactivas** a **Habilitado para todas las pruebas interactivas**.

