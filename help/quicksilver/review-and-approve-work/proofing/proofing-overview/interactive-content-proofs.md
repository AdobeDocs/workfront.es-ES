---
product-area: documents
navigation-topic: proofing-overview
title: Resumen de las pruebas de contenido interactivo
description: El contenido interactivo ofrece varios métodos para atraer a los espectadores. Las agencias pueden medir el éxito de sus campañas utilizando el análisis recopilado de las respuestas a este contenido.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
TQID: https://experienceleague.adobe.com/y8EiNqvee6b7TAcYVxDMudQgy0njwI0EKG3EvKE-OSQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 604
ht-degree: 100%

---

# Resumen de las pruebas de contenido interactivo

<!-- Audited: 01/2024 -->

El contenido interactivo ofrece varios métodos para atraer a los espectadores. Las agencias pueden medir el éxito de sus campañas utilizando el análisis recopilado de las respuestas a este contenido.

Algunos ejemplos de contenido interactivo son:

* Sitios web
* Vídeos incrustados o de streaming
* Titulares interactivos
* Animaciones HTML5
* Micrositios
* Correos electrónicos interactivos

## Acerca de la creación de pruebas para contenido interactivo

Puede crear una prueba para el contenido interactivo de una de las siguientes maneras:

* Cree una prueba a partir de un archivo ZIP que contenga el contenido interactivo.

  Adobe Workfront desempaqueta el contenido del archivo ZIP y lo almacena en un servidor de Workfront. Como se almacena de esta manera, puede estar seguro de que el contenido permanecerá igual durante todo el ciclo de revisión de la prueba.

* Especifique la URL para el contenido.

  Esta es la forma más sencilla de crear una prueba para el contenido interactivo. También es la única manera de revisar el contenido de forma interactiva, a medida que los usuarios lo experimenten en Internet.

  Con este enfoque, un servidor externo desconocido para Workfront almacena y aloja el contenido.

  Recomendamos este método para sitios web grandes porque es difícil recopilar todos los archivos que forman un sitio web grande. Sin embargo, dado que el contenido de la prueba se almacena de forma externa, Workfront no puede protegerlo de los cambios realizados por los desarrolladores que trabajan en ella, por lo que es posible que no pueda confiar en que el contenido permanezca igual durante todo el ciclo de revisión de la prueba.

## Acerca de la preparación de contenido interactivo en un archivo ZIP para la revisión

Cuando empaquete contenido interactivo en un archivo ZIP para la revisión, asegúrese de incluir las siguientes especificaciones:

* Todos los recursos, como CSS, JavaScript, vídeos, sonidos e imágenes, deben incluirse en el archivo del paquete.
* El contenido interactivo debe incluir el archivo principal (index.html, index.htm). Si este archivo no se coloca en la ubicación raíz, la herramienta busca automáticamente en la carpeta para encontrarlo. No es necesario que el nombre del archivo principal sea index.html/index.htm; sin embargo, solo puede haber un archivo .html/.htm ubicado en la ubicación principal.
* El archivo debe contener al menos una página web de archivo estático.
* El tamaño máximo del paquete es de 500 MB.
* En el caso de los archivos .zip creados en iOS, la herramienta identifica automáticamente la carpeta en la que se encuentra el contenido.
* Los proyectos interactivos solo se admiten como archivos .zip. Los envíos de archivos .zip estándar fallarán.
* El sitio web debe ser seguro (HTTPS).

  Esto no es un requisito cuando se utiliza el Visor de corrección de escritorio.

  Para obtener más información, consulte [Explicación del visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* El sitio web debe poderse ver en un iframe,

  Esto no es un requisito cuando se utiliza el Visor de corrección de escritorio.

  Para obtener más información, consulte [Explicación del visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Acerca de la creación de una prueba interactiva

Después de preparar el archivo del paquete ZIP, cree una prueba interactiva.

Para obtener más información, consulte [Crear una prueba para contenido interactivo en un archivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

O bien, si está usando Workfront Proof, consulte la sección [Generar una prueba para contenido interactivo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) en el artículo [Generar pruebas en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Acerca de la revisión de pruebas interactivas

Le recomendamos que utilice el Visor de corrección de escritorio independiente como visor predeterminado para las revisiones interactivas. Sin embargo, si las políticas de su organización no permiten el uso de la aplicación Visor de corrección de escritorio, su administrador de Workfront puede configurar su sistema para que pueda revisar el contenido interactivo, comprimido en un archivo ZIP, en el visor de corrección web. Para obtener información comparativa sobre el visor de corrección de escritorio y el visor de corrección de web, consulte [Información general sobre las diferencias entre el visor de corrección web y el visor de corrección de escritorio](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
