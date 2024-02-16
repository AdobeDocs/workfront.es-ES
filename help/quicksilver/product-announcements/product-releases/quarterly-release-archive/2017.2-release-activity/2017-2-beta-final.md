---
content-type: release-notes
navigation-topic: product-releases-archive
title: Final de la versión beta 2017.2
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 28 de junio de 2017. Estará disponible en el entorno de producción el 26 de julio de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# Final de la versión beta 2017.2

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2017.2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 28 de junio de 2017. Estará disponible en el entorno de producción el 26 de julio de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2017.2, consulte [información general sobre la actividad de la versión 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versión beta final de 2017.2 incluye mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Determinar la disponibilidad del visualizador de pruebas de vídeo HTML5 (ProofHQ y Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Compatibilidad con certificados SHA-256 para SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Tipo previo para atributos de asignación](#type-ahead-for-mapping-attributes)
* [Mejora de la API: Acceso a asignaciones de usuarios](#api-enhancement-access-user-allocations)

**Para todos los usuarios:**

* [Planificador de recursos](#resource-planner)
* [Nueva área de programación en un proyecto (Generador de equipos)](#new-scheduling-area-in-a-project-team-builder)
* [Programación de Recursos: Mostrar Menos Elementos por Defecto](#resource-scheduling-show-fewer-items-by-default)
* [Programación de recursos: Mostrar indicador de colocación y asignación excesiva al arrastrar tareas y problemas](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Horario de recursos: las asignaciones de usuarios ya no se redondean a la media hora más cercana](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exportación del informe de utilización en formatos TSV y PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [Final de la versión beta 2017.2](#user-calendar-enhancements-in-the-my-work-area%22)
* [Final de la versión beta 2017.2](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [La decisión sobre la revisión se muestra en el área Mi trabajo (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [Visualización de pruebas de medios enriquecidos en resoluciones preestablecidas (ProofHQ y Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Ver la URL de las páginas secundarias en los comentarios sobre las pruebas de medios enriquecidos (ProofHQ y Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Creación de vistas personalizadas basadas en vistas estándar existentes (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrado del área de informes (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Visualización de los valores mínimo y máximo en los informes (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Notificación en la aplicación para la aprobación de pruebas](#in-app-notification-for-proof-approval)
* [Mejoras de Mobile](#mobile-improvements)
* [Se agregó una barra diagonal a las instrucciones de filtro para los valores de campo que contienen comas](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Tarifas de facturación múltiples](#multiple-billing-rates)
* [Nuevo campo Hora presupuestada de recurso](#new-resource-budgeted-hour-field)
* [Mostrar la función del usuario en el área &quot;Asignado a&quot; de la página de detalles de tareas y problemas](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nueva área de programación en un proyecto (Generador de equipos) {#new-scheduling-area-in-a-project-team-builder}

El área de Programación de un proyecto (anteriormente conocida como Generador de equipos) se ha rediseñado con una interfaz de usuario actualizada e intuitiva. La nueva funcionalidad de programación ahora se asemeja más a la funcionalidad de programación de recursos disponible actualmente en otras áreas de Workfront.

Las mejoras incluyen:

* Ver las asignaciones de recursos actuales para los miembros del equipo del proyecto, lo que permite tomar decisiones más informadas al realizar asignaciones
* Representación visual de las duraciones de las tareas en la escala de tiempo de programación
* Filtrar la información mostrada en la cronología de programación
* Agregue y elimine usuarios fácilmente del equipo del proyecto, directamente desde la cronología de programación

La siguiente funcionalidad está disponible en otras áreas de la herramienta al programar recursos, pero no está disponible al programar recursos en el área de Team Scheduling:

* Configurar tareas principales para que se muestren en la cronología de la programación
* Configurar nombres de proyectos para que se muestren en la cronología de programación
* Modificar asignaciones de usuarios mediante la herramienta Intercambiar
* Filtrar por portafolio, programas y proyectos

Para obtener más información sobre la funcionalidad disponible en el área de Programación de equipos, consulte &quot;Introducción a la programación de recursos&quot;.

## Programación de Recursos: Mostrar Menos Elementos por Defecto {#resource-scheduling-show-fewer-items-by-default}

De forma predeterminada, ahora se muestran un máximo de 10 elementos de trabajo por día en la cronología de programación de un usuario determinado. Puede expandir la lista para ver todas las tareas y problemas asignados actualmente a ese usuario.

Esto le permite examinar con mayor facilidad la cronología de la programación cuando a los usuarios se les asignan muchas tareas y problemas.

Antes de este cambio, todas las tareas y problemas se mostraban siempre para todos los usuarios.

Para obtener más información sobre la asignación de tareas y problemas a los usuarios en la cronología de programación, consulte &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

## Programación de recursos: Mostrar indicador de colocación y asignación excesiva al arrastrar tareas y problemas {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Al asignar una tarea o un problema a un usuario en la cronología de la programación mediante arrastrar y soltar, ahora se muestra la siguiente información antes de liberar la tarea o el problema y completar la asignación:

* Se muestra un indicador de colocación en la fila del usuario. Esto le permite ver dónde se está asignando un elemento antes de realizar la asignación.
* Si las asignaciones de los usuarios están habilitadas en la cronología de programación, se muestran los indicadores rojos de sobreasignación si al completar la asignación, el usuario se sobreasigna.

Antes de estos cambios, no se mostraba información antes de publicar la tarea o el problema.

Para obtener más información sobre la asignación de tareas y problemas a los usuarios en la cronología de programación, consulte &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

## Horario de recursos: las asignaciones de usuarios ya no se redondean a la media hora más cercana {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Cuando se asignan varios usuarios a una tarea o un problema, o cuando una tarea o un problema abarca varios días, Workfront intenta distribuir las horas planificadas de manera uniforme entre los usuarios y los días asignados. Las horas se redondean a la centésima más cercana de forma predeterminada (por ejemplo, 1,33).

Anteriormente, cuando se modificaban manualmente las horas distribuidas, las horas se ajustaban y redondeaban a la media hora más cercana (por ejemplo, 1,33 se redondeaba a 1,5).

Ahora, las horas ya no se ajustan y se redondean a la media hora más cercana (por ejemplo, 1,33 sigue siendo 1,33).

## Mejora de la API: Acceso a asignaciones de usuarios {#api-enhancement-access-user-allocations}

Ahora puede acceder al sombreado de asignación de usuarios a través de la API de Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exportación del informe de utilización en formatos TSV y PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Ahora puede exportar el informe Utilización de un proyecto en los formatos TSV y PDF, además del formato XLSX.

Antes de este cambio, el informe Utilización solo se podía exportar en formato XLSX.

Para obtener más información sobre la exportación del informe Utilización, consulte [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## La decisión sobre la revisión se muestra en el área Mi trabajo (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Ahora, cuando visualice las aprobaciones de revisión en la pestaña Mis aprobaciones del área Mi trabajo, la decisión sobre la prueba se muestra en el área Mi trabajo y permanece hasta que haga clic en el nuevo botón Actualizar en Workfront o hasta la próxima vez que actualice la página del explorador.

Antes de este cambio, no había indicios de que ya se hubiera tomado una decisión sobre la prueba y esta permanecía en la pestaña Mis aprobaciones hasta que actualizó el explorador.

Para obtener más información, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Visualización de pruebas de medios enriquecidos en resoluciones preestablecidas (ProofHQ y Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

En una versión anterior del entorno de vista previa, presentamos la capacidad de ajustar la resolución de las pruebas de medios enriquecidos especificando una resolución personalizada o arrastrando la imagen a la resolución deseada.

Ahora puede seleccionar entre las opciones de resolución preestablecidas de varios teléfonos, tabletas, portátiles y equipos de escritorio.

Para obtener más información, consulte &quot;Visualización de una resolución de ajuste preestablecido&quot; en [Cambiar la resolución de prueba interactiva en el visor de pruebas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Ver la URL de las páginas secundarias en los comentarios sobre las pruebas de medios enriquecidos (ProofHQ y Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Esta función está disponible actualmente en el entorno de producción.

Ahora, cuando comenta una subpágina en una prueba de medios enriquecidos, la URL de la subpágina se muestra en el comentario.

Antes de este cambio, no estaba claro a qué subpágina se refería el comentario.

Para obtener más información, consulte

## Determinar la disponibilidad del visualizador de pruebas de vídeo HTML5 (ProofHQ y Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Como administrador de Workfront en ProofHQ, puede determinar si los usuarios de su organización tienen acceso al nuevo visualizador de pruebas de HTML5 para las pruebas de vídeo.

Para obtener más información sobre cómo configurar esta opción en Workfront, consulte en .

## Creación de vistas personalizadas basadas en vistas estándar existentes (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Ahora puede crear una vista personalizada basada en una vista estándar. Las opciones Columnas, Orden y Filtros de la vista estándar se incluyen en la nueva vista de forma predeterminada.

Antes de este cambio, para crear una vista personalizada, tenía que crear la vista desde cero. 

Para obtener más información, consulte [Creación de una vista personalizada](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) in [Crear y administrar vistas personalizadas en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtrado del área de informes (ProofHQ) {#filter-the-reporting-area-proofhq}

De forma predeterminada, los datos que se muestran en la ficha Informes incluyen toda la información del sistema de ProofHQ. Ahora puede utilizar filtros para mostrar únicamente información que sea relevante para sus necesidades. 

Para obtener más información, consulte [Filtrado de informes](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) in  [Ejecutar informes en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Visualización de los valores mínimo y máximo en los informes (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Ahora puede configurar si los valores mínimo y máximo se muestran en el gráfico al ver los informes.

Para obtener más información, consulte [Visualización de informes](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) in  [Ejecutar informes en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Compatibilidad con certificados SHA-256 para SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Ahora admitimos el algoritmo hash seguro 256 (SHA-256) al configurar Workfront para SSO con SAML 2.0. Antes de esta versión, solo admitíamos el algoritmo hash seguro 1 (SHA-1).

Para obtener más información sobre la configuración de Workfront con SAML 2.0, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Tipo previo para atributos de asignación {#type-ahead-for-mapping-attributes}

El tipo de campo Valor predeterminado del cuadro de diálogo Asignación de atributos se ha actualizado a un campo de escritura anticipada. Antes de este cambio, el tipo de campo Valor predeterminado era un menú desplegable.

Este cambio se aplica a los siguientes protocolos SSO:

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 no es compatible con la asignación de atributos.

## Mejoras de Mobile {#mobile-improvements}

>[!NOTE]
>
> La aplicación móvil se lanza de forma independiente de la aplicación principal de Workfront. La funcionalidad descrita en esta sección se lanza a principios de agosto.

Verá las siguientes funciones agregadas en las aplicaciones móviles, tanto para las plataformas Android como iOS:

* Envío de solicitudes desde la aplicación móvil
* Nueva entrada de hoja de horas en la aplicación móvil
* Edición de formularios personalizados desde la aplicación móvil
* Solicitudes de aprobación de pruebas en la aplicación móvil

Habrá un programa beta público para algunas de estas funciones para la plataforma Android.

Para obtener más información sobre el próximo programa beta para móviles, consulte la  [&quot;Betas&quot;](https://support.workfront.com/hc/en-us/sections/115000743248) página.

Para obtener más información sobre el uso de la aplicación móvil de Workfront, consulte .  

## Se agregó una barra diagonal a las instrucciones de filtro para los valores de campo que contienen comas {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Cuando crea un filtro en modo de texto y filtra valores de campo que contienen comas, debe agregar una barra diagonal (&quot;/&quot;) antes de las comas que separan los valores para asegurarse de que el valor se lea como una opción de filtro. Esto solo se aplica a los siguientes tipos de campo:

* Dropdowns
* Botones de radio
* Casillas de verificación

Antes de este cambio, no se podía filtrar por campos que tuvieran opciones con comas.

Para obtener más información sobre este cambio, consulte [Resumen de filtros](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Tarifas de facturación múltiples {#multiple-billing-rates}

Ahora puede agregar varias invalidaciones de tarifas de facturación para el mismo rol en el nivel de proyecto. Con esta nueva funcionalidad, puede definir intervalos de fechas para cada anulación de tarifa de facturación. Durante el intervalo de fechas especificado, se aplica una tarifa de facturación diferente a la función de trabajo asignada a las tareas de un proyecto. Las tarifas de facturación se multiplican por las horas en el proyecto para calcular los ingresos. Los ingresos calculados dentro del intervalo de fechas de una tarifa de facturación permanecen bloqueados a esa tarifa y no se actualizan a medida que se actualizan las tarifas de los roles en el proyecto. En el caso de los ingresos reales, no se recalculará ninguna hora registrada antes de anular la tasa de facturación para reflejar la tasa de facturación actual. Las horas registradas antes de que se agregara la anulación de tarifa de facturación al proyecto se asociarán a la tarifa de facturación del rol en ese momento.

Antes de este cambio, podía anular la tarifa de facturación de un rol una sola vez y los ingresos reales se recalcularían para reflejar la tarifa de facturación actual para todas las horas registradas antes de que se cambiara la tarifa de facturación.

Para obtener más información sobre las tarifas de facturación y los ingresos, consulte [Resumen de facturación e ingresos](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para obtener más información sobre la anulación de tarifas de facturación para roles de trabajo en el nivel de proyecto, consulte [Resumen de anulación de Tarifas de facturación de rol y cálculo de ingresos en un proyecto](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Planificador de recursos {#resource-planner}

Con esta versión, presentamos la primera fase del Planificador de recursos, que forma parte del rediseño de la nueva pestaña Planificación en el área de Personas. Mediante el Planificador de recursos, puede presupuestar la cantidad de horas que los usuarios de sus Conjuntos de recursos están asignados en todos los proyectos actuales de los cuales usted es el Administrador de recursos. Puede ver los siguientes números de asignación por proyecto, rol y usuario en el Planificador de recursos:

* Horas disponibles
* Horas planificadas
* Horas presupuestadas
* Desviación de hora (entre las horas presupuestadas y las planificadas)
* Diferencia de hora neta (entre las horas disponibles y las presupuestadas)

Para obtener más información sobre el uso del Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nuevo campo Hora presupuestada de recurso {#new-resource-budgeted-hour-field}

Para admitir la nueva funcionalidad de Planning y el Planificador de recursos, se ha agregado un nuevo campo al Report Builder, que le permite informar sobre las horas presupuestadas del recurso. Este campo registra la cantidad de horas presupuestadas de un recurso en un proyecto. Este campo no está disponible cuando se presupuestan recursos utilizando la funcionalidad Planificación de recursos de legado.

Para obtener más información sobre el uso de horas presupuestadas en el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Notificación en la aplicación para la aprobación de pruebas {#in-app-notification-for-proof-approval}

Cuando se le designe como aprobador de una prueba, recibirá una notificación en la aplicación sobre la aprobación de la prueba a la espera de su decisión. La notificación muestra el siguiente texto: `<User name>` desea que usted apruebe esta revisión&quot;. Si la información del usuario no está disponible, la notificación cambia a &quot;Esta prueba requiere su aprobación&quot;.

Antes de esta mejora, la única indicación visual de que había sido designado aprobador de una prueba era una nueva solicitud de prueba en su área de Mi trabajo.

Para obtener más información sobre las notificaciones en la aplicación, consulte [Visualización y administración de notificaciones en la aplicación](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Mostrar la función del usuario en el área &quot;Asignado a&quot; de la página de detalles de tareas y problemas {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Ahora, al ver la página de detalles de una tarea o un problema, se muestra una función de trabajo debajo del nombre del usuario asignado en el área Asignado a. Este rol representa el rol del usuario que coincide con la asignación de rol de la tarea o problema. Si la tarea o el problema no está asignado a un rol, se muestra el rol principal del usuario asignado.

Antes de este cambio, solo se mostraba el título del usuario debajo de su nombre en el área Asignado a. 
