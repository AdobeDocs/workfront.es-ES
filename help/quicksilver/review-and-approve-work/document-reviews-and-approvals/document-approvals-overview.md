---
product-area: documents
navigation-topic: approvals
title: Resumen de revisión y aprobación unificadas
description: Obtenga más información acerca de la revisión y aprobación unificadas con tecnología Workfront y Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 93eab1106953bfc7324f4b7cc99d3442364a56cd
workflow-type: tm+mt
source-wordcount: '3865'
ht-degree: 0%

---


# Resumen de revisión y aprobación unificadas

La revisión y la aprobación unificadas reúnen Adobe Workfront y Adobe Frame.io en una única experiencia profundamente conectada: se eliminan las diferencias entre la administración de marketing, la revisión creativa y la entrega de contenido.
Los coordinadores de proyectos administran el trabajo en Workfront mientras los creativos, los especialistas en marketing y las partes interesadas revisan y aprueban los recursos en el visor Frame.io de nivel profesional, todo sin mover archivos entre herramientas desconectadas.

![Diagrama que muestra el flujo de trabajo unificado de revisión y aprobación, con coordinadores de proyecto que administran el trabajo en Workfront y revisores y aprobadores que proporcionan comentarios y toman decisiones en el visor Frame.io.](assets/Unified-Review-Approvals-Image.png)


## Requisitos de integración

* Workfront y Frame.io deben implementarse en la misma organización de Identity Management system (IMS).

* Los usuarios solo pueden pertenecer a una instancia de Workfront dentro de la organización IMS.

* La instancia de Workfront debe habilitarse en la experiencia unificada de Adobe y en el almacenamiento empresarial de Adobe.


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

* El almacenamiento empresarial de Adobe requiere nombres únicos para objetos del mismo nivel con el mismo elemento principal en el árbol de jerarquías.
* Los documentos no pueden tener el mismo nombre si pertenecen al mismo proyecto.
* Los nombres de objeto no pueden contener ninguno de los siguientes caracteres especiales: \ / : * ? &quot; | &lt; >
* Los nombres de objeto están limitados a un máximo de 255 caracteres.

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

## Introducción a la revisión y aprobación unificadas

