---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Información general de la sección Actualizaciones
description: La sección Actualizaciones de un objeto muestra los comentarios que los usuarios realizan sobre el objeto o las actualizaciones del sistema que realizan un seguimiento de los cambios en el objeto.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 7bef757c24adc7791cb3b258ae6c33f3c0eec818
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 3%

---


# Información general de la sección Actualizaciones

<!-- Audited: 1/2024 -->

<!--take "legacy" and "new commenting" and "production" or "preview" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->


<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en Producción para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la programación actual de versiones, consulte [Información general sobre la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

>[!IMPORTANT]
>
>Actualmente estamos rediseñando la experiencia de comentarios en Adobe Workfront.
>
>Según los objetos para los que acceda a la experiencia de comentarios, es posible que vea la siguiente funcionalidad para la sección Actualizaciones:
>* La nueva experiencia
>* La experiencia heredada
>* La nueva experiencia y la experiencia heredada
>
>Para obtener más información sobre la nueva experiencia de comentarios y su disponibilidad, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
><Span class="preview"> La experiencia de comentarios heredada se ha eliminado de proyectos, tareas, problemas y documentos en el entorno de vista previa. </span>
>
>La nueva experiencia de comentarios solo está disponible para la sección Actualizaciones de los objetos de Workfront y no está disponible al acceder a las actualizaciones desde las áreas siguientes:
>
> * Inicio
> * Panel de resumen en listas
> * Panel de resumen en plantillas de horas
> * Panel de resumen en el Distribuidor de cargas de trabajo
>
><span class="preview">La nueva experiencia de comentarios está disponible en el panel Resumen en listas, plantillas de horas y el Distribuidor de cargas de trabajo en el entorno de vista previa y en el entorno de producción para los clientes que han elegido el proceso de versión rápido.
















## Información general de la sección Actualizaciones

La sección Actualizaciones de un objeto muestra las actualizaciones del sistema y hasta 200 de las actualizaciones más recientes realizadas por los usuarios en los últimos 90 días.

<div class="preview">

![Actualiza la sección](assets/updates-tab-with-unified-experience-for-issues-all-tab.png)

</div>

En función de los objetos para los que acceda a la experiencia de comentarios, es posible que encuentre la siguiente experiencia en la sección Actualizaciones:

* Experiencia de comentarios nueva y heredada para los siguientes objetos:

   * Proyecto
   * Tarea (incluye Historias)
   * Problema
   * Documento

     >[!TIP]
     >
     >Utilice la opción Nuevos comentarios para mostrar la nueva experiencia de comentarios (cuando la active) o la experiencia de comentarios heredada (cuando la desactive). La nueva experiencia de comentarios es la predeterminada. Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Solo la nueva experiencia de comentarios para los objetos enumerados a continuación. No hay opción para habilitar la experiencia de comentarios heredada para estos objetos:

   * Meta

     >[!NOTE]
     >
     >Debe tener una licencia adicional de Adobe Workfront Goals para poder acceder a esta área de Workfront. Para obtener más información, consulte [Requisitos para utilizar Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * Tarjeta en un tablero
   * Equipo
   * Plantilla
   * Tarea de plantilla
   * Hoja de horas
   * Programar
   * Portafolio
   * Usuario

* Solo la experiencia de comentarios heredada para los siguientes objetos:

   * Iteraciones

     No hay opción de habilitar la nueva experiencia de comentarios para iteraciones. Para obtener más información, consulte [Administrar comentarios de iteración](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md).

### Información general sobre la sección Actualizaciones en la nueva experiencia de comentarios

<div class="preview">

![Actualiza la sección](assets/updates-tab-after-unified-experience-for-tasks-all-tab.png)

</div>

>[!NOTE]
>
>La nueva experiencia de comentarios no está disponible para iteraciones.

* La sección Actualizaciones muestra información en las siguientes pestañas de la nueva experiencia de comentarios:

   * **Comentarios**: muestra los comentarios realizados por los usuarios y las respuestas a dichos comentarios. Utilice la ficha Comentarios para agregar nuevos comentarios o responder a los existentes. Para obtener información sobre la actualización de objetos en la nueva experiencia de comentarios, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).
   * **Actividad del sistema**: Muestra actualizaciones del sistema que son mensajes informativos que Workfront crea para registrar ciertos eventos en un objeto. Por ejemplo, los cambios de estado, nombre o campos personalizados se capturan con las actualizaciones del sistema. El administrador del grupo o de Workfront puede habilitar las actualizaciones del sistema para los objetos. <span class="preview">Cualquier respuesta realizada a los registros de actividad del sistema en la experiencia de comentarios heredada se rellena en la pestaña Actividad del sistema como de solo lectura.</span> Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).
   * <span class="preview">**Todo (solo lectura)**: muestra tanto los comentarios del usuario como los de la actividad del sistema en un solo lugar. Esta es una pestaña de solo vista. No puede responder a comentarios ni etiquetar a otros usuarios en comentarios existentes en la pestaña Todos. Para responder a un comentario específico, utilice el vínculo de la pestaña Todos a la pestaña Comentarios. Para obtener información sobre la actualización de objetos en la nueva experiencia de comentarios, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).</span>

