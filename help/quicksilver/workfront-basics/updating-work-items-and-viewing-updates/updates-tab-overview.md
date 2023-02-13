---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Información general de la ficha Actualizaciones
description: La pestaña Actualizaciones muestra hasta 200 de las actualizaciones más recientes realizadas en los últimos 90 días.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 799a2f3463ee98d57b13edfda8a0c93629439ea3
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 6%

---

# Información general de la ficha Actualizaciones

La pestaña Actualizaciones muestra hasta 200 de las actualizaciones más recientes realizadas en los últimos 90 días. Puede responder a las actualizaciones de los siguientes objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Proyectos</li> 
     <li>Portafolios</li> 
     <li>Programas</li> 
     <li>Plantillas</li> 
     <li>Tareas de plantilla</li> 
     <li>Tareas</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Problemas</li> 
     <li>Iteraciones</li> 
     <li>Historias</li> 
     <li>Usuarios</li> 
     <li>Documentos</li> 
     <li>Plantillas de horas</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizaciones que también aparecen en objetos de mayor rango

Como se muestra en la tabla siguiente, las respuestas a las actualizaciones de ciertos objetos también aparecen en la ficha Actualizaciones de los objetos de mayor clasificación.

Por ejemplo, cuando agrega una actualización a una tarea, la actualización aparece en la ficha Actualizaciones de la tarea y en la ficha Actualizaciones del proyecto que la contiene.

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
 </tbody> 
</table>

>[!NOTE]
>
>Las respuestas agregadas a las actualizaciones del sistema no se resumen en el objeto principal. Solo las respuestas directas en un objeto secundario y las respuestas agregadas a actualizaciones existentes se resumen en los objetos principales.

Para obtener información sobre la jerarquía de objetos en Adobe Workfront, consulte [Explicación de los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Limitaciones de la pestaña Actualizaciones

### Limitaciones para usuarios y equipos

No puede realizar actualizaciones en los equipos. La ficha Actualizaciones de los equipos se rellena con actualizaciones introducidas en los siguientes objetos:

* Usuarios
* Plantillas de horas
* Historias
* Iteraciones

En la ficha Actualizaciones para usuarios y equipos, puede ver las actualizaciones introducidas en los últimos 90 días.

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
