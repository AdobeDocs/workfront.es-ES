---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.2 Beta 3
description: En esta página se describen todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
TQID: https://experienceleague.adobe.com/OKzzIQnrWd9qvpM-vrh-jVLI3s120i1FaBdQxGpbMcY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1379
ht-degree: 98%

---

# Actividad de la versión 2017.2 Beta 3

En esta página se describen todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para obtener una lista de todos los cambios realizados en la versión 2017.2, consulte [Información general sobre la actividad de la versión 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versión 2017.2 Beta 2 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Restauración de elementos en lotes desde la papelera de reciclaje](#restoring-items-in-bulk-from-the-recycle-bin)
* [La información del usuario se sincroniza de Workfront a ProofHQ (ProofHQ y Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Para todos los usuarios:** 

* [Ver usuarios suscritos](#view-subscribed-users)
* [Configurar cómo se muestran los hitos en el gráfico Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Incluir la leyenda del gráfico Gantt al exportar a PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Ver aprobaciones de revisión en Mi área de trabajo (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Ver los nombres de los usuarios al atender solicitudes de aprobación de revisión desde Mi área de trabajo (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Visor de corrección mejorado para revisiones de vídeo (ProofHQ y Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Ver revisiones de medios enriquecidos en resoluciones alternativas (ProofHQ y Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Nuevo objeto “Creador de revisión” en el informe de versión del documento (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Nueva funcionalidad del conjunto de recursos eliminada temporalmente de la vista previa](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Restauración de elementos en lotes desde la papelera de reciclaje {#restoring-items-in-bulk-from-the-recycle-bin}

Ahora puede restaurar hasta diez proyectos, tareas, problemas o documentos eliminados a la vez.

Antes de este cambio, solo se podía restaurar un elemento eliminado a la vez.

Para obtener más información acerca de cómo restaurar elementos, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Ver usuarios suscritos {#view-subscribed-users}

Ahora puede ver quién se suscribe a un elemento ampliando el número de suscriptores que se muestra junto al vínculo de suscripción.

Antes de esta mejora, no era posible ver quién estaba suscrito a un elemento.

Para obtener más información acerca de la suscripción a elementos, consulte [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Configuración de la vista de los hitos en el gráfico Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Ahora dispone de dos opciones para ver la información de los hitos en un gráfico Gantt. Puede configurar uno de los siguientes indicadores de hito o ambos:

* Diamantes de hito (icono)

  Este icono aparece en el gráfico Gantt después de cualquier tarea asociada a un hito.

* Líneas de hito

  Se muestra una línea después de cualquier tarea asociada con el hito, que abarca todas las tareas del gráfico Gantt.

Antes de este cambio, solo había una opción para permitir que los hitos se mostraran en un gráfico Gantt, llamado “hitos”. Esta opción habilitó tanto el icono de diamante de hito como la línea de hito. Estos indicadores no se han podido separar.

Para obtener más información acerca de cómo configurar cómo se muestra la información en el gráfico Gantt, consulte [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Incluir la leyenda del gráfico Gantt al exportar a un PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Al exportar el gráfico Gantt a un PDF, ahora puede seleccionar si desea exportar también el pie de ilustración del diagrama junto con el propio diagrama. Los elementos incluidos en el pie de ilustración son solo las opciones que ha habilitado para que se muestren en el gráfico Gantt en la interfaz de usuario. Estas opciones se incluyen en la leyenda si existen en las tareas del proyecto. Por ejemplo, si habilita la visualización de hitos en el gráfico Gantt, el pie de ilustración también los mostrará, pero solo si hay al menos una tarea asociada a un hito.

Antes de este cambio, no se podía excluir el pie de ilustración del PDF exportado, y el pie de ilustración incluía todas las opciones y marcadores posibles del Gantt, independientemente de si estaban habilitados o existían en la interfaz de usuario.

Para obtener más información acerca de cómo exportar el gráfico Gantt, consulte [Exportar el gráfico Gantt al PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## La información del usuario se sincroniza de Workfront a ProofHQ (ProofHQ y Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

La información del usuario (nombre y correo electrónico) ahora se sincroniza de Workfront a ProofHQ cuando los usuarios se crean o actualizan en Workfront. 

Para obtener más información sobre la sincronización de usuarios de Workfront a ProofHQ , consulte .

## Nuevo objeto “Creador de revisiones” en el informe Versión del documento (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Ahora, al crear un informe de versión del documento, aparece un nuevo objeto Creador de pruebas. Este objeto permite generar informes con información sobre el usuario que ha creado la prueba. 

El nuevo objeto Creador de revisión del informe Versión del documento contiene todos los campos disponibles con el objeto Usuario existente en otros tipos de informes de objetos.

>[!NOTE]
>
> Esta información solo está disponible en el informe desde el momento en que se introdujo esta función por primera vez en los entornos de vista previa o producción correspondientes; la información de los informes relativa al objeto Solicitante antes de que se introdujera esta funcionalidad no está disponible.

Puede acceder al objeto Creador de revisión al crear un informe de versión de documento, tal como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información acerca del informe del objeto Versión del documento, consulte la sección [Explicación de los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Explicación de los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Ver aprobaciones de revisión en el área de Mi trabajo (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Todas las aprobaciones de revisión que ha enviado para su aprobación ahora se muestran en el área Mi trabajo, en la pestaña **Trabajo enviado para su aprobación**.

Antes de este cambio, la pestaña **Trabajo enviado para su aprobación** no incluía aprobaciones de revisión.

Las aprobaciones de revisión solo se muestran cuando se cumplen los siguientes criterios:

* La aprobación está actualmente pendiente
* El proceso de aprobación se asigna a un usuario con licencia de Workfront (no se muestran los procesos de aprobación asignados a usuarios sin licencia de Workfront)
* Los procesos de aprobación se iniciaron después de publicar esta funcionalidad (no se muestran los procesos de aprobación iniciados antes de publicar esta funcionalidad)

Para obtener más información, consulte [Ver aprobaciones](../../../../review-and-approve-work/manage-approvals/view-approvals.md) en [Ver aprobaciones](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Ver nombres de usuarios al abordar solicitudes de aprobación de revisión desde Mi área de trabajo (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Ahora, al aprobar las aprobaciones de revisión desde el área de Mi trabajo, se muestra el nombre del usuario que solicitó la aprobación.

Para obtener más información, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Visor de corrección mejorado para revisiones de vídeo (ProofHQ y Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

El visor de corrección tanto en Workfront como en ProofHQ se está actualizando con una nueva apariencia, una arquitectura HTML 5 para un mejor rendimiento y compatibilidad con nuevas funcionalidades.

El nuevo visor de corrección incluye las siguientes mejoras:

* Revisión de fotograma a fotograma
* Almacenamiento en búfer de vídeo
* Funcionalidad de búsqueda en la lista de comentarios
* Cualquier acción establecida en el comentario se muestra en cada comentario de la lista de comentarios
* Modo de pantalla completa
* Revisar contenido más rápido o más despacio
* Corrector ortográfico al añadir comentarios y respuestas

### Vista previa

El nuevo visor de corrección está disponible para probarse en los siguientes entornos de vista previa:

* Entorno de vista previa de ProofHQ

  Para obtener más información sobre el entorno de vista previa de ProofHQ, consulte [Entorno de la zona protegida de previsualización: Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Entorno de vista previa de Workfront, cuando su cuenta está habilitada con revisiones

  Para obtener más información sobre el entorno de vista previa de Workfront, consulte [Entorno de la zona protegida de previsualización de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

En esta versión, el nuevo visor de corrección solo admite la revisión de vídeo. Esto significa que todas las revisiones de vídeo aprovechan el nuevo visor de corrección, mientras que todas las revisiones de medios estáticas y enriquecidas siguen aprovechando el visor de corrección existente.

### Producción

Cuando se incluye en el entorno de producción con la versión 17.2, los administradores pueden elegir si el visor de corrección nuevo o heredado es adecuado para los usuarios de su organización. De forma predeterminada, se utilizará el visor de corrección heredado.

Para obtener información sobre cómo utilizar el nuevo visor de corrección de vídeo, consulte  

## Ver revisiones de medios enriquecidos en resoluciones alternativas (ProofHQ y Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Ahora puede ajustar la resolución de las revisiones de medios enriquecidos especificando una resolución personalizada o arrastrando la imagen a la resolución deseada.

Antes de este cambio, podía revisar las pruebas utilizando únicamente la resolución inherente a la pantalla o al dispositivo en el que estaba revisando el contenido.

Puede utilizar el modo de comparación para comparar diferentes resoluciones de revisión.

Para obtener más información, consulte [Abrir revisiones en el visor de corrección de escritorio](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Nueva funcionalidad del conjunto de recursos eliminada temporalmente de la vista previa {#new-resource-pool-functionality-temporarily-removed-from-preview}

Debido a problemas de desarrollo, hemos decidido eliminar la nueva pestaña de Planificación de recursos y volver a denominarla Planificación de recursos heredada con su nombre original “Planificación de recursos”.

La nueva funcionalidad de conjuntos de recursos también se ha eliminado con este cambio. La nueva pestaña de Planificación de recursos y la funcionalidad de los conjuntos de recursos volverán al entorno de la zona protegida de previsualización a finales de junio de 2017.
