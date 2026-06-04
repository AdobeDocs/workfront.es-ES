---
product-area: documents
navigation-topic: approvals
title: Introducción al Revisor de contenido de Workfront
description: Utilice el colaborador de IA del revisor de contenido de Workfront para evaluar el contenido con respecto a las directrices de marca durante los flujos de trabajo de revisión y aprobación.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 775
ht-degree: 4%

---

# Introducción al Revisor de contenido de Workfront

El revisor de contenido es un colaborador de IA, un tipo de agente de IA que se puede agregar a sus proyectos, tareas y documentos. Los colaboradores de IA se pueden configurar en el área de Configuración y asignar igual que los usuarios.

En Workfront, el Revisor de contenido ayuda a aumentar la velocidad del contenido y mejorar el cumplimiento de la marca a lo largo del proceso de revisión y aprobación. Puede agregar revisores de contenido a las plantillas de aprobación o incluirlos en solicitudes de revisión y aprobación individuales.

## Requisitos de acceso

Para configurar revisores de contenido en Workfront, debe ser administrador del sistema.

Cualquier usuario puede agregar el Revisor de contenido a una solicitud de revisión y aprobación.

## Requisitos

* La instancia de Workfront debe tener habilitadas las aprobaciones unificadas.
* Su organización debe tener GenStudio Foundation.
   * El Revisor de contenido de Workfront proporciona la funcionalidad disponible en GenStudio Foundation para los flujos de trabajo de revisión y aprobación de recursos. No es necesario que acceda directamente a GenStudio Foundation para completar su trabajo. El acceso a la funcionalidad de GenStudio Foundation a través del Revisor de contenido se encuentra dentro de los términos del contrato de Workfront.
* Adobe debe tener registrado un acuerdo de Adobe Gen AI.
Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* El revisor de contenido no está disponible en entornos de espacio aislado.


## Tipos de archivos compatibles {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Tipo de archivo no compatible"
>abstract="Este revisor de contenido no admite el tipo de archivo seleccionado. Cargue un tipo de archivo admitido o quite el revisor de contenido para enviar la solicitud."

El Revisor de contenido puede revisar los siguientes tipos de archivos:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF no animado (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Si carga un tipo de archivo no compatible, la opción Revisor de contenido no estará disponible al crear un flujo de trabajo de aprobación.

## Configurar directrices de marca

El Revisor de contenido de Workfront utiliza las directrices de marca al revisar el contenido. Los administradores de Workfront pueden configurar las directrices de marca en el área Configuración de Workfront. Las marcas creadas en GenStudio Foundation también están disponibles en Workfront.

Para configurar las directrices de marca, los administradores del sistema deben:

1. [Conceder acceso a los permisos de marca](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Cree y administre marcas para el revisor de contenido](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Crear revisores de contenido

Una vez que se ha configurado al menos una marca, los administradores de Workfront pueden empezar a crear revisores de contenido en el área de configuración. Puede crear varios revisores de contenido centrados en diferentes directrices:

* **Imagen**: este revisor de contenido revisará el recurso en relación con las directrices de marca de imagen que configuró en Workfront. [!BADGE Beta]{type=Positive tooltip="Esta función se encuentra actualmente en fase beta."}
   * Los administradores del sistema deben firmar el acuerdo beta para habilitar esta función.
* **Voz de marca**: el revisor de contenido revisará el recurso en relación con las directrices de voz de marca que configuró en Workfront.

Los revisores de contenido se pueden asignar a plantillas de aprobación y a solicitudes de revisión y aprobación individuales.

Para obtener más información, consulte [Configuración de colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Agregar revisores de contenido para revisar y aprobar solicitudes

Los usuarios pueden agregar revisores de contenido a plantillas de aprobación existentes o a solicitudes de revisión y aprobación individuales.

### Plantillas de aprobación

Si su organización agrega con frecuencia las mismas personas a las solicitudes de revisión y aprobación, los usuarios de licencias estándar pueden crear plantillas de aprobación en el área Configuración de Workfront.

Los usuarios pueden añadir revisores de contenido a las plantillas de aprobación para comprobar automáticamente si la marca cumple los requisitos cuando se utiliza una plantilla para crear una solicitud.

Una vez creadas, las plantillas de aprobación se pueden aplicar a los recursos del área Documentos de un proyecto, tarea o problema.

Para obtener más información, consulte [Crear una plantilla de flujo de trabajo de aprobación para los documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![lista de plantillas que muestra revisores de IA](assets/ai-review-templates.png)

### Solicitud de revisión y aprobación individual

Cuando los usuarios crean solicitudes de revisión y aprobación individuales, pueden agregar un Revisor de contenido con otros participantes o pueden crear una única solicitud únicamente con el Revisor de contenido para comprobar la conformidad de la marca.

Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Se agregó un revisor de contenido a la solicitud de aprobación individual](assets/new-stage.png)

## Ver puntuación y comentarios del revisor de contenido

Segundos después de enviar la solicitud de revisión y aprobación con un revisor de contenido, la puntuación y los comentarios del revisor de contenido están disponibles en el panel Resumen del documento, aunque otros participantes sigan revisando y tomando decisiones.

Los propietarios de aprobación también reciben un correo electrónico que les notifica que se ha completado una revisión del recurso. En el correo electrónico, haz clic en **Ir a revisar** y ver la puntuación y los comentarios en Workfront.

El Revisor de contenido no está diseñado para tomar decisiones en el flujo de trabajo de revisión y aprobación. Solo proporciona una puntuación y recomendaciones para alinear el recurso con los requisitos de marca especificados.

Si el recurso no cumple las directrices de marca, el creativo puede cargar una nueva versión y el propietario de la aprobación puede crear una segunda solicitud de revisión y aprobación con el revisor de contenido.

Para obtener más información sobre la visualización de puntuaciones y comentarios, consulte [Ver puntuación y comentarios del revisor de contenido](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

