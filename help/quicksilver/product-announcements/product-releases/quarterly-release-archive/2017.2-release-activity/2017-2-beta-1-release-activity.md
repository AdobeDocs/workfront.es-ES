---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.2 Beta 1
description: Esta página describe todos los cambios disponibles en el entorno de Vista previa con el lanzamiento de la versión 2017.2 Beta 1 La funcionalidad de esta página estaba disponible en el entorno de vista previa el 10 de mayo de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
TQID: https://experienceleague.adobe.com/7-k8GZcbnM1UfLn-wl1bRWRvHrPjiljtvu8iUa3kLCw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1363
ht-degree: 99%

---

# Actividad de la versión 2017.2 Beta 1

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 1. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 10 de mayo de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

La versión 2017.2 Beta 1 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Restaurar documentos](#restore-documents)
* [Nuevo banner de vista previa con información de lanzamiento](#new-preview-banner-with-release-information) 
* [Disponibilidad de la API 7](#api-7-availability)

**Para todos los usuarios:**

* [Suscribirse a tareas y problemas](#subscribe-to-tasks-and-issues)
* [Mejoras en la programación de recursos](#resource-scheduling-improvements)
* [Comparar pruebas](#compare-proofs)
* [Nuevo campo para conjuntos de recursos para usuarios y proyectos](#new-field-for-resource-pools-for-users-and-projects)
* [Apariencia actualizada en la lista de paneles de control](#updated-look-and-feel-in-the-dashboard-list)
* [Eliminación de la funcionalidad de respaldos en Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Reordenar columnas en cualquier lista con arrastrar y soltar (se está eliminando la funcionalidad)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Restaurar documentos {#restore-documents}

Los administradores de Workfront ahora pueden restaurar documentos individuales que se eliminaron en los últimos 30 días. 

Antes de este cambio, los administradores de Workfront solo podían restaurar proyectos, tareas y problemas (incluidos los documentos eliminados junto con el proyecto, tarea o problema eliminados).

Para obtener más información, consulte [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Nuevo banner de vista previa con información de lanzamiento {#new-preview-banner-with-release-information}

El banner azul en la parte superior del entorno de vista previa ahora muestra el nombre de la versión y el número de versión del entorno de vista previa. Al hacer clic en el nombre de la versión, accederá a un artículo del sitio de ayuda en el que puede encontrar más información sobre la versión de vista previa actual. Para obtener más información sobre el entorno de vista previa de espacio aislado, consulte [Entorno de La zona protegida de previsualización de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## Disponibilidad de la API 7 {#api-7-availability}

La API 7 ya está disponible e incluye objetos nuevos y actualizados.

Para obtener más información, consulte [Novedades de la versión 7 de la API](../../../../wf-api/api/new-api-version-7.md).

## Suscribirse a tareas y problemas {#subscribe-to-tasks-and-issues}

Workfront envía notificaciones sobre los artículos que tienes asignados o que te pertenecen.

A partir de la versión actual, si desea seguir elementos que no están asignados a usted, pero que podrían afectar a su trabajo, puede suscribirse a ellos.

Puede suscribirse a problemas y tareas para los que tiene permisos al menos de visualización. Cuando se agrega un nuevo comentario al problema o la tarea a la que se suscribe, se le notificará por correo electrónico ese comentario.

Para obtener más información acerca de la suscripción a problemas y tareas, vea [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Mejoras en el horario de los recursos {#resource-scheduling-improvements}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el equilibrador de carga de trabajo, consulte [Información general del equilibrador de carga de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Las siguientes mejoras están disponibles al programar recursos:

* [Ver más elementos en la cronología de programación de recursos en una sola vista](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Configurar el nombre del proyecto para que se muestre en las tareas y los problemas en la cronología de programación](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Configurar si las tareas principales se muestran en la cronología de programación](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Expandir o contraer más fácilmente todas las tareas y problemas en la cronología de programación](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [La información sobre funciones y usuarios permanece en la parte superior de la cronología de programación al desplazarse](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Ver más elementos en la cronología de programación de recursos en una sola vista {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Al programar recursos para un equipo o para cualquier proyecto del que sea gerente de recursos, tareas y problemas ahora ocupan menos espacio vertical en la cronología de programación. Esto le permite ver más tareas y problemas en una sola vista.

Si decide mostrar los nombres de los proyectos en cada tarea y problema en la escala de tiempo de programación, el espacio vertical de cada tarea y problema se expande, lo que se traduce en menos tareas y problemas que se muestran en una sola vista.

Para obtener más información sobre la programación de recursos, consulte “Introducción a la programación de recursos”.

### Configurar el nombre del proyecto para que se muestre en las tareas y los problemas en la cronología de programación {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Cuando se programan recursos para un equipo o para cualquier proyecto del que es administrador de recursos, ahora puede configurar el nombre del proyecto para que se muestre en cada tarea y problema en la cronología de programación. Esto permite a los usuarios que ven la cronología de programación ver rápidamente el nombre del proyecto donde reside la tarea o el problema.

Para obtener más información, consulte “Introducción a la programación de recursos”.

### Configurar si las tareas principales se muestran en la cronología de programación {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Al programar recursos para proyectos de los que es el administrador de recursos, ahora puede configurar si las tareas principales se muestran en la cronología de programación cuando la opción Modo de finalización de resumen del proyecto se establece en Manual.

Antes de este cambio, las tareas principales siempre se mostraban en la cronología de programación cuando el modo de finalización de resumen del proyecto se establecía en Manual. 

Cuando el modo de finalización de resumen del proyecto está establecido en Automático, las tareas principales no se pueden mostrar en la cronología de programación. Esta experiencia no ha cambiado.

Para obtener más información, consulte “Introducción a la programación de recursos”.

### Expandir o contraer más fácilmente todas las tareas y problemas en la cronología de programación {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Hay disponible un nuevo vínculo que le permite contraer más fácilmente todas las tareas y problemas en la cronología de programación.

Para obtener más información, consulte “Introducción a la programación de recursos”.

### La información sobre funciones y usuarios permanece en la parte superior de la cronología de programación al desplazarse {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Ahora, cuando se desplaza hacia abajo en la cronología de programación para ver información adicional, el nombre de función y el nombre de usuario permanecen en la parte superior del área de Usuarios y funciones en la cronología de programación, lo que facilita ver a qué usuario y función están asociados las tareas y los problemas.

Antes de este cambio, el nombre de función y el nombre de usuario se desplazaban fuera de la vista actual.

Para obtener más información sobre la programación de recursos, consulte “Introducción a la programación de recursos”.

## Comparar pruebas {#compare-proofs}

Ahora puede comparar dos pruebas de documento dentro de cualquier lista de documentos única, como en la pestaña Documentos de un proyecto, tarea, problema, portafolio o dentro del área principal de Documentos en la barra de navegación global. 

Las dos pruebas se muestran dentro de la herramienta de revisión y aprobación, y puede revisar cada documento mientras lo compara en una vista en paralelo.

Para obtener más información, consulte [Comparar pruebas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Nuevo campo de conjuntos de recursos para usuarios y proyectos {#new-field-for-resource-pools-for-users-and-projects}

La versión R1.5 introdujo nuevas funciones en torno a la planificación de recursos en el entorno de vista previa. Esta funcionalidad le permite crear nuevos conjuntos de recursos, que son colecciones de usuarios.

Ahora puede asociar estos conjuntos de recursos a proyectos y también a usuarios. Ahora verá un nuevo campo llamado “Conjuntos de recursos” en el proyecto, así como en el objeto de usuario.

Para obtener más información sobre los nuevos conjuntos de recursos y cómo se pueden asociar a proyectos y usuarios, consulte [Información general de los conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Apariencia actualizada en la lista del panel de control {#updated-look-and-feel-in-the-dashboard-list}

Ahora, la lista del panel de control es más moderna y escalable.

Anteriormente, esta funcionalidad solo estaba disponible para los usuarios inscritos en Acceso anticipado. Ahora está disponible para todos los usuarios en el entorno de vista previa. Se pondrá a disposición de todos los usuarios en el entorno de producción con la versión 2017.2. 

Para obtener más información sobre los paneles de control, consulte [Crear un panel de control](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Eliminación de la funcionalidad Endosos en Workfront {#removing-the-endorsements-functionality-in-workfront}

Al evaluar la funcionalidad contenida en el flujo de navegación de actualización, hemos identificado Endosos como una función de baja adopción y bajo uso. En 2017.2, la siguiente funcionalidad relacionada con los endosos se eliminará de Workfront a partir de la versión 2017.2 (esta funcionalidad ya no está disponible en la vista previa):

* La pestaña Endosos del área de perfil de usuario;
* El objeto Endosos se eliminará del explorador de API. Si está extrayendo informes de API para los objetos “Endoso” o “Uso compartido de endosos”, las llamadas no serán válidas después de eliminar este objeto.

La siguiente funcionalidad seguirá estando en la aplicación web:

* El endoso de un usuario por parte de otro usuario que se hizo antes de la eliminación de esta función permanecerá en el flujo de actualización del autor del endoso. 

Los endosos no han sido un objeto notificable, por lo tanto, no hay cambios en los informes de este objeto.

## Reordenar columnas en cualquier lista con arrastrar y soltar (se está eliminando la funcionalidad) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

La funcionalidad para cambiar el orden de las columnas en cualquier lista arrastrando una columna desde una ubicación y soltándola en otra se está eliminando del acceso anticipado en el entorno de producción con la versión 2017.2 y ya no estará disponible para ningún usuario. 

Para obtener más información acerca de esta funcionalidad, consulte [Modificar la anchura y el orden de las columnas](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
