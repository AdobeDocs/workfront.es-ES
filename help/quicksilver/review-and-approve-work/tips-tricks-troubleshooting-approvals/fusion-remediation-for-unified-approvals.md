---
product-area: documents
navigation-topic: approvals
title: Actualización de escenarios de Workfront Fusion para una revisión y aprobación unificadas
description: Haga un inventario, clasifique y corrija los escenarios de Workfront Fusion basados en las pruebas de Workfront heredadas a medida que su organización adopta el almacenamiento en la nube de Adobe y la revisión y aprobación unificadas.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: a3ef3b4ea00298e23ebc8b6196c951417e75eebe
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 1%

---

# Actualización de escenarios de Workfront Fusion para una revisión y aprobación unificadas

Los escenarios de Workfront Fusion creados en Workfront Proofing heredados no funcionan automáticamente con los proyectos de Adobe Cloud Storage. Los módulos específicos de prueba, los ganchos web y los puntos de conexión de API tienen equivalentes directos en algunos casos y cambios significativos en otros. Este artículo le ayuda a realizar un inventario de los escenarios afectados, clasificarlos y decidir una ruta de corrección antes de llevar los equipos que dependen de esos escenarios a su implementación del almacenamiento en la nube de Adobe.

Los escenarios con ámbitos de proyectos de Workfront heredados siguen funcionando como hoy en día. El trabajo de corrección descrito en este artículo se aplica a los escenarios que tiene intención de ejecutar con proyectos de almacenamiento en la nube de Adobe.

>[!IMPORTANT]
>
>El conector Unified Review and Approvals de Adobe Workfront ya está disponible en Workfront Fusion. Se recomienda utilizar este conector para situaciones más sencillas y fiables al utilizar Fusion con el almacenamiento en la nube de Adobe.
>
>Para obtener información e instrucciones, consulte [Módulos unificados de revisión y aprobaciones de Adobe Workfront](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules) en la documentación de Workfront Fusion.

Utilice este artículo para realizar un inventario y clasificar escenarios y comprender la mejor manera de actualizar los escenarios de Fusion para tener en cuenta el almacenamiento en la nube de Adobe.

Para obtener un resumen de alto nivel de los cambios que se producen cuando su organización se traslada a Workfront en el almacenamiento en la nube de Adobe, consulte [Traslado a Workfront en el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## Cambios para los proyectos de almacenamiento en la nube de Fusion on Adobe

Los escenarios de Fusion existentes creados en Workfront Proof dependen de módulos específicos de prueba, déclencheur de ganchos web y puntos finales de API que no forman parte del modelo de datos unificado de revisión y aprobación. La siguiente tabla asigna tipos de escenarios comunes a su impacto esperado y ruta hacia adelante:

| Tipo de escenario | Impacto | Ruta hacia adelante |
|---|---|---|
| Creación y enrutamiento de pruebas | Pausa | Vuelva a compilar con la API de aprobaciones unificadas en el tercer trimestre de 2026 |
| Webhooks del estado de prueba | Pausa | Vuelva a compilar con nuevos déclencheur de evento de aprobación en el tercer trimestre de 2026 |
| Déclencheur de carga de documento | Parcial: se requiere una nueva prueba | Auditoría y pruebas posteriores a la migración en el tercer trimestre de 2026 |
| Notificaciones de recordatorio de aprobación | Pausa | Reemplazar por plazos de la plantilla de aprobación |
| Enrutamiento de decisión de aprobación | Pausa | Volver a generar con nuevos campos de estado de decisión |
| Informes de aprobación personalizados | Parcial: los nombres de campo pueden cambiar | Asignar campos heredados al nuevo esquema |


## Clasificar cada escenario como Editar, Reconstruir o Retirar

El trabajo que requiere cada escenario depende de lo que haga y de lo que esté disponible en la revisión y aprobación unificadas. Utilice las siguientes clasificaciones:

* **Editar**: la acción existente relacionada con la revisión tiene un equivalente directo en la revisión y aprobación unificadas, y puede actualizar el escenario para usar la nueva acción.
* **Reconstruir**: los pasos subyacentes han cambiado significativamente o existen nuevas capacidades que el escenario debería usar, por lo que el escenario debe reconstruirse desde cero.
* **Retirar**: La funcionalidad nativa de revisión y aprobación unificadas, como las plantillas de aprobación de varias fases con los recordatorios de fecha límite, reemplaza la función para la que se creó el escenario.

Revise cada escenario con respecto a la lógica empresarial específica para decidir su clasificación.

## Enfoque de corrección

Utilice el siguiente método para planificar y ejecutar la remediación de Fusion:

1. **Inventario actual.** Obtenga una lista completa de los escenarios de Fusion activos y etiquete todos los que hagan referencia a la creación de pruebas, el estado de las pruebas, las aprobaciones de documentos o el enrutamiento de aprobación. No espere hasta que el almacenamiento en la nube de Adobe esté habilitado.
1. **Clasifique cada escenario** como Editar, Reconstruir o Retirar según los criterios de la sección anterior.
1. **Pause los escenarios que dependen de la revisión** antes de traer equipos que dependan de ellos al programa piloto de almacenamiento en la nube de Adobe. La ejecución de automatizaciones basadas en pruebas anticuadas en el nuevo modelo puede producir errores silenciosos o acciones duplicadas.
1. **Use plantillas de aprobación para reemplazar la lógica de enrutamiento simple.** Las plantillas de aprobación nativas de varias fases con automatización de plazos pueden gestionar muchos casos de uso que anteriormente requerían Fusion. Para obtener más información, consulte [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Use el conector de revisión y aprobaciones unificadas de Adobe Workfront al reconstruir.** Los conectores actualizados exponen módulos creados específicamente para la revisión y aprobación unificadas y hacen que las reconstrucciones sean considerablemente más sencillas y fiables. No recomendamos la reconstrucción con la versión 22 de la API de Workfront de antemano.
1. **Pruebe escenarios reconstruidos de extremo a extremo en una instancia de zona protegida** antes de habilitarlos en la producción. Preste especial atención a las cargas útiles de suscripción de evento: los nombres de campo y el esquema difieren de los eventos de prueba heredados.

>[!TIP]
>
>Muchas organizaciones han acumulado escenarios de Fusion que eran soluciones alternativas para las lagunas en las pruebas heredadas. Las funciones de revisión y aprobación unificadas nativas, incluidas las plantillas de aprobación, los recordatorios de fecha límite y el enrutamiento de varias fases, eliminan por completo la necesidad de algunos de estos escenarios. A medida que clasifique cada escenario, evalúe si una función nativa puede reemplazarla. Retirar un escenario suele ser un resultado más limpio a largo plazo que reconstruirlo.

## Artículos relacionados

* [Migración a Workfront en el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Resumen de revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
