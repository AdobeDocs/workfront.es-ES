---
product-area: documents
navigation-topic: approvals
title: Ver puntuación y comentarios del comprobador por IA
description: Segundos después de enviar la solicitud de aprobación, puede ver la puntuación y los comentarios del revisor de IA en el panel Resumen del documento.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 838e8f3d-0ea6-4844-a261-ef7b0e78a755
TQID: 'https://experienceleague.adobe.com/iPlcSTaPI-zhmWvRvO81RKFYnIzUoJqzM70mNcxrVbs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%
---
# Ver puntuación y comentarios del comprobador por IA

Segundos después de enviar la solicitud de revisión y aprobación, puede ver la puntuación y los comentarios del revisor de IA en el panel Resumen del documento.

El revisor de IA no está diseñado para tomar decisiones en el flujo de trabajo de revisión y aprobación. Solo proporciona una puntuación y recomendaciones para alinear el recurso con los requisitos de marca especificados.

![comentarios del revisor de IA](assets/ai-reviewer-output.png)

## Comprender cómo se calculan las puntuaciones

El revisor de IA calcula las puntuaciones de forma diferente en función del tipo de revisión:

* Revisión de imagen: Esta puntuación refleja la proporción de directrices aprobadas respecto a directrices fallidas.
* Revisión de copia: Esta puntuación utiliza una ponderación equilibrada de resultados subjetivos y objetivos. Las directrices objetivas (que se muestran en &quot;Corrección&quot;) se ponderan tres veces más que las directrices subjetivas (que se muestran en &quot;Considerar&quot;).

Como las directrices objetivas tienen más peso en las revisiones de textos, recomendamos escribir directrices concretas y mensurables en su marca. Para obtener más información, consulte la sección [Prácticas recomendadas para escribir directrices de marca](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md#best-practices-for-writing-brand-guidelines) en el artículo Crear y administrar marcas para el revisor de IA.

## Ver puntuación y comentarios

Puede ver la puntuación y los comentarios del revisor de IA en el panel Resumen del documento o en la pestaña Aprobaciones de la página Detalles del documento.

1. En el correo electrónico de notificación de Workfront, haga clic en **Ir a revisión**.

   O

   Vaya al área Documentos donde se carga el documento y abra el panel Resumen del documento.
1. Haga clic en **Puntuación**.
   ![ver puntuación del documento](assets/view-score.png)

En la ventana de puntuación y comentarios, el revisor de IA explica cómo el recurso no cumple las directrices especificadas.
![Los comentarios del revisor de IA requieren atención](assets/ai-reviewer-needs-attention.png)

## Cargue una nueva versión y vuelva a añadir AI Reviewer

Si necesita ajustar el recurso en función de los comentarios del revisor de IA, puede cargar una nueva versión e iniciar una nueva revisión.

Para obtener más información, vea [Cargar una nueva versión del documento y solicitar la aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md).
