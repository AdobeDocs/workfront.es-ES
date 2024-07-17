---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.2 Beta 3
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2 de Beta 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Actividad de la versión 2017.2 Beta 3

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2 de Beta 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 24 de mayo de 2017. Estará disponible en el entorno de producción entre finales de julio y principios de agosto de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para obtener una lista de todos los cambios realizados en 2017.2, consulte [Resumen de la actividad de la versión 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versión 2 de Beta 2017.2 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Restaurando elementos de forma masiva desde la papelera de reciclaje](#restoring-items-in-bulk-from-the-recycle-bin)
* [La información del usuario se sincroniza de Workfront a ProofHQ (ProofHQ y Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Para Todos Los Usuarios:** 

* [Ver usuarios suscritos](#view-subscribed-users)
* [Configurar cómo se muestran los hitos en el gráfico Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Incluir la leyenda del gráfico Gantt al exportar a PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Ver aprobaciones de revisión en Mi área de trabajo (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Ver nombres de usuarios al atender solicitudes de aprobación de revisión desde Mi área de trabajo (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Visor de pruebas mejorado para pruebas de vídeo (ProofHQ y Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Ver revisiones de medios enriquecidos en resoluciones alternativas (ProofHQ y Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Nuevo objeto &#39;Creador de revisión&#39; en el informe de versión del documento (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Nueva funcionalidad de conjunto de recursos eliminada temporalmente de la vista previa](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Restauración de elementos en lote desde la papelera de reciclaje {#restoring-items-in-bulk-from-the-recycle-bin}

Ahora puede restaurar hasta 10 proyectos, tareas, problemas o documentos eliminados a la vez.

Antes de este cambio, solo se podía restaurar un elemento eliminado a la vez.

Para obtener más información acerca de cómo restaurar elementos, vea [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Ver usuarios suscritos {#view-subscribed-users}

Ahora puede ver quién se suscribe a un elemento ampliando el número de suscriptores que se muestra junto al vínculo de suscripción.

Antes de esta mejora, no tenía visibilidad de quién está suscrito a ningún elemento.

Para obtener más información acerca de la suscripción a elementos, vea [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Configurar cómo se muestran los hitos en el gráfico Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Ahora hay dos opciones para ver la información de los hitos en un gráfico Gantt. Puede configurar uno o ambos de los siguientes indicadores de hito:

* Diamantes de hito (icono)

  Este icono aparece en el diagrama de Gantt después de cualquier tarea asociada a un hito.

* Líneas de hito

  Se muestra una línea después de cualquier tarea asociada con el hito, que abarca todas las tareas del gráfico Gantt.

Antes de este cambio, solo había una opción para permitir que los hitos se mostraran en un gráfico Gantt, llamado &quot;hitos&quot;. Esta opción habilitó tanto el icono de diamante de hito como la línea de hito. Estos indicadores no se han podido separar.

Para obtener más información acerca de cómo configurar cómo se muestra la información en el gráfico Gantt, vea [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Incluir la leyenda del gráfico Gantt al exportar a un PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Al exportar el diagrama de Gantt a un PDF, ahora puede seleccionar si desea exportar también el pie de ilustración del diagrama junto con el propio diagrama. Los elementos incluidos en el pie de ilustración son solo las opciones que ha habilitado para mostrarse en el gráfico Gantt en la interfaz de usuario. Estas opciones se incluyen en la leyenda si existen en las tareas del proyecto. Por ejemplo, si habilita la visualización de hitos en el gráfico Gantt, el pie de ilustración también los mostrará, pero solo si hay al menos una tarea asociada a un hito.

Antes de este cambio, no se podía excluir el pie de ilustración del PDF exportado, y el pie de ilustración incluía todas las opciones y marcadores posibles del Gantt, independientemente de si estaban habilitados o existían en la interfaz de usuario.

Para obtener más información acerca de cómo exportar el diagrama de Gantt, vea [Exportar el diagrama de Gantt al PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## La información del usuario se sincroniza de Workfront a ProofHQ (ProofHQ y Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

La información del usuario (nombre y correo electrónico) ahora se sincroniza de Workfront a ProofHQ cuando los usuarios se crean o actualizan en Workfront. 

Para obtener más información sobre la sincronización de usuarios de Workfront a ProofHQ , consulte .

## Nuevo objeto &quot;Creador de pruebas&quot; en el informe Versión del documento (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Ahora, al crear un informe de versión del documento, aparece un nuevo objeto Creador de pruebas. Este objeto permite generar informes con información sobre el usuario que ha creado la prueba. 

El nuevo objeto Creador de pruebas del informe Versión del documento contiene todos los campos disponibles con el objeto Usuario existente en otros tipos de informes de objetos.

>[!NOTE]
>
> Esta información solo está disponible en el informe desde el momento en que se introdujo esta función por primera vez en los entornos de Previsualización o Producción respectivos; la información de los informes relativa al objeto Solicitante antes de que se introdujera esta funcionalidad no está disponible.

Puede acceder al objeto Creador de revisión al crear un informe de versión de documento, tal como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información acerca del informe del objeto Document Version, vea la sección [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Ver aprobaciones de revisión en el área de Mi trabajo (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Todas las aprobaciones de revisión que ha enviado para su aprobación ahora se muestran en el área Mi trabajo, en la ficha **Trabajo enviado para su aprobación**.

Antes de este cambio, la ficha **Trabajo enviado para su aprobación** no incluía aprobaciones de revisión.

Las aprobaciones de pruebas solo se muestran cuando se cumplen los siguientes criterios:

* La aprobación está actualmente pendiente
* El proceso de aprobación se asigna a un usuario con licencia de Workfront (no se muestran los procesos de aprobación asignados a usuarios sin licencia de Workfront)
* Los procesos de aprobación se iniciaron después de publicar esta funcionalidad (no se muestran los procesos de aprobación iniciados antes de publicar esta funcionalidad)

Para obtener más información, consulte [Ver aprobaciones](../../../../review-and-approve-work/manage-approvals/view-approvals.md) en [Ver aprobaciones](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Ver nombres de usuarios al abordar solicitudes de aprobación de revisión desde Mi área de trabajo (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Ahora, al aprobar las aprobaciones de revisión desde el área de Mi trabajo, ahora se muestra el nombre del usuario que solicitó la aprobación.

Para obtener más información, consulte [Aprobación de trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación de trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Visor de pruebas mejorado para pruebas de vídeo (ProofHQ y Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

El visualizador de pruebas tanto en Workfront como en ProofHQ se está actualizando con una nueva apariencia, una arquitectura HTML 5 para un mejor rendimiento y compatibilidad con nuevas funcionalidades.

El nuevo visor de revisión incluye las siguientes mejoras:

* Revisión fotograma a fotograma
* Almacenamiento en búfer de vídeo
* Funcionalidad de búsqueda en la lista de comentarios
* Cualquier acción establecida en el comentario se muestra en cada comentario de la lista de comentarios
* Modo de pantalla completa
* Revisar contenido más rápido o más lento
* Corrector ortográfico al agregar comentarios y respuestas

### Vista previa

El nuevo visor de revisión está disponible para probarse en los siguientes entornos de vista previa:

* Entorno de vista previa de ProofHQ

  Para obtener más información sobre el entorno de vista previa de ProofHQ, consulte [Previsualizar entorno de prueba de espacio aislado- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Entorno de vista previa de Workfront, cuando su cuenta está habilitada con revisión

  Para obtener más información sobre el entorno de vista previa de Workfront, consulte  [Entorno De Zona Protegida De Vista Previa De Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

En esta versión, el nuevo visor de revisión solo admite la revisión de vídeo. Esto significa que todas las pruebas de vídeo aprovechan el nuevo visualizador de pruebas, mientras que todas las pruebas de medios estáticas y enriquecidas siguen aprovechando el visualizador de pruebas existente.

### Producción

Cuando se incluye en el entorno de producción con la versión 17.2, los administradores pueden elegir si el visualizador de pruebas nuevo o heredado es adecuado para los usuarios de su organización. De forma predeterminada, se utilizará el visor de revisión heredado.

Para obtener información sobre cómo utilizar el nuevo visor de revisión de vídeo, consulte  

## Visualización de pruebas de medios enriquecidos en resoluciones alternativas (ProofHQ y Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Ahora puede ajustar la resolución de las pruebas de medios enriquecidos especificando una resolución personalizada o arrastrando la imagen a la resolución deseada.

Antes de este cambio, podía revisar las pruebas utilizando únicamente la resolución inherente a la pantalla o al dispositivo en el que estaba revisando el contenido.

Puede utilizar el modo de comparación para comparar diferentes resoluciones de pruebas.

Para obtener más información, consulte [Abrir pruebas en el Visor de revisiones de escritorio](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Nueva funcionalidad de conjunto de recursos eliminada temporalmente de la vista previa {#new-resource-pool-functionality-temporarily-removed-from-preview}

Debido a los desafíos de desarrollo, hemos decidido eliminar la nueva pestaña de Planificación de recursos y cambiar el nombre de la pestaña de Planificación de recursos heredada por su nombre original de &quot;Planificación de recursos&quot;.

La nueva funcionalidad de conjuntos de recursos también se ha eliminado con este cambio. La nueva pestaña de Planificación de recursos y la funcionalidad de los conjuntos de recursos volverán al entorno de vista previa de espacio aislado a finales de junio de 2017.
