---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Información general de la sección Actualizaciones
description: La sección Actualizaciones de un objeto muestra los comentarios que los usuarios realizan sobre el objeto o las actualizaciones del sistema que realizan un seguimiento de los cambios en el objeto.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 5b9ee4d5d792d78f127f88bac3a0e4fea5cdf788
workflow-type: tm+mt
source-wordcount: '1174'
ht-degree: 4%

---

# Información general de la sección Actualizaciones

<!--take "Beta" references out when we remove the beta-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>\
<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">Para obtener más información sobre la programación actual de versiones, consulte [Resumen de la versión del cuarto trimestre de 2023](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>Actualmente estamos rediseñando la experiencia de comentarios en Adobe Workfront.
>
>Según el entorno y los objetos desde los que acceda a la experiencia de comentario, es posible que vea diferentes funcionalidades en la sección Actualizaciones.
>
>Para obtener más información sobre la nueva experiencia de comentarios y su disponibilidad, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>La nueva experiencia de comentarios solo está disponible para la sección Actualizaciones y no para las áreas siguientes:
>
> * Página de inicio
> * Panel de resumen en listas
> * Panel de resumen en plantillas de horas

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old note, removed with August 2023: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the new commenting experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

The Updates section of an object displays comments that users make on the object or system updates that track changes to the object.

-->

## Información general de la sección Actualizaciones

* La sección Actualizaciones de un objeto muestra hasta 200 de las actualizaciones más recientes realizadas en los últimos 90 días.

  ![](assets/updates-tab-before-unified-experience-for-issues.png)

* La sección Actualizaciones se muestra para los siguientes objetos:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td> 
      <ul> 
      <li>Documentos</li> 
      <li>Metas</li> 
      <li>Problemas</li> 
      <li>Iteraciones</li> 
      <li>Proyectos</li> 
      <li>Programas</li> 
      <li>Portafolios</li> 
      </ul> </td> 
    <td> 
      <ul> 
      <li>Historias*</li> 
      <li>Tareas</li> 
      <li>Plantillas</li> 
      <li>Tareas de plantilla</li> 
      <li>Plantillas de horas</li> 
      <li>Usuarios</li>
      <li>Tarjetas en un tablero</li>
      </ul> </td> 
    </tr> 
  </tbody> 
  </table>

  *Las historias son tareas. Toda la información relacionada con las tareas también está disponible para las historias.

La información de la sección Actualizaciones está organizada de forma diferente, según el entorno desde el que acceda a ella.


### Información general de la sección Actualizaciones actuales

<!--October 26 - replace current with legacy-->

* La sección Actualizaciones actuales muestra la siguiente información:

   * **Actualizaciones de usuarios**: Comentarios de los usuarios y respuestas a dichos comentarios.
   * **Actualizaciones del sistema**: mensajes informativos que Workfront crea para registrar ciertos eventos en un objeto. Por ejemplo, puede capturar los cambios de estado, nombre o campos personalizados con actualizaciones del sistema. El administrador del grupo o de Workfront puede habilitar las actualizaciones del sistema para los objetos. Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Los objetos siguientes no registran las actualizaciones del sistema:

   * Equipo
   * Plantilla
   * Tarea de plantilla

### Información general sobre la sección Actualizaciones en la nueva experiencia de comentarios

Para obtener información sobre las funciones disponibles para la nueva experiencia de comentarios y los objetos, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--update screen shot and maybe save it under a new name??? with the August 17 release - also make sure you have some people tagged, similar to what we show in the old UI-->

<span class="preview">![](assets/updates-tab-after-unified-experience-for-tasks.png)</span>

* La sección Actualizaciones muestra información en las siguientes pestañas de la nueva experiencia de comentarios:

   * **Comentarios**: muestra los comentarios realizados por los usuarios y las respuestas a dichos comentarios. Para obtener información sobre la actualización de objetos en la nueva experiencia de comentarios, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).
   * **Actividad del sistema**: Muestra actualizaciones del sistema que son mensajes informativos que Workfront crea para registrar ciertos eventos en un objeto. Por ejemplo, puede capturar los cambios de estado, nombre o campos personalizados con actualizaciones del sistema. El administrador del grupo o de Workfront puede habilitar las actualizaciones del sistema para los objetos. Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--enable this when we release the new update stream to ALL other objects and only if Anna's bug was fixed to include this - on or before October 2023: 

  * The following objects don't have a System Activity tab:

  * Team
  * Template
  * Template Task
    -->

* Actualmente, puede agregar comentarios y responder a actualizaciones utilizando la nueva experiencia de comentarios en los siguientes objetos:


   * Proyectos
   * Tareas (e historias)
   * Problemas
   * Documentos
   * Metas

  >[!NOTE]
  >
  >Debe tener una licencia adicional para acceder a los objetivos de Workfront. Para obtener más información, consulte [Requisitos para utilizar Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * Tarjetas en un tablero

  >[!NOTE]
  >
  > Puede agregar y ver actualizaciones a las tarjetas en el área de Tableros al habilitar las secciones Comentarios y Actividad del sistema en una tarjeta. Para obtener más información, consulte [Añadir una tarjeta ad hoc a un tablero](../../agile/get-started-with-boards/add-card-to-board.md).


  <span class="preview">

   * Plantillas
   * Tareas de plantilla
   * Plantillas de horas
   * Usuarios
   * Portafolios
   * Programas

  >[!NOTE]
  >
  >    No puede mostrar la nueva experiencia de comentarios para iteraciones.

  </span>

<!--hidden in August 2023 and replaced by the list above: 

  <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
      <tr> 
      <td> 
        <ul> 
        <li><p>Goals</p>
        <li>Cards in the Boards area*</li>
          This is the only experience for goals and cards.
        </li> 
        <li>Projects</li>
        </ul> </td> 
      <td> 
        <ul> 
        <li>Issues</li> 
        <li>Tasks</li>
        <li>Documents</li>
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

  *You can add and view updates to cards in the Board areas when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md). 
  -->



