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
source-git-commit: c4e1961092883f523d04adaacd58129a0379783d
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Información general sobre la integración de Frame.io

La integración de Workfront y Frame.io permite a los coordinadores de proyectos administrar proyectos y planificar el trabajo en Workfront, mientras que los creativos, los especialistas en marketing y las partes interesadas pueden revisar y aprobar los recursos en Frame.io.

## Basado en el almacenamiento empresarial de Adobe

El núcleo de esta integración es el almacenamiento empresarial de Adobe, una solución de almacenamiento basada en la nube que sirve como repositorio central para los recursos de los productos empresariales de Adobe, incluidos Workfront, Frame.io y Creative Cloud.

Entre las ventajas clave del almacenamiento empresarial de Adobe se incluyen:

* Capa de almacenamiento unificada para recursos creativos y de administración de trabajo
* Permisos centralizados a través de Adobe IMS para el control de acceso seguro
* Visibilidad completa de los recursos en las aplicaciones de Workfront, Frame.io y Creative Cloud <!--coming soon?-->
* Almacenamiento escalable y administración de cuotas para las necesidades empresariales

Para obtener más información, consulte [Información general sobre el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

#### Límites de revisión de vídeo

Las solicitudes de revisión de vídeo tienen un límite anual establecido en el 10 % del total de licencias de usuario Workfront pagadas de una organización (estándar y básica). Este límite se aplica en el nivel de organización.

Los administradores de Workfront recibirán notificaciones cuando el uso alcance el 80 % y el 100 % del límite.

Este límite no se aplica a los clientes de Frame.io Enterprise.

#### Tipos de archivo compatibles con el visor Frame.io

El visor Frame.io es compatible con todos los tipos comunes de vídeo, imagen, audio, PDF y MS® Office. Para obtener una lista detallada de los archivos compatibles, consulte [Tipos en Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acceso y licencias para el visor Frame.io

El visor Frame.io está disponible para todos los usuarios de Workfront con una licencia de pago. No se requiere ninguna licencia Frame.io adicional para utilizar el visor Frame.io para revisiones y aprobaciones con esta integración.

Si su organización desea aprovechar las ventajas de la funcionalidad Frame.io adicional, como cargar recursos directamente en proyectos en Frame.io, puede adquirir una licencia empresarial de Frame.io. Póngase en contacto con su representante de cuentas de Adobe para programar una demostración y explorar las ventajas de la solución Frame.io completa.

La funcionalidad de revisión de Workfront no está disponible con esta integración.

## Potente administración de proyectos en Workfront

Con la integración de Workfront y Frame.io, los coordinadores de proyectos pueden aprovechar las potentes capacidades de administración de proyectos de Workfront para planificar, rastrear y administrar el trabajo.

Para obtener más información acerca de la administración de proyectos en Workfront, vea [Proyectos: índice de artículos](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

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

<!--* External document providers-->
* Acceso a pruebas
* Visualizador de documentos en Workfront
* Documentos favoritos
* Solicitar documentos


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->



