---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versión final de 2017.2 Beta
description: En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 28 de junio de 2017. Estará disponible en el entorno de producción el 26 de julio de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
TQID: https://experienceleague.adobe.com/7tfTmpf1SXBHaK8rlrRGMLI-ikA-w6jqmQhMlVkKawQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 2332
ht-degree: 98%

---

# Versión final de 2017.2 Beta

En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 28 de junio de 2017. Estará disponible en el entorno de producción el 26 de julio de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para obtener una lista de todos los cambios realizados en la versión 2017.2, consulte [Información general sobre la actividad de la versión 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versión final 2017.2 de Beta incluye mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Determinar la disponibilidad del visualizador de corrección de vídeo de HTML5 (ProofHQ y Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Admitir certificados SHA-256 para SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Escritura anticipada para atributos de asignación](#type-ahead-for-mapping-attributes)
* [Mejora de la API: acceso a asignaciones de usuarios](#api-enhancement-access-user-allocations)

**Para todos los usuarios:**

* [Planificador de recursos](#resource-planner)
* [Nueva área de programación en un proyecto (Generador de equipos)](#new-scheduling-area-in-a-project-team-builder)
* [Programación de recursos: mostrar menos elementos de forma predeterminada](#resource-scheduling-show-fewer-items-by-default)
* [Programación de recursos: mostrar indicador de pérdida y asignación excesiva al arrastrar tareas y problemas](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Programación de recursos: las asignaciones de usuarios ya no se redondean a la media hora más cercana](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exportar el informe de utilización en formatos TSV y PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [Versión final de 2017.2 Beta](#user-calendar-enhancements-in-the-my-work-area%22)
* [Versión final de 2017.2 Beta](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Se muestra la decisión de la revisión en Mi área de trabajo (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [Ver pruebas de medios enriquecidos en resoluciones preestablecidas (ProofHQ y Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Ver la URL de las páginas secundarias en los comentarios de las revisiones de medios enriquecidos (ProofHQ y Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Crear vistas personalizadas basadas en vistas estándar existentes (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrar el área de informes (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Mostrar valores mínimos y máximos en los informes (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Notificación en la aplicación para la aprobación de la revisión](#in-app-notification-for-proof-approval)
* [Mejoras en la aplicación móvil](#mobile-improvements)
* [Se añadió una barra diagonal a las instrucciones de filtro para los valores de campo que contienen comas](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Múltiples tarifas de facturación](#multiple-billing-rates)
* [Nuevo campo de horas presupuestadas del recurso](#new-resource-budgeted-hour-field)
* [Mostrar la función del usuario en el área “Asignado a” de la página de detalles de tareas y problemas](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre el Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nueva área de programación en un proyecto (Generador de equipos) {#new-scheduling-area-in-a-project-team-builder}

El área de Programación de un proyecto (anteriormente conocida como Generador de equipos) se ha rediseñado con una interfaz de usuario actualizada y más intuitiva. La nueva funcionalidad de programación ahora se asemeja más a la funcionalidad de programación de recursos disponible actualmente en otras áreas de Workfront.

Las mejoras incluyen:

* Ver las asignaciones de recursos actuales para los miembros del equipo del proyecto, lo que permite tomar decisiones más informadas al realizar asignaciones
* Representación visual de las duraciones de las tareas en la cronología de programación
* Filtrar la información mostrada en la cronología de programación
* Añada y elimine usuarios fácilmente del equipo del proyecto, directamente desde la cronología de programación

La siguiente funcionalidad está disponible en otras áreas de la herramienta al programar recursos, pero no está disponible al programar recursos en el área de programación de equipos:

* Configurar tareas principales para que se muestren en la cronología de programación
* Configurar nombres de proyectos para que se muestren en la cronología de programación
* Modificar asignaciones de usuarios mediante la herramienta de intercambio
* Filtrar por portafolio, programas y proyectos

Para obtener más información sobre la funcionalidad disponible en el área Horario de equipo, consulte &quot;Introducción al horario de recursos&quot;.

## Horario de recursos: mostrar menos elementos de forma predeterminada {#resource-scheduling-show-fewer-items-by-default}

De forma predeterminada, ahora se muestran un máximo de 10 elementos de trabajo por día en la cronología de programación de un usuario determinado. Puede expandir la lista para ver todas las tareas y problemas asignados actualmente a ese usuario.

Esto le permite examinar con mayor facilidad la cronología de la programación cuando a los usuarios se les asignan muchas tareas y problemas.

Antes de este cambio, todas las tareas y problemas se mostraban siempre para todos los usuarios.

Para obtener más información sobre la asignación de tareas y problemas a los usuarios en la cronología de programación, consulte &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

## Horario de recursos: mostrar indicador de soltar y asignación excesiva al arrastrar tareas y problemas {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Al asignar una tarea o un problema a un usuario en la cronología de la programación mediante arrastrar y soltar, ahora se muestra la siguiente información antes de liberar la tarea o el problema y completar la asignación:

* Se muestra un indicador de soltar en la fila del usuario. Esto le permite ver dónde se está asignando un elemento antes de realizar la asignación.
* Si las asignaciones de los usuarios están habilitadas en la cronología de programación, se muestran los indicadores rojos de asignación excesiva si al completar la asignación, hay una sobreasignación del usuario.

Antes de estos cambios, no se mostraba información antes de publicar la tarea o el problema.

Para obtener más información sobre la asignación de tareas y problemas a los usuarios en la cronología de programación, consulte &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

## Horario de recursos: las asignaciones de usuarios ya no se redondean a la media hora más cercana {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Cuando se asignan varios usuarios a una tarea o un problema, o cuando una tarea o un problema abarca varios días, Workfront intenta distribuir las horas planificadas de manera uniforme entre los usuarios y los días asignados. Las horas se redondean a la centésima más cercana de forma predeterminada (por ejemplo, 1,33).

Anteriormente, cuando se modificaban manualmente las horas distribuidas, las horas se ajustaban y redondeaban a la media hora más cercana (por ejemplo, 1,33 se redondeaba a 1,5).

Ahora, las horas ya no se ajustan y se redondean a la media hora más cercana (por ejemplo, 1,33 sigue siendo 1,33).

## Mejora de la API: acceso a asignaciones de usuarios {#api-enhancement-access-user-allocations}

Ahora puede acceder al sombreado de asignación de usuarios a través de la API de Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exportación del informe de utilización en los formatos TSV y PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Ahora puede exportar el informe de utilización de un proyecto en los formatos TSV y PDF, además del formato XLSX.

Antes de este cambio, el informe de utilización solamente se podía exportar en formato XLSX.

Para obtener más información sobre la exportación del informe de utilización, consulte [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en [Información general sobre el informe utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## La decisión de la revisión se muestra en el área Mi trabajo (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Ahora, cuando visualice las aprobaciones de revisión en la pestaña Mis aprobaciones del área Mi trabajo, la decisión de la revisión se muestra en el área Mi trabajo y permanece allí hasta que haga clic en el nuevo botón Actualizar en Workfront o hasta la próxima vez que actualice la página del explorador.

Antes de este cambio, no había indicios de que ya se hubiera tomado una decisión de la prueba y esta permanecía en la pestaña Mis aprobaciones hasta que actualizara el explorador.

Para obtener más información, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Visualización de revisiones de medios enriquecidos en resoluciones de ajuste preestablecido (ProofHQ y Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

En una versión anterior del entorno de vista previa, hablamos de la posibilidad de ajustar la resolución de las revisiones de medios enriquecidos especificando una resolución personalizada o arrastrando la imagen a la resolución deseada.

Ahora puede seleccionar entre las opciones de resolución de ajuste preestablecido de varios teléfonos, tabletas, portátiles y equipos de escritorio.

Para obtener más información, consulte “Visualización de una resolución de ajuste preestablecido” en [Cambiar la resolución de revisión interactiva en el visualizador de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Visualización de la URL a las subpáginas en los comentarios de revisiones de medios enriquecidos (ProofHQ y Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Esta función ya está disponible en el entorno de producción.

Ahora, cuando comente una subpágina en una revisión de medios enriquecidos, la URL de la subpágina se muestra en el comentario.

Antes de este cambio, no estaba claro a qué subpágina se refería el comentario.

Para obtener más información, consulte

## Determinar la disponibilidad del visor de corrección de vídeo HTML5 (ProofHQ y Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Como administrador de Workfront en ProofHQ, puede determinar si los usuarios de su organización tienen acceso al nuevo visor de corrección HTML5 para las revisiones de vídeo.

Para obtener más información sobre la configuración de esta opción en Workfront, consulte.

## Creación de vistas personalizadas basadas en vistas estándar existentes (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Ahora puede crear una vista personalizada basada en una vista estándar. Las opciones Columnas, Orden y Filtros de la vista estándar se incluyen en la nueva vista de forma predeterminada.

Antes de este cambio, para poder crear una vista personalizada, tenía que crear la vista desde cero. 

Para obtener más información, consulte [Creación de una vista personalizada](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) en [Creación y administración de vistas personalizadas en Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtro del área de creación de informes (ProofHQ) {#filter-the-reporting-area-proofhq}

De forma predeterminada, los datos que se muestran en la ficha Informes incluyen toda la información del sistema de ProofHQ. Ahora puede utilizar filtros para mostrar únicamente información que sea relevante para sus necesidades. 

Para obtener más información, consulte [Filtro de creación de informes](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) en  [Ejecutar informes en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Visualización de los valores mínimo y máximo en los informes (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Ahora puede configurar si los valores mínimo y máximo se muestran en el gráfico al ver los informes.

Para obtener más información, consulte [Visualización de informes](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) en  [Ejecutar informes en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Compatibilidad con certificados SHA-256 para SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Ahora admitimos el algoritmo hash seguro 256 (SHA-256) al configurar Workfront para SSO con SAML 2.0. Antes de esta versión, solo admitíamos el algoritmo hash seguro 1 (SHA-1).

Para obtener más información sobre la configuración de Workfront con SAML 2.0, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Escritura anticipada para atributos de asignación {#type-ahead-for-mapping-attributes}

El tipo de campo Valor predeterminado del cuadro de diálogo Asignación de atributos se ha actualizado a un campo de escritura anticipada. Antes de este cambio, el tipo de campo Valor predeterminado era un menú desplegable.

Este cambio se aplica a los siguientes protocolos SSO:

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 no es compatible con la asignación de atributos.

## Mejoras para móviles {#mobile-improvements}

>[!NOTE]
>
> La aplicación móvil se lanza de forma independiente de la aplicación principal de Workfront. La funcionalidad descrita en esta sección se lanza a principios de agosto.

Verá la siguiente funcionalidad incorporada en las aplicaciones móviles, tanto para plataformas Android como iOS:

* Envío de solicitudes desde la aplicación móvil
* Nueva entrada de plantilla de horas en la aplicación móvil
* Edición de formularios personalizados desde la aplicación móvil
* Solicitudes de aprobación de pruebas en la aplicación móvil

Habrá un programa beta público para algunas de estas características para la plataforma Android.

Para obtener más información sobre el próximo programa beta para móviles, consulte la página [“Betas”](https://support.workfront.com/hc/en-us/sections/115000743248).

Para obtener más información sobre el uso de la aplicación móvil de Workfront, consulte .  

## Se ha añadido una barra diagonal a las instrucciones de filtro para los valores de campo que contienen comas {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Cuando crea un filtro en modo de texto y filtra valores de campo que contienen comas, debe agregar una barra diagonal (“/”) antes de las comas que separan los valores para asegurarse de que el valor se lea como una opción de filtro. Esto solo se aplica a los siguientes tipos de campo:

* Menús desplegables
* Botones de radio
* Casillas de verificación

Antes de este cambio, no se podía filtrar por campos que tuvieran opciones con comas.

Para obtener más información acerca de este cambio, consulte [Información general sobre filtros](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Múltiples tarifas de facturación {#multiple-billing-rates}

Ahora puede añadir varias anulaciones de tarifas de facturación para la misma función en el nivel de proyecto. Con esta nueva funcionalidad, puede definir intervalos de fechas para cada anulación de tarifa de facturación. Durante el intervalo de fecha especificado, se aplica una tarifa de facturación diferente a la función asignada a las tareas de un proyecto. Las tarifas de facturación se multiplican por las horas del proyecto para calcular los ingresos. Los ingresos calculados dentro del intervalo de fecha de una tarifa de facturación permanecen bloqueados en esa tarifa y no se actualizan a medida que se actualizan las tarifas de las funciones en el proyecto. En el caso de los ingresos reales, no se recalculará ninguna hora registrada antes de anular la tarifa de facturación para reflejar la tarifa de facturación actual. Las horas registradas antes de que se agregara la anulación de tarifa de facturación al proyecto se asociarán a la tarifa de facturación de la función en ese momento.

Antes de este cambio, podía anular la tarifa de facturación de una función una sola vez y los ingresos reales se recalcularían para reflejar la tarifa de facturación actual para todas las horas registradas antes de que se cambiara la tarifa de facturación.

Para obtener más información sobre las tarifas de facturación y los ingresos, consulte [Información general sobre facturación e ingresos](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para obtener más información sobre la anulación de tarifas de facturación para las funciones en el nivel de proyecto, consulte [Información general sobre cómo anular las tarifas de facturación de funciones y calcular los ingresos de un proyecto](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Planificador de recursos {#resource-planner}

Con esta versión, presentamos la primera fase del Planificador de recursos, que forma parte del rediseño de la nueva pestaña Planificación del área Personas. Mediante el Planificador de recursos, puede presupuestar la cantidad de horas que los usuarios de sus conjuntos de recursos están asignados en todos los proyectos actuales de los cuales es el gerente de recursos. Puede ver los siguientes números de asignación por proyecto, función y usuario en el Planificador de recursos:

* Horas disponibles
* Horas planificadas
* Horas presupuestadas
* Variación de horas (entre las horas presupuestadas y las planificadas)
* Diferencia de horas netas (entre las horas disponibles y las presupuestadas)

Para obtener más información sobre el uso del Planificador de recursos, consulte [Información general sobre el Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nuevo campo de horas presupuestadas del recurso {#new-resource-budgeted-hour-field}

Para admitir la nueva funcionalidad Planificación y el Planificador de recursos, se ha añadido un nuevo campo al Report Builder, que le permite informar sobre las horas presupuestadas del recurso. Este campo registra la cantidad de horas presupuestadas de un recurso en un proyecto. Este campo no está disponible cuando se presupuestan recursos utilizando la funcionalidad de planificación de recursos heredada.

Para obtener más información sobre el uso de horas presupuestadas en el Planificador de recursos, consulte [Información general sobre el Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Notificación en la aplicación para la aprobación de pruebas {#in-app-notification-for-proof-approval}

Cuando se le designe aprobador de una prueba, se le notificará en la aplicación que la aprobación de la prueba está a la espera de su decisión. La notificación mostrará el siguiente texto: “`<User name>` desea que apruebe esta prueba”. Si la información del usuario no está disponible, la notificación cambiará a “Esta prueba requiere su aprobación”.

Antes de esta mejora, la única indicación visual de que se le había designado aprobador de una prueba era una nueva solicitud de prueba en el área Mi trabajo.

Para obtener más información sobre las notificaciones en la aplicación, consulte [Ver y administrar notificaciones en la aplicación](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Mostrar la función del usuario en el área “Asignado a” de la página de detalles de tareas y problemas {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Ahora, al ver la página de detalles de una tarea o un problema, se muestra una función debajo del nombre del usuario asignado en el área Asignado a. Esta función representa la función del usuario que coincide con la asignación de función de la tarea o problema. Si la tarea o el problema no se ha asignado a una función, se muestra la función principal del usuario asignado.

Antes de este cambio, solo se mostraba la forma de tratamiento del usuario debajo de su nombre en el área Asignado a. 
