---
product-area: documents
navigation-topic: proofing-overview
title: Resumen del reprocesamiento de documentos para pruebas
description: Cuando envía un documento (DOCX, PDF, XLSX, AI) para pruebas, Adobe Workfront lo vuelve a procesar para que se pueda mostrar en el visor de pruebas sin la aplicación de software que utilizó para crearlo.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Resumen del reprocesamiento de documentos para pruebas

Cuando envía un documento (DOCX, PDF, XLSX, AI) para pruebas, Adobe Workfront lo vuelve a procesar para que se pueda mostrar en el visor de pruebas sin la aplicación de software que utilizó para crearlo. 

Cada página del documento aparece en el visor de pruebas como una imagen en miniatura. Al hacer clic en una miniatura, puede hacer zoom en una versión de mapa de bits de esa página al 100 %, 200 % y 400 %. Para pruebas que superen los 800 mm de altura o anchura, el nivel máximo de zoom es del 200%.

Los colores del documento se muestran en sRGB con la conversión de color de la última biblioteca de Adobes. El visor de pruebas es compatible con cualquier perfil de International Color Consortium (ICC) incrustado en el documento.

Todo el texto de la fuente se extrae en su capa siempre y cuando se incluya la extensión de archivo correcta al cargar el documento en el sistema. El texto incluido como imágenes o curvas no se muestra.

>[!NOTE]
>
>Actualmente, Workfront admite documentos que contienen hasta 2000 páginas. Esto incluye pruebas combinadas. Para obtener más información, consulte [Creación de una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Sugerencias generales

* Dado que los archivos PDF son los más estandarizados y fiables, recomendamos convertir los documentos a este formato antes de cargarlos.
* Utilice la última versión posible del software para crear sus documentos originales.
* Si no está seguro de qué configuración utilizar al guardar o exportar documentos en la aplicación donde los creó, utilice la configuración predeterminada. 
* Asegúrese de incrustar todas las fuentes que utilice en un documento dentro de él. Si utiliza fuentes personalizadas, el documento sólo mostrará esas fuentes en los equipos en los que estén instaladas.
* Si es posible, coloque todos los elementos de texto en las capas superiores del diseño. Esto debería garantizar que el texto se extrae y se pueda seleccionar en la herramienta Anotación de texto .
* Coloque todas las imágenes y elementos del documento dentro de él. Si los vincula desde fuentes externas, como otro archivo del equipo, no aparecerán en la prueba que cree.
* Cree el documento siguiendo los estándares recomendados para su tipo y optimícelo antes de cargarlo. Esto garantizará que el documento se abra correctamente en el visor de pruebas, así como en todas las demás aplicaciones y plataformas.
* En el software de diseño, intente ejecutar las opciones de &quot;comprobación previa&quot; para ver si el documento genera advertencias. Estas opciones están disponibles en la mayoría de las aplicaciones como vista previa de salida, producción de impresión, etc. Consulte la documentación de su aplicación para obtener más información.
* Asegúrese de que los ajustes de color sean coherentes en todo el documento.
* Si el documento está protegido de acciones como copiar archivos, es posible que la herramienta de extracción de pruebas no pueda acceder a su contenido.

## Tiempos de proceso

Normalmente, el procesamiento tarda unos segundos por página. Sin embargo, varios factores pueden prolongar esto, como tráfico de red/ancho de banda, velocidades de conexión local y velocidades de conexión internacional (para usuarios fuera de Estados Unidos). Lo siguiente también puede afectar al tiempo de procesamiento:

* Para documentos e imágenes estáticos: recuento de páginas, dimensiones de página, volumen de texto, imagen y complejidad de objetos (elementos como varios elementos vectoriales, capas, transparencias).
* Para vídeos: duraciones largas, dimensiones grandes y códecs utilizados.
* Para capturas web: tiempos de carga de las páginas web y dimensiones de la página.

## Pasos del proceso

Los archivos enviados siguen algunos o todos los pasos siguientes:

1. **Envío**. Al cargar un documento en el sistema, lo hace mediante la página New proof o utilizando una interfaz de programación de aplicaciones (API). 
1. **Cola**. Durante los períodos de tráfico intenso, es posible que Workfront tenga que poner en cola los envíos para evitar sobrecargar el sistema. La mayoría de las pruebas permanecen solo unos segundos en cola. 
1. **Procesando.** Los archivos llegan a los equipos de procesamiento según el tipo de contenido. Utilizamos diferentes herramientas para procesar pruebas de vídeo, capturas web, imágenes estáticas y documentos. Los contenedores de medios enriquecidos (ZIP) y los envíos de captura web interactiva no requieren procesamiento.
