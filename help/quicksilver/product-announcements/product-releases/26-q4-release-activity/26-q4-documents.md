---
title: Mejoras en los documentos del cuarto trimestre de 2026
description: Mejoras en los documentos del cuarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 3%

---

# Mejoras en los documentos del cuarto trimestre de 2026

Esta página describe las mejoras realizadas en los documentos con la versión del cuarto trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del cuarto trimestre de 2026, consulte [Información general de la versión del cuarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## Acceso directo de prueba desde vínculos de correo electrónico de aprobación

>[!NOTE]
>
>Vista previa: N/D
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Cuando un documento tiene una prueba adjunta, el vínculo &quot;Ir a revisión&quot; de los correos electrónicos de aprobación ahora abre el visor de pruebas directamente, para que los revisores y aprobadores puedan iniciar su revisión de inmediato. Si un documento no tiene prueba, el vínculo continúa abriendo la sección Aprobaciones del documento, como antes.

<!--

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

-->

## Establecer un espacio de trabajo de Frame.io en plantillas de proyecto

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Si su organización utiliza el almacenamiento en la nube de Adobe y tiene una licencia de Frame.io Enterprise, ahora puede elegir un espacio de trabajo de Frame.io en Detalles del proyecto, en una plantilla de proyecto. Los proyectos creados a partir de la plantilla utilizan automáticamente el espacio de trabajo definido en la plantilla, por lo que los proyectos se dirigen al espacio de trabajo Frame.io deseado sin necesidad de realizar ninguna acción adicional al crear el proyecto.

El nuevo campo enumera los espacios de trabajo de Frame.io a los que tiene permiso para asignar proyectos. El campo permanece editable en la plantilla en cualquier momento; los cambios se aplican únicamente a los proyectos creados después de la actualización, de modo que los proyectos existentes conservan su espacio de trabajo original.

Una vez creado un proyecto a partir de la plantilla, su campo de espacio de trabajo Frame.io es de solo lectura y está vinculado al espacio de trabajo en Frame.io.

Si no tiene una licencia empresarial de Frame.io, los proyectos seguirán yendo al espacio de trabajo predeterminado para Workfront.

Para obtener más información, consulte [Editar plantillas de proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) y [Administrar información en el área Información general del proyecto](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md).

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## Mensaje personalizado en la línea de asunto del correo electrónico

>[!NOTE]
>
>Vista previa: N/D
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Cuando se establece un mensaje personalizado en la aprobación de un documento, ese mensaje ahora también aparece en la línea de asunto del correo electrónico de solicitud de aprobación, precedido de la fecha de vencimiento cuando se establece una. Esto permite a los revisores ver qué necesita atención y por cuándo directamente desde su bandeja de entrada, sin abrir el correo electrónico.

Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--

## Redesigned Versions panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Versions panel in the new Documents area has a new design:

* Versions are labeled V1, V2, and so on to drive consistency with Frame.io.
* Each version shows its approval status, such as "Approved" or "Withdrawn", directly in the list.
* The panel now lists only Version history — there's no longer a separate "latest file" entry at the top.

Previously, versions were timestamped instead of numbered.

For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Redesigned Approvals panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Approvals panel in the new Documents area now shows approval history across versions:

* The panel lists the approval workflow for every version that has one, not just the current version.
* Withdrawn workflows stay in the list, so you can still review their prior decisions.
* Expand any version to see its stages, approver decisions, decision rule, and due dates without leaving the panel.

Previously, the Approvals panel only showed the current version's workflow.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

-->

## Adjuntar imágenes a comentarios en objetos de almacenamiento de Adobe Cloud

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 30 de julio de 2026
>Producción para todos: 30 de julio de 2026
>[!BADGE Fuera del horario]{type=Neutral}

Las organizaciones que utilizan el almacenamiento en la nube de Adobe como parte de la revisión y aprobación unificadas ahora pueden adjuntar archivos de imagen directamente a los comentarios, manteniendo los comentarios, el contexto y los elementos visuales de soporte juntos en un único hilo de comentarios rastreable. Esto cierra una brecha anterior en la que solo las organizaciones con almacenamiento heredado de Workfront podían adjuntar imágenes a los comentarios.

Todos los formatos de imagen de tipo multimedia ahora son compatibles con las organizaciones de almacenamiento en la nube de Adobe. (Los comentarios de objetos heredados siguen admitiendo archivos .jpg, .gif y .png únicamente). Los archivos que no son de imagen no son compatibles con los comentarios de objetos de almacenamiento heredados o de la nube de Adobe.

Para obtener más información, consulte [Trabajo de actualización](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Vinculación de recursos de Experience Manager Assets con Adobe Cloud Storage

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Si su organización utiliza el almacenamiento en la nube de Adobe, puede vincular recursos individuales de Experience Manager Assets a cualquier objeto de Workfront que admita documentos. El contenido vinculado se sincroniza automáticamente: los cambios realizados en Experience Manager Assets aparecen en Workfront y puede extraer nuevas versiones del recurso sin salir de Workfront.

La vinculación cuenta con la tecnología del Asesor de contenido, por lo que también obtiene Búsqueda por IA, sugerencias inteligentes, análisis breves de campañas y mucho más al seleccionar contenido.

Para obtener más información, consulte [Vincular contenido de Experience Manager Assets con Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md).
