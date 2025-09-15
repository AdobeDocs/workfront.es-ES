---
product-area: documents
navigation-topic: approvals
title: Información general sobre la integración de Frame.io
description: Información general sobre la integración de Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Información general sobre la integración de Frame.io

La integración de Workfront y Frame.io permite a los coordinadores de proyectos administrar proyectos y planificar el trabajo en Workfront, mientras que los creativos, los especialistas en marketing y las partes interesadas pueden revisar y aprobar los recursos en Frame.io.

## Basado en Adobe Enterprise Storage Management

El núcleo de esta integración es Adobe Enterprise Storage Management (ESM), una solución de almacenamiento basada en la nube que sirve como repositorio central para los activos de los productos empresariales de Adobe, incluidos Workfront y Frame.io.

Entre las ventajas clave de la gestión de almacenamiento empresarial de Adobe se incluyen:

* Capa de almacenamiento unificada para recursos creativos y de administración de trabajo
* Permisos centralizados a través de Adobe IMS para el control de acceso seguro
* Visibilidad completa de los recursos en las aplicaciones de Workfront, Frame.io y Creative Cloud <!--coming soon?-->
* Almacenamiento escalable y administración de cuotas para las necesidades empresariales

Para obtener más información, consulte [Información general sobre la administración de almacenamiento empresarial de Adobe](help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisión y aprobación unificadas

La integración de Workfront y Frame.io utiliza la funcionalidad de aprobación unificada de Workfront para administrar revisiones y aprobaciones. Con las aprobaciones unificadas, puede:

* Cree y administre revisiones y aprobaciones directamente desde Workfront
* Seguimiento del estado de las revisiones y aprobaciones en tiempo real
* Centralice los comentarios y las aprobaciones en un solo lugar
* Asegúrese de que todas las partes interesadas tengan acceso a las versiones más recientes de los recursos
* Utilice los revisores de IA para automatizar las revisiones de cumplimiento de marca
* y más

Para obtener más información, consulte [Aprobaciones de documentos unificados: índice de artículo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Uso del visor Frame.io

La integración también se conecta con el visor Frame.io. El visor Frame.io proporciona

* Herramientas de marcado y comentarios
* Historial y comparación de versiones
* Comentarios con marca de tiempo para críticas de vídeo
* Acceso móvil para revisiones y aprobaciones sobre la marcha

Para obtener más información, consulte [Introducción a la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Limitaciones de revisión de vídeo

<!--need to confirm these-->

#### Tipos de archivo compatibles con el visor Frame.io

El visor Frame.io es compatible con todos los tipos comunes de vídeo, imagen, audio, PDF y MS® Office. Para obtener una lista detallada de los archivos compatibles, consulte [Tipos en Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acceso y licencias para el visor Frame.io

El visor Frame.io está disponible para todos los usuarios de Workfront con una licencia de pago. No se requiere ninguna licencia Frame.io adicional para utilizar el visor Frame.io para revisiones y aprobaciones con esta integración.

Si su organización desea aprovechar las ventajas de la funcionalidad Frame.io adicional, como cargar recursos directamente en proyectos en Frame.io, puede adquirir una licencia empresarial de Frame.io. <!--link to Frame.io enterprise license info or who to contacT?-->

La funcionalidad de revisión de Workfront no está disponible con esta integración.

## Potente administración de proyectos en Workfront

Con la integración de Workfront y Frame.io, los coordinadores de proyectos pueden aprovechar las potentes capacidades de administración de proyectos de Workfront para planificar, rastrear y administrar el trabajo.

Para obtener más información acerca de la administración de proyectos en Workfront, vea [Proyectos: índice de artículos](/help/quicksilver/manage-work/projects/projects-toc.md).

### Convenciones de nomenclatura y estructura forzadas

Debido a que esta integración se crea mediante ESM, existen algunas convenciones de estructura y nomenclatura obligatorias que se deben tener en cuenta al administrar proyectos y documentos.

* Los nombres de objeto deben ser únicos y no se pueden duplicar
* ESM requiere nombres únicos para los objetos del mismo nivel con el mismo elemento principal en el árbol de jerarquías
* Los documentos no pueden tener el mismo nombre si pertenecen al mismo proyecto

Teniendo en cuenta estas limitaciones, Workfront cambia automáticamente el nombre de los objetos o documentos según sea necesario para evitar conflictos.

### Administración de documentos en Workfront

Los documentos se administran en el nivel de proyecto con esta integración y no se pueden cargar en tareas o problemas en este momento.

El acceso a los documentos también se administra en el nivel de proyecto. Si un usuario tiene acceso a un proyecto, puede acceder a todos los documentos asociados con ese proyecto.

<!--Documents can't be dragged as full folders.-->

### Documentar las limitaciones de experiencia

Debido a que esta integración se crea mediante ESM, existen algunas limitaciones para la experiencia del documento original en Workfront:

#### Limitaciones

En esta integración no se incluirán las siguientes capacidades:

* Proveedores de documentos externos
* Acceso a pruebas
* Visualizador de documentos en Workfront


#### Limitaciones temporales

Por ahora, las siguientes capacidades no están disponibles:

* Documentos favoritos
* Solicitar documentos
* Envío de documentos a Adobe Experience Manager Assets
* Aprobaciones en varias etapas
* Cargar documentos a comentarios o actualizaciones en Workfront
* Cargar documentos a tareas o problemas en Workfront



