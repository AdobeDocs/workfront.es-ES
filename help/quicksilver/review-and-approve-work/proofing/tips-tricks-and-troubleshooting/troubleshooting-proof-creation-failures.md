---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Solución de problemas de creación de pruebas
description: El proceso de creación de pruebas incluye tanto la importación como la generación de pruebas. En ocasiones, al crear una prueba, es posible que un archivo no se importe o que la prueba no se genere tras la importación del archivo.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Solución de problemas de creación de pruebas

El proceso de creación de pruebas incluye tanto la importación como la generación de pruebas. En ocasiones, al crear una prueba, es posible que un archivo no se importe o que la prueba no se genere tras la importación del archivo.

>[!NOTE]
>
> Si el documento que intenta probar no coincide con ninguno de los criterios enumerados en esta sección, póngase en contacto con el servicio de asistencia técnica de Adobe Workfront para obtener más información.

## Motivos del error de importación

* Ha creado una prueba combinada que contiene más de 50 archivos.

## Razones del error de generación de prueba

* El tipo de archivo no es compatible.\
   Para obtener una lista de los tipos de archivo admitidos, consulte [Información general sobre los tipos de archivos de prueba compatibles y los límites de tamaño](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La estructura de archivos no es estándar para el tipo de archivo.
* El archivo está protegido con contraseña o tiene deshabilitada la copia de contenido.

   A diferencia de otros tipos de archivos, los archivos de PDF se pueden generar en pruebas si la configuración de seguridad para la copia de contenido está definida en Permitido en el PDF.

* La longitud de la página o el recuento de páginas supera el límite.

   La longitud máxima de página permitida es de 195 pulgadas después de la rasterización; el recuento máximo de páginas permitido es de 1000 páginas para una sola prueba.

* El archivo está dañado o dañado.
* La fecha límite del flujo de trabajo para una nueva versión de prueba ya es anterior.

   Esto sucede cuando se crea una nueva versión de prueba con un método de prueba rápida y **Generar pruebas automáticamente al cargar documentos** está seleccionado. La nueva versión de prueba intenta cumplir los plazos del flujo de trabajo desde la prueba generada anteriormente. La generación de pruebas falla si estos plazos están en el pasado. Para remediar esto, puede establecer las fechas límite del flujo de trabajo en la versión anterior en el futuro o generar una nueva versión de prueba. Si genera una nueva versión, utilice **Más > Nueva versión > Prueba** y seleccione **Plazos de flujo de trabajo futuros**.

* Al probar los archivos de PDF, los motivos del error en la generación de pruebas incluyen:

   * Las fuentes y las imágenes están vinculadas desde fuentes externas (por ejemplo, desde el sistema de archivos local)

      Las fuentes y las imágenes deben incrustarse en el archivo PDF para que se muestren en otro equipo o en la prueba de Workfront.

   * El archivo PDF contiene capas vacías o campos transparentes o superpuestos.

      Si no puede determinar qué capa u objeto causa esto, exporte el diseño/documento como un PDF optimizado (de este modo se eliminarán todos los elementos no deseados).