## Actualizaciones que también aparecen en objetos de mayor clasificación

Los comentarios o las respuestas realizados a las actualizaciones sobre determinados objetos también aparecen en la sección Actualizaciones de los objetos de mayor clasificación.

Por ejemplo, cuando se agrega una actualización a una tarea, la actualización aparece en la sección Actualizaciones de la tarea y en la sección Actualizaciones del proyecto que contiene la tarea.

>[!NOTE]
>
>Al habilitar la nueva experiencia de comentarios, los comentarios se muestran en los siguientes objetos de mayor clasificación:
>
>* Problemas
>* Proyectos
>* Tareas
>
>Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

En la tabla siguiente se muestran los objetos cuyos comentarios también aparecen en los objetos de mayor clasificación:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objeto en el que se añadió la actualización original</strong> </th> 
   <th> <p><strong>Objeto de mayor clasificación donde también aparece la actualización original</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Problema</td> 
   <td>Proyecto</td> 
  </tr> 
  <tr> 
   <td>Tarea</td> 
   <td>Proyecto</td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Programa, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Documento </td> 
   <td>Objeto donde se adjunta el documento, proyecto </td> 
  </tr> 
  <tr> 
   <td>Programar</td> 
   <td>Portafolio</td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td>Equipo</td> 
  </tr> 
  <tr> 
   <td>Hoja de horas</td> 
   <td>Usuario, equipo</td> 
  </tr> 
  <tr> 
   <td>Tarea de plantilla</td> 
   <td>Plantilla</td> 
  </tr> 
  <tr> 
   <td>Historia</td> 
   <td>Iteración, equipo</td> 
  </tr> 
  <tr> 
   <td>Iteración</td> 
   <td>Equipo</td> 
  </tr>

<tr> 
   <td>Metas</td> 
   <td>Resultado, actividad</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Las respuestas agregadas a las actualizaciones del sistema no se acumulan en el objeto principal. Solo las respuestas directas sobre un objeto secundario y las respuestas agregadas a actualizaciones existentes se acumulan en objetos principales.
>
>Para obtener información sobre la jerarquía de objetos en Adobe Workfront, consulte [Explicación de los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> No es posible responder a las actualizaciones del sistema en la nueva experiencia de comentarios. Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

## Limitaciones de la sección Actualizaciones

Existen algunas limitaciones en la sección Actualizaciones de un equipo y al introducir actualizaciones en nombre de otros usuarios.

### Limitaciones para usuarios y equipos

No puede agregar nuevos comentarios en la sección Actualizaciones de un equipo.

<span class="preview">Puede agregar una respuesta a una actualización que vea en un equipo. La respuesta se muestra en la sección Actualizaciones del equipo, así como en la sección Actualizaciones del objeto al que pertenece. </span>

La sección Actualizaciones para equipos se rellena con actualizaciones introducidas en los siguientes objetos:

* Usuarios
* Plantillas de horas
* Historias
* Iteraciones

En la sección Actualizaciones para usuarios y equipos, puede ver las actualizaciones introducidas en los últimos 90 días.

Si desea ver todas las actualizaciones realizadas en un usuario o equipo, más allá del límite de 90 días, puede crear un informe para notas. El informe no debe tener un filtro de tiempo que muestre todas las actualizaciones realizadas para usuarios o equipos. Para obtener más información, consulte [Creación de un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitaciones al introducir comentarios en nombre de otro usuario

Los administradores de Adobe Workfront y de grupos pueden iniciar sesión como otros usuarios y realizar acciones en Workfront, como introducir comentarios.

Para obtener más información, consulte [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Cualquier comentario hecho en nombre de otro usuario se indica en el comentario.

<!--might need to update this note when the new commenting experience will be the only experience; also - how will this affect the areas that will keep the old experience, like Iterations?-->

>[!NOTE]
>
>Al utilizar la nueva experiencia de comentarios, el comentario se agrega como el usuario que ha iniciado sesión como otro usuario y no hay indicación de que esté agregando un comentario en nombre de otra persona.
>
>Por ejemplo, si un administrador de Workfront inicia sesión como otro usuario, el usuario asociado con el comentario es el administrador de Workfront. Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


Un administrador de grupo puede realizar comentarios en nombre de otra persona, pero no puede eliminar ese comentario. Solo un administrador de Adobe Workfront puede eliminar un comentario que haya realizado en nombre de otro usuario.

## Ver actualizaciones del sistema en elementos de trabajo con el informe Entrada de diario

El informe Entrada de cuaderno muestra las actualizaciones del sistema desde el área Actualizaciones de proyectos, tareas y problemas.

El informe permite ver lo siguiente:

* Cuántos cambios de estado se han producido
* Cuando se eliminó una tarea o un problema
* Cómo cambiaron los valores de los campos personalizados importantes durante el transcurso de un proyecto
* Qué fechas importantes cambiaron durante el transcurso de un proyecto
* Si la prioridad ha cambiado durante el transcurso de un proyecto
* Si el propietario de un proyecto ha cambiado

Para obtener más información, consulte [Informe sobre el área de Actualizaciones](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
