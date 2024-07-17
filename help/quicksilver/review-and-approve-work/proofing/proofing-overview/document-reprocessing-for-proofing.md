---
product-area: documents
navigation-topic: proofing-overview
title: Resumen del reprocesamiento de documentos para revisión
description: Al enviar un documento (DOCX, PDF, XLSX, AI) para su revisión, Adobe Workfront lo vuelve a procesar de modo que se pueda mostrar en el visor de revisión sin la aplicación de software utilizada para crearlo.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Resumen del reprocesamiento de documentos para revisión

Al enviar un documento (DOCX, PDF, XLSX, AI) para su revisión, Adobe Workfront lo vuelve a procesar de modo que se pueda mostrar en el visor de revisión sin la aplicación de software utilizada para crearlo. 

Cada página del documento aparece en el visor de revisión como una imagen en miniatura. Al hacer clic en una miniatura, puede ampliar una versión de mapa de bits de esa página al 100%, 200% y 400%. Para pruebas que superen los 800 mm de altura o anchura, el nivel de zoom máximo es del 200%.

Los colores del documento se muestran en sRGB con la conversión de color de la biblioteca de Adobes más reciente. El visor de revisión admite cualquier perfil del Consorcio internacional de color (ICC) incrustado en el documento.

Todo el texto de la fuente se extrae en su capa siempre que se incluya la extensión de archivo correcta al cargar el documento en el sistema. El texto incluido como imágenes o curvas no se muestra.

>[!NOTE]
>
>Workfront admite actualmente documentos que contienen hasta 2000 páginas. Esto incluye pruebas combinadas. Para obtener más información, consulte [Crear una revisión de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Sugerencias generales

* Como los archivos de PDF son los más estandarizados y fiables, recomendamos convertir los documentos a este formato antes de cargarlos.
* Utilice la última versión posible del software para crear los documentos originales.
* Si no está seguro de qué configuración utilizar al guardar o exportar los documentos en la aplicación donde los creó, utilice la configuración predeterminada. 
* Asegúrese de incrustar todas las fuentes que utilice en un documento dentro de él. Si utiliza fuentes personalizadas, el documento sólo las mostrará en los equipos en los que estén instaladas. Sin embargo, como las fuentes personalizadas no están incluidas en el sistema de prueba, no puede utilizarlas al generar el archivo, ni siquiera cuando están incrustadas.
* Si es posible, coloque todos los elementos de texto en las capas superiores del diseño. Esto debe garantizar que el texto se extraiga y se pueda seleccionar en la herramienta Anotación de texto.
* Coloque todas las imágenes y elementos del documento dentro de él. Si los vincula desde fuentes externas, como otro archivo del equipo, no se mostrarán en la prueba que cree.
* Cree su documento utilizando los estándares recomendados para su tipo y optimícelo antes de cargarlo. Esto garantizará que el documento se abra correctamente en el visualizador de pruebas, así como en todas las demás aplicaciones y plataformas.
* En el software de diseño, intente ejecutar las opciones de &quot;comprobación preliminar&quot; para ver si el documento genera advertencias. Estas opciones están disponibles en la mayoría de las aplicaciones como previsualización de salida, producción de impresión, etc. Consulte la documentación de la aplicación para obtener más información.
* Asegúrese de que la configuración de color sea coherente en todo el documento.
* Si el documento está protegido frente a acciones como la copia de archivos, es posible que la herramienta de extracción de revisión no pueda acceder a su contenido.

## Tiempos del proceso

Normalmente, el procesamiento tarda unos segundos por página. Sin embargo, varios factores pueden prolongar esto, como el tráfico/ancho de banda de la red, las velocidades de conexión local y las velocidades de conexión internacional (para usuarios fuera de Estados Unidos). Lo siguiente también puede afectar al tiempo de procesamiento:

* Para documentos e imágenes estáticos: recuento de páginas, dimensiones de página, volumen de texto, complejidad de imágenes y objetos (elementos como varios elementos vectoriales, capas, transparencias).
* Para vídeos: duraciones largas, dimensiones grandes y códecs utilizados.
* Para capturas web: tiempos de carga de páginas web y dimensiones de página.

## Pasos del proceso

Los archivos enviados siguen algunos o todos los pasos siguientes:

1. **Envío**. Al cargar un documento en el sistema, lo hace mediante la página Nueva prueba o mediante una interfaz de programación de aplicaciones (API). 
1. **Cola**. Durante períodos de mucho tráfico, es posible que Workfront tenga que poner en cola los envíos para evitar sobrecargar el sistema. La mayoría de las pruebas solo permanecen unos segundos en cola. 
1. **Procesando.** Los archivos llegan a los equipos de procesamiento según el tipo de contenido. Utilizamos diferentes herramientas para procesar pruebas de vídeo, capturas web, imágenes estáticas y documentos. Los contenedores de medios enriquecidos (ZIP) y los envíos de capturas web interactivas no requieren procesamiento.
