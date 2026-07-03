---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Solucionar errores de creación de pruebas
description: El proceso de creación de pruebas incluye la importación y la generación de pruebas. A veces, al crear una prueba, es posible que no se importe un archivo o que no se genere la prueba después de importar el archivo.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 100%

---


# Solucionar errores de creación de pruebas

El proceso de creación de pruebas incluye la importación y la generación de pruebas. A veces, al crear una prueba, es posible que no se importe un archivo o que no se genere la prueba después de importar el archivo.

>[!NOTE]
>
> Si el documento que está intentando probar no coincide con ninguno de los criterios enumerados en esta sección, póngase en contacto con el servicio de asistencia de Adobe Workfront para obtener más información.

## Razones del error de la importación

* Ha creado una prueba combinada que contiene más de 50 archivos.

## Razones del error de generación de pruebas

* No se admite el tipo de archivo.\
  Para obtener una lista de los tipos de archivo admitidos, consulte [Información general sobre tipos de archivos de revisión admitidos y los límites de tamaño](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La estructura de archivos es una estructura no estándar para el tipo de archivo.
* El archivo está protegido con una contraseña o tiene deshabilitada la copia de contenido.

  A diferencia de otros tipos de archivos, los archivos PDF pueden generarse en pruebas si su configuración de seguridad para la copia de contenido está establecida en permitido en el PDF.

* La longitud o el recuento de páginas supera el límite.

  La longitud máxima de página permitida es de 195 pulgadas tras la rasterización; el número máximo de páginas permitido es de 1.000 páginas para una sola prueba.

* El archivo está dañado o corrupto.
* La fecha límite del flujo de trabajo para una nueva versión de prueba ya ha pasado.

  Esto ocurre cuando se está creando una nueva versión de prueba utilizando un método de prueba rápida y se selecciona **Generar automáticamente revisiones al subir documentos**. La nueva versión de la prueba intenta tomar los plazos del flujo de trabajo de la prueba generada anteriormente. La generación de pruebas falla si estos plazos ya han vencido. Para solucionarlo, puede establecer los plazos del flujo de trabajo en la versión anterior en el futuro o generar una nueva versión de la prueba. Si genera una nueva versión, use **Más > Nueva versión > Prueba** y seleccione **Plazos del flujo de trabajo en el futuro**.

* Al revisar los archivos del PDF, las razones del error de generación de revisiones incluyen:

   * Las fuentes y las imágenes están vinculadas desde fuentes externas (como el sistema de archivos local)

     Las fuentes y las imágenes deben incrustarse en el archivo del PDF para poder mostrarse en otro equipo o dentro de Workfront Proof.

   * El archivo de PDF contiene capas vacías o campos transparentes o superpuestos.

     Si no puede determinar qué capa u objeto es el causante, exporte el diseño/documento como un PDF optimizado (esto elimina todos los elementos no deseados).

