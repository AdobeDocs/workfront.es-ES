---
product-area: documents
navigation-topic: approvals
title: Introducción a la integración de Frame.io
description: Introducción a la integración de Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: a3edfadc447a763c638cc926b386272890697f81
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 2%

---

# Introducción a la integración de Frame.io

La integración de Workfront y Frame.io mantiene a los creativos, los especialistas en marketing y las partes interesadas alineados con un flujo de trabajo fluido. Acceda a actualizaciones en tiempo real, evite trabajos duplicados y asegúrese de que los recursos se aprueban antes del lanzamiento.

Para obtener más información sobre Frame.io, consulte [Introducción a Frame.io](https://support.frame.io/en/collections/49298-getting-started).

Debe tener la integración de Workfront y Frame.io configurada en la instancia de Workfront. Para obtener más información, consulte [Resumen de la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md#integration-requirements).

<!--## Integration requirements

* Workfront and Frame.io must be deployed to the same Identity Management system (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience.

* The integration is configured by Adobe Professional Services. -->

## Inicio y planificación del trabajo en Workfront

Los coordinadores de proyectos pueden crear proyectos y planificar el trabajo en Workfront. Los proyectos creados en una instancia con la integración de Frame.io habilitada utilizan el almacenamiento empresarial de Adobe, que permite almacenar y administrar los recursos dentro del ecosistema de Adobe.

Si su organización tiene una licencia de Frame.io Enterprise, los proyectos creados en Workfront también son visibles en Frame.io, lo que permite a los usuarios interactuar y cargar recursos en cualquier producto.

Para obtener información sobre el almacenamiento empresarial de Adobe o los proyectos en Frame.io, consulte

* [Información general de Workspace: Proyectos](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Información general sobre Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Revisión y aprobación de recursos

Una vez finalizado el recurso, el coordinador del proyecto puede iniciar el proceso formal de revisión y aprobación en Workfront.

Una vez creado el flujo de trabajo de aprobación, los revisores y aprobadores pueden utilizar el visor Frame.io para agregar comentarios y marcar el recurso. También pueden tomar la decisión de aprobación en el visor de Frame.io.

Para obtener más información sobre la configuración de proyectos, consulte

* [Crear un proyecto](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
* [Información general sobre la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)

### Iniciar revisiones y aprobaciones formales en Workfront

Los coordinadores de proyectos pueden crear aprobaciones y revisiones únicas o plantillas de aprobación reutilizables. Pueden asignar revisores, aprobadores o una combinación de ambos:

* **Los revisores** pueden agregar comentarios y marcar los recursos. Una vez finalizada, puede marcar su revisión como completada. No es necesario marcar la revisión como completada para que el recurso avance en el proceso de aprobación.
* **Los aprobadores** pueden agregar comentarios y marcar los recursos. Deben tomar la decisión de adelantar el proceso de aprobación.

#### Creación de un flujo de trabajo de revisión y aprobación

Los revisores y aprobadores se pueden añadir a un flujo de trabajo de aprobación de un solo uso o a una plantilla de aprobación reutilizable:

* **Aprobaciones de un solo uso**: en el proyecto o tarea donde reside el recurso, el coordinador del proyecto puede asignar revisores y aprobadores y establecer un límite de finalización. Se recuerda a los revisores y aprobadores por correo electrónico 72 horas antes del plazo, 24 horas antes del plazo y, a continuación, en el propio plazo.

  Para obtener más información, vea [Crear una solicitud de revisión o aprobación de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

* **Plantillas de aprobación**: en el área Configuración de Workfront, los coordinadores de proyectos pueden crear plantillas de aprobación reutilizables. En una plantilla, los usuarios pueden agregar revisores y aprobadores, y especificar un periodo de finalización. Cuando la plantilla de aprobación se aplica a un recurso, la fecha límite se calcula a partir del periodo de tiempo especificado.

  Una vez creada una plantilla, se puede aplicar a un recurso para iniciar el proceso formal de revisión y aprobación en Workfront.

  Para obtener más información, consulte [Crear una plantilla de aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


  ![Asignar plantilla](assets/assign-template.png)

### Revisión y aprobación de recursos en el visor de Frame.io

Una vez iniciado el flujo de trabajo de revisión y aprobación en Workfront, los revisores y aprobadores pueden acceder al visor de Frame.io para añadir comentarios, marcar el recurso y tomar una decisión.

Para obtener más información, consulte [Revisar y aprobar con el visor Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

#### Acceso al visor de Frame.io

Los usuarios pueden acceder al visor Frame.io de las siguientes maneras:

* Notificaciones por correo electrónico de Workfront
* El widget Mi aprobación en el área de Inicio de Workfront

>[!NOTE]
>
>Se notifica a los usuarios externos de Workfront por correo electrónico y se les pedirá que creen un inicio de sesión de Frame.io para revisar y aprobar los recursos.

![abrir el visor de fotogramas desde Inicio](assets/open-fio-viewwer.png)

#### Agregar comentarios y marcar recursos

Los comentarios y el marcado de recursos se pueden ver en el visor de Frame.io. Para obtener más información sobre el uso del visor Frame.io, consulte [Comentarios sobre el contenido](https://help.frame.io/en/articles/9105251-commenting-on-your-media).

#### Tomar una decisión

Una vez completada toda la actividad de revisión, los aprobadores deben tomar una de las siguientes decisiones:

* **Aprobar**: el recurso no necesita cambios y está listo para usarse.
* **Necesita trabajo**: el recurso necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el recurso debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Los revisores pueden marcar su revisión como completada dentro de Workfront, pero esto no es necesario para que el recurso avance en el proceso de aprobación.

Para obtener más información sobre las decisiones en Workfront, consulte [Resumen del estado de decisión del documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Visor de fotogramas y decisión](assets/decision-fio.png)


### Seguimiento de métricas de revisión y aprobación

Los coordinadores de proyecto pueden monitorizar el progreso de todas las aprobaciones en vuelo en el área de inicio de Workfront o con informes personalizados en los paneles del lienzo:

* **Tablero personalizado**: cree un tablero de informes en el área Tableros de lienzo para mostrar información detallada y de alto nivel acerca de las revisiones y aprobaciones con la funcionalidad de Aprobaciones unificadas. Para obtener información sobre cómo empezar, consulte [Crear un tablero de informes para revisión y aprobaciones](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Widget de inicio de métricas de aprobación de documento**: muestra 2 gráficos con información sobre el tiempo promedio de aprobación y las decisiones, así como vistas de lista de aprobaciones pendientes y vencidas.
  ![Todas las aprobaciones](assets/all-approvals.png)