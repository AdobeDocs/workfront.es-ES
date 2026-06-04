---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión Beta 1 2018.2
description: En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.2 de Beta 1. La funcionalidad se publicó en el entorno de vista previa el 22 de marzo de 2018. Estará disponible en el entorno de producción en junio de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
TQID: https://experienceleague.adobe.com/H5f7NknmUezFvDKRQJy4eDhvsnZIBjdyeneCqPh5Ico
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1178
ht-degree: 100%

---

# Actividad de la versión Beta 1 2018.2

En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.2 de Beta 1. La funcionalidad se publicó en el entorno de vista previa el 22 de marzo de 2018. Estará disponible en el entorno de producción en junio de 2018.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para obtener una lista de todos los cambios realizados en la versión 2018.2, consulte [Información general sobre la actividad de la versión 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versión 2018.2 de Beta 1 incluye las siguientes mejoras:

* [Modificar fechas de las tareas en el gráfico Gantt](#modify-task-dates-in-the-gantt-chart)
* [Acceder al gráfico Gantt del proyecto desde la pestaña Actualizaciones](#access-the-project-gantt-chart-from-the-updates-tab) (eliminado temporalmente)

* [Se han vuelto a introducir varios vínculos a documentos en la lista de documentos](#various-links-re-introduced-to-documents-on-the-document-list)
* [Mejoras en la vista de usuario en el Planificador de recursos](#user-view-improvements-in-the-resource-planner)
* [Nueva experiencia de lista de proyectos](#new-project-list-experience)
* [Nueva pestaña Buscar actualizaciones](#new-look-for-updates-tab)
* [Mejoras para móviles](#mobile-improvements)

## Modificar fechas de las tareas en el gráfico Gantt {#modify-task-dates-in-the-gantt-chart}

Ahora puede arrastrar la burbuja de la tarea para cambiar las fechas planificadas de inicio y de finalización en el gráfico Gantt. Con este cambio, puede aplicar escenarios hipotéticos a su proyecto sin afectar a la escala de tiempo.

Antes de este cambio, las fechas de las tareas solo se podían cambiar en la lista de tareas o en el nivel de tarea.

Para obtener más información, consulte [Actualizar información en el gráfico Gantt de lista de tareas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Acceder al gráfico Gantt del proyecto desde la pestaña Actualizaciones {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Esta funcionalidad se ha eliminado temporalmente del entorno de vista previa.

Ahora puede acceder al nuevo gráfico Gantt del proyecto desde la pestaña Actualizaciones. Cuando un usuario cambia la Fecha de confirmación de una tarea de forma que afecta a la escala de tiempo del proyecto, se puede ver el impacto en el gráfico Gantt del proyecto.

Antes de este cambio, el vínculo Escala de tiempo del proyecto abría el gráfico Gantt heredado.

Para obtener más información, consulte [Información general sobre la fecha de confirmación](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Para obtener más información, consulte [Información general del Optimizador de portafolios](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Se han vuelto a introducir varios vínculos a documentos de la lista de documentos {#various-links-re-introduced-to-documents-on-the-document-list}

En la versión 18.1, se eliminaron varios vínculos de los documentos de la lista de documentos y se movieron a otras áreas de la interfaz (algunos como un botón situado junto al nombre del documento y otros en un menú desplegable del botón). En esta versión, los siguientes vínculos se vuelven a introducir debajo del nombre del documento y ahora están disponibles en documentos individuales dentro de la lista de documentos:

* Generar revisión (disponible cuando aún no se ha generado una revisión)
* Abrir revisión (disponible cuando se genera una revisión)
* Detalles del documento (disponible cuando aún no se ha generado una revisión)
* Detalles de revisión (disponible cuando se genera una revisión)
* Imprimir resumen

Las siguientes acciones no se vuelven a introducir como vínculos en el documento dentro de la lista de documentos:

* Compartir (sigue disponible como botón en el menú)
* Extraer/Insertar (aún disponible en el menú desplegable Más del menú)

Para obtener más información, consulte las siguientes secciones:

*  en 

## Mejoras en la vista de usuario del Planificador de recursos {#user-view-improvements-in-the-resource-planner}

La vista de usuario del Planificador de recursos ahora incorpora las siguientes mejoras:

* La vista de usuario es ahora la vista predeterminada y reemplaza a la vista de proyecto.
* Filtros mejorados que extraen información de toda la base de datos, en lugar de solo la información de la pantalla.
* Modo de pantalla completa.
* Ahora, el rendimiento es más rápido y más eficiente.

   * Nuevos límites de número de usuarios, proyectos, funciones y tareas que se pueden mostrar.
   * Carga diferida para una carga más rápida de los usuarios.

La siguiente funcionalidad se ha deshabilitado temporalmente en el Planificador de recursos:

* Exportar los datos del Planificador de recursos al usar la vista de usuario.

Antes de estas mejoras, había informado de que el Planificador de recursos tardaba en cargarse y de que había observado incongruencias en los datos mostrados. Con estas mejoras, esto debería haberse solucionado ya.

Para obtener más información sobre las áreas del Planificador de recursos, consulte [Información general sobre la navegación por el Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Nueva experiencia de lista de proyectos {#new-project-list-experience}

Ahora hay disponible una nueva experiencia al ver una lista de proyectos. Esta experiencia incluye un mayor rendimiento y una navegación más fluida y rápida por las listas. Solo las listas de la pestaña Proyectos del área Proyectos de Workfront se han actualizado a esta nueva experiencia.

En su mayor parte, los cambios afectan a la velocidad y la eficacia de la lista. También se han introducido los siguientes cambios visibles:

* La lista muestra de forma predeterminada hasta 2000 elementos.

  Antes de esta mejora, la lista mostraba 100 elementos.

* Las agrupaciones están contraidas de forma predeterminada.

  Antes de este cambio, las agrupaciones aparecían expandidas de forma predeterminada.

* El área para seleccionar una fila se ha expandido a toda la fila.

Las siguientes funciones se han deshabilitado temporalmente en las listas de proyectos especificadas:

* Cambio de tamaño de columna (esta funcionalidad se volvió a introducir en la versión 2018.2 de Beta 5)
* Reordenación de columnas
* Los campos del icono de estado se muestran en blanco (esta funcionalidad se volvió a introducir en la versión 2018.2 de Beta 5)
* No se puede acceder al gráfico Gantt (esta funcionalidad se volvió a introducir en la versión 2018.2 de Beta 3).

Para obtener más información sobre el trabajo en listas, consulte [Introducción a las listas en Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Nueva pestaña Buscar actualizaciones {#new-look-for-updates-tab}

>[!NOTE]
>
>Para algunos usuarios, es posible que la nueva pestaña Actualizaciones no se muestre en el entorno Vista previa. Nuestro equipo de desarrollo está solucionando el problema y trabajando para resolverlo lo antes posible.

La apariencia de la pestaña Actualizaciones ha cambiado para que esté más alineada con otras áreas de la interfaz. Este cambio se aplica a proyectos, tareas, problemas y documentos.

La siguiente tabla muestra las actualizaciones realizadas en la pestaña Actualizaciones:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tarea</strong> </p> </th> 
   <th> <p><strong>Acción anterior de usuario</strong> </p> </th> 
   <th> <p><strong>Nueva acción de usuario</strong> </p> </th> 
   <th> <p><strong>Para obtener más información, consulte...</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Registro de horas en una plantilla de horas</p> </td> 
   <td> <p>Hacer clic en el vínculo Registrar tiempo</p> </td> 
   <td> <p>Hacer clic en el botón Registrar tiempo</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Hora de registro</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtrado de actualizaciones del sistema en la pestaña Actualizaciones</p> </td> 
   <td> <p>Hacer clic en el vínculo Filtrar actualizaciones del sistema</p> </td> 
   <td> <p>Dehabilitar el conmutador Mostrar registro de actividad</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualización de actualizaciones del sistema en la pestaña Actualizaciones</p> </td> 
   <td> <p>Hacer clic en Mostrar todas las actualizaciones</p> </td> 
   <td> <p>Habilitar el conmutador Mostrar registro de actividad</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Etiquetado de otros usuarios en una actualización o comentario</p> </td> 
   <td> <p>Hacer clic en el icono Incluir a otros en esta actualización</p> </td> 
   <td> <p>Añadir usuarios y equipos en el campo Notificar</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que solo los usuarios de su compañía vean un objeto</p> </td> 
   <td> <p>Hacer clic en el icono Más</p> </td> 
   <td> <p>Habilitar el conmutador Privado para mi compañía</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que los usuarios externos a la compañía vean un objeto</p> </td> 
   <td> <p>Hacer clic en el icono Más</p> </td> 
   <td> <p>Desactivar el conmutador Privado para mi compañía</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Etiquetar a otros en las actualizaciones</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Añadir una respuesta o una actualización a un comentario o una actualización</p> </td> 
   <td> <p>Hacer clic en el botón Comentario.</p> </td> 
   <td> <p>Hacer clic en el botón Responder o Actualizar</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Actualizar estado de la tarea</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Actualizar condición para tareas y problemas</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Añadir una actualización a un documento</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mejoras para móviles {#mobile-improvements}

La aplicación móvil incluye las siguientes mejoras:

* Los vínculos compartidos con usted en otras aplicaciones móviles ahora se abren en la aplicación móvil de Workfront.

  Para obtener más información sobre cómo compartir vínculos, consulte .

  Esta actualización se lanzará en iOS en algún momento de esta semana y la actualización de Android se realizará poco después.

* Hemos actualizado nuestros requisitos de compatibilidad con la plataforma iOS para que sea compatible con el iPhone X.

  Para obtener más información sobre los dispositivos móviles y sistemas operativos compatibles, consulte .
