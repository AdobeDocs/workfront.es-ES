---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Información general sobre la sección Actualizaciones
description: La sección Actualizaciones muestra hasta 200 de las actualizaciones más recientes realizadas en los últimos 90 días.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# Información general sobre la sección Actualizaciones

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

La sección Actualizaciones de un objeto muestra los comentarios que los usuarios hacen en las actualizaciones de objeto o del sistema que realizan un seguimiento de los cambios en el objeto.

## Información general sobre la sección Actualizaciones

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

La sección Actualizaciones de un objeto muestra hasta 200 de las actualizaciones más recientes realizadas en los últimos 90 días.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

La sección Actualizaciones muestra la siguiente información:

* Observaciones de los usuarios y respuestas a esas observaciones.
* Actualizaciones del sistema que son mensajes informativos que Workfront crea para registrar ciertos eventos en un objeto. Por ejemplo, puede capturar los cambios de estado, nombre o campos personalizados con actualizaciones del sistema. El administrador de Workfront o de grupos puede habilitar las actualizaciones del sistema para los objetos. Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

La sección Actualizaciones se muestra para los siguientes objetos:

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
     <li>Historias</li> 
     <li>Tareas</li> 
     <li>Plantillas</li> 
     <li>Tareas de plantilla</li> 
     <li>Plantillas de horas</li> 
     <li>Usuarios</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## Actualizaciones que también aparecen en objetos de mayor rango

Como se muestra en la tabla siguiente, las respuestas a las actualizaciones de ciertos objetos también aparecen en la sección Actualizaciones de los objetos de mayor clasificación.

Por ejemplo, cuando agrega una actualización a una tarea, la actualización aparece en la sección Actualizaciones de la tarea y en la sección Actualizaciones del proyecto que contiene la tarea.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objeto donde se agregó la actualización original</strong> </th> 
   <th> <p><strong>Objeto de clasificación superior donde también aparece la actualización original</strong> </p> </th> 
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
   <td>Objeto al que se adjunta el documento, Proyecto </td> 
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
>Las respuestas agregadas a las actualizaciones del sistema no se resumen en el objeto principal. Solo las respuestas directas en un objeto secundario y las respuestas agregadas a actualizaciones existentes se resumen en los objetos principales.
>
>Para obtener información sobre la jerarquía de objetos en Adobe Workfront, consulte [Explicación de los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Limitaciones de la sección Actualizaciones

### Limitaciones para usuarios y equipos

No puede realizar actualizaciones en los equipos. La sección Actualizaciones de los equipos se rellena con actualizaciones introducidas en los siguientes objetos:

* Usuarios
* Plantillas de horas
* Historias
* Iteraciones

En la sección Actualizaciones para usuarios y equipos, puede ver las actualizaciones introducidas en los últimos 90 días.

Si desea ver todas las actualizaciones realizadas en un usuario o equipo, más allá del límite de 90 días, puede crear un informe para las notas. El informe no debe tener un filtro de tiempo que muestre todas las actualizaciones realizadas para usuarios o equipos. Para obtener más información, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitaciones al introducir comentarios en nombre de otro usuario

Los administradores de Adobe Workfront y los administradores de grupos pueden iniciar sesión como otros usuarios y realizar acciones en Workfront, como introducir comentarios. (Para obtener más información, consulte [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Cualquier comentario realizado en nombre de otro usuario se indica en el comentario.

Un administrador de grupo puede realizar comentarios en nombre de otra persona, pero no puede eliminarlos. Solo los administradores de Adobe Workfront pueden eliminar un comentario que hayan realizado en nombre de otro usuario.

## Ver actualizaciones del sistema de elementos de trabajo con el informe Entrada de diario

El informe Entrada de diario muestra las actualizaciones del sistema desde el área Actualizaciones de proyectos, tareas y problemas.

El informe permite ver:

* Cuántos cambios de estado se han producido
* Cuando se elimina una tarea o un problema
* Cambio de los valores de campos personalizados importantes durante el curso de un proyecto
* Qué fechas importantes han cambiado durante el curso de un proyecto
* Si la prioridad ha cambiado durante el curso de un proyecto
* Si el propietario de un proyecto ha cambiado

Para obtener más información, consulte [Informe del área Actualizaciones](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
