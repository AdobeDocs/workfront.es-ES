---
product-area: documents
navigation-topic: proofing-overview
title: Revisar el contenido interactivo en la extensión del visor de revisión web
description: La herramienta de revisión de Adobe Workfront es una extensión del explorador que le permite probar el contenido interactivo en un archivo ZIP o con una dirección URL.
author: Courtney
feature: Digital Content and Documents
source-git-commit: 5650ebfbf115908cbf2b89ffeab0551a4ecacc2d
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# Revisión del contenido interactivo con la herramienta de revisión de Adobe Workfront

<span class="preview">La herramienta Adobe Workfront Review estará disponible el 7 de noviembre de 2024. Esta extensión se encuentra en la versión beta.</span>

La herramienta de revisión de Adobe Workfront es una extensión de explorador basada en web que le permite probar el contenido interactivo en un archivo ZIP o con una dirección URL. La herramienta de revisión de Adobe Workfront está disponible en los siguientes exploradores:

* Firefox
* Chrome
* Edge

Para los sitios web que impiden abrir su sitio en iFrames, como Figma, recomendamos utilizar el Visor de pruebas de escritorio.


## Hacer que la herramienta de revisión de Adobe Workfront sea el visor predeterminado para las pruebas de URL y ZIP

Para utilizar la herramienta de revisión web para pruebas de URL y ZIP, un administrador de Workfront debe ajustar la configuración predeterminada para las pruebas interactivas.

1. En el menú principal de Workfront, haga clic en **Revisión**.
1. Haga clic en **Configuración de la cuenta** y luego haga clic en la ficha **Configuración**.
1. En la sección **Valores predeterminados de prueba**, busque **Visor de pruebas de escritorio para la revisión interactiva** y haga clic en **Configurar**.
1. En el menú desplegable, elija **Deshabilitado**. Las pruebas interactivas creadas a partir de una URL o un archivo ZIP ahora se abren automáticamente en la herramienta Adobe Workfront Review, que es un explorador basado en web.
1. Haga clic en **Guardar**.

>[!NOTE]
>
>Este cambio se aplica a todas las pruebas interactivas en los entornos de Previsualización y Producción. Se recomienda probar la nueva experiencia en el entorno de vista previa antes de habilitarla en producción. Puede volver fácilmente al Visor de escritorio cambiando la configuración de la cuenta a **Habilitada para todas las pruebas interactivas**.

## Hacer que la herramienta de revisión de Adobe Workfront sea el visor predeterminado solo para pruebas ZIP

Para utilizar la herramienta de revisión web solo para pruebas ZIP, un administrador de Workfront debe ajustar la configuración predeterminada para las pruebas interactivas.

1. En el menú principal de Workfront, haga clic en **Revisión**.
1. Haga clic en **Configuración de la cuenta** y luego haga clic en la ficha **Configuración**.
1. En la sección **Valores predeterminados de prueba**, busque **Visor de pruebas de escritorio para la revisión interactiva** y haga clic en **Configurar**.
1. En el menú desplegable, elija **Habilitado solo para pruebas interactivas creadas a partir de una dirección URL**. Las pruebas interactivas creadas a partir de un archivo ZIP ahora se abren automáticamente en la herramienta Adobe Workfront Review, que es un explorador basado en web. Las pruebas interactivas creadas a partir de una URL siguen abiertas en el Visor de pruebas de escritorio.
1. Haga clic en **Guardar**.

>[!NOTE]
>
>Este cambio se aplica a todas las pruebas interactivas en los entornos de Previsualización y Producción. Se recomienda probar la nueva experiencia en el entorno de vista previa antes de habilitarla en producción. Puede volver fácilmente al Visor de escritorio cambiando la configuración de la cuenta a **Habilitada para todas las pruebas interactivas**.

## Instalación de la extensión

Los revisores y aprobadores deben instalar la herramienta de revisión de Adobe Workfront. en uno de los siguientes exploradores:

* [Extensión de Firefox](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Extensión de Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

Una vez instalada la extensión, las pruebas interactivas se abren en la herramienta de revisión de Adobe Workfront automáticamente.

>[!IMPORTANT]
>
>Debe quitar la extensión heredada de Web Viewer para utilizar la herramienta de revisión de Adobe Workfront.




