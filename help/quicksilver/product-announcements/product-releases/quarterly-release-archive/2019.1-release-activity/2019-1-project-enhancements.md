---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Mejoras de proyectos en 2019.1
description: Esta página describe todas las mejoras del proyecto incluidas en la versión 2019.1. La funcionalidad está disponible actualmente en el entorno de vista previa. Estará disponible en el entorno de producción de en .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# Mejoras de proyectos en 2019.1

Esta página describe todas las mejoras del proyecto incluidas en la versión 2019.1. La funcionalidad está disponible actualmente en el entorno de vista previa. Estará disponible en el entorno de producción de en .

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para obtener una lista de todos los cambios realizados en 2019.1, consulte &quot;Información general de la actividad de la versión 2019.1&quot;.

**Para administradores**

* [Restaurar plantillas de la papelera](#restore-templates-from-the-recycle-bin)
* [Mostrar marcas de hora para los campos de fecha de inicio](#show-timestamps-for-date-fields-in-home)
* [Todos los tipos de duración disponibles en Preferencias de proyecto](#all-duration-types-available-under-project-preferences)

**Para todos los usuarios**

* [Mejoras de Agile](#agile-improvements)
* [Agregar tareas y problemas de una lista a una iteración](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [Nuevos tamaños de papel para la exportación del gráfico Gantt](#new-paper-sizes-for-gantt-chart-export)
* [Se eliminó el acceso a los cuadros de diálogo del gráfico Gantt mientras se encontraba en el modo de edición](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [Ver información de tarea en el gráfico Gantt de lista de proyectos de un programa o Portfolio](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [Acceder al gráfico Gantt de lista de tareas en las plantillas](#access-the-task-list-gantt-chart-on-templates)
* [Se cambió el nombre de la vista de proyecto en el gráfico Gantt](#renamed-the-project-view-on-the-gantt-chart)
* [Escenarios hipotéticos en el gráfico Gantt de lista de tareas](#what-if-scenarios-in-the-task-list-gantt-chart)
* [Mejoras en la lista de tareas](#task-list-improvements)
* [Mostrar listas en pantalla completa](#display-lists-in-full-screen)
* [Listas nuevas en áreas adicionales](#new-lists-in-additional-areas)
* [Enviar un informe enviado en formato XLSX](#send-a-delivered-report-in-xlsx-format)
* [Exportar registros de auditoría](#export-audit-logs)

## Restaurar plantillas desde la papelera de reciclaje {#restore-templates-from-the-recycle-bin}

Los administradores de Workfront ahora pueden restaurar las plantillas desde la papelera de reciclaje. Al igual que con otros elementos eliminados, puede restaurar una plantilla hasta 30 días después de su eliminación.

Para obtener más información, consulte &quot;Restauración de elementos eliminados&quot;.

## Mostrar marcas de hora para los campos de fecha en Inicio {#show-timestamps-for-date-fields-in-home}

Como administrador de Workfront, ahora puede elegir mostrar u ocultar las marcas de tiempo de las fechas de vencimiento en la Lista de trabajos y el Calendario mediante plantillas de diseño. De forma predeterminada, las marcas de tiempo son visibles tanto para los usuarios de plantillas como para los que no son plantillas.

Para obtener más información, consulte &quot;Personalización del área de inicio&quot; en el artículo &quot;Creación y administración de plantillas de diseño&quot;.

## Todos los tipos de duración disponibles en Preferencias de proyecto {#all-duration-types-available-under-project-preferences}

Al establecer el tipo predeterminado de duración de tarea y problema en Configuración > Preferencias de proyecto, puede utilizar cualquiera de las siguientes opciones:

Simple

Condicionada por el esfuerzo

Asignación calculada

Trabajo calculado

Anteriormente, si establecía Simple o Condicionada por el esfuerzo como tipo de duración predeterminado, no podía elegir Asignación calculada y Trabajo calculado.

Para obtener más información sobre la configuración de los valores predeterminados de tipo de duración de tarea y problema, consulte &quot;Preferencias de tareas y problemas&quot;

## Mejoras de Agile {#agile-improvements}

Las siguientes mejoras ya están disponibles en la herramienta Agile:

Kanban

Agregar tareas y problemas al Panel Kanban desde cualquier lista de tareas o informe.

Anteriormente, solo se podían agregar tareas al panel Kanban desde el registro de asuntos pendientes. No ha podido añadir problemas.

Filtre el panel Kanban por usuarios individuales del equipo.

Para obtener más información, consulte &quot;Uso del Panel Kanban&quot;.

Ver y administrar problemas en el registro de asuntos pendientes de Kanban.

Para obtener más información, consulte &quot;Uso del Panel Kanban.

Anteriormente, no se podían agregar ni administrar problemas en un panel Kanban.

Scrum

Filtre el guion gráfico de iteraciones por usuarios individuales del equipo.

Para obtener más información, consulte &quot;Uso del guion gráfico de Scrum Agile&quot;.

Anteriormente, no se podía filtrar por usuario en los paneles Kanban o de Scrum.

## Agregar tareas y problemas de una lista a una iteración {#add-tasks-and-issues-from-a-list-to-an-iteration}

Ahora puede utilizar una tarea o una lista de problemas, un informe o un panel para agregar historias a una iteración. También puede tener varios equipos asignados historias en una iteración.

Anteriormente, sólo se podía agregar un artículo a una iteración desde la página de detalles de tareas o problemas, y sólo se podían agregar artículos a las iteraciones creadas por el equipo.

Para obtener más información, consulte &quot;Creación y administración de iteraciones de Agile&quot;.

## Envío de un informe enviado en formato XLSX {#send-a-delivered-report-in-xlsx-format}

Ahora puede programar la entrega de un informe en formato MS Excel (.xlsx), además de todos los demás formatos actuales.

Anteriormente, un informe solo se podía entregar en los siguientes formatos:

HTML

PDF

MS Excel (.xls)

TSV

Para obtener información sobre la programación de informes para su envío, consulte &quot;Configuración de envíos de informes&quot;.

## Mejoras en la lista de tareas {#task-list-improvements}

[actualización 18.3 de Beta 4 de la cual se eliminó esto]

Las listas de tareas recién rediseñadas se han vuelto a habilitar, después de una breve eliminación durante la versión 18.3 beta 4. También hemos introducido las siguientes funciones adicionales en las listas de tareas que no formaban parte de la versión original:

Sustituir el menú que aparece al hacer clic con el botón derecho por un icono Más al editar en línea una tarea.

Las opciones disponibles en el menú que se muestra al hacer clic con el botón derecho cuando se editan en línea varias tareas se han trasladado a los iconos que se muestran en la parte superior de la lista de tareas.

De forma predeterminada, las listas de tareas muestran 2000 tareas.

Cuando Workfront vuelve a calcular las escalas de tiempo, los signos de interrogación adyacentes a las tareas cuyas fechas se están actualizando se han reemplazado por áreas grises.

Para obtener información sobre la edición de tareas en línea, vea &quot;Copiar y duplicar tareas&quot; y &quot;Crear relaciones de predecesoras encadenando tareas&quot;.

Para obtener información sobre cómo recalcular las escalas de tiempo de un proyecto, consulte &quot;Recalcular escalas de tiempo para proyectos&quot;.

## Mostrar listas en pantalla completa {#display-lists-in-full-screen}

Cuando una lista de proyectos o tareas es más grande que el tamaño de la pantalla, la lista ahora se muestra automáticamente en toda la ventana del explorador mientras se desplaza. Esto aumenta la cantidad de información que se ve al mismo tiempo y permite hacer listas más fáciles de administrar.

Puede mostrar las siguientes listas en pantalla completa:

Una lista de proyectos en las siguientes pestañas y subpestañas:

Proyectos en los que participo

Proyectos de mi propiedad

Todos los proyectos

Pestaña Proyectos en un Portfolio

Pestaña Proyectos en un programa

Una lista de tareas en las siguientes pestañas:

Ficha Tareas de un proyecto

Pestaña Subtareas de una tarea

Para obtener información sobre la visualización de objetos en listas, consulte &quot;Visualización de elementos en una lista&quot;.

## Listas nuevas en áreas adicionales {#new-lists-in-additional-areas}

Hemos mejorado el rendimiento y la apariencia de las listas de proyectos y tareas en las siguientes áreas:

Fichas Portfolio y Programas del área Proyectos

Pestaña Subtareas en el nivel de tarea

Antes de esta mejora, las nuevas listas solo estaban disponibles en las siguientes áreas:

Pestaña Proyectos del área Proyectos

Pestaña Tareas en el nivel de proyecto

Para obtener información sobre la visualización de objetos en listas, consulte &quot;Visualización de elementos en una lista&quot;.

## Ver información de tareas en el diagrama de Gantt de lista de proyectos en un programa o Portfolio {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

Ahora puede ver información sobre las tareas de un proyecto en el diagrama de Gantt de lista de proyectos dentro de un programa o Portfolio.

Anteriormente, la información sobre las tareas sólo se podía ver en el Diagrama de Gantt de lista de proyectos de la ficha Proyectos.

Para obtener más información, consulte &quot;Visualización de información en el diagrama de Gantt&quot;.

## Escenarios hipotéticos en el gráfico Gantt de lista de tareas {#what-if-scenarios-in-the-task-list-gantt-chart}

Ahora puede realizar las siguientes acciones en las tareas de un proyecto cuando se muestren en el modo de edición del gráfico Gantt:

Añadir tareas

Eliminar tareas

Tareas de edición en línea

Duplicar tareas

Reorganizar tareas

Modificar subtareas

Aunque puede ver cómo afectan los cambios a la cronología del proyecto, no se guardan inmediatamente. Puede guardarlos para actualizar permanentemente la cronología del proyecto o puede cancelarlos.

Anteriormente, no se podían obtener vistas previas de los cambios en la lista de tareas en el gráfico Gantt.

Para obtener información sobre la edición de tareas en el diagrama de Gantt, consulte &quot;Actualización de información en el diagrama de Gantt de lista de tareas&quot;.

## Acceso al diagrama de Gantt de lista de tareas en plantillas {#access-the-task-list-gantt-chart-on-templates}

Ahora puede acceder al gráfico Gantt de lista de tareas dentro de una plantilla de proyecto.

Anteriormente, no se podía ver el gráfico Gantt en la lista de tareas dentro de una plantilla.

Para obtener más información, consulte &quot;Introducción al gráfico Gantt&quot;.

## Nuevos tamaños de papel para la exportación del gráfico Gantt {#new-paper-sizes-for-gantt-chart-export}

Ahora puede imprimir el gráfico Gantt en los tamaños de papel A1 y A2.

Anteriormente, solo se podía exportar a Carta, Legal, Libro mayor, A3 (disponible solo para algunos idiomas) y A4.

Para obtener más información, consulte &quot;Exportación del gráfico Gantt a PDF&quot;.

## Se cambió el nombre de la vista de proyecto en el gráfico Gantt {#renamed-the-project-view-on-the-gantt-chart}

Se ha cambiado el nombre de la opción de vista &quot;Proyecto&quot; en el gráfico Gantt a &quot;Ajustar todo&quot;. La opción de visualización sigue funcionando como antes. El nuevo nombre pretende ser más descriptivo de lo que se ve cuando se selecciona la opción.

Para obtener más información, consulte &quot;Visualización de información en el diagrama de Gantt&quot;.

## Se ha eliminado el acceso a los cuadros de diálogo del gráfico Gantt en el modo de edición {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

Ya no puede acceder al cuadro de diálogo Asignaciones avanzadas mientras el gráfico Gantt se encuentra en modo de edición. Solo puede realizar ediciones en línea mientras el gráfico Gantt de la lista de tareas está en modo de edición.

Anteriormente, se podía acceder al cuadro de diálogo Asignaciones avanzadas mientras el diagrama de Gantt estaba en modo de edición, pero se guardaban los cambios realizados en el diagrama de Gantt y se cerraba el modo de edición.

Para obtener más información sobre la edición del gráfico Gantt de lista de tareas, consulte &quot;Actualización de información en el gráfico Gantt de lista de tareas&quot;.

## Exportar registros de auditoría {#export-audit-logs}

Ahora puede exportar entradas del registro de auditoría a un archivo CSV. Puede exportar hasta 50 000 entradas de registro de auditoría a un archivo CSV al mismo tiempo.

Para obtener más información, consulte &quot;Administración de registros de auditoría&quot;.