* Los objetos siguientes no tienen una ficha Actividad del sistema <span class="preview">o una pestaña Todos:</span>

   * Equipo
   * Plantilla
   * Tarea de plantilla
   * Tarjeta ad hoc

* Los objetos siguientes no tienen un <span class="preview">Pestaña Todos:</span>

   * Metas


### Información general sobre la sección Actualizaciones heredadas

<!--when we remove legacy, make this section an "Iterations-only" section-->

![](assets/updates-tab-before-unified-experience-for-tasks.png)

La sección Actualizaciones heredadas muestra la siguiente información:

* **Actualizaciones de usuarios**: Comentarios de los usuarios y respuestas a dichos comentarios.
* **Actualizaciones del sistema**: mensajes informativos que Workfront crea para registrar ciertos eventos en un objeto. Por ejemplo, puede capturar los cambios de estado, nombre o campos personalizados con actualizaciones del sistema. El administrador del grupo o de Workfront puede habilitar las actualizaciones del sistema para los objetos. Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Los objetos siguientes no registran las actualizaciones del sistema:

* Equipo
* Plantilla
* Tarea de plantilla
* Iteraciones


## Actualizaciones que también aparecen en objetos de mayor clasificación

Los comentarios, las respuestas o las actualizaciones del sistema de ciertos objetos también aparecen en la sección Actualizaciones de los objetos de mayor clasificación.

Por ejemplo, cuando se agrega una actualización a una tarea, la actualización aparece en la sección Actualizaciones de la tarea y en la sección Actualizaciones del proyecto que contiene la tarea.

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
   <td><p>Usuario, equipo</p>
   <p><b>NOTA</b></p>
   <p>Los comentarios de la plantilla de horas se muestran en la sección Actualizaciones del usuario que realiza el comentario y en la sección Actualizaciones de su equipo de inicio.</p>
   </td> 
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
   <td>Resultado</td> 
   <td>Meta</td> 
  </tr> 
  <tr> 
   <td>Actividad</td> 
   <td>Meta</td> 
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

Tenga en cuenta lo siguiente al ver las actualizaciones para usuarios y equipos:

* No puede agregar nuevos comentarios en la sección Actualizaciones de un equipo.

* Puede agregar una respuesta a una actualización que vea en un equipo. La respuesta se muestra en la sección Actualizaciones del equipo, así como en la sección Actualizaciones del objeto al que pertenece.

* La sección Actualizaciones para equipos se rellena con actualizaciones introducidas en los siguientes objetos:

   * Usuarios
   * Hojas de horas*
   * Historias
   * Iteraciones*

  * No están disponibles para la nueva experiencia de comentarios.

* En la sección Actualizaciones para usuarios y equipos, puede ver las actualizaciones introducidas en los últimos 90 días.

  Si desea ver todas las actualizaciones realizadas en un usuario o equipo, más allá del límite de 90 días, puede crear un informe para notas. El informe no debe tener un filtro de tiempo que muestre todas las actualizaciones realizadas para usuarios o equipos. Para obtener más información, consulte [Creación de un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitaciones al introducir comentarios en nombre de otro usuario

Los administradores de Adobe Workfront y de grupos pueden iniciar sesión como otros usuarios y realizar acciones en Workfront, como introducir comentarios.

Para obtener más información, consulte [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Tenga en cuenta lo siguiente al iniciar sesión como otro usuario y agregar comentarios:

* Cualquier comentario hecho en nombre de otro usuario se indica en el comentario.

* Un administrador de grupo puede realizar comentarios en nombre de otra persona, pero no puede eliminar ese comentario. Solo un administrador de Adobe Workfront puede eliminar un comentario que haya realizado en nombre de otro usuario.

* Un administrador de grupo o Workfront solo puede editar un comentario que haya agregado en nombre de otro usuario cuando cierra la sesión como usuario y vuelve a iniciarla como si fuera él mismo. No pueden eliminar un comentario en nombre de otro usuario.

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
