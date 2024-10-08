---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2018.2 de Beta 1
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.2 Beta 1. La funcionalidad se publicó en el entorno de vista previa el 22 de marzo de 2018. Estará disponible en el entorno de producción en junio de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# Actividad de la versión 2018.2 de Beta 1

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.2 Beta 1. La funcionalidad se publicó en el entorno de vista previa el 22 de marzo de 2018. Estará disponible en el entorno de producción en junio de 2018.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para obtener una lista de todos los cambios realizados en 2018.2, consulte [Resumen de la actividad de la versión 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versión 2018.2 de Beta 1 incluye las siguientes mejoras:

* [Modificar fechas de tarea en el gráfico Gantt](#modify-task-dates-in-the-gantt-chart)
* [Acceder al gráfico Gantt del proyecto desde la ficha Actualizaciones](#access-the-project-gantt-chart-from-the-updates-tab) (Eliminado temporalmente)

* [Se han vuelto a introducir varios vínculos a documentos de la lista de documentos](#various-links-re-introduced-to-documents-on-the-document-list)
* [Mejoras en la vista de usuario en el Planificador de recursos](#user-view-improvements-in-the-resource-planner)
* [Nueva experiencia de lista de proyectos](#new-project-list-experience)
* [Nueva ficha Buscar actualizaciones](#new-look-for-updates-tab)
* [Mejoras de Mobile](#mobile-improvements)

## Modificar fechas de tarea en el diagrama de Gantt {#modify-task-dates-in-the-gantt-chart}

Ahora puede arrastrar la burbuja de tareas para cambiar las fechas planificadas de inicio y finalización en el gráfico Gantt. Con este cambio, puede aplicar escenarios hipotéticos a su proyecto sin afectar a la cronología.

Antes de este cambio, las fechas de las tareas solo se podían cambiar en la lista de tareas o en el nivel de tarea.

Para obtener más información, vea [Actualizar información en la lista de tareas Diagrama de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Acceda al diagrama de Gantt del proyecto desde la pestaña Actualizaciones {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Esta funcionalidad se ha eliminado temporalmente del entorno de vista previa.

Ahora puede acceder al nuevo gráfico Gantt del proyecto desde la pestaña Actualizaciones. Cuando un usuario cambia la fecha de confirmación de una tarea de forma que afecta a la cronología del proyecto, puede ver el impacto en el gráfico Gantt del proyecto.

Antes de este cambio, el vínculo Escala de tiempo del proyecto abría el Diagrama de Gantt heredado.

Para obtener más información, consulte [Resumen de la fecha de confirmación](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Para obtener más información, consulte [Descripción general de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Se han vuelto a introducir varios vínculos a documentos de la lista de documentos {#various-links-re-introduced-to-documents-on-the-document-list}

En la versión 18.1, se eliminaron varios vínculos de los documentos de la lista de documentos y se movieron a otras áreas de la interfaz (algunos como un botón situado junto al nombre del documento y otros en un menú desplegable del botón ). Los siguientes vínculos se vuelven a introducir debajo del nombre del documento con esta versión y ahora están disponibles en documentos individuales dentro de la lista de documentos:

* Generar revisión (disponible cuando aún no se ha generado una revisión)
* Abrir prueba (disponible cuando se genera una prueba)
* Detalles del documento (disponible cuando aún no se ha generado una prueba)
* Detalles de la prueba (disponible cuando se genera una prueba)
* Imprimir resumen

Las siguientes acciones no se vuelven a introducir como vínculos en el documento dentro de la lista de documentos:

* Compartir (sigue disponible como botón en el menú)
* Desproteger / Proteger (aún disponible en el menú desplegable Más del menú)

Para obtener más información, consulte las secciones siguientes:

*  in 

## Mejoras en la vista de usuarios del Planificador de recursos {#user-view-improvements-in-the-resource-planner}

La vista de usuario del Planificador de recursos ahora contiene las siguientes mejoras:

* La vista de usuario es ahora la vista predeterminada y reemplaza a la vista de proyecto.
* Filtros mejorados que extraen información de toda la base de datos, en lugar de solo la información de la pantalla.
* Modo de pantalla completa.
* Ahora, el rendimiento es más rápido y eficiente.

   * Nuevos límites para el número de usuarios, proyectos, funciones y tareas que se pueden mostrar.
   * Carga diferida para una carga más rápida de los usuarios.

La siguiente funcionalidad se ha deshabilitado temporalmente en el Planificador de recursos:

* Exportar los datos del Planificador de recursos al usar la Vista de usuario.

Antes de estas mejoras, había informado de que el Planificador de recursos tardaba en cargarse y de que había observado incongruencias en los datos mostrados. Con estas mejoras, ahora deberían eliminarse.

Para obtener más información sobre las áreas del Planificador de recursos, consulte [Resumen de navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Nueva experiencia de lista de proyectos {#new-project-list-experience}

Ahora hay disponible una nueva experiencia al ver una lista de proyectos. Esta experiencia incluye un mayor rendimiento y una navegación por listas más suave y rápida. Solo las listas de la pestaña Proyectos del área Proyectos de Workfront se han actualizado a esta nueva experiencia.

En su mayor parte, los cambios están en la velocidad y la eficacia de la lista. También se han introducido los siguientes cambios visibles:

* La lista muestra de forma predeterminada hasta 2000 elementos.

  Antes de esta mejora, la lista mostraba 100 elementos.

* Las agrupaciones se contraen de forma predeterminada.

  Antes de este cambio, las agrupaciones se expandían de forma predeterminada.

* El área para seleccionar una fila se ha expandido a toda la fila.

Las siguientes funciones se han deshabilitado temporalmente en las listas de proyectos especificadas:

* Cambio de tamaño de columna (esta funcionalidad se volvió a introducir en la versión 2018.2 de Beta 5)
* Reordenación de columnas
* Los campos del icono de estado se muestran en blanco (esta funcionalidad se volvió a introducir en la versión 2018.2 de Beta 5)
* No se puede acceder al gráfico Gantt (esta funcionalidad se volvió a introducir en la versión 2018.2 de Beta 3).

Para obtener más información sobre cómo trabajar en listas, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Nueva pestaña Buscar actualizaciones {#new-look-for-updates-tab}

>[!NOTE]
>
>Para algunos usuarios, es posible que la nueva pestaña Actualizaciones no se muestre en el entorno de Vista previa. Nuestro equipo de desarrollo está solucionando el problema y trabajando para resolverlo lo antes posible.

El aspecto de la pestaña Actualizaciones ha cambiado para estar más alineada con otras áreas de la interfaz. Este cambio se aplica a proyectos, tareas, problemas y documentos.

La siguiente tabla muestra las actualizaciones realizadas en la pestaña Actualizaciones:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tarea</strong> </p> </th> 
   <th> <p><strong>Acción anterior del usuario</strong> </p> </th> 
   <th> <p><strong>Nueva acción de usuario</strong> </p> </th> 
   <th> <p><strong>Para obtener más información, consulte...</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Registrar las horas en una plantilla de horas</p> </td> 
   <td> <p>Haga clic en el vínculo Registrar tiempo</p> </td> 
   <td> <p>Haga clic en el botón Registrar tiempo</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Hora de registro</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtrado de actualizaciones del sistema en la ficha Actualizaciones</p> </td> 
   <td> <p>Haga clic en el vínculo Filtrar actualizaciones del sistema</p> </td> 
   <td> <p>Desactive la opción Mostrar registro de actividad</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabajo de actualización</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualización de actualizaciones del sistema en la ficha Actualizaciones</p> </td> 
   <td> <p>Haga clic en Mostrar todas las actualizaciones</p> </td> 
   <td> <p>Activar la opción Mostrar registro de actividad</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabajo de actualización</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Etiquetado de otros usuarios en una actualización o comentario</p> </td> 
   <td> <p>Haga clic en el icono Incluir a otros en esta actualización</p> </td> 
   <td> <p>Agregar usuarios y equipos en el campo Notificar</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabajo de actualización</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que solo los usuarios de su empresa vean un objeto</p> </td> 
   <td> <p>Haga clic en el icono Bloquear</p> </td> 
   <td> <p>Activar la opción Privado a Mi compañía</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que los usuarios externos a la compañía vean un objeto</p> </td> 
   <td> <p>Haga clic en el icono Bloquear</p> </td> 
   <td> <p>Desactivar la opción Privado a Mi compañía</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar una respuesta o una actualización a un comentario o una actualización</p> </td> 
   <td> <p>Haga clic en el botón Comentario</p> </td> 
   <td> <p>Haga clic en el botón Responder o Actualizar</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabajo de actualización</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Actualizar estado de la tarea</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Actualizar condición para tareas y problemas</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Agregar una actualización a un documento</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mejoras de Mobile {#mobile-improvements}

La aplicación móvil incluye las siguientes mejoras:

* Los vínculos compartidos con usted en otras aplicaciones móviles ahora se abren en la aplicación móvil de Workfront.

  Para obtener más información sobre cómo compartir vínculos, consulte .

  Esta actualización se lanzará a iOS a veces esta semana y la actualización de Android debe realizarse poco después.

* Hemos actualizado nuestros requisitos de soporte para la plataforma iOS para admitir iPhone X.

  Para obtener más información acerca de los dispositivos móviles y sistemas operativos compatibles, consulte .
