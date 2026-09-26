---
product-area: documents
navigation-topic: approvals
title: Introducción al Revisor de IA de Workfront
description: Utilice Workfront AI Reviewer para evaluar el contenido con respecto a las directrices de marca durante los flujos de trabajo de revisión y aprobación.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%
---
# Introducción al Revisor de IA de Workfront

AI Reviewer es un colaborador de IA, un tipo de agente de IA que se puede agregar a sus proyectos, tareas y documentos. Los colaboradores de IA se pueden configurar en el área de Configuración y asignar igual que los usuarios.

En Workfront, el revisor de IA ayuda a aumentar la velocidad del contenido y mejorar el cumplimiento de la marca a lo largo del proceso de revisión y aprobación. Puede agregar revisores de IA a las plantillas de aprobación o incluirlos en solicitudes de revisión y aprobación individuales.

## Requisitos de acceso

Para configurar revisores de IA en Workfront, debe ser administrador del sistema.

Cualquier usuario puede agregar el revisor de IA a una solicitud de revisión y aprobación.

## Requisitos

* La instancia de Workfront debe tener habilitadas las aprobaciones unificadas.
* Su organización debe tener GenStudio Foundation.
  * El revisor de IA de Workfront proporciona la funcionalidad disponible en GenStudio Foundation para los flujos de trabajo de revisión y aprobación de recursos. No es necesario que acceda directamente a GenStudio Foundation para completar su trabajo. El acceso a la funcionalidad de GenStudio Foundation a través de AI Reviewer se encuentra dentro de los términos de su contrato de Workfront.
* Adobe debe tener registrado un acuerdo de Adobe Gen AI.
Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* El revisor de IA no está disponible en entornos de espacio aislado.


## Tipos de archivos compatibles {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Tipo de archivo no compatible"
>abstract="Este comprobador por IA no admite el tipo de archivo seleccionado. Cargue un tipo de archivo compatible o elimine el Revisor de IA para enviar la solicitud."

El revisor de IA puede revisar los siguientes tipos de archivos:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF no animado (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Si carga un tipo de archivo no admitido, la opción AI Reviewer no estará disponible al crear un flujo de trabajo de aprobación.

## Configurar directrices de marca

Workfront AI Reviewer utiliza las directrices de marca al revisar el contenido. Los administradores de Workfront pueden configurar las directrices de marca en el área Configuración de Workfront. Las marcas creadas en GenStudio Foundation también están disponibles en Workfront.

Para configurar las directrices de marca, los administradores del sistema deben:

1. [Conceder acceso a los permisos de marca](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Cree y administre marcas para el revisor de IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Creación de comprobadores por IA

Una vez que se ha configurado al menos una marca, los administradores de Workfront pueden empezar a crear revisores de IA en el área de configuración. Puede crear varios revisores de IA centrados en diferentes directrices:

* **Imagen**: este revisor de IA revisará el recurso en relación con las directrices de marca de imagen que configuró en Workfront. [!BADGE Beta]{type=Positive tooltip="Esta función se encuentra actualmente en fase beta."}
  * Los administradores del sistema deben firmar el acuerdo beta para habilitar esta función.
* **Voz de marca**: el revisor de IA revisará el recurso en relación con las directrices de voz de marca que configuró en Workfront.

Los revisores de IA se pueden asignar a plantillas de aprobación y a solicitudes de revisión y aprobación individuales.

Para obtener más información, consulte [Configuración de colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Qué evalúa AI Reviewer {#what-ai-reviewer-evaluates}

El revisor de IA evalúa el contenido de forma diferente en función del tipo de directriz: Imagen o Voz de marca.

### Imagen

AI Reviewer evalúa:

* **Composición**: punto focal, fondo, recorte, marcos creativos
* **Iluminación y estado de ánimo**: uso de luz, vitalidad, optimismo
* **Diversidad e inclusión**: Representación de personas (raza, sexo, edad, capacidad)

El revisor de IA no evalúa:

* **Uso del logotipo**: ubicación, espacio libre, tamaño, versión correcta del logotipo
* **Paleta de color**: compatibilidad con el color de la marca, evitar colores no aprobados
* **Tipografía**: Familia de fuentes, grosores, espaciado, alineación
* **Estilo de ilustración**: coherencia con el enfoque de ilustración de la marca
* **Accesibilidad**: compatibilidad con el contraste, legibilidad

### Voz de marca

AI Reviewer evalúa:

* **Tono de voz**: conversacional, claro, humano, alineado con la personalidad de la marca
* **Jerga/formalidad**: evitar palabras de moda, elitismo o formalidad excesiva
* **Mensajería**: ánimo, honestidad, posicionamiento responsable (por ejemplo, para temas de IA)

El revisor de IA no evalúa:

* **Legal/cumplimiento**: uso de marcas comerciales, exenciones de responsabilidad legal y reglas de localización

Para obtener instrucciones sobre cómo escribir directrices de marca que se alineen con lo que evalúa el revisor de IA, consulte [Crear y administrar marcas para el revisor de IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Agregar revisores de IA a solicitudes de revisión y aprobación

Los usuarios pueden agregar revisores de IA a las plantillas de aprobación existentes o a solicitudes de revisión y aprobación individuales.

### Plantillas de aprobación

Si su organización agrega con frecuencia las mismas personas a las solicitudes de revisión y aprobación, los usuarios de licencias estándar pueden crear plantillas de aprobación en el área Configuración de Workfront.

Los usuarios pueden agregar revisores de IA a las plantillas de aprobación para comprobar automáticamente la conformidad de la marca cuando se utiliza una plantilla para crear una solicitud.

Una vez creadas, las plantillas de aprobación se pueden aplicar a los recursos del área Documentos de un proyecto, tarea o problema.

Para obtener más información, consulte [Crear una plantilla de flujo de trabajo de aprobación para los documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![lista de plantillas que muestra revisores de IA](assets/ai-review-templates.png)

### Solicitud de revisión y aprobación individual

Cuando los usuarios crean solicitudes de revisión y aprobación individuales, pueden agregar un revisor de IA con otros participantes o pueden crear una única solicitud con solo el revisor de IA para comprobar el cumplimiento de la marca.

Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


Se agregó ![revisor de IA a la solicitud de aprobación individual](assets/new-stage.png)

## Ver puntuación y comentarios del comprobador por IA

Segundos después de enviar la solicitud de revisión y aprobación con un revisor de IA, la puntuación y los comentarios del revisor de IA están disponibles en el panel Resumen del documento, incluso si otros participantes siguen revisando y tomando decisiones.

Los propietarios de aprobación también reciben un correo electrónico que les notifica que se ha completado una revisión del recurso. En el correo electrónico, haz clic en **Ir a revisar** y ver la puntuación y los comentarios en Workfront.

El revisor de IA no está diseñado para tomar decisiones en el flujo de trabajo de revisión y aprobación. Solo proporciona una puntuación y recomendaciones para alinear el recurso con los requisitos de marca especificados.

Si el recurso no cumple las directrices de marca, el creativo puede cargar una nueva versión y el propietario de la aprobación puede crear una segunda solicitud de revisión y aprobación con el revisor de IA.

Para obtener más información sobre la visualización de puntuaciones y comentarios, consulte [Ver puntuación y comentarios del revisor de IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

