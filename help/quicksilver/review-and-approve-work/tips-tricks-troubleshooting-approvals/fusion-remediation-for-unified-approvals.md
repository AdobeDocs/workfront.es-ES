---
product-area: documents
navigation-topic: approvals
title: Actualización de escenarios de Workfront Fusion para una revisión y aprobación unificadas
description: Inventario, clasificación y corrección de escenarios de Workfront Fusion basados en las pruebas de Workfront heredadas a medida que su organización adopta el almacenamiento empresarial de Adobe y la revisión y aprobación unificadas.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: 0a635f80338cef38dec7d32391596ca9ccd2fd6c
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 1%

---

# Actualización de escenarios de Workfront Fusion para una revisión y aprobación unificadas

Los escenarios de Workfront Fusion creados en Workfront Proofing heredados no funcionan automáticamente con los proyectos de Adobe Enterprise Storage. Los módulos específicos de prueba, los ganchos web y los puntos de conexión de API tienen equivalentes directos en algunos casos y cambios significativos en otros. Este artículo le ayuda a realizar un inventario de los escenarios afectados, clasificarlos y decidir una ruta de corrección antes de llevar los equipos que dependen de esos escenarios a su implementación de almacenamiento empresarial de Adobe.

Los escenarios con ámbitos de proyectos de Workfront heredados siguen funcionando como hoy en día. El trabajo de corrección descrito en este artículo se aplica a los escenarios que tiene intención de ejecutar con proyectos de almacenamiento empresarial de Adobe.

Se espera que los conectores Fusion con compatibilidad nativa para la revisión y aprobación unificadas estén disponibles en el tercer trimestre de 2026. Planifique la reconstrucción ahora, pero le recomendamos que espere a que se creen los nuevos conectores antes de compilarlos. Los escenarios serán más sencillos y fiables de lo que sustituyen.

Las directrices de automatización detalladas se publicarán junto con la versión del conector Fusion del tercer trimestre de 2026. Utilice este artículo para realizar un inventario y clasificar escenarios ahora, de modo que esté listo para actuar una vez que las directrices estén disponibles.

Para obtener un resumen de alto nivel de los cambios que se producen cuando su organización se traslada a Workfront en el almacenamiento empresarial de Adobe, consulte [Mover a Workfront en el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## Cambios para los proyectos de almacenamiento empresarial de Fusion on Adobe

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

1. **Inventario actual.** Obtenga una lista completa de los escenarios de Fusion activos y etiquete todos los que hagan referencia a la creación de pruebas, el estado de las pruebas, las aprobaciones de documentos o el enrutamiento de aprobación. No espere hasta que el almacenamiento empresarial de Adobe esté habilitado.
1. **Clasifique cada escenario** como Editar, Reconstruir o Retirar según los criterios de la sección anterior.
1. **Pause los escenarios que dependen de la revisión** antes de traer equipos que dependan de ellos al programa piloto de almacenamiento empresarial de Adobe. La ejecución de automatizaciones basadas en pruebas anticuadas en el nuevo modelo puede producir errores silenciosos o acciones duplicadas.
1. **Use plantillas de aprobación para reemplazar la lógica de enrutamiento simple.** Las plantillas de aprobación nativas de varias fases con automatización de plazos pueden gestionar muchos casos de uso que anteriormente requerían Fusion. Para obtener más información, consulte [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Espere a que se actualicen los conectores Fusion en el tercer trimestre de 2026 antes de volver a compilarlos.** Los conectores actualizados exponen módulos creados específicamente para la revisión y aprobación unificadas y hacen que las reconstrucciones sean considerablemente más sencillas y fiables. No recomendamos la reconstrucción con la versión 22 de la API de Workfront de antemano. Si continúa con un escenario en el que el tiempo es esencial, planifique volver a visitar ese trabajo una vez que se publiquen los nuevos conectores.
1. **Pruebe escenarios reconstruidos de extremo a extremo en una instancia de zona protegida** antes de habilitarlos en la producción. Preste especial atención a las cargas útiles de suscripción de evento: los nombres de campo y el esquema difieren de los eventos de prueba heredados.

>[!TIP]
>
>Muchas organizaciones han acumulado escenarios de Fusion que eran soluciones alternativas para las lagunas en las pruebas heredadas. Las funciones de revisión y aprobación unificadas nativas, incluidas las plantillas de aprobación, los recordatorios de fecha límite y el enrutamiento de varias fases, eliminan por completo la necesidad de algunos de estos escenarios. A medida que clasifique cada escenario, evalúe si una función nativa puede reemplazarla. Retirar un escenario suele ser un resultado más limpio a largo plazo que reconstruirlo.

## Artículos relacionados

* [Migración a Workfront en Adobe enterprise storage](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Resumen de revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
