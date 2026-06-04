---
product-area: documents
navigation-topic: proofing-overview
title: Información general del reprocesamiento de documentos para revisión
description: Cuando envía un documento (DOCX, PDF, XLSX, AI) para revisión, Adobe Workfront lo reprocesa para que se pueda visualizar en el visor de revisión sin necesidad de la aplicación de software que utilizó para crearlo.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
TQID: https://experienceleague.adobe.com/giMfktfCHbpzATLm-1ZrKi1bkoc4OeFlAqXYu-YWQtA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 632
ht-degree: 99%

---

# Información general del reprocesamiento de documentos para revisión

Cuando envía un documento (DOCX, PDF, XLSX, AI) para revisión, Adobe Workfront lo reprocesa para que se pueda visualizar en el visor de revisión sin necesidad de la aplicación de software que utilizó para crearlo. 

Cada página del documento aparece en el visor de revisión como una imagen en miniatura. Al hacer clic en una miniatura, puede ampliar una versión de mapa de bits de esa página al 100, 200 y 400 %. Para pruebas que superen los 800 mm de altura o anchura, el nivel de zoom máximo es del 200%.

Los colores de su documento se muestran en sRGB con conversión de color de la última biblioteca de Adobe. El visor de revisión admite cualquier perfil del Consorcio Internacional del Color (ICC) incrustado en el documento.

Todo el texto de la fuente se extrae en su capa siempre que se incluya la extensión de archivo correcta al cargar el documento en el sistema. El texto incluido como imágenes o curvas no se muestra.

>[!NOTE]
>
>Workfront admite actualmente documentos que contienen hasta 2000 páginas. Esto incluye pruebas combinadas. Para obtener más información, consulte [Crear una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Sugerencias generales

* Como los archivos de PDF son los más estandarizados y fiables, recomendamos convertir los documentos a este formato antes de cargarlos.
* Utilice la última versión posible del software para crear los documentos originales.
* Si no está seguro de qué configuraciones usar al guardar o exportar sus documentos en la aplicación donde los creó, utilice las configuraciones predeterminadas. 
* Asegúrese de incrustar todas las fuentes que utilice en un documento dentro de él. Si utiliza fuentes personalizadas, el documento sólo las mostrará en los equipos en los que estén instaladas. Sin embargo, dado que las fuentes personalizadas no están incluidas en el sistema de revisión, no se pueden usar fuentes personalizadas al generar el archivo, incluso cuando están incrustadas.
* Si es posible, coloque todos los elementos de texto en las capas superiores del diseño. Esto debe garantizar que el texto se extraiga y se pueda seleccionar en la herramienta Anotación de texto.
* Coloque todas las imágenes y elementos del documento dentro de él. Si los vincula desde fuentes externas, como otro archivo del equipo, no se mostrarán en la prueba que cree.
* Cree su documento utilizando los estándares recomendados para su tipo y optimícelo antes de cargarlo. Esto garantizará que el documento se abra correctamente en el visualizador de revisiones, así como en todas las demás aplicaciones y plataformas.
* En el software de diseño, intente ejecutar las opciones de &quot;comprobación preliminar&quot; para ver si el documento genera advertencias. Estas opciones están disponibles en la mayoría de las aplicaciones como previsualización de salida, producción de impresión, etc. Consulte la documentación de su aplicación para obtener más información.
* Asegúrese de que la configuración de color sea coherente en todo el documento.
* Si su documento está protegido contra acciones como la copia de archivos, la herramienta de extracción de revisión puede no ser capaz de acceder a su contenido.

## Tiempos del proceso

Normalmente, el procesamiento tarda unos segundos por página. Sin embargo, varios factores pueden prolongar esto, como el tráfico de red/ancho de banda, la velocidad de conexión local y la velocidad de conexión internacional (para usuarios fuera de los EE. UU.). Lo siguiente también puede afectar al tiempo de procesamiento:

* Para documentos e imágenes estáticos: recuento de páginas, dimensiones de página, volumen de texto, complejidad de imágenes y objetos (elementos como varios elementos vectoriales, capas, transparencias).
* Para videos: largas duraciones, grandes dimensiones y códecs utilizados.
* Para capturas web: tiempos de carga de páginas web y dimensiones de página.

## Pasos del proceso

Los archivos enviados siguen algunos o todos los pasos siguientes:

1. **Envío**. Al cargar un documento en el sistema, lo hace mediante la página Nueva prueba o mediante una interfaz de programación de aplicaciones (API). 
1. **Cola**. Durante períodos de mucho tráfico, es posible que Workfront tenga que poner en cola los envíos para evitar sobrecargar el sistema. La mayoría de las pruebas solo permanecen unos segundos en cola. 
1. **Procesamiento.** Los archivos llegan a los equipos de procesamiento según el tipo de contenido. Utilizamos diferentes herramientas para procesar revisiones de videos, capturas web, imágenes estáticas y documentos. Los contenedores de medios enriquecidos (ZIP) y los envíos de capturas web interactivas no requieren procesamiento.