Para comenzar con la revisión y aprobación unificadas, consulte [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

## Preguntas frecuentes

### Introducción a la revisión y aprobación unificadas

+++ Amplíe para ver las preguntas más frecuentes sobre cómo empezar con la revisión y la aprobación unificadas.

**¿Qué es la revisión y aprobación unificadas?**

La revisión y aprobación unificadas es una integración nativa entre Adobe Workfront y Adobe Frame.io que reúne la administración del trabajo y la revisión creativa en un único sistema conectado. Los coordinadores de proyectos planifican y rastrean el trabajo en Workfront, mientras que los revisores y aprobadores utilizan el visor Frame.io de nivel profesional para proporcionar comentarios, marcar recursos y tomar decisiones de aprobación, sin tener que alternar entre herramientas independientes o mover archivos manualmente.

La revisión y la aprobación ocupan un lugar central en cada operación de contenido. Es donde convergen el trabajo creativo, las aportaciones de las partes interesadas y las decisiones empresariales. Cuando ese proceso se propaga a través de herramientas desconectadas (hilos de correo electrónico, mensajes de chat, marcas de capturas de pantalla), las consecuencias se agravan: tiempo de salida al mercado más lento, comentarios perdidos, confusión de versiones y tiempo empleado en administrar archivos en lugar de crear contenido.

La revisión y la aprobación unificadas resuelven esto al reemplazar el mosaico de herramientas de revisión desconectadas por un sistema moderno, una única fuente de verdad que vive donde ya sucede el trabajo.

**¿Cuáles son los requisitos para utilizar esta integración?**

Para utilizar la revisión y aprobación unificadas, se deben cumplir las siguientes condiciones:

* Workfront y Frame.io deben implementarse en la misma organización de Adobe Identity Management System (IMS).

* Los usuarios solo pueden pertenecer a una instancia de Workfront dentro de la organización IMS.

* La instancia de Workfront debe habilitarse en la experiencia unificada de Adobe y en el almacenamiento empresarial de Adobe.

* Los clientes de Workfront deben tener un SKU V2 (puede que se requiera un evento de contratación; póngase en contacto con el representante de la cuenta de Adobe).

**¿Necesito una licencia de Frame.io para usar esta integración?**

No. El visor Frame.io se incluye automáticamente para todos los usuarios de Workfront con una licencia de pago sin coste adicional. No necesita una licencia Frame.io independiente para revisar y aprobar recursos a través de Workfront.

Si su organización desea acceder a funciones adicionales de Frame.io, como cargar recursos directamente en proyectos en Frame.io, puede adquirir una licencia de Frame.io Enterprise. Póngase en contacto con el representante de su cuenta de Adobe para obtener más información.

**¿Esto reemplaza a Workfront Proof?**

Sí. Cuando la revisión y la aprobación unificadas están habilitadas, el visor de Frame.io se convierte en la superficie de revisión principal en Workfront y reemplaza a Workfront Proof.

Los clientes existentes conservarán el acceso a la funcionalidad de revisión de Workfront para cualquier proyecto creado antes de que se habilitara la integración.

**¿Cómo obtengo acceso a la revisión y aprobación unificadas?**

**¿Qué debo hacer para obtener acceso?**

Para acceder a la revisión y aprobación unificadas, su organización debe estar en un SKU de Workfront V2. Si actualmente no tiene un SKU V2, será necesario un evento de contratación con Adobe. En primer lugar:

* Póngase en contacto con el representante de su cuenta de Adobe para confirmar si su plan de Workfront actual admite la revisión y aprobación unificadas.

* Si se necesita una actualización de SKU, el representante de la cuenta le guiará a través del proceso de contratación.

* Una vez que su cuenta esté en el SKU correcto, Adobe Professional Services configurará la integración para su organización.

   * Si no está seguro de quién es su representante de cuentas de Adobe, puede ponerse en contacto con nosotros a través del portal de asistencia de Adobe o visitar Experience League para obtener opciones de contacto.

+++

### Funcionamiento de la revisión y aprobación unificadas

+++ Amplíe para ver las preguntas más frecuentes sobre cómo funciona la revisión unificada y la aprobación.

**¿Cómo funciona el flujo de trabajo de revisión y aprobación?**

El flujo de trabajo sigue estos pasos generales:

1. Un coordinador de proyectos crea un proyecto en Workfront y carga o vincula recursos.

1. Cuando un recurso está listo para revisarse, el coordinador crea un flujo de trabajo de aprobación, ya sea una aprobación de un solo uso o mediante la aplicación de una plantilla de aprobación reutilizable.

1. Los revisores y aprobadores asignados reciben una notificación por correo electrónico y pueden abrir el recurso directamente en el visor de Frame.io.

1. Los revisores pueden agregar comentarios y marcas. Los aprobadores deben tomar una decisión formal.

1. El coordinador rastrea el estado en tiempo real desde Workfront.

**¿Cuál es la diferencia entre un revisor y un aprobador?**

Los revisores pueden agregar comentarios y marcar los recursos en el visor Frame.io. Cuando terminan, marcan su revisión como completada. Sin embargo, no es necesario que realicen esta acción para que avance el flujo de trabajo de aprobación.

Los aprobadores deben tomar una de las siguientes decisiones para avanzar en el flujo de trabajo de aprobación:

* **Aprobar**: el recurso está listo para usarse tal cual.

* **Necesita trabajo**: el recurso requiere cambios y debe volver a enviarse como una nueva versión para que se vuelva a aprobar.

**¿Qué tipos de flujos de trabajo de aprobación puedo crear?**

* **Aprobaciones de un solo uso**: puede crear una aprobación de un solo uso directamente en un documento de un proyecto, tarea o problema. Puede asignar revisores y aprobadores, establecer plazos y configurar varias fases si es necesario. Los recordatorios de correo electrónico automatizados se envían 72 horas antes, 24 horas antes y dentro del plazo.

* **Plantillas de aprobación**: puede crear plantillas reutilizables en la instalación de Workfront. Una plantilla define los revisores, los aprobadores y un periodo de tiempo de finalización relativo. Si es necesario, puede crear varias fases. Una vez aplicada una plantilla a un recurso, la fecha límite se calcula automáticamente.

**¿Cómo participan los usuarios externos en las revisiones?**

Se notifica a los usuarios externos de Workfront por correo electrónico cuando se les asigna una revisión o aprobación. Se le pedirá que cree un inicio de sesión de Frame.io para acceder al visor y participar en el proceso de revisión.

**¿Cómo realizo un seguimiento del progreso de revisión y aprobación?**

Los coordinadores de proyectos pueden supervisar todas las aprobaciones en vuelo de varias formas:

* El widget Mis aprobaciones en el área de Inicio de Workfront proporciona un resumen en tiempo real de las aprobaciones pendientes y vencidas.

* El widget Métricas de aprobación de documento muestra los tiempos de aprobación promedio y los desgloses de decisión.

* Los paneles de informes personalizados se pueden crear en los paneles del lienzo para obtener una visibilidad más profunda de la actividad de revisión y aprobación.

+++


### Revisión y aprobación de recursos y vídeos

+++ Amplíe para ver las preguntas más frecuentes sobre la revisión y aprobación de recursos y vídeos.

**¿Hay algún límite en las críticas de vídeo?**

Sí. Las solicitudes de revisión de vídeo tienen un límite anual establecido en el 10 % del total de licencias de usuario de Workfront pagadas de su organización (estándar y básica). Este límite se aplica a nivel de organización.

Los administradores de Workfront recibirán notificaciones en la aplicación cuando el uso alcance el 80 % y el 100 % del límite.

Este límite no se aplica a los clientes de Frame.io Enterprise. Si su organización revisa regularmente grandes volúmenes de contenido de vídeo, póngase en contacto con el representante de su cuenta de Adobe para obtener más información sobre las licencias de Frame.io Enterprise.

**¿Puede aparecer el mismo usuario en varias fases de un flujo de trabajo de aprobación?**

Sí. Se puede asignar a un usuario varias fases dentro del mismo flujo de trabajo de aprobación.

**¿Puedo agregar etapas para crear un flujo de trabajo de aprobación de varias etapas?**

Sí. Se admiten flujos de trabajo de aprobación de varias etapas, lo que le permite enrutar los recursos a través de rondas secuenciales de revisión y aprobación con diferentes participantes en cada etapa.

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**¿Pueden las plantillas de aprobación incluir grupos o equipos, o solo usuarios individuales?**

Actualmente, las plantillas de aprobación admiten usuarios y equipos individuales.

**¿Se notifica a los aprobadores por correo electrónico cuando tienen algo que revisar?**

Sí. Los aprobadores y revisores reciben notificaciones por correo electrónico cuando se les asigna una revisión o aprobación. Los correos electrónicos de recordatorio automatizados también se envían 72 horas antes del plazo, 24 horas antes y dentro del propio plazo.

Actualmente, la capacidad de personalizar los mensajes de notificación por correo electrónico no está disponible, pero está en la hoja de ruta del producto.

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**¿Puedo mantener una fase de revisión privada de otros participantes?**

Actualmente no hay ninguna función de fase privada. Para que una revisión sea privada con respecto a otros participantes, se recomienda crear una copia independiente del recurso específicamente para ese grupo de revisión. Actualmente, los comentarios no están segmentados por grupo de participantes dentro de un solo activo.

Tenga en cuenta que el historial de versiones, incluidas las versiones anteriores y actuales, siempre es visible para cualquiera que tenga acceso a la vista de ese recurso.

**¿Se pueden marcar los comentarios como resueltos?**

Sí. Los comentarios se pueden marcar como resueltos en el visor de Frame.io.

**¿Qué herramientas de marcado y anotación están disponibles en el visor Frame.io?**

El visor Frame.io incluye un conjunto completo de herramientas de marcado visual, incluido el dibujo a mano alzada y formas estándar como círculos, flechas y cuadrados. En el caso de los recursos de vídeo, los comentarios tienen una marca de tiempo con precisión de fotograma, por lo que los comentarios siempre están vinculados al momento exacto del clip y no solo a una marca de tiempo general.

**¿Aparecerán los comentarios realizados en el visor Frame.io en el proyecto Workfront?**

Los comentarios y anotaciones permanecen dentro del visor de Frame.io para que conserven su contexto completo, incluidas las marcas de tiempo y las marcas visuales. Esto puede evolucionar en futuras versiones.

**¿Es posible agregar comentarios a una versión descargada de un recurso (por ejemplo, un PDF)?**

Actualmente no es compatible, pero es una función solicitada comúnmente que está en consideración para una versión futura.

**¿Puedo revisar varios recursos juntos como un grupo?**

Próximamente se ofrecerán opciones mejoradas de revisión masiva. Mientras tanto, los recursos de diferentes tipos de archivo, como un vídeo y un documento de Word, se pueden incluir juntos en una revisión de recursos agrupada.

**¿Es la revisión unificada y la aprobación solo para vídeo o admite otros tipos de archivo?**

La revisión y aprobación unificadas están diseñadas para todos los tipos de recursos, no solo para vídeo. El visor Frame.io se ha actualizado considerablemente para admitir imágenes, documentos, PDF y otros formatos de archivo comunes, además del vídeo.

Para obtener una lista completa de los tipos de archivo admitidos, consulte la documentación de tipos de archivo compatibles con Frame.io en Experience League.

**¿Puedo compartir recursos externamente con partes interesadas que no tienen acceso a Workfront?**

Sí. Assets se puede compartir externamente. Se notifica a los usuarios externos por correo electrónico y se les pedirá que creen un inicio de sesión de Frame.io para acceder al visor y participar en la revisión.

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### Administración de archivos y almacenamiento

+++ Amplíe para ver las preguntas más frecuentes sobre el almacenamiento y la administración de archivos.

**¿Qué es el almacenamiento empresarial de Adobe y cómo se relaciona con esta integración?**

El almacenamiento empresarial de Adobe es la capa de almacenamiento común que conecta Workfront, Frame.io y Adobe Creative Cloud. Assets se encuentra en un solo lugar y es accesible a través de las herramientas sin transferencias manuales de archivos. Los creativos pueden funcionar correctamente y los revisores siempre ven la versión más reciente.

Entre las ventajas clave del almacenamiento empresarial de Adobe se incluyen:

* Una sola capa de almacenamiento para todos los recursos de trabajo en curso en Workfront y Frame.io

* Control de acceso centralizado administrado mediante Adobe Identity Management System (IMS)

* Visibilidad completa de los recursos: sin variación de la versión ni pérdida de metadatos

* Administración de almacenamiento escalable y de nivel empresarial

**¿Hay requisitos de nomenclatura o estructura para archivos y proyectos?**

Sí. Dado que la integración utiliza el almacenamiento empresarial de Adobe, se aplican las siguientes convenciones:

* Los nombres de objeto y documento deben ser únicos dentro del mismo elemento principal en la jerarquía de carpetas.

* Los documentos del mismo proyecto no pueden compartir un nombre.

* Los nombres de programas, portafolios, proyectos, plantillas, tareas, problemas, documentos y carpetas de documentos no pueden contener los siguientes caracteres especiales: `\ / : * ? " | < >` y están limitados a 255 caracteres.

Workfront cambia automáticamente el nombre de los objetos o documentos según sea necesario para evitar conflictos.

**¿Qué tipos de archivo se admiten en el visor Frame.io?**

El visor Frame.io admite más de 40 formatos de archivo, incluidos todos los tipos comunes de vídeo, imagen, audio, PDF y Microsoft Office. El soporte de vídeo incluye reproducción nativa para formatos profesionales como ProRes, H.265 y DNxHD, con soporte para archivos de hasta 500 GB.

Frame.io se creó específicamente para la revisión creativa, lo que significa que gestiona toda la gama de tipos de recursos con los que trabajan los equipos creativos y de marketing.

+++

### Permisos y acceso

+++ Amplíe para ver las preguntas más frecuentes sobre permisos y acceso.

**¿Cómo se administran los permisos de usuario?**

Los permisos de usuario se establecen y controlan en Workfront y fluyen automáticamente a Frame.io. No puede invitar a usuarios ni modificar permisos directamente en Frame.io para esta integración. Toda la administración de acceso debe realizarse utilizando el modal de uso compartido de proyectos en Workfront.

La tabla siguiente muestra cómo se asignan los permisos de Workfront a los permisos de Frame.io:

<table>
  <thead>
    <tr>
      <th>Permiso de Workfront</th>
      <th>Permiso Frame.io</th>
    </tr>
  </thead>
  <tbody>
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
  </tbody>
</table>

+++


### Integraciones y funciones avanzadas

+++ Amplíe para ver las preguntas más frecuentes sobre integraciones y funciones avanzadas.

**¿Cómo afecta esto a las integraciones de complementos de Creative Cloud existentes con Adobe Express y GenStudio?**

Las integraciones que admiten la experiencia del visor Frame.io están actualmente en desarrollo para Adobe Express y GenStudio Performance Marketing. Las nuevas integraciones se basarán en el mismo sistema unificado de revisión y aprobación, por lo que aprovecharán el visor de Frame.io para obtener una experiencia de revisión coherente en los tres productos.

**¿Frame.io está integrado en Workfront o los usuarios navegan a una interfaz independiente?**

Los usuarios pueden iniciar el visor de Frame.io directamente desde Workfront. Toda la actividad de revisión y aprobación tiene lugar dentro del visor de Frame.io y se sincroniza automáticamente con Workfront.

**¿Puedo enviar recursos aprobados a Adobe Experience Manager (AEM)?**

Sí. Una vez que un recurso completa el ciclo de revisión y aprobación, puede transferirlo a Adobe Experience Manager Assets para su almacenamiento y distribución finales. Esto conecta Workfront para la administración del trabajo, Frame.io para la revisión y AEM para la administración de recursos digitales en un supply chain de contenido unificado.

Para obtener más información, vea [Usar Adobe Experience Manager con la integración Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**¿Cómo encaja la revisión y aprobación unificadas en Adobe GenStudio?**

La revisión y la aprobación unificadas son un componente básico de Adobe GenStudio: la visión más amplia de Adobe para un supply chain de contenido conectado. GenStudio conecta Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets y GenStudio for Performance Marketing en un flujo de trabajo unificado desde la información breve de la campaña hasta la entrega de contenido.

Dentro de ese ecosistema, la revisión y la aprobación sirven como el punto de entrega crítico entre la creación y la entrega. Es donde el trabajo creativo cumple con los aportes de las partes interesadas, la calidad se valida y el contenido se borra para publicarse. Cuando ese traspaso es rápido, visible y confiable, desbloquea la velocidad en todo el contenido de supply chain: la IA puede acelerar la creación, la automatización puede manejar la distribución, pero un cuello de botella en la revisión limita las ganancias en ambos lados. Al conectar Workfront y Frame.io, se elimina ese cuello de botella.

**¿Qué es la característica Revisor de IA?**

La revisión y aprobación unificadas incluyen una función de revisor de IA que automatiza las comprobaciones de conformidad de marca como parte del proceso de revisión. El revisor de IA puede evaluar los recursos en función de las directrices de marca y marcar los problemas potenciales antes de que los revisores humanos participen, lo que ayuda a los equipos a detectar los problemas antes y avanzar más rápido.

Para obtener más información sobre la configuración y el uso de AI Reviewer, consulte la documentación de Workfront en Experience League.

+++

### Contratos, SKU y almacenamiento

+++ Amplíe para ver las preguntas más frecuentes sobre contratos, SKU y almacenamiento.

**¿Cuándo estarán disponibles para mí la revisión y aprobación unificadas?**

La revisión y aprobación unificadas ya están disponibles. El acceso requiere una actualización a un SKU de Workfront V2. Si el contrato se firmó antes de que los SKU V2 estuvieran disponibles, puede obtener acceso de una de las dos maneras siguientes:

* Tras la renovación: el acceso se activará en la próxima fecha de renovación del contrato.

* Nueva contratación anticipada: el equipo de su cuenta de Adobe puede volver a contratarle antes para añadir los nuevos SKU y, al mismo tiempo, mantener la fecha de finalización del contrato existente. No hay aumento de precio cuando se cambia a un paquete equivalente.

Póngase en contacto con su representante de cuentas de Adobe para determinar la mejor ruta para su organización.

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**¿La actualización al SKU V2 me proporciona más almacenamiento?**

Sí. Con el SKU V2, cada usuario con licencia recibe 60 GB de almacenamiento, frente a los 30 GB de la versión anterior.

**¿Cómo puedo elegir entre almacenamiento empresarial de Adobe y almacenamiento de Workfront heredado?**

El almacenamiento empresarial habilita la experiencia del visor Frame.io y es necesario para una revisión y aprobación unificadas. El almacenamiento heredado sigue utilizando el visualizador de Workfront Proof (ProofHQ) como predeterminado.

Si su organización tiene una combinación de flujos de trabajo simples y flujos de trabajo de revisión más complejos, puede priorizar qué flujos de trabajo migrar primero.

El almacenamiento empresarial le ofrece la flexibilidad de implementar la nueva experiencia de forma incremental, empezando por los flujos de trabajo que más se beneficiarán.

**¿Cómo se administran las licencias de Frame.io?**

Después de firmar el SKU V2, todos los usuarios de Workfront tendrán acceso al visor Frame.io para los flujos de trabajo de revisión y aprobación; para ello, no se requiere una licencia empresarial Frame.io independiente.

Si su organización necesita funciones adicionales de Frame.io Enterprise, como

* Marca de agua avanzada (dinámica y forense)
* Administración de derechos digitales con eliminación automática de recursos
* Credenciales de contenido para contenido generado por IA
* Metadatos creativos personalizados
* Integraciones de cámara a nube
* Su propio espacio de trabajo para el trabajo creativo en curso

Puede trabajar con el equipo de su cuenta de Adobe para determinar la cantidad adecuada de licencias de Frame.io Enterprise. Todas las licencias se administran mediante Adobe Admin Console.

+++

### Zona protegida y despliegue

+++ Amplíe para ver las preguntas más frecuentes sobre la zona protegida y el despliegue.

**¿Puedo probar la revisión y aprobación unificadas en un entorno de espacio aislado?**

Parcialmente. Los flujos de trabajo de aprobación se pueden probar en un entorno de zona protegida de Workfront. Sin embargo, la experiencia del visor Frame.io no está disponible en la zona protegida. La prueba de la propia superficie de revisión requiere un entorno de producción.

Para limitar la exposición durante el despliegue, puede habilitar la revisión y aprobación unificadas para un grupo específico dentro del entorno de producción de Workfront. Esto le permite ejecutar una prueba piloto de destino con un conjunto de usuarios más pequeño antes de implementarla de forma más amplia.

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### Pruebas interactivas y HTML

+++ Amplíe para ver las preguntas más frecuentes sobre las pruebas interactivas y HTML.

**¿La revisión unificada y la aprobación admiten pruebas interactivas o direcciones URL de HTML?**

Los archivos Zip HTML son compatibles actualmente con las revisiones interactivas. La compatibilidad con URL de HTML (revisión de URL web activa) está en la hoja de ruta y se espera que ocurra en el tercer trimestre.

Consulte las notas de la versión de Workfront en Experience League para ver las actualizaciones.

+++

### Fusión y automatización

+++ Amplíe para ver las preguntas más frecuentes sobre Fusion y automatización.

**¿Necesito que Workfront Fusion utilice la revisión y aprobación unificadas?**

No. La revisión y la aprobación unificadas son una integración de producto nativa y no requieren Fusion. El flujo de trabajo está integrado directamente en Workfront.

**¿Estarán disponibles los conectores Fusion para su revisión y aprobación unificadas?**

Sí. Las acciones de fusión para la revisión y aprobación unificadas están actualmente en desarrollo y se espera que estén disponibles en el tercer trimestre. Consulte las notas de la versión de Workfront en Experience League para ver las actualizaciones cuando estén disponibles.

**¿Se puede usar Fusion para almacenar en déclencheur automáticamente una revisión cuando se carga un documento?**

Sí. Este tipo de automatización es posible mediante los webhooks de Workfront en combinación con Fusion.

**¿Cómo se verán afectados los flujos de trabajo de Fusion existentes creados en Workfront Proof?**

El impacto variará según la forma en que se cree cada flujo de trabajo. En general:

* **Editar o actualizar**: Los flujos de trabajo donde la acción existente relacionada con la revisión tiene un equivalente directo en las aprobaciones unificadas se pueden actualizar para utilizar la nueva acción.

* **Reconstruir**: Es posible que los flujos de trabajo en los que los pasos subyacentes han cambiado significativamente o en los que existen nuevas capacidades deban reconstruirse desde cero.

Una vez que las API de Fusion para las aprobaciones unificadas estén disponibles, se obtendrá una imagen más clara. Se recomienda auditar los flujos de trabajo de Fusion existentes y evaluarlos con las nuevas capacidades de aprobaciones unificadas en ese momento.

+++






