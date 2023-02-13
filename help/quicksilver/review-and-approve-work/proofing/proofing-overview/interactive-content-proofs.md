---
product-area: documents
navigation-topic: proofing-overview
title: Información general sobre pruebas de contenido interactivo
description: El contenido interactivo ofrece varios métodos para atraer visitantes. Las agencias pueden medir el éxito de sus campañas utilizando análisis recopilados de las respuestas a este contenido.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Información general sobre pruebas de contenido interactivo

El contenido interactivo ofrece varios métodos para atraer visitantes. Las agencias pueden medir el éxito de sus campañas utilizando análisis recopilados de las respuestas a este contenido.

Algunos ejemplos de contenido interactivo son:

* Sitios web
* Vídeos incrustados o de flujo continuo
* Banners interactivos
* animaciones de HTML5
* Micrositios
* Correos electrónicos interactivos

Este artículo proporciona lo siguiente sobre la prueba de contenido interactivo:

## Acerca de la creación de pruebas para contenido interactivo

Puede crear una prueba de contenido interactivo de una de las siguientes maneras:

* Cree una prueba a partir de un archivo ZIP que contenga el contenido interactivo.

   Adobe Workfront descomprime el contenido del archivo ZIP y lo almacena en un servidor de Workfront. Como se almacena de esta manera, puede confiar en que el contenido permanezca igual durante todo el ciclo de revisión de la prueba.

* Especifique la dirección URL para el contenido.

   Esta es la forma más sencilla de crear una prueba de contenido interactivo. Esta es también la única forma de revisar el contenido de forma interactiva, ya que los usuarios lo experimentan en Internet.

   Con este método, un servidor externo desconocido para Workfront almacena y aloja el contenido.

   Recomendamos este método para sitios web grandes porque es difícil reunir todos los archivos que conforman un sitio web grande. Sin embargo, como el contenido de la prueba se almacena de forma externa, Workfront no puede protegerlo de los cambios realizados por los desarrolladores que trabajan en él, por lo que es posible que no pueda confiar en que el contenido permanezca igual durante todo el ciclo de revisión de la prueba.

## Acerca de la preparación de contenido interactivo en un archivo ZIP para pruebas

Cuando agrupe contenido interactivo en un archivo ZIP para pruebas, asegúrese de que incluye las siguientes especificaciones:

* Todos los recursos, como CSS, JavaScript, vídeos, sonidos e imágenes, deben incluirse en el archivo del paquete.
* El contenido interactivo debe incluir el archivo principal (index.html, index.htm). Si este archivo no se coloca en la ubicación raíz, la herramienta busca automáticamente la carpeta para encontrarla. El archivo principal no necesita llamarse index.html/index.htm, sin embargo, solo puede haber un archivo .html/.htm colocado en la ubicación principal.
* El archivo debe contener al menos una página web de archivo estático.
* El tamaño máximo del paquete es de 500 MB.
* En el caso de los archivos .zip creados en iOS, la herramienta identifica automáticamente la carpeta donde se encuentra el contenido
* Los proyectos interactivos solo son compatibles como archivos .zip. Los envíos de archivos .zip estándar fallarán.
* El sitio web debe ser seguro (HTTPS).

   Este no es un requisito cuando se utiliza el Visor de prueba de escritorio.

   Para obtener más información, consulte [Comprender el Visor de pruebas de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Se debe permitir que el sitio web se vea en un iframe.

   Este no es un requisito cuando se utiliza el Visor de prueba de escritorio.

   Para obtener más información, consulte [Comprender el Visor de pruebas de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Acerca de la creación de una prueba interactiva

Después de preparar el archivo del paquete ZIP, cree una prueba interactiva.

Para obtener más información, consulte [Crear una prueba de contenido interactivo en un archivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

O bien, si está utilizando Workfront Proof, consulte la sección [Generar una prueba de contenido interactivo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generati) en el artículo [Generar pruebas en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Acerca de la revisión de pruebas interactivas

Se recomienda utilizar el Visor de prueba de escritorio independiente como visor predeterminado para pruebas interactivas. Sin embargo, si las políticas de su organización no permiten el uso de la aplicación Desktop Proofing Viewer, el administrador de Workfront puede configurar el sistema para que pueda revisar el contenido interactivo, incluido en un archivo ZIP, en el visor de pruebas web. Para obtener información comparativa sobre el Visor de prueba de escritorio y el Visor de prueba web, consulte [Diferencias entre el visor de pruebas web y el visor de pruebas de escritorio](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
