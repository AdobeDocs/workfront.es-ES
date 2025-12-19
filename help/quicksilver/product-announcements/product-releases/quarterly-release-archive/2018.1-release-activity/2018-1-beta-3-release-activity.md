---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión Beta 3 2018.1
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión Beta 3 2018.1. La funcionalidad estaba disponible en el entorno de vista previa el 7 de enero de 2018. Estará disponible en el entorno de producción a principios de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 88%

---

# Actividad de la versión Beta 3 2018.1

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión Beta 3 2018.1. La funcionalidad estaba disponible en el entorno de vista previa el 7 de enero de 2018. Estará disponible en el entorno de producción a principios de 2018.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en 2018.1, consulte [Información general sobre la actividad de la versión 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versión 2018.1 de Beta 3 contiene mejoras tanto para administradores de Workfront como para otros usuarios:

**Para los administradores**

* [Mejoras para administradores de grupos](#group-administrator-improvements)

**Para todos los usuarios**

* [Mejoras en el visor de revisión de HTML5](#html5-proofing-viewer-improvements)
* [Mejoras de revisión en Workfront](#proofing-improvements-within-workfront)
* [Mejoras en el área de inicio](#home-area-improvements) 
* [Mejoras de Agile](#agile-improvements)
* [Mejoras en el gráfico Gantt](#gantt-chart-improvements)
* [Configuración de Planificador de recursos](#resource-planner-improvements)

## Mejoras para administradores de grupos {#group-administrator-improvements}

* [Se ha actualizado la IU para restablecer la contraseña para los administradores del grupo](#reset-password-ui-updated-for-group-administrators)
* [Opciones de configuración de nivel de acceso para administradores de grupo](#access-level-setup-options-for-group-administrators)
* [Crear perfiles de plantilla de horas para grupos](#create-timesheet-profiles-for-groups)
* [Recuperar elementos eliminados para usuarios como administrador de grupos](#recover-deleted-items-for-users-as-a-group-administrator)

### Se ha actualizado la interfaz de usuario de restablecer contraseña para administradores de grupos {#reset-password-ui-updated-for-group-administrators}

Como administrador de grupos, cuando restablece la contraseña de otro usuario, se le pide su propia contraseña antes de poder cambiar la suya. La interfaz de usuario de se ha actualizado para reflejar esta funcionalidad. Antes de este cambio, la interfaz de usuario mostraba que se requería la contraseña del administrador de Workfront.

Para obtener más información sobre cómo restablecer contraseñas para otros usuarios, consulte [Editar el perfil de un usuario](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Para obtener más información sobre las capacidades de un administrador de grupo, consulte la sección &quot;Capacidades de los administradores de grupo&quot; en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Opciones de configuración de nivel de acceso para administradores de grupos {#access-level-setup-options-for-group-administrators}

Como administrador de Workfront, ahora puede controlar si los administradores de grupos pueden iniciar sesión como otros usuarios o si pueden restablecer las contraseñas de otros usuarios. Se ha añadido una nueva configuración en el nivel de acceso para habilitar o deshabilitar este acceso. Antes de este cambio, todos los administradores de grupos podían iniciar sesión como otros usuarios y restablecer las contraseñas de otros usuarios de forma predeterminada. Este cambio afecta solamente el nivel de acceso del planificador.

Para obtener más información acerca de cómo configurar el nivel de acceso de los usuarios, vea [Conceder acceso a los usuarios](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Para obtener más información sobre las capacidades de un administrador de grupo, consulte la sección &quot;Capacidades de los administradores de grupo&quot; en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Crear perfiles de plantillas de horas para grupos {#create-timesheet-profiles-for-groups}

Como administrador de grupos, ahora puede crear perfiles de plantilla de horas para los grupos que administre y asociarlos a los grupos que administre o a los usuarios de estos grupos. Los perfiles de plantillas de horas garantizan que las hojas de horas se creen automáticamente para los usuarios asociados a ellas.

Antes de este cambio, solamente un administrador de Workfront podía crear perfiles de plantillas de horas.

Para obtener más información sobre cómo crear perfiles de plantillas de horas, consulte [Crear, editar y asignar perfiles de plantillas de horas](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Para obtener más información sobre las capacidades de un administrador de grupo, consulte la sección &quot;Capacidades de los administradores de grupo&quot; en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Recuperar elementos eliminados para usuarios como administrador de grupos {#recover-deleted-items-for-users-as-a-group-administrator}

Si un proyecto está asociado a un grupo del que usted es administrador del grupo, puede recuperar el proyecto o cualquiera de sus tareas, problemas o documentos eliminados de la papelera de reciclaje. Antes de este cambio, solo un administrador de Workfront podía recuperar elementos de la papelera de reciclaje.

Para obtener más información acerca de cómo recuperar elementos eliminados en Workfront, vea [Restaurar elementos eliminados](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obtener más información sobre las capacidades de un administrador de grupo, consulte la sección &quot;Capacidades de los administradores de grupo&quot; en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## Mejoras del visor de revisión de HTML5  {#html5-proofing-viewer-improvements}

* [Modo de comparación](#compare-mode)
* [Filtrar la lista de comentarios](#filter-the-comment-list)
* [La lista de comentarios se busca después de introducir el primer carácter](#comment-list-is-searched-after-the-first-character-is-entered)

### Modo de comparación {#compare-mode}

Ahora puede utilizar el modo de comparación en el visor de corrección de HTML5 cuando visualice revisiones estáticas y de vídeo. 

El modo de comparación en el visor de corrección de HTML5 difiere del visor de corrección heredado en los siguientes aspectos:

* Al iniciar el modo de comparación, la versión más reciente se desplaza a la derecha, mientras que la versión que se está comparando se abre a la izquierda.

  Anteriormente, la versión más reciente se desplazaba a la izquierda, mientras que la versión que se estaba comparando se abría a la derecha.

* Puede elegir la versión de una revisión que quiera comparar directamente desde el visor de corrección. 
* El nivel de zoom y la posición actuales de las revisiones dentro del visor de corrección se mantienen al entrar en la navegación simultánea.
* Nueva opción Restablecer al utilizar la navegación simultánea.
* Al salir del modo de comparación, puede elegir la prueba que desea cerrar. 

  Anteriormente, la versión anterior siempre se cerraba.

* Varias mejoras en la apariencia y la facilidad de uso.

Para obtener más información, consulte [Comparar revisiones en el visor de corrección](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtrar la columna de comentarios {#filter-the-comment-list}

Ahora puede filtrar comentarios en la lista de comentarios. Puedes filtrar por usuario, acciones, no leídos, etc.

### La lista de comentarios se busca después de introducir el primer carácter {#comment-list-is-searched-after-the-first-character-is-entered}

Ahora, al buscar en la lista de comentarios, la lista se filtra automáticamente después de escribir el primer carácter.

Antes de este cambio, había que escribir al menos 3 caracteres en el campo de búsqueda antes de que se filtrara la lista de comentarios.

Para obtener más información, consulte.

## Mejoras de revisión en Workfront {#proofing-improvements-within-workfront}

* [Vincular pruebas de Workfront Proof a Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Ya no se puede quitar una prueba de un documento](#can-no-longer-remove-a-proof-from-a-document)
* [Apariencia actualizada al generar y abrir pruebas](#updated-look-and-feel-when-generating-and-opening-proofs)

### Vinculación de pruebas de Workfront Proof a Workfront {#link-proofs-from-workfront-proof-to-workfront}

Ahora puede vincular pruebas de documentos que ya existen en su cuenta de Workfront Proof a Workfront.

Antes de este cambio, no se podía acceder a las pruebas que ya existían en Workfront Proof en Workfront. 

Para obtener más información, consulte [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) en [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Ya no se puede quitar una prueba de un documento {#can-no-longer-remove-a-proof-from-a-document}

Ya no puede quitar una prueba de un documento. En su lugar, para eliminar una prueba, debe eliminar todo el documento.

Esta mejora reduce el riesgo de que los usuarios eliminen de forma involuntaria todas las versiones de un documento revisado. 

Para obtener información acerca de cómo eliminar un documento, consulte [Eliminar una prueba](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) en [Eliminar una prueba](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Apariencia actualizada al generar y abrir pruebas {#updated-look-and-feel-when-generating-and-opening-proofs}

Ahora hay una animación actualizada cuando se genera una prueba.

## Mejoras en el área de inicio {#home-area-improvements}

Se han realizado las siguientes mejoras en el área de inicio:

* [Ver aprobaciones de revisión desde el área de inicio](#view-proof-approvals-from-the-home-area)
* [Los campos predeterminados se muestran al configurar la plantilla de diseño para los elementos del área de inicio](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Ver aprobaciones de revisión desde el área de inicio {#view-proof-approvals-from-the-home-area}

Ahora puede ver las aprobaciones de revisión en el área de inicio, además de las aprobaciones estándar.

Anteriormente, se podían ver las aprobaciones de Workfront, pero no se podían ver las aprobaciones de una revisión.  

Para obtener más información, consulte [Usar el área de inicio](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Los campos predeterminados se muestran al configurar la plantilla de diseño para los elementos del área de inicio {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Anteriormente, los campos predeterminados no eran visibles desde la plantilla de diseño.

Para obtener más información, consulte “Creación y administración de plantillas de diseño”.

## Mejoras de Agile {#agile-improvements}

* [Añadir tareas y problemas a la iteración directamente desde la página Detalles de la tarea o problema](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Incluir problemas en el registro de asuntos pendientes y el tablero de historias de Scrum para un equipo Agile](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Aplicar agrupaciones y filtros al registro de asuntos pendientes para un equipo Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Crear una iteración en blanco y actualizarla más tarde](#create-a-blank-iteration-and-update-it-later)
* [Los campos “Enfoque” y “Capacidad” se rellenan previamente al crear una iteración](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Añadir tareas y problemas a la iteración directamente desde la página Detalles de la tarea o problema {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Ahora puede agregar tareas y problemas que actualmente están asignados a un equipo Agile a una iteración directamente desde la tarea o el problema.

Anteriormente, solo se podían añadir tareas a una iteración desde el registro de asuntos pendientes. 

Para obtener más información, consulte [Crear una iteración](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) en [Crear una iteración](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Incluir problemas en el registro de asuntos pendientes de Scrum y el tablero de historias para un equipo Agile {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Los problemas ahora se incluyen de forma predeterminada en el registro de asuntos pendientes de su equipo de Agile al utilizar la metodología Scrum Agile (los problemas no se muestran en el registro de asuntos pendientes de un equipo de Agile al utilizar la metodología Kanban).

Antes de este cambio, solo se podían agregar tareas al registro de pendientes. Si desea agregar un problema, primero tenía que convertirlo en una tarea antes de que se pudiera agregar.

Para obtener información sobre el uso de los problemas en el registro de pendientes, consulte  [Administrar el registro de pendientes de Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Aplicar agrupaciones y filtros al registro de pendientes para un equipo ágil {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Las opciones de Agrupación y Filtro ahora están disponibles en el registro de asuntos pendientes de Agile, lo que le permite organizar el registro de asuntos pendientes por agrupaciones, así como filtrar por tareas y problemas específicos.

Antes de este cambio, podía aplicar en las vistas al registro de asuntos pendientes de Agile.

Para obtener más información, consulte  [Administrar el registro de pendientes de Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) en  [Administrar el registro de pendientes de Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Crear una iteración en blanco y actualizarla más tarde {#create-a-blank-iteration-and-update-it-later}

Ya no es necesario añadir una tarea o un problema a una iteración para crearla. Puede crear una iteración en blanco y añadir tareas y problemas más adelante.

Para obtener más información, consulte [Crear una iteración](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Los campos “Enfoque” y “Capacidad” se rellenan previamente al crear una iteración {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Ahora, al crear una iteración, los campos &quot;Enfoque&quot; y &quot;Capacidad&quot; se rellenan previamente con los valores medios de todas las iteraciones anteriores que haya creado su equipo. Si su equipo no ha creado ninguna iteración anterior, estos campos aparecen como 0.

Anteriormente, estos campos siempre tenían el valor 0.

Para obtener más información, consulte [Crear una iteración](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Mejoras en el gráfico Gantt {#gantt-chart-improvements}

* [Habilitar el modo de edición en el gráfico Gantt](#enable-edit-mode-in-the-gantt-chart)
* [Quitar predecesoras al editar el gráfico Gantt](#remove-predecessors-when-editing-the-gantt-chart)

### Habilitar el modo de edición en el gráfico Gantt {#enable-edit-mode-in-the-gantt-chart}

Cuando se habilita el modo de edición en el gráfico Gantt, se pueden realizar cambios en la información dentro del gráfico. Antes de este cambio, no se podía editar la información en el gráfico Gantt. Solo se podía editar la información de la tarea en la lista de tareas.

Para obtener información acerca de la edición en el gráfico Gantt, consulte [Actualizar información en el gráfico Gantt de lista de tareas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Quitar predecesoras al editar el gráfico Gantt {#remove-predecessors-when-editing-the-gantt-chart}

Mediante el modo Editar del gráfico Gantt, ahora puede eliminar las relaciones de predecesoras entre las tareas del gráfico Gantt de un proyecto. Antes de esta mejora, se podía eliminar la relación de predecesoras sólo en la lista de tareas o en el nivel de tarea.

Para obtener información acerca de la edición en el gráfico Gantt, consulte [Actualizar información en el gráfico Gantt de lista de tareas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Configuración de Planificador de recursos {#resource-planner-improvements}

* [Presupuesto con duración cero en el Planificador de recursos](#budget-with-zero-duration-in-the-resource-planner)

* [Mostrar datos por coste en el Planificador de recursos](#show-data-by-cost-in-the-resource-planner)

### Presupuesto con duración cero en el Planificador de recursos {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Esta función se ha eliminado del entorno de vista previa y se lanzará con la versión 18.1.

Ahora puede presupuestar los recursos en el Planificador de recursos para cualquier fecha, dentro o fuera del lapso de tiempo del proyecto. Antes de esta mejora, podía presupuestar los recursos solo para las fechas dentro del lapso de tiempo del proyecto.

Para obtener más información sobre cómo presupuestar recursos en el Planificador de recursos, consulte la sección “Presupuestación de recursos en el Planificador de recursos” en [Información general del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Mostrar datos por coste en el Planificador de recursos {#show-data-by-cost-in-the-resource-planner}

Ahora puede mostrar la información en el Planificador de recursos por coste, además de los valores de Horas y FTE. Puede mostrar los costes en el Planificador de recursos cuando lo esté viendo en las vistas Vista por proyecto o Vista por función. No puede mostrar los costes cuando está viendo el Planificador de recursos en la vista Vista por usuario.

Para obtener más información sobre cómo ver el Planificador de recursos por valores de horas, FTC o costes, consulte [Información general de navegación del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
