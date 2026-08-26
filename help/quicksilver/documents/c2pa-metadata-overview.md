---
product-area: documents
navigation-topic: documents-navigation-topic
title: Metadatos de C2PA en Adobe Workfront
description: Descubra qué son los metadatos de C2PA y cómo los conserva Adobe Workfront en los documentos que carga, almacena y descarga.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Metadatos de C2PA en Adobe Workfront

Los metadatos de C2PA son información segura y a prueba de manipulaciones que se transfiere con un fragmento de contenido. Cuando se utiliza IA generativa (GenAI) para crear o modificar un archivo de imagen, vídeo o audio, los metadatos de C2PA registran ese hecho para que cualquier persona que reciba el archivo pueda ver cómo se creó.

Los metadatos de C2PA se basan en el estándar abierto [C2PA](https://c2pa.org/).

## Composición de los metadatos de C2PA

Los metadatos de C2PA incluyen:

* Nombre del proveedor que suministró la herramienta GenAI.
* Nombre y número de versión del sistema GenAI utilizado para crear o modificar el contenido.
* La fecha y la hora en que se creó o alteró el contenido.
* Un identificador único.

Los metadatos de C2PA no incluyen información de identificación personal (PII).

## Cómo gestiona Workfront los metadatos de C2PA

Adobe Workfront no modifica los metadatos de los archivos con los que trabaja. Cuando se carga un archivo que ya contiene metadatos de C2PA, Workfront conserva esa información sin cambios, ya que el archivo se almacena y se descarga desde Workfront.

Como los metadatos están incrustados en el propio archivo, permanecen intactos a través de los flujos de trabajo de Workfront, por lo que la información de procedencia permanece con el contenido cuando sale de Workfront.
