---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Convertir objetos heredados al almacenamiento en la nube de Adobe
description: Conozca los tres casos en los que puede convertir un objeto de almacenamiento de Workfront heredado al almacenamiento en la nube de Adobe y comprender qué se mueve y qué permanece durante cada conversión.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---
# Convertir objetos heredados al almacenamiento en la nube de Adobe

En la mayoría de los casos, los objetos de Workfront solo se pueden mover, copiar y convertir entre modelos de almacenamiento similares. Por ejemplo, puede mover una tarea de un proyecto de almacenamiento en la nube de Adobe a otro proyecto de almacenamiento en la nube Adobe. En tres casos específicos, puede convertir un objeto de almacenamiento de Workfront heredado al almacenamiento en la nube de Adobe:

* Convertir una tarea de almacenamiento de Workfront heredada en un proyecto de almacenamiento en la nube de Adobe
* Conversión de una cartera de productos de almacenamiento de Workfront heredados en una cartera de productos de almacenamiento en la nube de Adobe
* Crear un proyecto de almacenamiento en la nube de Adobe a partir de una plantilla de almacenamiento de Workfront heredada

Para ver la orientación al traslado y las diferencias en el almacenamiento en la nube de Adobe, consulta [Traslado a Workfront en el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## Convertir una tarea heredada en un proyecto de almacenamiento en la nube de Adobe

Para convertir una tarea de almacenamiento de Workfront heredada en un proyecto de almacenamiento en la nube de Adobe, utilice el flujo de conversión a proyecto existente en la tarea. Durante la conversión:

* Las subtareas y los problemas se mueven al nuevo proyecto.
* Los documentos adjuntos a la tarea y sus flujos de trabajo de aprobación permanecen en el proyecto original.
* Se eliminan las aprobaciones de trabajo y los enlaces de objetos de resolución.
* Se elimina la tarea original.

## Conversión de una cartera heredada en una cartera de almacenamiento en la nube de Adobe

Un administrador de Workfront puede convertir una cartera de productos de almacenamiento de Workfront heredados en una cartera de productos de almacenamiento de nube de Adobe desde el área de Configuración. Después de la conversión:

* Ya no puede mover proyectos de almacenamiento de Workfront heredados al portafolio.
* Todos los proyectos nuevos creados en la cartera utilizan el almacenamiento en la nube de Adobe.
* Frame.io es el visor de documentos en los proyectos de almacenamiento en la nube de Adobe del portafolio.
* Los proyectos secundarios que utilizan almacenamiento de Workfront heredado permanecen en el almacenamiento heredado.
* Los programas secundarios permanecen en el almacenamiento heredado.

>[!NOTE]
>
>Un programa secundario heredado se convierte automáticamente en almacenamiento en la nube de Adobe solo cuando alguien le agrega manualmente un proyecto de almacenamiento en la nube de Adobe.

Para obtener más información, consulte [Convertir portafolios heredados al almacenamiento en la nube de Adobe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

## Crear un proyecto de almacenamiento en la nube de Adobe a partir de una plantilla heredada

Cuando crea un proyecto a partir de una plantilla de almacenamiento de Workfront heredada, la casilla de verificación **Crear este proyecto en Adobe Cloud Storage** del cuadro de diálogo de creación de proyectos determina el tipo de almacenamiento del nuevo proyecto. El comportamiento de la casilla de verificación depende de dónde cree el proyecto:

* **Fuera de un portafolio**: la casilla de verificación está disponible y desactivada de forma predeterminada. Selecciónelo para crear el nuevo proyecto en el almacenamiento en la nube de Adobe.
* **Dentro de un portafolio de almacenamiento en la nube de Adobe**: La casilla de verificación está seleccionada y bloqueada. El nuevo proyecto debe coincidir con el tipo de almacenamiento del portafolio.
* **Dentro de un portafolio de almacenamiento de Workfront heredado**: La casilla de verificación no está disponible. El nuevo proyecto utiliza el almacenamiento heredado de Workfront.

Para obtener más información, consulte [Crear proyectos](/help/quicksilver/manage-work/projects/create-projects/create-project.md).
