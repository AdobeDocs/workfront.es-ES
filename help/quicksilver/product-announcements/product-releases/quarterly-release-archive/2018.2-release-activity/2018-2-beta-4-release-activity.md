---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión Beta 4 2018.2
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión Beta 4 2018.2. La funcionalidad estará disponible en el entorno de vista previa el 17 de mayo de 2018. Estará disponible en el entorno de producción en julio de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 100%

---

# Actividad de la versión Beta 4 2018.2

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión Beta 4 2018.2.La funcionalidad estará disponible en el entorno de vista previa el 17 de mayo de 2018. Estará disponible en el entorno de producción en julio de 2018.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en la versión 2018.2, consulte  [Información general de actividades de la versión 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versión 2018.2 de Beta 4 contiene las siguientes mejoras para administradores de Workfront y otros usuarios:

**Para los administradores**

* [Configuración del sistema: Información de sesión en páginas externas](#system-setting-session-information-in-external-pages)

**Para todos los usuarios**

* [Mejoras de límite de trabajo en curso (WIP) en el tablero Kanban](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Interfaz mejorada para configurar los estados de un equipo ágil](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Lista de trabajos actualizada (panel izquierdo) en el área de inicio](#updated-work-list-left-panel-in-the-home-area)
* [Nuevo Visor de corrección de escritorio para revisar contenido interactivo (medios enriquecidos)](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content)
* [Exportar la vista de usuario en el Planificador de recursos](#export-the-user-view-in-the-resource-planner)
* [Soporte para Google Team Drives](#support-for-google-team-drives)
* [Nuevo límite de exportación para el gráfico Gantt](#new-export-limit-for-the-gantt-chart)
* [La opción de pegar desde el portapapeles ahora se muestra atenuada cuando se utiliza Internet Explorer o Safari](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Nuevo entorno beta para Android junto con nuevas funciones](#new-beta-environment-for-android-along-with-new-features)
* [Ejemplos de filtros para mensajes de suscripciones a eventos](#examples-of-filters-for-event-subscriptions-messages)

## Mejoras en el límite de trabajo en curso (WIP) en el tablero Kanban {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Configurar límites de trabajo en curso (WIP) para cada columna en el tablero Kanban

Ahora puede configurar los límites de Trabajo en curso (WIP) por cada columna del tablero Kanban. 

Antes de este cambio, solo se podía configurar un límite de WIP que se aplicara a todas las columnas del tablero Kanban. 

Para obtener más información, consulte la sección  [Configurar el límite de trabajo en curso (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) en el artículo  [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Actualizar el límite de trabajo en curso (WIP) directamente desde el tablero Kanban

Ahora, los integrantes del equipo con derechos de edición en el equipo pueden actualizar el límite de trabajo en curso directamente desde el tablero Kanban.

Antes de este cambio, solo podía actualizar el límite de trabajo en curso desde el área Configuración de equipo.

Para más información, consulte en el artículo.

## Interfaz mejorada para configurar estados para un equipo ágil {#improved-interface-for-configuring-statuses-for-an-agile-team}

La interfaz para configurar los estados de un equipo ágil se ha actualizado con las siguientes mejoras:

* Nueva apariencia
* Reordenar columnas de estado mediante arrastrar y soltar 

Para más información, consulte los siguientes artículos:

* [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Lista de trabajos actualizada (panel izquierdo) en el área de inicio {#updated-work-list-left-panel-in-the-home-area}

La Lista de trabajos en el área de Inicio contiene las siguientes mejoras:

* Los elementos no leídos ahora se destacan con negrita y un punto azul.

  Los elementos que se ven fuera del área de Inicio siguen mostrándose como No leídos en el área de Inicio.

  Para obtener más información, consulte [Mostrar elementos en la Lista de trabajos en el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Los problemas ahora se distinguen con un icono de problema que se muestra junto al problema.
* Las aprobaciones ahora se distinguen por tipo de aprobación, y se muestra el tipo de aprobación. Los tipos de aprobación posibles son Tarea, Proyecto, Problema, Acceso, Documento, Hoja de horas y Prueba.

  Antes de este cambio, las aprobaciones solo se distinguían por la palabra “Aprobación”.

* Los elementos ahora se distinguen por si están listos para iniciarse. Las opciones posibles son Listo para el inicio, No está listo o Trabajando en.

  Esta información no se muestra para aprobaciones porque las aprobaciones siempre están listas para iniciarse.

* Se muestra un icono de documento debajo del nombre del elemento cada vez que se adjunta un documento al elemento.
* Ahora puede contraer y expandir las agrupaciones dentro de la Lista de trabajos para controlar mejor qué información está visible. Las agrupaciones son Atrasado, Proyectos, Fechas y Finalizado.

  De forma predeterminada, la sección Esta semana se expande y todas las demás agrupaciones se contraen.

* Seleccione si desea ordenar los artículos por fecha planificada de finalización o fecha de confirmación.
* El número de elementos de cada agrupación ahora se muestra entre paréntesis junto al título de la agrupación.

  Este número no está disponible para la agrupación completada.

  Para obtener más información, consulte [Mostrar elementos en la Lista de trabajos en el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Cambiar el tamaño de la Lista de trabajos mediante arrastrar y soltar. Puede cambiar el tamaño de la Lista de trabajos para consumir hasta la mitad de la pantalla. El tamaño que establezca se conservará la próxima vez que acceda a Inicio.

  Antes de este cambio, no se podía cambiar el tamaño de la Lista de trabajos.

* Para las solicitudes, ahora se muestra el avatar del usuario que realizó la solicitud, con el texto “[Approver_name] desea su aprobación”.
* Al crear una nueva tarea personal, el botón “Tareas pendientes” ahora se denomina “Personal”.

  Para obtener más información, consulte [Crear elementos de trabajo desde el área de inicio](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) en el artículo [Crear elementos de trabajo desde el área de inicio](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Los elementos atrasados se indican como Retrasados solamente después de una hora después de la Fecha planificada de finalización.

Para obtener más información sobre el área de Inicio, consulte [Usar el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nuevo Visor de corrección de escritorio para revisar contenido interactivo (medios enriquecidos) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

El nuevo Visor de corrección de escritorio le permite revisar el contenido interactivo. A diferencia del Visor de corrección heredado existente y del nuevo visor de revisión que se ejecuta en el explorador, el Visor de corrección de escritorio es una aplicación que se ejecuta en la estación de trabajo.

Antes del nuevo Visor de corrección de escritorio, solo podía probar el contenido interactivo en el Visor de corrección heredado. 

El Visor de corrección de escritorio incluye las siguientes mejoras con respecto al Visor de corrección heredado para revisar contenido interactivo:

* Revisar sitios no seguros (HTTP)

  El Visor de corrección heredado le permitía revisar solo sitios seguros (HTTPS)

* Revise los sitios protegidos por iframe (sitios protegidos contra la visualización dentro de un iframe).

  El Visor de corrección heredado heredados no admitía la revisión de sitios protegidos contra la visualización dentro de un iframe.

* Ver contenido con resoluciones preconfiguradas para varios dispositivos. Por ejemplo, puede ver cómo se muestra el contenido en varias resoluciones de escritorio estándar o en dispositivos individuales como un iPhone 8. 

Para obtener más información sobre cómo descargar, instalar y usar el Visor de corrección de escritorio, consulte .

Para obtener información acerca de las diferencias de funcionalidad entre el Visor de corrección de escritorio y los visores de corrección basados en explorador, consulte [Diferencias entre el visor de corrección web y la información general del Visor de corrección de escritorio](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exportar la vista de usuario en el Planificador de recursos {#export-the-user-view-in-the-resource-planner}

Se ha deshabilitado temporalmente la exportación de datos desde el planificador de recursos al mostrarlos en la vista de usuario para resolver algunos problemas de rendimiento. Con esta versión, se vuelve a habilitar la exportación de datos al mostrar el Planificador de recursos en la vista de usuario.

Para obtener más información sobre cómo exportar los datos del Planificador de recursos a Excel, consulte la sección “Opción de exportación” en [Información general sobre la navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Para participar en nuestro programa beta actual para el Planificador de recursos, consulte [Beta de rendimiento del Planificador de recursos.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront)

## Configuración del sistema: Información de sesión en páginas externas {#system-setting-session-information-in-external-pages}

El administrador de Workfront ahora puede restringir el uso de información de sesión (por ejemplo, ID de sesión) al crear una página externa.

Antes de este cambio, los usuarios que podían crear páginas externas podían utilizar cualquier información de sesión al incrustar otros sitios en un panel de Workfront. 

Para obtener más información sobre cómo configurar las preferencias del sistema en Workfront, consulte [Configurar las preferencias de seguridad del sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Compatible con Google Team Drives {#support-for-google-team-drives}

Ahora puede vincular un documento o una carpeta ubicada en Google Team Drive desde Workfront.

Antes de esta mejora, se podía vincular un documento o una carpeta ubicada únicamente en Mi unidad de Google.

Para obtener más información sobre cómo vincular documentos y carpetas de varias aplicaciones a Workfront, consulte [Vincular documentos desde aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Nuevo límite de exportación para el gráfico Gantt {#new-export-limit-for-the-gantt-chart}

Ahora puede exportar hasta 500 tareas en el gráfico Gantt.

Anteriormente, solo se podían exportar hasta 250 tareas.

Para obtener más información, consulte [Exportar el gráfico Gantt a PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## La opción de pegar desde el portapapeles ahora se muestra atenuada cuando se utiliza Internet Explorer o Safari {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

La opción de pegar desde el portapapeles ahora se muestra atenuada al utilizar los navegadores Internet Explorer o Safari, con información sobre herramientas que explica que solo los navegadores Chrome y Firefox son compatibles con esta función.

Antes de este cambio, esta opción no se mostraba al usar Internet Explorer o Safari. 

Para obtener más información acerca de cómo pegar imágenes del portapapeles, consulte [Pegar imágenes desde el portapapeles](../../../../documents/managing-documents/paste-image-clipboard.md).

## Nuevo entorno beta para Android junto con nuevas funciones {#new-beta-environment-for-android-along-with-new-features}

Ahora puede experimentar las funciones más recientes en las que está trabajando nuestro equipo para la aplicación móvil antes de que se publiquen al público en general, registrándose para probar la versión beta. Actualmente, este entorno solo es compatible con la aplicación móvil de Workfront para teléfonos Android.

Para obtener más información sobre cómo registrarse para probar la versión beta de la aplicación móvil de Workfront, consulte .

Las siguientes mejoras ya están disponibles en la versión beta de la aplicación móvil:

* Nueva página de Cuenta

  Ahora puede consultar la información de su cuenta, así como gestionar la configuración de su móvil, enviar comentarios o desconectarse desde la nueva página de Cuenta.

  Antes de esta mejora, no podía ver la información de su cuenta en la aplicación móvil y podía acceder a su configuración, enviar comentarios y cerrar la sesión desde el menú principal de Workfront.

* Nuevo panel inferior de navegación

  Ahora hay disponible una barra de navegación más destacada en la parte inferior de la pantalla que inicia todas las áreas de la aplicación móvil.

  Antes de esta mejora, las áreas de funcionalidad se enumeraban en el menú principal de Workfront. El menú principal de Workfront se ha eliminado y se ha sustituido por la nueva barra de navegación inferior.

  Para obtener más información sobre la configuración de la nueva barra de navegación, consulte la sección “Configuración de la aplicación móvil” .

* Nueva vista de lista de notificaciones

  Una apariencia mejorada de la lista Notificaciones le permite diferenciar fácilmente las notificaciones de la lista según qué tipo sean y si se hayan leído.

* El cuadro de búsqueda se ha movido a una posición más destacada.

* Nueva experiencia de inicio de sesión. La experiencia de inicio de sesión es nueva y optimizada.

* Nueva experiencia tutorial

  Ahora hay disponibles nuevos tutoriales para guiar brevemente a los usuarios a través de la aplicación cuando inician sesión por primera vez. Antes de esta experiencia, los tutoriales se iniciaban únicamente cuando los usuarios accedían a áreas específicas de funcionalidad.

## Ejemplos de filtros para mensajes de suscripciones a eventos {#examples-of-filters-for-event-subscriptions-messages}

Para demostrar cómo puede filtrar suscripciones de eventos para recibir solo los mensajes relevantes para su organización, ahora hay disponibles fragmentos de código de ejemplo para filtrar el flujo de eventos que llegan a los extremos. Para obtener más información sobre cómo ver los ejemplos de filtrado, consulte [Filtrar mensajes de suscripción de eventos](../../../../wf-api/api/filter-event-sub-messages.md).
