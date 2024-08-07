---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.2 de Beta 1
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 1. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 10 de mayo de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Actividad de la versión 2017.2 de Beta 1

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión 2017.2 Beta 1. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 10 de mayo de 2017.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

La versión 2017.2 de Beta 1 contiene mejoras para administradores de Workfront y otros usuarios:

**Para administradores:**

* [Restaurar documentos](#restore-documents)
* [Nuevo titular de vista previa con información de la versión](#new-preview-banner-with-release-information) 
* [Disponibilidad de API 7](#api-7-availability)

**Para Todos Los Usuarios:**

* [Suscribirse a tareas y problemas](#subscribe-to-tasks-and-issues)
* [Mejoras en la programación de recursos](#resource-scheduling-improvements)
* [Comparar revisiones](#compare-proofs)
* [Nuevo campo para conjuntos de recursos para usuarios y proyectos](#new-field-for-resource-pools-for-users-and-projects)
* [Aspecto actualizado en la lista de paneles](#updated-look-and-feel-in-the-dashboard-list)
* [Quitar la funcionalidad de endosos en Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Reordenar columnas en cualquier lista con arrastrar y soltar (se está eliminando la funcionalidad)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Restaurar documentos {#restore-documents}

Los administradores de Workfront ahora pueden restaurar documentos individuales que se eliminaron en los últimos 30 días. 

Antes de este cambio, los administradores de Workfront solo podían restaurar proyectos, tareas y problemas (incluidos los documentos eliminados junto con el proyecto, la tarea o el problema eliminados).

Para obtener más información, vea [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Nuevo titular de vista previa con información de la versión {#new-preview-banner-with-release-information}

El banner azul en la parte superior del entorno de vista previa de espacio aislado ahora muestra el nombre de la versión y el número de versión del entorno de vista previa. Al hacer clic en el nombre de la versión, accederá a un artículo del sitio de ayuda en el que puede encontrar más información sobre la versión de vista previa actual. Para obtener más información sobre el entorno de vista previa de espacio aislado, consulte [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## Disponibilidad de API 7 {#api-7-availability}

La API 7 ya está disponible e incluye objetos nuevos y actualizados.

Para obtener más información, consulte [Novedades de la versión 7](../../../../wf-api/api/new-api-version-7.md) de la API.

## Suscribirse a tareas y problemas {#subscribe-to-tasks-and-issues}

Workfront envía notificaciones sobre los artículos que tienes asignados o que te pertenecen.

A partir de la versión actual, si desea seguir elementos que no están asignados a usted pero que podrían afectar a su trabajo, puede suscribirse a ellos.

Puede suscribirse a problemas y tareas para los que tiene permisos al menos de Ver. Cuando se agrega un nuevo comentario al problema o la tarea a la que se suscribe, se le notificará por correo electrónico ese comentario.

Para obtener más información acerca de la suscripción a problemas y tareas, vea [Suscribirse a elementos en Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Mejoras en Resource Scheduling {#resource-scheduling-improvements}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Las siguientes mejoras están disponibles al programar recursos:

* [Ver más elementos en la escala de tiempo de programación de recursos en una sola vista](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Configurar el nombre del proyecto para que se muestre en las tareas y problemas de la cronología de programación](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Configurar si las tareas principales se muestran en la escala de tiempo de programación](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Expandir o contraer más fácilmente todas las tareas y problemas en la escala de tiempo de programación](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [La información sobre roles y usuarios permanece en la parte superior de la cronología de programación al desplazarse](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Ver más elementos en la escala de tiempo de programación de recursos en una sola vista {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Al programar recursos para un equipo o para cualquier proyecto del que sea gerente de recursos, las tareas y los problemas ahora consumen menos espacio vertical en la escala de tiempo de la programación. Esto le permite ver más tareas y problemas en una sola vista.

Si decide mostrar los nombres de los proyectos en cada tarea y problema en la escala de tiempo de la programación, el espacio vertical de cada tarea y problema se expande, lo que da como resultado menos tareas y problemas que se muestran en una sola vista.

Para obtener más información sobre la programación de recursos, consulte  &quot;Introducción a la programación de recursos&quot;.

### Configurar el nombre del proyecto para que se muestre en las tareas y los problemas de la cronología de programación {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Al programar recursos para un equipo o para cualquier proyecto del que sea gerente de recursos, ahora puede configurar el nombre del proyecto para que se muestre en cada tarea y problema en la cronología de la programación. Esto permite a los usuarios que ven la cronología de la programación ver rápidamente el nombre del proyecto donde reside la tarea o el problema.

Para obtener más información, consulte Introducción a la programación de recursos.

### Configurar si las tareas principales se muestran en la cronología de programación {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Al programar recursos para proyectos para los que es el Administrador de recursos, ahora puede configurar si las tareas principales se muestran en la escala de tiempo de programación cuando la opción Modo de finalización de resumen del proyecto se establece en Manual.

Antes de este cambio, las tareas principales siempre se mostraban en la escala de tiempo de la programación cuando el modo de finalización de resumen del proyecto se establecía en manual. 

Cuando el modo de finalización de resumen del proyecto está establecido en automático, las tareas principales no se pueden mostrar en la escala de tiempo de la programación. Esta experiencia no ha cambiado.

Para obtener más información, consulte Introducción a la programación de recursos.

### Expandir o contraer más fácilmente todas las tareas y problemas de la cronología de programación {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Hay disponible un nuevo vínculo que le permite contraer más fácilmente todas las tareas y problemas en la cronología de la programación.

Para obtener más información, consulte Introducción a la programación de recursos.

### La información sobre roles y usuarios permanece en la parte superior de la cronología de programación al desplazarse {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Ahora, cuando se desplaza hacia abajo en la escala de tiempo de la programación para ver información adicional, el nombre de rol y el nombre de usuario permanecen en la parte superior del área Usuarios y roles de la escala de tiempo de la programación, lo que facilita ver con qué usuario y rol están asociados las tareas y los problemas.

Antes de este cambio, el nombre de función y el nombre de usuario se desplazaban fuera de la vista actual.

Para obtener más información sobre la programación de recursos, consulte  &quot;Introducción a la programación de recursos&quot;.

## Comparar revisiones {#compare-proofs}

Ahora puede comparar dos pruebas de documento dentro de cualquier lista de documentos única, como en la ficha Documentos de un proyecto, tarea, problema, portafolio o dentro del área principal Documentos en la barra de exploración global. 

Las dos pruebas se muestran dentro de la herramienta de revisión y aprobación, y puede probar cada documento mientras lo compara en una vista en paralelo.

Para obtener más información, consulte [Comparar pruebas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Nuevo campo para conjuntos de recursos para usuarios y proyectos {#new-field-for-resource-pools-for-users-and-projects}

La versión R1.5 introdujo nuevas funciones en torno a la planificación de recursos en el entorno de vista previa. Esta funcionalidad le permite crear nuevos conjuntos de recursos, que son colecciones de usuarios.

Ahora puede asociar estos conjuntos de recursos con proyectos y con usuarios. Ahora verá un nuevo campo llamado &quot;Conjuntos de recursos&quot; en el proyecto, así como en el objeto de usuario.

Para obtener más información sobre los nuevos conjuntos de recursos y cómo se pueden asociar a proyectos y usuarios, vea [Resumen de los conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Aspecto actualizado en la lista de paneles {#updated-look-and-feel-in-the-dashboard-list}

Ahora, al ver una lista de tableros, el aspecto es más moderno y escalable.

Anteriormente, esta funcionalidad solo estaba disponible para los usuarios inscritos en Acceso anticipado. Ahora está disponible para todos los usuarios en el entorno de vista previa. Se pondrá a disposición de todos los usuarios en el entorno de producción con la versión 2017.2. 

Para obtener más información acerca de los paneles, vea [Crear un panel](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Eliminación de la funcionalidad Endosos en Workfront {#removing-the-endorsements-functionality-in-workfront}

Al evaluar la funcionalidad contenida en el flujo de actualización, hemos identificado Endosos como una función de baja adopción y bajo uso. En 2017.2, las siguientes funcionalidades relacionadas con los endosos se eliminarán de Workfront a partir de la versión 2017.2 (estas funcionalidades ya no están disponibles en Vista previa):

* La pestaña Endosos del área de perfil de usuario;
* El objeto Endosos se eliminará del explorador de API. Si está extrayendo informes de API para los objetos &quot;Endoso&quot; o &quot;Uso compartido de endosos&quot;, las llamadas no serán válidas después de eliminar este objeto.

La siguiente funcionalidad seguirá estando en la aplicación web:

* El endoso de un usuario por parte de otro usuario que se hizo antes de la eliminación de esta función permanecerá en el flujo de actualización del endosante. 

Los endosos no han sido un objeto de informe, por lo que no hay cambios en los informes de este objeto.

## Reordenar columnas en cualquier lista con arrastrar y soltar (se está eliminando la funcionalidad) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

La funcionalidad para cambiar el orden de las columnas en cualquier lista arrastrando una columna desde una ubicación y soltándola en otra se está eliminando del acceso anticipado en el entorno de producción con la versión 2017.2 y ya no estará disponible para ningún usuario. 

Para obtener más información acerca de esta funcionalidad, vea [Modificar el ancho y el orden de las columnas](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
