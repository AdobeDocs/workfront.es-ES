---
product-area: documents
navigation-topic: approvals
title: Resumen de revisión y aprobación unificadas
description: Obtenga más información acerca de la revisión y aprobación unificadas con tecnología Workfront y Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: d35e6c33479ed051aaa87b07ddf38811fffc0cc0
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# Resumen de revisión y aprobación unificadas

La revisión y aprobación unificadas con tecnología Workfront y Frame.io permiten a los coordinadores de proyectos administrar proyectos y planificar el trabajo en Workfront, mientras que los creativos, los especialistas en marketing y las partes interesadas pueden revisar y aprobar los recursos en Frame.io.

## Requisitos de integración

* Workfront y Frame.io deben implementarse en la misma organización de Identity Management system (IMS).

* Los usuarios solo pueden pertenecer a una instancia de Workfront dentro de la organización IMS.

* La instancia de Workfront debe habilitarse en la experiencia unificada de Adobe y en el almacenamiento empresarial de Adobe.

* Adobe Professional Services debe configurar la integración.


## Basado en el almacenamiento empresarial de Adobe

La revisión y aprobación unificadas se basan en el almacenamiento empresarial de Adobe, una solución de almacenamiento basada en la nube que sirve como repositorio central de recursos en los productos empresariales de Adobe, incluidos Workfront y Frame.io. <!--, and Creative Cloud.-->

Entre las ventajas clave del almacenamiento empresarial de Adobe se incluyen:

* Capa de almacenamiento unificada para recursos creativos y de administración de trabajo
* Permisos centralizados con el sistema Adobe Identity Management (IMS) para el control de acceso seguro
* Visibilidad completa de recursos entre Workfront y Frame.io <!--, and Creative Cloud apps -->
* Almacenamiento escalable y administración de cuotas para las necesidades empresariales

Para obtener más información, consulte [Información general sobre el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisión y aprobación unificadas

Con la revisión y la aprobación unificadas, puede:

* Cree y administre revisiones y aprobaciones directamente desde Workfront
* Seguimiento del estado de las revisiones y aprobaciones en tiempo real
* Centralice los comentarios y las aprobaciones en un solo lugar
* Asegúrese de que todas las partes interesadas tengan acceso a las versiones más recientes de los recursos
* Utilice los revisores de IA para automatizar las revisiones de cumplimiento de marca
* y más

Para obtener más información, consulte [Aprobaciones de documentos unificados: índice de artículo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Uso del visor Frame.io

Utilice el visor de Frame.io para revisar y aprobar recursos. El visor Frame.io proporciona

* Herramientas de marcado y comentarios
* Historial y comparación de versiones
* Comentarios con marca de tiempo para críticas de vídeo
* Acceso móvil para revisiones y aprobaciones sobre la marcha

Para obtener más información, consulte [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Límites de revisión de vídeo

Hay un límite anual para las solicitudes de revisión de vídeo establecido en el 10 % del total de licencias de usuario de Workfront pagadas de una organización: Estándar y Ligeras. Este límite se aplica en el nivel de organización.

Los administradores de Workfront reciben notificaciones cuando el uso alcanza el 80 % y el 100 % del límite.

Este límite no se aplica a los clientes de Frame.io Enterprise.

#### Tipos de archivo compatibles con el visor Frame.io

El visor Frame.io es compatible con todos los tipos comunes de vídeo, imagen, audio, PDF y MS® Office. Para obtener una lista detallada de los archivos compatibles, consulte [Tipos de archivo compatibles en Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acceso y licencias para el visor Frame.io

El visor Frame.io es el visor predeterminado para todos los flujos de trabajo de revisión y aprobación de Workfront. Se incluye automáticamente para todos los usuarios de Workfront con una licencia de pago. No se requiere ninguna licencia adicional de Frame.io para utilizar el visor de Frame.io en las revisiones y aprobaciones.

Si su organización desea aprovechar las ventajas de la funcionalidad Frame.io adicional disponible con esta integración, como cargar recursos directamente en proyectos en Frame.io, puede adquirir una licencia de Frame.io Enterprise. Póngase en contacto con su representante de cuentas de Adobe para programar una demostración y explorar las ventajas de la solución Frame.io completa.

La funcionalidad de revisión de Workfront no está disponible con esta integración.

## Potente administración de proyectos en Workfront

Los coordinadores de proyectos pueden aprovechar las potentes funciones de administración de proyectos de Workfront para planificar, rastrear y administrar el trabajo.

Para obtener más información acerca de la administración de proyectos en Workfront, vea [Proyectos: índice de artículos](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Convenciones de nomenclatura y estructura forzadas

Debido a que la revisión y la aprobación unificadas se crean mediante el almacenamiento empresarial de Adobe, hay algunas convenciones de estructura y nomenclatura obligatorias que se deben tener en cuenta al administrar proyectos y documentos.

* Los nombres de objeto deben ser únicos y no se pueden duplicar
* El almacenamiento empresarial de Adobe requiere nombres únicos para objetos del mismo nivel con el mismo elemento principal en el árbol de jerarquías
* Los documentos no pueden tener el mismo nombre si pertenecen al mismo proyecto
* Los nombres de documento no pueden contener ninguno de los siguientes caracteres especiales: \ / : * ? &quot; | &lt; >
* Los nombres de documento están limitados a un máximo de 255 caracteres

Teniendo en cuenta estas limitaciones, Workfront cambia automáticamente el nombre de los objetos o documentos según sea necesario para evitar conflictos.

### Uso compartido y permisos

Como parte de la integración, los permisos de usuario se controlan en Workfront y fluyen a Frame.io. Esto significa que no puede invitar a un usuario a un proyecto en Frame.io ni modificar los permisos de usuario en Frame.io. Estas acciones deben realizarse mediante el modal Uso compartido de proyectos en Workfront.

En la tabla siguiente se muestra cómo se asignan los permisos de Workfront a los permisos de Frame.io:

<table>
<tr>
<th>Permiso de usuario de Workfront</th>
<th>Permiso de usuario de Frame.io</th>
</tr>
<tr>
<td>Administrar</td>
<td>Editar y compartir</td>
</tr>
<tr>
<td>Aportar</td>
<td>Editar y compartir</td>
</tr>
<tr>
<td>Ver</td>
<td>Solo comentario</td>
</tr>
</table>



### Administración de documentos en Workfront

Los documentos cargados en Workfront se almacenan en Adobe enterprise storage y se puede acceder a ellos desde Workfront y Frame.io. Al cargar un documento en una tarea o un problema de Workfront, se crea una carpeta generada por el sistema en Adobe Enterprise Storage que hereda los permisos de la tarea o el problema. Todos los documentos cargados en esa tarea o problema se almacenan en esa carpeta y heredan los permisos de ella. Para obtener más información sobre los documentos de Workfront, consulte [Información general sobre el área de nuevos documentos](/help/quicksilver/documents/managing-documents/documents-area.md) y [Permisos de objetos e información general sobre el nivel de acceso para el modelo de almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Documentar las limitaciones de experiencia

No se incluyen las siguientes capacidades de documentos:

<!--* External document providers-->
* Acceso a la revisión en Workfront
* Visualizador de documentos en Workfront
* Documentos favoritos
* Solicitar documentos










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->