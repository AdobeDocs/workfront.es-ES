---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Información general sobre la sección Actualizaciones
description: La sección Actualizaciones de un objeto muestra los comentarios que los usuarios hacen en las actualizaciones de objeto o del sistema que realizan un seguimiento de los cambios en el objeto.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 25625291f691f7858634d9961fccb4465008dc3c
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 4%

---

# Información general sobre la sección Actualizaciones

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

>[!NOTE]
>
>Actualmente estamos rediseñando la experiencia de comentarios en Adobe Workfront.
>
>Para obtener más información sobre la nueva experiencia de comentarios, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Puede acceder a la nueva experiencia para los siguientes objetos:
> * Problemas, al activar el comentario Beta.
   >
   >     Esta funcionalidad solo está disponible para la sección Actualizaciones de los problemas y no está disponible para las siguientes áreas:
   >
   >     * Página de inicio
   >     * Panel Resumen en listas
   >     * Panel Resumen en hojas de horas
>
> * Metas

   >
   >   La nueva experiencia de comentarios es la predeterminada para los objetivos. Debe tener una licencia adicional para acceder a los objetivos de Workfront. Para obtener más información, consulte [Requisitos para utilizar los objetivos de Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    Para obtener información sobre cómo comentar objetivos, consulte [Administrar comentarios de objetivo en objetivos de Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).


La sección Actualizaciones de un objeto muestra los comentarios que los usuarios hacen en las actualizaciones de objeto o del sistema que realizan un seguimiento de los cambios en el objeto.

## Información general sobre la sección Actualizaciones

La información de la sección Actualizaciones está organizada de forma diferente, en función del entorno desde el que se acceda a ella.

### Información general sobre la sección Actualizaciones actuales

La sección Actualizaciones de un objeto muestra hasta 200 de las actualizaciones más recientes realizadas en los últimos 90 días.

![](assets/updates-tab-before-unified-experience-for-issues.png)

La sección Actualizaciones actuales muestra la siguiente información:

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

### Información general sobre la sección Actualizaciones de la experiencia de comentarios de la versión beta

![](assets/updates-tab-after-unified-experience-for-issues.png)

La sección Actualizaciones muestra información en las fichas siguientes de la nueva experiencia de comentarios:

* **Comentarios**: Muestra los comentarios realizados por los usuarios y las respuestas a esos comentarios. Para obtener información sobre la actualización de objetos en la nueva experiencia de comentarios, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).
* **Actividad del sistema**: Muestra las actualizaciones del sistema que son mensajes informativos que Workfront crea para registrar ciertos eventos en un objeto. Por ejemplo, puede capturar los cambios de estado, nombre o campos personalizados con actualizaciones del sistema. El administrador de Workfront o de grupos puede habilitar las actualizaciones del sistema para los objetos. Para obtener más información, consulte [Configurar actualizaciones del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Actualmente, puede realizar comentarios y responder a las actualizaciones mediante la experiencia de comentarios beta en los siguientes objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><p>Metas</p>
     <p>Esta es la experiencia predeterminada para los objetivos</p>
     </li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li>Problemas</li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

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
>
> No es posible responder a las actualizaciones del sistema en la nueva experiencia Beta de comentarios. Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

## Limitaciones de la sección Actualizaciones

Existen algunas limitaciones en la sección Actualizaciones de un equipo y al introducir actualizaciones en nombre de otros usuarios.

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
