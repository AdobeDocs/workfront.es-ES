---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Solucionar errores de creación de pruebas
description: El proceso de creación de pruebas incluye la importación y la generación de pruebas. En ocasiones, al crear una prueba, es posible que un archivo no se pueda importar o que la prueba no se genere después de importar el archivo.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Solucionar errores de creación de pruebas

El proceso de creación de pruebas incluye la importación y la generación de pruebas. En ocasiones, al crear una prueba, es posible que un archivo no se pueda importar o que la prueba no se genere después de importar el archivo.

>[!NOTE]
>
> Si el documento que intenta revisar no coincide con ninguno de los criterios enumerados en esta sección, póngase en contacto con el soporte técnico de Adobe Workfront para obtener más información.

## Razones del error de importación

* Ha creado una prueba combinada que contiene más de 50 archivos.

## Razones del error de generación de pruebas

* No se admite el tipo de archivo.\
  Para obtener una lista de los tipos de archivo admitidos, vea [Información general sobre los tipos de archivo de revisión admitidos y los límites de tamaño](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La estructura de archivos es una estructura no estándar para el tipo de archivo.
* El archivo está protegido con una contraseña o tiene deshabilitada la copia de contenido.

  A diferencia de otros tipos de archivos, los archivos de PDF se pueden generar en pruebas si la configuración de seguridad para copiar contenido está establecida en Permitido en el PDF.

* La longitud o el recuento de páginas supera el límite.

  La longitud máxima de página permitida es de 195 pulgadas después de la rasterización; el recuento máximo de páginas permitido es de 1000 páginas para una sola prueba.

* El archivo está dañado.
* La fecha límite del flujo de trabajo para una nueva versión de prueba es anterior.

  Esto ocurre cuando está creando una nueva versión de revisión mediante un método de revisión rápida y **Generar automáticamente revisiones al cargar documentos** está seleccionado. La nueva versión de prueba intenta tomar los plazos del flujo de trabajo de la prueba generada anteriormente. La generación de pruebas falla si estos plazos ya han vencido. Para solucionarlo, puede establecer los plazos del flujo de trabajo en la versión anterior en el futuro o generar una nueva versión de la prueba. Si genera una nueva versión, use **Más > Nueva versión > Prueba** y seleccione **Plazos del flujo de trabajo en el futuro**.

* Al revisar los archivos del PDF, los motivos del error de generación de pruebas incluyen:

   * Las fuentes y las imágenes están vinculadas desde fuentes externas (como el sistema de archivos local)

     Las fuentes y las imágenes deben incrustarse en el archivo del PDF para poder mostrarse en otro equipo o dentro de Workfront Proof.

   * El archivo de PDF contiene capas vacías o campos transparentes o superpuestos.

     Si no puede determinar qué capa u objeto causa esto, exporte el diseño/documento como un PDF optimizado (se eliminan todos los elementos no deseados).

