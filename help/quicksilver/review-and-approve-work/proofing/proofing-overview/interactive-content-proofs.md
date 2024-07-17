---
product-area: documents
navigation-topic: proofing-overview
title: Resumen de pruebas de contenido interactivo
description: El contenido interactivo ofrece varios métodos para atraer a los visualizadores. Las agencias pueden medir el éxito de sus campañas utilizando análisis recopilados de las respuestas a este contenido.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Resumen de pruebas de contenido interactivo

<!-- Audited: 01/2024 -->

El contenido interactivo ofrece varios métodos para atraer a los visualizadores. Las agencias pueden medir el éxito de sus campañas utilizando análisis recopilados de las respuestas a este contenido.

Algunos ejemplos de contenido interactivo son:

* Sitios web
* Vídeos incrustados o de flujo continuo
* Titulares interactivos
* Animaciones de HTML5
* Micrositios
* Correos electrónicos interactivos

## Acerca de la creación de pruebas para contenido interactivo

Puede crear una prueba para el contenido interactivo de una de las siguientes maneras:

* Cree una prueba a partir de un archivo ZIP que contenga el contenido interactivo.

  Adobe Workfront desempaqueta el contenido del archivo ZIP y lo almacena en un servidor de Workfront. Como se almacena de esta manera, puede confiar en que el contenido permanecerá igual durante todo el ciclo de revisión de pruebas.

* Especifique la URL para el contenido.

  Esta es la forma más sencilla de crear una prueba para el contenido interactivo. También es la única manera de revisar el contenido de forma interactiva, a medida que los usuarios lo experimenten en Internet.

  Con este enfoque, un servidor externo desconocido para Workfront almacena y aloja el contenido.

  Recomendamos este método para sitios web grandes porque es difícil recopilar todos los archivos que conforman un sitio web grande. Sin embargo, dado que el contenido de la prueba se almacena de forma externa, Workfront no puede protegerlo de los cambios realizados por los desarrolladores que trabajan en ella, por lo que es posible que no pueda confiar en que el contenido permanezca igual durante todo el ciclo de revisión de la prueba.

## Preparar contenido interactivo en un archivo ZIP para la revisión

Cuando agrupe contenido interactivo en un archivo ZIP para la revisión, asegúrese de que incluye las siguientes especificaciones:

* Todos los recursos, como CSS, JavaScript, vídeos, sonidos e imágenes, deben incluirse en el archivo del paquete.
* El contenido interactivo debe incluir el archivo principal (index.html, index.htm). Si este archivo no se coloca en la ubicación raíz, la herramienta busca automáticamente en la carpeta para encontrarlo. No es necesario que el nombre del archivo principal sea index.html/index.htm; sin embargo, sólo puede haber un archivo .html/.htm ubicado en la ubicación principal.
* El archivo debe contener al menos una página web de archivo estático.
* El tamaño máximo de paquete es 500 MB.
* En el caso de los archivos .zip creados en iOS, la herramienta identifica automáticamente la carpeta en la que se encuentra el contenido.
* Los proyectos interactivos solo se admiten como archivos .zip. Los envíos de archivos .zip estándar fallarán.
* El sitio web debe ser seguro (HTTPS).

  Esto no es un requisito al usar el Visor de corrección de escritorio.

  Para obtener más información, consulte [Comprender el Visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Se debe permitir que el sitio web se vea en un iframe.

  Esto no es un requisito al usar el Visor de corrección de escritorio.

  Para obtener más información, consulte [Comprender el Visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Creación de una prueba interactiva

Después de preparar el archivo del paquete ZIP, cree una prueba interactiva.

Para obtener más información, consulte [Crear una prueba para contenido interactivo en un archivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

O bien, si está usando Workfront Proof, vea la sección [Generar una revisión para contenido interactivo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) en el artículo [Generar revisiones en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Acerca de la revisión de pruebas interactivas

Le recomendamos que utilice el Visor de pruebas de escritorio independiente como visor predeterminado para las pruebas interactivas. Sin embargo, si las políticas de su organización no permiten el uso de la aplicación Desktop Proofing Viewer, su administrador de Workfront puede configurar su sistema para que pueda revisar el contenido interactivo, incluido en un archivo ZIP, en el visualizador de pruebas web. Para obtener información comparativa acerca del Visor de corrección de escritorio y el Visor de corrección de Web, vea [Diferencias entre el Visor de corrección de Web y la descripción general del Visor de corrección de escritorio](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
