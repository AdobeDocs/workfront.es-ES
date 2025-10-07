---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión final de Beta 2017.3
description: Esta página describe todos los cambios más recientes disponibles en el entorno de vista previa con la versión final de Beta 2017.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 12 de septiembre de 2017. Estuvo disponible en el entorno de producción a principios de noviembre de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f5044d457ebf203269e8007075e98ba4c136660f
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 100%

---

# Actividad de la versión final de Beta 2017.3

Esta página describe todos los cambios más recientes disponibles en el entorno de vista previa con la versión final de Beta 2017.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 12 de septiembre de 2017. Estuvo disponible en el entorno de producción a principios de noviembre de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en 2017.3, consulte [Información general de la actividad de la versión 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versión final de Beta 2017.3 incluye mejoras para administradores de Workfront y otros usuarios:

**Para los administradores**

* [Nueva configuración para recuperar solicitudes en el área de configuración de aprobación](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Configurar funciones de prueba predeterminadas](#configure-default-proof-roles)

**Para todos los usuarios**

* [Área de inicio (se ha actualizado mi área de trabajo)](#home-area-updated-my-work-area)

* [Plantilla de diseño actualizada para admitir el área de inicio](#updated-layout-template-to-support-the-home-area)

* [Kanban para Agile](#kanban-for-agile)
* [Incluir problemas en el Registro de asuntos pendientes de Scrum para un Equipo ágil](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Incluir problemas en el panel de historias de Scrum Agile](#include-issues-on-the-scrum-agile-story-board)
* [Aplicar agrupaciones y filtros al registro de asuntos pendientes para un Equipo ágil](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Devuelve la funcionalidad de @Tagging mejorada en el entorno de vista previa](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [Las actualizaciones del sistema de filtros en el flujo de actualizaciones ahora son persistentes entre objetos](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Visualizar datos en el informe de utilización](#visualize-data-in-the-utilization-report)
* [Mejora del rendimiento del informe de utilización](#utilization-report-performance-improvement)
* [Mejoras en el documento: interfaz optimizada](#document-enhancements-streamlined-interface)
* [Mejoras de revisión en Workfront](#proofing-enhancements-within-workfront)
* [Mejoras de revisión tanto en Workfront Proof como en Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Formato de texto enriquecido para actualizaciones y correos electrónicos](#rich-text-formatting-for-updates-and-emails)
* [Nuevo rediseño del gráfico Gantt](#new-gantt-chart-redesign)
* [Los informes integrados contienen descripciones actualizadas](#built-in-reports-contain-updated-descriptions)
* [Personalización de marca en informes, listas y paneles de control exportados](#branding-in-exported-reports-lists-and-dashboards)
* [Mejoras al copiar tareas y mover tareas o problemas](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Nueva agrupación para informes de horas presupuestadas de recursos: fecha de asignación](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Mejoras del Planificador de recursos](#resource-planner-improvements)
* [Mejoras móviles](#mobile-improvements)
* [Integración de Workfront con Slack](#workfront-integration-with-slack)
* [Mejoras de Outlook 365](#outlook-365-improvements)
* [Cambios de API](#api-changes)

## Área de inicio (se ha actualizado mi área de trabajo) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Esta funcionalidad no se lanzará al entorno de producción con la versión 17.3; permanecerá en la versión de vista previa hasta principios de 2018.

La nueva área de Inicio proporciona una vista alternativa y mejorada de los mismos datos que están disponibles actualmente en el área de Mi trabajo. El área de Inicio proporciona los siguientes beneficios sobre el área Mi trabajo:

* Una interfaz más ágil e intuitiva
* Rendimiento mejorado

La siguiente funcionalidad está disponible en el área Mi trabajo, pero aún no se ha implementado en el área de Inicio:

* Ver su calendario personal
* Actualizar tareas y problemas con formato de texto enriquecido
* Aprobar pruebas
* Ver una lista de los trabajos enviados para su aprobación
* Crear un problema ad hoc en un proyecto
* Ver solo las aprobaciones que se le han delegado

Para obtener más información sobre cómo usar el área de inicio nueva, vea [Usar el área de inicio](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Plantilla de diseño actualizada para admitir el área de inicio {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Esta funcionalidad no se lanzará al entorno de producción con la versión 17.3; permanecerá en la versión de vista previa hasta principios de 2018.

Como administrador de Workfront, puede determinar si los usuarios de su organización tienen acceso al área de Inicio configurando la plantilla de diseño a la que están asignados. Los usuarios que no tengan asignada una plantilla de diseño siempre pueden acceder al área de Inicio.

Para obtener más información, consulte “Personalización del inicio” en “Creación y administración de plantillas de diseño”

## Kanban para Agile  {#kanban-for-agile}

Los equipos de Agile ahora pueden utilizar una metodología Kanban dentro de Workfront, además de la metodología Scrum Agile ya compatible.

Las metodologías Agile de Scrum y Kanban en Workfront difieren en los siguientes aspectos:

**Ventajas de usar Kanban en Workfront**

* Mostrar el Registro de asuntos pendientes en el tablero de historias ágil Kanban.

  Para obtener más información, consulte.

* Configura los elementos del Registro de asuntos pendientes para que se añadan automáticamente al tablero de historias ágil Kanban cuando otros elementos se muevan a un estado que equivalga a Completado.

  Para obtener más información, consulte [Configurar historias para que se añadan automáticamente desde el registro de asuntos pendientes](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) en [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure un límite de trabajo en curso (WIP) para que se muestre en el panel de historias ágil de Kanban.

  Para obtener más información, consulte [Configurar el límite de trabajo en curso (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) en [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Ventajas de usar Scrum en Workfront**

* Agregue un conjunto de historias a una iteración Agile y cree un guion gráfico para esa iteración.
* Incluir problemas en el guion gráfico de Scrum.
* Incluye problemas en el registro de pendientes de un equipo ágil.

  Para obtener más información, consulte [Configurar cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Las subtareas se pueden mostrar en el guion gráfico de Scrum.
* Vea un gráfico de evolución para ver el progreso de las historias durante la iteración.

  Para obtener más información, consulte [Información general del gráfico de evolución Agile](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Para obtener más información sobre cómo habilitar y configurar Kanban para un equipo ágil, consulte [Decidir sobre una metodología ágil](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) en [Crear un equipo ágil](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Incluir problemas en el registro de asuntos pendientes de Scrum para un equipo ágil {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Esta funcionalidad se eliminó del entorno de producción el 14 de noviembre de 2017. Está previsto que se vuelva a introducir en el entorno de vista previa a principios de 2018 con un diseño mejorado y una mayor estabilidad. Estará disponible en el entorno de producción con la versión 2018.1.

Ahora puedes incluir problemas en el registro de asuntos pendientes de tu equipo ágil cuando usas la metodología ágil Scrum (los problemas no se muestran en el registro de asuntos pendientes de un equipo ágil cuando se usa la metodología Kanban). Los equipos de Scrum agile existentes deben habilitar esta funcionalidad para que se incluyan los problemas. Los problemas se incluyen automáticamente en el registro de pendientes para los equipos de Scrum Agile creados después de la versión 2017.3.

Antes de este cambio, solo se podían agregar tareas al registro de pendientes. Si desea agregar un problema, primero tenía que convertirlo en una tarea antes de que se pudiera agregar.

Dado que ahora tiene acceso a algo más que a las tareas del registro de asuntos pendientes, todas las vistas de tareas personalizadas que antes estaban disponibles en el registro de asuntos pendientes se copian y se agregan al registro de asuntos pendientes como vistas de elementos de trabajo pendientes personalizadas.

Para obtener información sobre el uso de los problemas en el registro de pendientes, consulte [Administrar el registro de pendientes Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Para obtener información sobre cómo habilitar la disponibilidad de problemas en el registro de pendientes de un equipo de Agile Scrum, consulte [Configurar cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Incluir problemas en el panel de historias de Scrum Agile {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Esta funcionalidad se eliminó del entorno de producción el 14 de noviembre de 2017. Está previsto que se vuelva a introducir en el entorno de vista previa a principios de 2018 con un diseño mejorado y una mayor estabilidad. Estará disponible en el entorno de producción con la versión 2018.1.

Ahora puede incluir problemas en el guion gráfico al utilizar la metodología Scrum agile.

Para obtener más información, consulte [Configurar columnas de estado en el panel de historias ágiles](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) en [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Aplicar agrupaciones y filtros al registro de pendientes para un equipo ágil {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Esta funcionalidad se eliminó del entorno de producción el 14 de noviembre de 2017. Está previsto que se vuelva a introducir en el entorno de vista previa a principios de 2018 con un diseño mejorado y una mayor estabilidad. Estará disponible en el entorno de producción con la versión 2018.1.

Las opciones de Agrupación y Filtro ahora están disponibles en el registro de asuntos pendientes de Agile, lo que le permite organizar el registro de asuntos pendientes por agrupaciones, así como filtrar por tareas y problemas específicos.

Antes de este cambio, podía aplicar en las vistas al registro de pendientes de Agile.

Para obtener más información, consulte [Administrar el registro de pendientes Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) en [Administrar el registro de pendientes Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Formato de texto enriquecido para actualizaciones y correos electrónicos {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Los cambios de formato que realice en el entorno de vista previa podrían volver al estado sin formato.

Ahora puede resaltar información importante dando formato a los comentarios y actualizaciones que realice en los objetos de Workfront. 

Con las herramientas Texto enriquecido, puede aplicar atributos de formato al texto, crear listas numeradas y con viñetas y agregar hipervínculos a recursos adicionales.

El formato aplicado a los comentarios en el flujo de actualización también se muestra en las notificaciones de actualización por correo electrónico. Para obtener más información sobre cómo dar formato a los comentarios, vea [Actualizar el trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Devuelve la funcionalidad de @Tagging mejorada en el entorno de vista previa {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Una vez más, puede utilizar el símbolo @ para etiquetar a otros usuarios en el flujo de actualización de todos los objetos del entorno de vista previa. En el pasado, @tagging colocaba el nombre y los apellidos del usuario etiquetado en el flujo de actualización. Ahora, la funcionalidad de @tagging mejorada solo muestra el nombre del usuario. Para obtener más información sobre cómo etiquetar usuarios en las actualizaciones, consulte [Etiquete a los usuarios en las actualizaciones](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Las actualizaciones del sistema de filtros en el flujo de actualizaciones ahora son persistentes entre objetos {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

La opción Filtrar actualizaciones del sistema ahora es persistente entre objetos del sitio de Workfront. Esto le permite ocultar las actualizaciones del sistema y ver solamente los comentarios del usuario en el flujo de actualización de un objeto, así como mantener esa configuración mientras navega a otros objetos.

Antes de este cambio, tenía que filtrar las actualizaciones del sistema para cada objeto a medida que navegaba por el sitio de Workfront.

Para obtener más información, consulte [Trabajo de actualización](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visualizar datos en el informe Utilización {#visualize-data-in-the-utilization-report}

 Ahora puede ver la información de ver información de utilización en un gráfico. 

Para obtener más información, consulte [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Mejora del rendimiento del informe de utilización {#utilization-report-performance-improvement}

>[!NOTE]
>
>Esta función se publicó en un parche después de la versión final Beta.

Ahora, al ejecutar un informe de utilización, se le pedirá que aplique un filtro antes de ejecutar el informe. Este cambio garantiza que la información más relevante se genere en el informe Utilización lo antes posible.

Para obtener más información sobre cómo ejecutar un informe de utilización, vea [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en [Información general sobre el informe de utilización de recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Mejoras en el documento: interfaz optimizada {#document-enhancements-streamlined-interface}

La experiencia del usuario para agregar documentos a Workfront es ahora más ágil e intuitiva. Ahora puede cargar un documento desde el sistema de archivos, solicitar un documento o vincular un archivo desde una aplicación de terceros (como Google o Dropbox), todo ello desde un sencillo menú desplegable. 

Anteriormente, estas opciones estaban disponibles al iniciar el cuadro de diálogo Agregar documentos. 

Para obtener más información, consulte el artículo:

* [Agregar documentos a Adobe Workfront desde su sistema de archivos](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Solicitar un documento](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Vinculación de documentos desde aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Con este cambio, ya no está disponible la opción de pegar una imagen o un documento desde el portapapeles.

## Mejoras de revisión en Workfront {#proofing-enhancements-within-workfront}

* [Experiencia del usuario mejorada y funcionalidad adicional](#improved-user-experience-and-additional-functionality)
* [Compartir directamente desde el visor de corrección](#share-directly-from-the-proofing-viewer)
* [Configurar funciones de prueba predeterminadas](#configure-default-proof-roles)

### Experiencia del usuario mejorada y funcionalidad adicional {#improved-user-experience-and-additional-functionality}

Además de mejorar la experiencia del usuario al crear pruebas en Workfront, ya están disponibles las siguientes funciones adicionales:

* Combinación de varios archivos en una sola prueba.
* Pruebe sitios web en múltiples resoluciones (se pueden crear pruebas individuales para cada resolución o combinarlas en una sola prueba).
* Edite el nombre del archivo durante el proceso de carga.
* Incluya campos personalizados en el formulario de creación de prueba.
* Agregue un mensaje personalizado a las notificaciones de prueba por correo electrónico.
* Configuración de prueba adicional 
* Validación de errores en tiempo real al revisar una dirección URL (anteriormente, tenía que esperar varios minutos antes de que se mostrara un error)

Para obtener más información, consulte.

>[!NOTE]
>
> Al crear una nueva prueba con flujo de trabajo automatizado, no se admite arrastrar y soltar para mover usuarios de una fase a otra. En su lugar, elimine el usuario de un paso y agréguelo a otro.

*La opción para mover usuarios de un paso a otro mediante arrastrar y soltar se volverá a incluir en la versión 2018.1.*

### Compartir directamente desde el visor de corrección {#share-directly-from-the-proofing-viewer}

Ahora puede compartir con usuarios específicos de Workfront directamente desde el visualizador de corrección.

>[!NOTE]
>
>Esta funcionalidad solo está disponible para nuevas pruebas (pruebas creadas después de la versión 2017.3) y solo para instancias de Workfront integradas con una cuenta de Workfront Proof Premium.

Antes de este cambio, solo podía compartir creando un vínculo y luego compartiéndolo con un usuario. 

Para obtener más información, consulte [Compartir una revisión en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en [Compartir una revisión en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Configurar funciones de prueba predeterminadas {#configure-default-proof-roles}

Ahora puede configurar las funciones de prueba predeterminadas que tienen los usuarios nuevos y los usuarios invitados para las nuevas pruebas dentro del sistema de Workfront. 

Esta es la función predeterminada a la que se asignan los usuarios en una prueba cuando esta se comparte con ellos. 

## Mejoras de revisión tanto en Workfront Proof como en Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Reiniciar y omitir en el visualizador de pruebas de vídeo de HTML5 (métodos abreviados del teclado)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Actualizaciones del visor de revisión de HTML5](#html5-proofing-viewer-updates)

### Reiniciar y omitir en el visualizador de pruebas de vídeo de HTML5 (métodos abreviados del teclado) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Ahora existen métodos abreviados de teclado en el visualizador de pruebas de HTML5 para vídeo que le permiten reiniciar el vídeo desde el principio y saltar al final del vídeo.

Para obtener más información sobre los métodos abreviados de teclado disponibles, consulte [Métodos abreviados de teclado en el visor de revisión de Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Actualizaciones del visor de revisión de HTML5 {#html5-proofing-viewer-updates}

El visor de HTML5 ahora admite pruebas estáticas.

Antes de este cambio, el visor de HTML5 solo admitía pruebas de vídeo. 

El visualizador de HTML incluye las siguientes funciones nuevas al revisar el contenido estático:

* Haga un único comentario con anotaciones en varias páginas cuando esté en vista única

  Anteriormente, esto solo era posible en la Vista continua o en la Vista de revista

* Navegar por las pruebas a través de las miniaturas de prueba

   * Identifique fácilmente la parte de la prueba que se está revisando. Esto es importante, especialmente cuando los usuarios trabajan con pruebas de mayor formato y páginas web largas, o en cualquier momento en que se necesita un nivel de zoom mayor para ver los detalles.
   * Cambiar el nivel de zoom
   * Panorámica del contenido

* Especifique valores personalizados en la herramienta Medición
* Al anotar texto dentro de una prueba en el visor de pruebas en Workfront Proof, puedes incluir opciones para indicar que el texto debe estar en negrita, cursiva o subrayado.

El visor de HTML5 todavía no admite todas las funciones disponibles actualmente en el visor de Flash existente. Las siguientes funciones no están disponibles actualmente, pero se incluirán en una versión futura:

* Compatibilidad con archivos multimedia enriquecidos
* Modo de comparación (vídeo y estático)
* Filtrar comentarios (vídeo y estáticos)
* Revisar hipervínculos en documentos (estáticos)
* Traducciones (vídeo y estáticas)
* Indicador de presencia que muestra los usuarios que actualmente están trabajando en la prueba
* Compartir pruebas

Para obtener más información sobre la revisión de pruebas estáticas en el visor de HTML5, consulte.

Como administrador de Workfront en Workfront Proof, puede determinar si los usuarios de su organización tienen acceso al nuevo visor de pruebas de HTML5 para pruebas de vídeo.

## Nuevo rediseño del gráfico Gantt {#new-gantt-chart-redesign}

El nuevo gráfico Gantt incluye las siguientes mejoras:

* Nuevos iconos y marcadores
* Nueva opción para acercar y alejar un lapso de tiempo específico
* Celdas de tarea más pequeñas en la parte de lista del gráfico
* Opciones rediseñadas para ajustes, impresión y cambio a Fechas proyectadas.

Para obtener más información acerca de cómo configurar opciones en el gráfico Gantt, vea [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Los informes integrados contienen descripciones actualizadas {#built-in-reports-contain-updated-descriptions}

Hemos actualizado las descripciones de los informes de sistema en Workfront para incluir información sobre el tipo de informe y los campos incluidos.  

Antes de este cambio, la mayoría de nuestros informes integrados no tenían descripciones o eran muy limitados.

Para obtener más información sobre los informes integrados, consulte [Uso de informes integrados de Adobe Workfront](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Personalización en informes, listas y paneles de control exportados {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Actualmente, esta función no está disponible en todos los clústeres del entorno de vista previa.

Si utiliza la promoción de la marca en Workfront, el logotipo que utiliza en la barra de navegación global se incluye ahora en los archivos .pdf que exporta desde Workfront.

Los siguientes archivos PDF incluirán el logotipo de su organización en el documento exportado:

* Listas exportadas
* Informes exportados y entregados
* Paneles impresos

Para obtener más información acerca de cómo exportar datos desde Workfront, vea [Exportar datos](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Mejoras al copiar tareas y mover tareas o problemas {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Hemos mejorado la forma de copiar una tarea o explorar una tarea o un problema, para facilitar la selección de un elemento principal para la tarea o el problema copiado o movido. Al seleccionar un elemento principal mientras copia una tarea, por ejemplo, ahora puede ver una jerarquía de tareas, con su relación principal-secundario, así como buscar un elemento principal en proyectos con muchas tareas.

Antes de este cambio, no había ningún campo de búsqueda en el paso **Seleccionar un elemento principal** y la jerarquía de tareas no estaba visible en la lista de tareas.

Para obtener más información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener más información sobre cómo mover problemas, consulte [Mover problemas](../../../../manage-work/issues/manage-issues/move-issues.md).

## Nueva configuración para recuperar solicitudes en el área de configuración de aprobación {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Hemos introducido una nueva configuración en el área de Configuración de aprobación en el sistema para permitir que los administradores de Workfront decidan si deben permitir que los usuarios recuperen un problema o solicitud cuyo primer estado esté pendiente de aprobación. Si se permite la revocación, el problema se elimina; si no se permite la revocación, los usuarios no pueden ver un botón de Revocar cuando el primer estado de un problema está pendiente de aprobación.

Antes de este cambio, siempre se permitía la revocación del problema. Cuando se recuperó la aprobación, se omitió por completo, lo que colocó el problema en su primer estado y no se adjuntó ninguna aprobación.

Para obtener más información acerca de la configuración de aprobación, vea [Configuración de la aprobación global](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Esta opción se desactivará de forma predeterminada cuando se publique esta función. La recuperación de problemas está habilitada de forma predeterminada para todas las organizaciones. Cuando se lance esta función, el administrador de Workfront debe habilitar manualmente esta configuración para mantener la funcionalidad tal como está en Workfront.

## Nueva agrupación para informes de horas presupuestadas de recursos: fecha de asignación {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Se ha agregado la capacidad de agrupar los resultados por fecha de asignación al generar un recurso de lista de horas presupuestadas.

Antes de este cambio, se podía mostrar la Fecha de asignación en la vista del informe y utilizarla en un filtro, pero no se podía utilizar este campo en una agrupación.

Para obtener más información sobre la fecha de asignación, consulte [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obtener más información sobre cómo generar un informe, consulte [Creación de un informe simple](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Configuración de Planificador de recursos {#resource-planner-improvements}

* [Planificador de recursos: Mostrar datos por ETP](#resource-planner-show-data-by-fte)
* [Planificador de recursos: mostrar datos por semana y trimestre](#resource-planner-show-data-by-week-and-quarter)
* [Planificador de recursos: ver por usuario](#resource-planner-view-by-user)
* [Planificador de recursos: arrastre y suelte los proyectos para establecer la prioridad](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Planificador de recursos: exporte los datos del Planificador de recursos a Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Planificador de recursos: mostrar datos por FTE {#resource-planner-show-data-by-fte}

Ahora se puede mostrar la asignación y disponibilidad de sus recursos por FTE en el Planificador de recursos. Antes de este cambio, solo se podían mostrar los valores en horas.

Para obtener más información sobre el uso del Planificador de recursos, consulte [Información general de navegación del planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificador de recursos: mostrar datos por semana y trimestre {#resource-planner-show-data-by-week-and-quarter}

Ahora puede cambiar el intervalo de lapso de tiempo para que el Planificador de recursos lo vea por semana o trimestre. Antes de este cambio, podía ver la asignación y disponibilidad de los recursos y presupuestarlos solamente por mes.

Para obtener más información sobre el uso de Filtrar el Planificador de recursos, consulte [Información general de navegación del planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificador de recursos: ver por usuario {#resource-planner-view-by-user}

Ahora puedes mostrar la información en el Planificador de Recursos primero por usuario y luego por proyectos, roles y tareas. También puedes mostrar la diferencia entre las Horas disponibles o FTE para los usuarios. Antes de este cambio, se podía mostrar la información en el filtro de Planificador de recursos por proyectos y roles.

Para obtener más información sobre el uso del filtro del Planificador de recursos, consulte [Información general de navegación del planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificador de Recursos: Arrastra y suelta proyectos para establecer la prioridad {#resource-planner-drag-and-drop-projects-to-establish-priority}

Ahora puede arrastrar y soltar proyectos en el orden de prioridad deseado. Antes de este cambio, solo se podía establecer la prioridad de los proyectos asignándoles manualmente un número.

Para obtener más información sobre el uso de filtro del Planificador de Recursos, consulta la [Información general de navegación del planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificador de Recursos: Exporta los datos del filtro del Planificador de recursos a Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Ahora puede exportar la información del Planificador de Recursos a un archivo de Excel.

Para obtener más información sobre el uso del Planificador de Recursos, consulta la [Descripción general del Planificador de Recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Mejoras para móviles {#mobile-improvements}

Hemos añadido la posibilidad de acceder a tus proyectos y gestionarlos desde la aplicación móvil de Workfront. Ahora puedes realizar lo siguiente usando la aplicación móvil de Workfront:

* Acceda a una lista de sus proyectos
* Acceda a una lista de tareas y subtareas de un proyecto
* Acceso a una lista de problemas de un proyecto
* Registrar un nuevo problema en un proyecto

Puede instalar esta funcionalidad cuando actualice su aplicación móvil de Workfront. La actualización estará disponible en las tiendas móviles Apple y Android en noviembre de 2017.

## Integración de Workfront con Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>La integración de Slack no está disponible actualmente. Estará disponible para su uso con el entorno de producción en noviembre de 2017.

Estamos lanzando una nueva integración entre Workfront y Slack. Si tu organización ya ha estado utilizando Slack para su comunicación, ahora puedes integrarlo con Workfront y realizar acciones comunes de Workfront sin salir de tus canales de comunicación en Slack. Ahora puede realizar las siguientes acciones desde su cuenta de Slack:

* Buscar un elemento en Workfront
* Acceso a sus listas de trabajo y aprobaciones
* Crear una tarea
* Crear un problema
* Suscríbete a cualquier elemento desde un vínculo que se haya compartido contigo para ese elemento
* Asignar tareas y problemas desde un vínculo compartido con usted a ellos
* Apruebe su trabajo
* Acceda a sus listas de Favoritos y Elementos recientes

Para obtener más información sobre cómo acceder a Workfront desde Slack, consulte [Uso de Workfront con Slack.](https://support.workfront.com/hc/es-es/sections/115000458033)

## Mejoras de Outlook 365 {#outlook-365-improvements}

Hemos realizado las siguientes mejoras en el complemento de Workfront para Outlook 365:

* Añade una tarea o un problema a un proyecto en Workfront: Ahora puedes convertir un correo electrónico en una tarea o un problema en Workfront utilizando el complemento de Outlook 365. En este proceso, puedes especificar el proyecto al que deseas añadir la tarea o el problema, así como un responsable y una fecha de vencimiento. Antes de esta mejora, solo podías enviar una solicitud a una cola de solicitudes o añadir una tarea personal a tu lista de Tareas en Progreso desde Outlook 365. 
* Preserva un enlace a los objetos de Workfront en el correo electrónico original convertido en tareas, problemas o solicitudes: Cuando conviertes un correo electrónico de Outlook 365 en una tarea, un problema o una solicitud, Outlook 365 preserva un enlace a la tarea o al problema que se convirtió a partir de ese correo dentro del correo electrónico original. Antes de este cambio, no había ninguna indicación en Outlook de si un correo electrónico había sido convertido en una tarea o enviado como solicitud. 

## Cambios de API {#api-changes}

* [Ya está disponible la API 8](#api-8-now-available)
* [Versiones eliminadas y obsoletas de la API](#removed-and-deprecated-versions-of-the-api)
* [Actividad de la versión final Beta de 2017.3](#updated-message-format-for-event-subscriptions)
* [Reintentos de suscripción a evento para mensajes no entregables](#event-subscription-retries-for-undeliverable-messages)

### Ya está disponible la API 8 {#api-8-now-available}

La versión 8 de la API de Workfront ya está disponible y le ofrece recursos nuevos y actualizados para sus integraciones de Workfront.

Para ver una lista de los cambios realizados en la API de Workfront, consulte [Actualizaciones de la versión 8](../../../../wf-api/api/new-api-version-8-updates.md) de la API.

### Versiones eliminadas y obsoletas de la API {#removed-and-deprecated-versions-of-the-api}

### Formato de mensaje actualizado para suscripciones a eventos

Para proporcionar información más útil para las integraciones que incluyen la API de suscripciones a eventos de Workfront, hemos cambiado el formato de mensaje saliente para los recursos admitidos, incluyendo los valores antiguos y nuevos asociados a esos recursos. Para evitar errores, cualquier integración que tenga al usar la API de suscripciones a eventos de Workfront deberá actualizarse con el nuevo formato, tal como se describe en [API de suscripción a eventos](../../../../wf-api/general/event-subs-api.md).

### Reintentos de suscripción a evento para mensajes no entregables {#event-subscription-retries-for-undeliverable-messages}

El marco de suscripción a evento de Workfront ahora proporciona un mecanismo para administrar los mensajes salientes activados por eventos que no se entregan a los extremos de los clientes. Para garantizar la entrega continua de mensajes, los clientes deben asegurarse de que los puntos finales que consumen mensajes salientes de suscripciones de evento estén correctamente configurados. Para obtener más información, consulte [Reintentos de suscripción a eventos](../../../../wf-api/api/event-sub-retries.md).
