---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2018.2 de Beta 5
description: Esta página describe todos los cambios más recientes disponibles en el entorno de vista previa con la versión 2018.2 de Beta 5. La funcionalidad está disponible en el entorno de vista previa desde el 1 de junio de 2018. Las mejoras de revisión incluidas en Beta 5 estarán disponibles en el entorno de vista previa el lunes, 4 de junio. Estará disponible en el entorno de producción en julio de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 100%

---

# Actividad de la versión 2018.2 de Beta 5

Esta página describe todos los cambios más recientes disponibles en el entorno de vista previa con la versión 2018.2 de Beta 5.La funcionalidad está disponible en el entorno de vista previa desde el 1 de junio de 2018. Las mejoras de revisión incluidas en Beta 5 estarán disponibles en el entorno de vista previa el lunes, 4 de junio. Estará disponible en el entorno de producción en julio de 2018.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en la versión 2018.2, consulte  [Información general de actividades de la versión 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versión 2018.2 de Beta 5 tiene las siguientes mejoras para los administradores de Workfront y otros usuarios:

**Para los administradores**

* [Ver cambios activados por el usuario con registros de auditoría](#view-user-triggered-changes-with-audit-logs)
* [Ver información de licencia como administrador de grupos](#view-license-information-as-a-group-administrator)

**Para todos los usuarios**

* [Vista de calendario en el área de inicio](#calendar-view-in-the-home-area)
* [Actualizaciones adicionales a la lista de trabajos (panel izquierdo) en Inicio](#additional-updates-to-the-work-list-left-panel-in-home)
* [Configurar límites de funciones para la programación automatizada de recursos](#configure-job-role-limits-for-automated-resource-scheduling)
* [Mejoras en la vista de proyectos y funciones del Planificador de recursos](#project-and-role-view-improvements-in-the-resource-planner)
* [Cambiar el tamaño de los anchos de columna de las listas de proyectos](#resize-column-widths-for-project-lists)
* [Icono de compatibilidad con las nuevas listas de proyectos](#icon-support-for-the-new-project-lists)
* [Añadir el campo “Miniatura grande” en las vistas del documento](#add-large-thumbnail-field-in-document-views)
* [Aumentar límite de exportación de Excel](#increase-excel-export-limit)
* [Filtros rápidos para listas de proyectos](#quick-filters-for-project-lists)
* [Colecciones de problemas de referencia en informes de proyectos y tareas](#reference-issue-collections-in-project-and-task-reports)
* [Nuevo menú Versión más sólido al añadir nuevas versiones de documento en Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Mejoras de Mobile en la aplicación móvil Beta de Android](#mobile-improvements-in-the-android-beta-mobile-app)
* [Mejoras en el Visor de corrección (Workfront y Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Mejoras de revisión en Workfront](#proofing-enhancements-in-workfront)
* [Mejoras de revisión en Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Vista de calendario en el área de Inicio {#calendar-view-in-the-home-area}

Ahora puede administrar sus programaciones y tareas de trabajo personales mediante la vista Calendario de inicio de Workfront. La vista Calendario de inicio le permite hacer lo siguiente:

* Establezca su propia programación para realizar las tareas de Workfront que se le han asignado
* Ver rápidamente las tareas que vencen próximamente o que han vencido
* Ver el total de horas asignadas en una semana
* Actualizar las tareas asignadas

Si utiliza un calendario en Outlook, puede integrarlo para que muestre los eventos de Outlook en la vista Calendario de inicio.

## Actualizaciones adicionales a la lista de trabajos (panel izquierdo) en Inicio {#additional-updates-to-the-work-list-left-panel-in-home}

Las siguientes mejoras ya están disponibles para la lista de trabajos en el área de Inicio:

* El número de elementos completados ahora se muestra entre paréntesis junto a la opción Completado en el menú desplegable Filtro.

  Anteriormente, el número de elementos completados no se mostraba en el menú Filtro. 

* Se muestran los elementos completados de las dos semanas anteriores.

  Anteriormente, se mostraban los elementos completados durante los tres meses previos.

  Para obtener información sobre cómo ver el trabajo completado en el área de Inicio, consulte [Mostrar elementos de la lista de trabajos en el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) en el artículo [Mostrar elementos de la lista de trabajos en el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Añada los campos Duración y Asignaciones para que se muestren cuando se seleccionen elementos en el área de Inicio.

  Anteriormente, el campo Asignaciones estaba disponible de forma predeterminada; sin embargo, si se eliminaba, no se podía volver a añadir. Anteriormente, el campo Duración no estaba disponible para añadirlo.

  Para obtener información sobre cómo añadir campos al área de Inicio, consulte “Crear y administrar plantillas de diseño”.

Para obtener más información sobre el uso del área de Inicio, consulte [Usar el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Ver cambios activados por el usuario con registros de auditoría {#view-user-triggered-changes-with-audit-logs}

Hemos creado los siguientes registros de auditoría para los administradores de Workfront con el fin de llevar el seguimiento de los cambios activados por el usuario:

* Registro de auditoría de usuario
* Registro de auditoría de nivel de acceso
* Registros de auditoría de grupo
* Registros de auditoría de intentos de inicio de sesión

Anteriormente, no había forma de llevar el seguimiento de los cambios dentro del sistema.

Para obtener más información, consulte [Ver y exportar registros de auditoría](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Ver información de licencia como administrador de grupos {#view-license-information-as-a-group-administrator}

Hemos creado una página Licencias de solo lectura para que los administradores de grupos vean el número de licencias de los grupos que administran.

Antes de este cambio, los administradores de grupos no podían ver la información de licencia.

Para obtener más información, consulte [Administradores de grupos](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Configurar límites de funciones para la programación automatizada de recursos {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

En la configuración de Programación automatizada de recursos, ahora puede asignar un límite a una función. Esto permite controlar el número de recursos, con la misma función, que se están asignando al trabajo.

Anteriormente, no se podía especificar cuántos usuarios de una función determinada podían recibir asignaciones de trabajo.

Para obtener más información, consulte “Asignar manualmente tareas y problemas no asignados en las áreas de programación”.

## Mejoras en la vista de proyectos y funciones del Planificador de recursos {#project-and-role-view-improvements-in-the-resource-planner}

Las vistas de proyectos y funciones del Planificador de recursos ahora tienen las siguientes mejoras:

* Filtros mejorados que extraen información de toda la base de datos, en lugar de solo la información de la pantalla.
* Modo de pantalla completa.
* Ahora, el rendimiento es más rápido y más eficiente.

   * Nuevos límites en el número de proyectos, funciones y usuarios que se pueden mostrar.
   * Carga diferida, para una carga más rápida de proyectos y funciones.

* Acceso rápido a proyectos y usuarios directamente desde el Planificador de recursos.
* Capacidad de arrastrar y soltar más rápida en la vista de proyectos para priorizar sus proyectos.

Antes de estas mejoras, había informado de que el Planificador de recursos tardaba en cargarse y de que había observado incongruencias en los datos mostrados. Con estas mejoras, esto debería haberse solucionado ya.

Para obtener información y comprender los nuevos límites del Planificador de recursos, consulte [Limitaciones de visualización del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Cambiar el tamaño de los anchos de columna de las listas de proyectos {#resize-column-widths-for-project-lists}

Como hemos estado trabajando en la mejora de la funcionalidad de nuestras listas, hemos deshabilitado temporalmente la capacidad de cambiar el tamaño de los anchos de las columnas en las siguientes listas de proyectos:

* Proyectos de mi propiedad
* Proyectos en los que participo
* Todos los proyectos

Con esta versión, ahora podemos cambiar de nuevo el tamaño de las columnas de todas las listas de proyectos.

Se han añadido mejoras adicionales a esta funcionalidad.

Ahora, cuando arrastra el borde derecho de una columna para cambiar su tamaño, la columna contigua de la derecha conserva su tamaño y hace que la lista sea más ancha, en lugar de modificarse también. Además, puede arrastrar el borde de una columna hacia la derecha más allá de los bordes de las columnas adyacentes.

Antes de esta mejora, se cambiaba proporcionalmente el tamaño de la columna contigua a la derecha de la columna a la que se le cambiaba el tamaño para que cupiera en la pantalla y no se podía arrastrar el borde de una columna más allá del borde derecho de la columna contigua.  

Para obtener información sobre cómo cambiar el tamaño de las columnas que se están reorganizando en las listas, consulte [Modificar el ancho y el orden de las columnas](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Para participar en nuestro programa de pruebas beta de las mejoras actuales de la lista, consulte [Nuevo estudio de listas.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront) (se requiere inicio de sesión)

## Icono de compatibilidad con las nuevas listas de proyectos {#icon-support-for-the-new-project-lists}

Como hemos estado trabajando en la mejora de la funcionalidad de nuestras listas, hemos deshabilitado temporalmente la visualización de los iconos de estado en las siguientes listas de proyectos:

* Proyectos de mi propiedad
* Proyectos en los que participo
* Todos los proyectos

Con esta versión, los iconos de estado se pueden volver a mostrar en las listas de proyectos para proyectos u otros objetos de una lista de proyectos.

Para obtener información sobre cómo trabajar en listas, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Añadir el campo “Miniatura grande” en las vistas del documento {#add-large-thumbnail-field-in-document-views}

Se añadió un nuevo campo denominado Miniatura grande a una vista del documento de una lista o informe. Cuando se selecciona en una vista de documento, este campo muestra una miniatura de 400 píxeles de ancho del documento en una lista o informe.

Antes de este cambio, solo podía añadir el campo Miniatura a una vista de documento, que muestra una miniatura del documento de entre 33 y 66 píxeles de ancho.

Para obtener información acerca de los campos de listas e informes, consulte [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Incremento del límite de exportación de Excel {#increase-excel-export-limit}

Se ha aumentado el límite de la cantidad de filas que se pueden exportar en un archivo de Excel. Ahora puede exportar lo siguiente:

* 65 000 filas en un archivo Excel .xls
* 100 000 filas en un archivo .xlsx de Excel

Los nuevos límites se aplican cuando exporta lo siguiente desde Workfront:

* Una lista o un informe de la interfaz web
* Una lista o un informe que utilice la API
* Un informe programado y enviado

Antes de esta mejora, solo se podían exportar 50 000 filas en cualquier archivo de Excel.

Para obtener información acerca de cómo exportar datos desde Workfront, consulte [Exportar datos](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Filtros rápidos para listas de proyectos {#quick-filters-for-project-lists}

Ahora puede aplicar un filtro rápido a las listas.

El propósito de un filtro rápido es ayudarle a desplazarse directamente a los elementos de las listas grandes que considere importantes, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con los demás.

Actualmente, los filtros rápidos solo están disponibles para las listas de proyectos en las siguientes subpestañas:

* Proyectos en los que participo
* Proyectos de mi propiedad
* Todos los proyectos

Para obtener información acerca de los filtros rápidos, consulte la sección “Aplicar filtros rápidos a listas” en [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Colecciones de problemas de referencia en informes de proyectos y tareas {#reference-issue-collections-in-project-and-task-reports}

Ahora puede hacer referencia a una colección de problemas en una vista de proyecto o tarea y filtro. Solo puede hacerlo utilizando el modo Texto mientras crea un informe.

Antes de esta mejora, solo se podía hacer referencia a una colección de tareas en una vista de proyecto o filtro.

Para obtener información sobre cómo hacer referencia a una colección en un informe, consulte [Colecciones de referencia en un informe](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Para obtener información sobre el uso del modo de texto, consulte [Información general sobre usos comunes del modo Texto](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>En el siguiente vídeo, el modo de texto de ejemplo para las colecciones de problemas era incorrecto. El modo de texto de ejemplo correcto está disponible en [Colecciones de referencia en un informe](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Menú Nueva versión más sólida al añadir nuevas versiones de documento en Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Ahora, al añadir nuevas versiones a los documentos en Workfront, el menú Nueva versión contiene opciones adicionales y ahora es coherente en todas las áreas de Workfront donde puede añadir una nueva versión.

Puede añadir una nueva versión del documento desde las siguientes áreas de Workfront:

* En el menú desplegable Más de la pestaña Documentos.
* Desde el menú Acciones de documento de la página de detalles del documento.
* Desde la pestaña Todas las versiones de la página de detalles del documento.

Antes de este cambio, solo el menú desplegable Más de la pestaña Documentos contenía todas las opciones para añadir una nueva versión.

Las siguientes opciones están ahora disponibles en el menú Nueva versión para todas las áreas en las que puede añadir una nueva versión:

* Revisión
* Solo documento
* Opciones vinculadas (desde Dropbox, Google Drive, etc.)
* Pegar desde el portapapeles (se trata de una nueva opción al añadir versiones)

Para obtener más información, consulte [Añadir documentos a Adobe Workfront desde el sistema de archivos](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) en el artículo [Añadir documentos a Adobe Workfront desde el sistema de archivos](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Mejoras en la aplicación móvil Beta de Android {#mobile-improvements-in-the-android-beta-mobile-app}

Las siguientes mejoras estarán disponibles en la versión Beta de Android de la aplicación móvil poco después del día de este lanzamiento:

* Acciones de deslizamiento

  Puede realizar actividades como ofrecerse voluntario para trabajar en una tarea, completar una tarea, marcar una notificación como vista o nueva, enviar un mensaje de texto o llamar a un contacto deslizando varios objetos en la aplicación móvil de Workfront.

  Con esta funcionalidad se han mejorado las siguientes áreas:

   * Mi trabajo e Inicio
   * Notificaciones
   * Contactos
   * Rutas de aprobación

* Nueva apariencia al ver la pestaña Detalles de un elemento

  La interfaz ha cambiado al ver un elemento en la versión Beta de Android de la aplicación móvil para que sea más fácil editarlo, completarlo o adjuntarle un documento.

* Nueva experiencia al registrar el tiempo

  El registro del tiempo es más rápido y sencillo que antes, con un botón de registro del tiempo de más fácil acceso y una interfaz más simplificada para el registro de horas.

Con esta versión, estas mejoras solo están disponibles para la versión Beta de Android de la aplicación móvil de Workfront. Actualmente, no están disponibles para iOS.

Para obtener más información sobre cómo registrarse para probar la versión beta y descargar la versión Beta de Android de la aplicación móvil de Workfront, consulte.

## Mejoras en el visor de corrección (Workfront y Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Página de resumen de impresión actualizada](#updated-print-summary-page)
* [Añadir usuarios a una prueba directamente desde el visor de corrección](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Mostrar todas las herramientas de marcado en el visualizador de corrección](#display-all-markup-tools-in-the-proofing-viewer)
* [Configurar opciones de ordenación predeterminadas en el visualizador de corrección](#configure-default-sorting-options-in-the-proofing-viewer)
* [Ver aprobaciones de documentos de Workfront en el visualizador de corrección de escritorio](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Configurar vínculos que abren nuevas pestañas y ventanas para abrirlas en el visualizador de corrección de escritorio](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Indicador de presencia en el visualizador de corrección](#presence-indicator-in-the-proofing-viewer)
* [Filtrar comentarios para mostrar una sola página para pruebas de URL interactivas en el visualizador de corrección de escritorio](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Visualizador de corrección de escritorio para contenido estático y de vídeo](#desktop-proofing-viewer-for-static-and-video-content)
* [Añadir dispositivos personalizados al sistema](#add-custom-devices-to-your-system)

### Página de resumen de impresión actualizada {#updated-print-summary-page}

La página Resumen de impresión se ha actualizado con una nueva apariencia y una funcionalidad mejorada.

Para obtener más información, consulte [Imprimir un resumen de prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Añadir usuarios a una prueba directamente desde el visualizador de corrección {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Ahora puede añadir usuarios a una prueba directamente desde el visualizador de corrección web y el de escritorio. 

Anteriormente, no se podía añadir usuarios individuales a una prueba. En su lugar, solo puede copiar la URL pública o el código incrustado.

Para obtener más información, consulte [Compartir una prueba añadiendo usuarios](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) en el artículo  [Compartir una prueba del visualizador de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Mostrar todas las herramientas de marcado en el visor de corrección {#display-all-markup-tools-in-the-proofing-viewer}

Ahora puede configurar la herramienta de marcado para que aparezca todo el tiempo en lugar de en un menú que tenga que abrir. Esto hace que sea más rápido cambiar entre herramientas. Cuando se configura de esta manera, las herramientas de marcado se muestran horizontalmente en la parte superior del visor de corrección web y del de escritorio.

Anteriormente, las herramientas de marcado solo estaban disponibles en un menú desplegable.

Para obtener más información acerca de cómo configurar esta opción de marcado, consulte [Configurar ajustes del visor de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Para obtener más información sobre el uso de opciones de marcado al revisar una prueba, consulte en el artículo

### Configurar las opciones de ordenación predeterminadas en el visor de corrección. {#configure-default-sorting-options-in-the-proofing-viewer}

Ahora, cuando cambia la opción de ordenación dentro de la lista de comentarios en una prueba, esa opción se convierte en la opción de ordenación predeterminada la próxima vez que abra cualquier prueba dentro del visor de corrección web o del de escritorio. 

Para obtener más información, consulte el artículo.

### Ver aprobaciones de documentos de Workfront en el visor de corrección de escritorio {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Ahora puede tomar una decisión de aprobación de documento de Workfront en el visor de corrección de escritorio.

Anteriormente, solo el visor de corrección web le permitía tomar una decisión de aprobación del documento de Workfront. 

Para obtener más información, consulte [Tomar una decisión sobre una prueba en el visor de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) del artículo [Tomar una decisión sobre una prueba en el visor de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Configurar vínculos que abren nuevas pestañas y ventanas para abrirlas en el visor de corrección de escritorio {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Al revisar el contenido interactivo en el Visor de corrección de escritorio, ahora puede configurar los vínculos que se abren en una nueva pestaña o ventana para que se abran en el visor de corrección de escritorio y pueda continuar con la revisión.

En el visor de corrección heredado, los vínculos que se abrían en una nueva pestaña o ventana no se podían revisar en el visor de corrección.

Para obtener más información, consulte [Configurar ajustes del visor de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Indicador de presencia en el visor de corrección {#presence-indicator-in-the-proofing-viewer}

Ahora, al revisar una prueba en el visor de corrección web o en el visor de corrección de escritorio, puede ver el avatar de cada usuario que esté viendo la revisión en la esquina superior derecha del visor de corrección.

Para obtener más información, consulte [Revisar una prueba simultáneamente con varios revisores](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtrar comentarios para mostrar una sola página para las pruebas de URL interactivas en el visor de corrección de escritorio {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Al revisar una URL en una prueba interactiva en el visor de corrección de escritorio, ahora puede filtrar los comentarios para mostrar los comentarios realizados únicamente en la página actual. 

Antes de este cambio, esta opción solo estaba disponible para pruebas estáticas.

Para obtener más información, consulte el artículo.

### Visor de corrección de escritorio para contenido estático y de vídeo {#desktop-proofing-viewer-for-static-and-video-content}

El visor de corrección de escritorio ahora admite contenido estático y de vídeo.

Anteriormente, solo admitía contenido interactivo.

Para obtener información acerca de cómo configurar pruebas estáticas y de vídeo para que se abran en el visor de corrección de escritorio, consulte [Configurar ajustes del visor de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Para obtener más información acerca del visor de corrección de escritorio, consulte [Revisión de pruebas en el visor de corrección de escritorio.](https://support.workfront.com/hc/es-es/sections/360000686434)

### Añadir dispositivos personalizados al sistema {#add-custom-devices-to-your-system}

Ahora puede añadir cualquier dispositivo personalizado al sistema, lo que permite a los usuarios revisar el contenido interactivo y simular cómo aparece en un dispositivo específico al revisar una prueba en el visor de corrección de escritorio.

Antes de este cambio, los usuarios solo podían elegir entre una lista de dispositivos estándar preconfigurados.

Para obtener información sobre cómo añadir dispositivos personalizados, consulte

Para obtener información sobre cómo los usuarios pueden seleccionar dispositivos al revisar el contenido interactivo, consulte [Cambiar la resolución de la prueba interactiva en el visor de corrección](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Mejoras de revisión en Workfront {#proofing-enhancements-in-workfront}

* [Compartir el vínculo de prueba directamente desde Workfront](#share-the-proof-link-directly-from-workfront)
* [Informe sobre datos de revisión adicionales en Workfront](#report-on-additional-proofing-data-in-workfront)
* [Ver datos históricos para aprobaciones de prueba en Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Compartir el vínculo de prueba directamente desde Workfront {#share-the-proof-link-directly-from-workfront}

Ahora puede generar un vínculo para una prueba en Workfront y compartirla directamente desde Workfront. También puede copiar la URL y distribuirla mediante un método alternativo.

Antes de este cambio, solo se podía copiar el vínculo de prueba en Workfront y distribuirlo mediante un método alternativo.

Para obtener más información, consulte [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en el artículo [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>El vínculo incrustado que está disponible actualmente se eliminará en una versión futura. Se podrá acceder al vínculo incrustado a través de la API de Workfront.

### Informar sobre datos de revisión adicionales en Workfront {#report-on-additional-proofing-data-in-workfront}

En los informes que contienen el objeto de versión del documento (como los informes Versión del documento y Aprobación de prueba), hay disponibles varios campos que permiten ver información adicional sobre la revisión.

* Fecha límite de revisión

  Muestra el día de la semana, la fecha, la hora del día y el año de la fecha límite de la revisión.

* Decisión de revisión

  Muestra el estado de decisión de la prueba (pendiente, cambios necesarios o aprobado).

* Nombre de revisión

  Muestra el nombre de la revisión.

* Páginas de revisión

  Muestra el número de páginas incluidas en la prueba.

* Progreso de revisión

  Muestra el estado de progreso de la prueba (enviada, abierta, comentada, decidida).

Para obtener más información sobre cada uno de estos campos, consulte  [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Ver datos históricos para aprobaciones de prueba en Workfront {#view-historical-data-for-proof-approvals-in-workfront}

En el informe de Aprobación de pruebas, puede añadir un campo que le permita ver las decisiones de aprobación de pruebas para pruebas que ya no están activas. Para ello, añada el campo Decisión del aprobador al informe.

Antes de este cambio, después de tomar una decisión sobre una prueba, la decisión ya no se podía mostrar en un informe de Workfront.

Para obtener más información, consulte  [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Mejoras de revisión en Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Crear una nueva versión de una prueba directamente desde el visor de revisión (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Nuevo vínculo de detalles de prueba en el visor de revisión y en el Visor de revisión de escritorio (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Crear una nueva versión de una prueba directamente desde el visor de pruebas (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Ahora puede crear una nueva versión de una prueba directamente desde el nuevo visor de pruebas y el Visor de pruebas de escritorio al realizar pruebas en Workfront Proof.

Anteriormente, esta opción solo estaba disponible en el Visualizador flash heredado.

Para obtener más información, consulte [Copia de pruebas en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) en el artículo  [Copia de revisiones en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Nuevo vínculo de detalles de prueba en el visor de revisión y en el Visor de revisión de escritorio (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Al ver una prueba en el visor de pruebas, los usuarios de Workfront Proof ahora pueden ir rápidamente a la página de detalles de prueba en Workfront Proof.

Para obtener más información, consulte &quot;Visualización de detalles de prueba&quot;.
