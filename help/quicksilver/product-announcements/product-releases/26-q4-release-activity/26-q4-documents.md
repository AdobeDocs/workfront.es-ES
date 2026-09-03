---
title: Mejoras en los documentos del cuarto trimestre de 2026
description: Mejoras en los documentos del cuarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '1012'
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

## Agregar equipos a aprobaciones para objetos mediante el almacenamiento en la nube de Adobe

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede agregar un equipo de Workfront como aprobador o revisor en una plantilla de aprobación o aprobación de documento, en lugar de agregar cada persona individualmente:

* Objetos en el almacenamiento en la nube de Adobe: Workfront agrega cada miembro del equipo activo de forma individual, por lo que la lista de aprobadores siempre refleja quién está actualmente en el equipo.
* Objetos que utilizan el almacenamiento heredado de Workfront: El equipo se añade como un solo participante de forma predeterminada, pero ahora puede elegir añadir cada miembro del equipo como un participante individual.
* En las plantillas de aprobación, Workfront almacena una referencia al equipo y la expande a los miembros activos cuando se aplica la plantilla a un documento, no cuando se guarda la plantilla.

Para obtener más información, consulte:

* [Crear un flujo de trabajo de aprobación en la nueva área de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Creación de un flujo de trabajo de aprobación en el área de documentos heredados](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Creación de una plantilla de flujo de trabajo de aprobación para documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

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

## Panel Versiones rediseñadas en el área de nuevos documentos

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Si su organización utiliza el almacenamiento en la nube de Adobe, el panel Versiones del área Nuevos documentos tiene un nuevo diseño:

* Las versiones están etiquetadas como V1, V2, etc. para aumentar la coherencia con Frame.io.
* Cada versión muestra su estado de aprobación, como &quot;Aprobado&quot; o &quot;Retirado&quot;, directamente en la lista.
* El panel ahora solo enumera el historial de versiones; ya no hay una entrada separada de &quot;último archivo&quot; en la parte superior.

Anteriormente, las versiones estaban marcadas con fecha y hora en lugar de numeradas.

Para obtener más información, consulte [Administrar versiones de documentos](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Panel de aprobaciones rediseñado en el área de nuevos documentos

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Si su organización utiliza el almacenamiento en la nube de Adobe, el panel Aprobaciones del área de Nuevos documentos ahora muestra el historial de aprobaciones entre versiones:

* El panel enumera el flujo de trabajo de aprobación para cada versión que tiene uno, no solo la versión actual.
* Los flujos de trabajo retirados permanecen en la lista, por lo que aún puede revisar sus decisiones anteriores.
* Expanda cualquier versión para ver sus etapas, decisiones de aprobador, regla de decisión y fechas de vencimiento sin salir del panel.

Anteriormente, el panel Aprobaciones solo mostraba el flujo de trabajo de la versión actual.

Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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
