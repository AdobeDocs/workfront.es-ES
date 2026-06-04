---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Mejoras del proyecto 2019.1
description: En esta página se describen todas las mejoras del proyecto incluidas en la versión 2019.1. La funcionalidad está disponible actualmente en el entorno de vista previa. Estará disponible en el entorno de producción en .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
TQID: https://experienceleague.adobe.com/cHyxMUlRSlpjq9pLWw-jBmewYCc7REao-zYdMQq861Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1467
ht-degree: 100%

---

# Mejoras del proyecto 2019.1

En esta página se describen todas las mejoras del proyecto incluidas en la versión 2019.1. La funcionalidad está disponible actualmente en el entorno de vista previa. Estará disponible en el entorno de producción en .

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para obtener una lista de todos los cambios realizados en 2019.1, consulte &quot;Información general sobre la actividad de la versión 2019.1&quot;.

**Para administradores**

* [Restaurar plantillas desde la papelera de reciclaje](#restore-templates-from-the-recycle-bin)
* [Mostrar marcas de hora para los campos de fecha en Inicio](#show-timestamps-for-date-fields-in-home)
* [Todos los tipos de duración disponibles en Preferencias de proyecto](#all-duration-types-available-under-project-preferences)

**Para todos los usuarios**

* [Mejoras de Agile](#agile-improvements)
* [Añadir tareas y problemas de una lista a una iteración](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [Nuevos tamaños de papel para la exportación del gráfico Gantt](#new-paper-sizes-for-gantt-chart-export)
* [Se ha eliminado el acceso a los cuadros de diálogo del gráfico Gantt en el modo de edición](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [Ver información sobre una tarea en el gráfico Gantt de lista de proyectos en un programa o portafolio](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [Acceso al gráfico Gantt de lista de tareas en plantillas](#access-the-task-list-gantt-chart-on-templates)
* [Se cambió el nombre de la vista de proyecto en el gráfico Gantt](#renamed-the-project-view-on-the-gantt-chart)
* [Escenarios hipotéticos en el gráfico Gantt de lista de tareas](#what-if-scenarios-in-the-task-list-gantt-chart)
* [Mejoras en la lista de tareas](#task-list-improvements)
* [Mostrar listas en pantalla completa](#display-lists-in-full-screen)
* [Listas nuevas en áreas adicionales](#new-lists-in-additional-areas)
* [Envío de un informe enviado en formato XLSX](#send-a-delivered-report-in-xlsx-format)
* [Exportar registros de auditoría](#export-audit-logs)

## Restaurar plantillas desde la papelera de reciclaje {#restore-templates-from-the-recycle-bin}

Ahora, los administradores de Workfront pueden restaurar las plantillas desde la papelera de reciclaje. Al igual que sucede con otros elementos eliminados, puede restaurar una plantilla hasta 30 días después de su eliminación.

Para obtener más información, consulte &quot;Restauración de elementos eliminados&quot;.

## Mostrar marcas de hora para los campos de fecha en Inicio {#show-timestamps-for-date-fields-in-home}

Como administrador de Workfront, ahora puede elegir mostrar u ocultar las marcas de tiempo de las fechas de vencimiento en la Lista de trabajos y el Calendario mediante plantillas de diseño. De forma predeterminada, las marcas de tiempo son visibles tanto para los usuarios de plantillas como para los que no lo son.

Para obtener más información, consulte &quot;Personalización del área de inicio&quot; en el artículo &quot;Creación y administración de plantillas de diseño&quot;.

## Todos los tipos de duración disponibles en Preferencias de proyecto {#all-duration-types-available-under-project-preferences}

Al establecer el tipo predeterminado de duración de tarea y problema en Configuración > Preferencias de proyecto, puede utilizar cualquiera de las siguientes opciones:

Simple

Condicionada por el esfuerzo

Asignación calculada

Trabajo calculado

Anteriormente, si establecía Simple o Condicionada por el esfuerzo como tipo de duración predeterminado, no podía elegir Asignación calculada y Trabajo calculado.

Para obtener más información sobre la configuración de los valores predeterminados de tipo de duración de las tareas y problemas, consulte &quot;Preferencias de tareas y problemas&quot;

## Mejoras de Agile {#agile-improvements}

Las siguientes mejoras ya están disponibles en la herramienta Agile:

Kanban

Añada tareas y problemas al tablero Kanban desde cualquier lista de tareas o informe.

Anteriormente, solo se podían añadir tareas al tablero Kanban desde el registro de asuntos pendientes. No se han podido añadir problemas.

Filtrar el tablero Kanban por usuarios individuales del equipo.

Para obtener más información, consulte “Uso del tablero Kanban”.

Ver y administrar problemas en el registro de asuntos pendientes de Kanban.

Para obtener más información, consulte “Uso del tablero Kanban”.

Anteriormente, no se podían añadir ni administrar problemas en un tablero Kanban.

Scrum

Filtrar el tablero de historias de iteraciones por usuarios individuales del equipo.

Para obtener más información, consulte “Uso del tablero de historias ágil de Scrum”.

Anteriormente, no se podía filtrar por usuario en los tableros Kanban o de Scrum.

## Añadir tareas y problemas de una lista a una iteración {#add-tasks-and-issues-from-a-list-to-an-iteration}

Ahora puede utilizar una lista de tareas o problemas, un informe o un panel de control para añadir historias a una iteración. También puede tener varios equipos con historias asignadas en una iteración.

Anteriormente, solo podía añadir un artículo a una iteración desde la página de detalles de tarea o de problemas, y solo podía añadir artículos a las iteraciones creadas por su equipo.

Para obtener más información, consulte “Creación y administración de iteraciones ágiles”.

## Envío de un informe recibido en formato XLSX {#send-a-delivered-report-in-xlsx-format}

Ahora puede programar la entrega de un informe en formato MS Excel (.xlsx), además de todos los demás formatos actuales.

Anteriormente, un informe solo se podía entregar en los siguientes formatos:

HTML

PDF

MS Excel (.xls)

TSV

Para obtener información sobre la programación de informes para enviar, consulte “Configuración de envíos de informes”.

## Mejoras en la lista de tareas {#task-list-improvements}

[actualización 18.3 Beta 4 de la cual se eliminó esta opción]

Las listas de tareas recién rediseñadas se han vuelto a habilitar, después de una breve eliminación durante la versión 18.3 Beta 4. También hemos introducido las siguientes características adicionales a las listas de tareas que no formaban parte de la versión original:

Sustitución del menú que aparece al hacer clic con el botón derecho por un icono Más al editar en línea una tarea.

Las opciones disponibles en el menú que se muestra al hacer clic con el botón derecho cuando se editan en línea varias tareas se han trasladado a los iconos que se muestran en la parte superior de la lista de tareas.

De forma predeterminada, las listas de tareas muestran 2000 tareas.

Cuando Workfront vuelve a calcular las cronologías, los signos de interrogación adyacentes a las tareas cuyas fechas se están actualizando se han reemplazado por áreas grises.

Para obtener información sobre la edición de tareas en línea, vea &quot;Copiar y duplicar tareas&quot; y &quot;Crear relaciones de predecesoras encadenando tareas&quot;.

Para obtener información sobre cómo recalcular las cronologías de un proyecto, consulte &quot;Recalcular cronologías para proyectos&quot;.

## Mostrar listas en pantalla completa {#display-lists-in-full-screen}

Cuando una lista de proyectos o tareas es más grande que el tamaño de la pantalla, la lista ahora se muestra automáticamente en toda la ventana del explorador mientras se desplaza. Esto aumenta la cantidad de información que se ve de una sola vez y permite crear listas más fáciles de administrar.

Se pueden mostrar en pantalla completa las siguientes listas:

Una lista de proyectos en las siguientes pestañas y subpestañas:

Proyectos en los que participo

Proyectos de mi propiedad

Todos los proyectos

Pestaña Proyectos de un portafolio

Pestaña Proyectos de un programa

Una lista de tareas en las siguientes pestañas:

Pestaña Tareas de un proyecto

Pestaña Subtareas de una tarea

Para obtener información sobre la visualización de objetos en listas, consulte “Visualización de elementos en una lista”.

## Listas nuevas en áreas adicionales {#new-lists-in-additional-areas}

Hemos mejorado el rendimiento y la apariencia de las listas de proyectos y tareas en las siguientes áreas:

Pestañas Portafolio y Programas del área Proyectos

Pestaña Subtareas en el nivel de tarea

Antes de esta mejora, las nuevas listas solo estaban disponibles en las siguientes áreas:

Pestaña Proyectos del área Proyectos

Pestaña Tareas en el nivel de proyecto

Para obtener información sobre la visualización de objetos en listas, consulte “Visualización de elementos en una lista”.

## Ver información sobre una tarea en el gráfico Gantt de lista de proyectos en un programa o portafolios {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

Ahora puede ver información sobre las tareas de un proyecto en el gráfico Gantt de la lista de proyectos dentro de un programa o portafolios.

Antes, la información sobre las tareas solo se podía ver en el gráfico Gantt de la lista de proyectos en la pestaña Proyectos.

Para obtener más información, consulte “Visualización de información en el gráfico Gantt”.

## Escenarios hipotéticos en el gráfico Gantt de lista de tareas {#what-if-scenarios-in-the-task-list-gantt-chart}

Ahora puede realizar las siguientes acciones en las tareas de un proyecto cuando se muestran en el modo de edición del gráfico Gantt:

Añadir tareas

Eliminar tareas

Tareas de edición en línea

Duplicar tareas

Reorganizar tareas

Modificar subtareas

Aunque se puede ver cómo afectan los cambios a la cronología del proyecto, estos no se guardan inmediatamente. Puede guardarlos para actualizar la cronología del proyecto permanentemente o puede cancelarlos.

Antes, no se podían obtener vistas previas de los cambios en la lista de tareas del gráfico Gantt.

Para obtener información sobre la edición de tareas en el gráfico Gantt, consulte “Actualizar información en el gráfico Gantt de la lista de tareas”.

## Acceso al gráfico Gantt de lista de tareas en plantillas {#access-the-task-list-gantt-chart-on-templates}

Ahora puede acceder al gráfico Gantt de lista de tareas dentro de una plantilla de proyecto.

Anteriormente, no se podía ver el gráfico Gantt en la lista de tareas dentro de una plantilla.

Para obtener más información, consulte “Introducción al gráfico Gantt”.

## Nuevos tamaños de papel para la exportación del gráfico Gantt {#new-paper-sizes-for-gantt-chart-export}

Ahora puede imprimir el gráfico Gantt en los tamaños de papel A1 y A2.

Anteriormente, solo se podía exportar a Carta, Legal, Libro mayor, A3 (disponible solo para algunos idiomas) y A4.

Para obtener más información, consulte “Exportación del gráfico Gantt a PDF”.

## Se cambió el nombre de la vista de proyecto en el gráfico Gantt {#renamed-the-project-view-on-the-gantt-chart}

Se ha cambiado el nombre de la opción de vista “Proyecto” en el gráfico Gantt a “Ajustar todo”. La opción de visualización sigue funcionando igual que antes. El nuevo nombre pretende ser más descriptivo de lo que se ve cuando se selecciona la opción.

Para obtener más información, consulte “Visualización de información en el gráfico Gantt”.

## Se ha eliminado el acceso a los cuadros de diálogo del gráfico Gantt en el modo de edición {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

Ya no es posible acceder al cuadro de diálogo Asignaciones avanzadas mientras el gráfico Gantt se encuentra en modo de edición. Solo puede realizar ediciones en línea mientras el gráfico Gantt de la lista de tareas está en modo de edición.

Antes, se podía acceder al cuadro de diálogo Asignaciones avanzadas mientras el gráfico Gantt estaba en modo de edición, pero los cambios realizados se guardaban en el gráfico Gantt y ello cerraba el modo de edición.

Para obtener más información sobre la edición del gráfico Gantt de una lista de tareas, consulte “Actualización de información en el gráfico Gantt de lista de tareas”.

## Exportar registros de auditoría {#export-audit-logs}

Ahora puede exportar entradas del registro de auditoría a un archivo CSV. Puede exportar hasta 50 000 entradas de registro de auditoría a un archivo CSV al mismo tiempo.

Para obtener más información, consulte “Administración de registros de auditoría”.
