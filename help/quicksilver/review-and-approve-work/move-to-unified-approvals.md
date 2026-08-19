---
product-area: documents
navigation-topic: approvals
title: Paso de aprobaciones de documentos heredados a aprobaciones unificadas
description: Comprenda qué sucede con los flujos de trabajo de aprobación de documentos existentes cuando su organización se desplaza a una versión de Workfront que admite aprobaciones unificadas.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: b612a50b7445732f90b7de2a216f4bca499fd96b
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%

---

# Paso de aprobaciones de documentos heredados a aprobaciones unificadas

Al pasar a una versión de Workfront compatible con el almacenamiento en la nube de Adobe, su organización también pasa de las aprobaciones de documentos heredados a las aprobaciones unificadas. Este artículo proporciona información sobre la funcionalidad que estará disponible en las aprobaciones unificadas, así como recomendaciones para los administradores de Workfront que mueven usuarios fuera de las aprobaciones de documentos heredados.


>[!IMPORTANT]
>
>Este cambio se aplica en toda la organización en cuanto pasa a una versión de Workfront que admita el almacenamiento en la nube de Adobe. No hay ningún grupo piloto ni opción de despliegue gradual para pasar de aprobaciones de documentos heredados a aprobaciones unificadas.<br>
>Para obtener más información sobre los cambios que se producen con el almacenamiento en la nube de Adobe, consulte [Mover a Workfront en el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Comprenda qué está cambiando desde las aprobaciones de documentos heredados a las aprobaciones unificadas

|  | Aprobaciones de documentos heredados | Aprobaciones unificadas |
| --- | --- | --- |
| Aprobadores y revisores | Aprobación solo por usuarios individuales | Aprobación o revisión por usuarios o equipos individuales |
| Plazos y recordatorios | No hay recordatorios automatizados | Recordatorios automatizados: 72 horas de salida, 24 horas de salida y en la fecha de vencimiento |
| Fases y rutas de aprobación | Una fase de aprobación, sin rutas paralelas | [Varias etapas de aprobación y rutas de revisión paralelas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Plantillas de aprobación | Cada aprobación configurada desde cero | [Plantillas reutilizables](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) disponibles en la instalación de Workfront |
| Revisión y marcado | Visualizador de revisiones | [Visualizador de revisiones](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) en objetos de almacenamiento de Workfront heredados o el visualizador [Frame.io](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) en objetos de almacenamiento en la nube de Adobe |
| Revisión asistida por IA | No disponible | Comprobaciones automáticas del cumplimiento de la marca con [Revisor de contenido](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Creación de informes | Informes heredados | Widgets de KPI de inicio y [paneles de lienzo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |



### ¿Qué les sucede a las aprobaciones en curso?

Las aprobaciones en vuelo creadas en aprobaciones de documentos heredadas seguirán funcionando como antes de la actualización. Sin embargo, cualquier nueva aprobación creada después de la actualización utilizará Aprobaciones unificadas.


## Preparación para la actualización

* Comparta el artículo [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) con los usuarios finales.
* Revise los escenarios de Workfront Fusion existentes. Si utiliza aprobaciones de documentos heredados con revisión, consulte [Actualizar escenarios de Workfront Fusion para una revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) antes de que su organización actualice.
* Configure un tablero de revisión y aprobación en Paneles de lienzo para reemplazar cualquier informe de aprobación heredado. Consulte [Crear un panel de revisión y aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) para obtener más información.


### Artículos de ayuda para usuarios finales

* [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Funcionalidad disponible para aprobaciones de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Resumen de revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Revisión y aprobación con el visor Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Usar las aprobaciones unificadas y la revisión de forma conjunta](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Información general del estado de decisión del documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Introducción al Revisor de contenido de Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
