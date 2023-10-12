---
title: Resumen de límites del proyecto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront tiene límites en cuanto a la cantidad de objetos que pueden asociarse a un proyecto. Existen límites de proyecto para mejorar el rendimiento del producto y la experiencia con Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Resumen de límites del proyecto

Adobe Workfront tiene límites en cuanto a la cantidad de objetos que pueden asociarse a un proyecto. Existen límites de proyecto para mejorar el rendimiento del producto y la experiencia con Workfront.

Los siguientes objetos asociados a proyectos tienen los límites siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tareas</p></td> 
   <td>  <p>El número máximo de tareas por proyecto es de 5000. Aparece un mensaje de advertencia cuando el número de tareas se acerca a este máximo. Cuando se alcanza el máximo, aparece un mensaje de error y no se pueden agregar tareas adicionales al proyecto.</p> <p>Para evitar alcanzar este máximo, mueva las tareas que estén cerradas a otro proyecto designado para tareas cerradas. Es posible que haya que ajustar los informes sobre estos proyectos.</p>

<b>IMPORTANTE</b>

En los proyectos en los que las tareas tienen muchas dependencias, puede producirse una degradación del rendimiento al calcular la escala de tiempo o al trabajar en el proyecto.

Por este motivo, recomendamos que el número de tareas en proyectos con dependencias complejas sea mucho menor que el máximo permitido de 5000 tareas.

Algunos ejemplos de dependencias entre tareas que podrían influir o impedir que se recalcule la escala de tiempo del proyecto son los siguientes:

<ul><li>Número de elementos secundarios</li>
   <li>Múltiples niveles de sangría de tarea</li>
   <li>Número de predecesoras</li>
   <li>Múltiples asignaciones</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemas</p></td> 
   <td>  <p>El número máximo de problemas por proyecto es de 10 000. Aparece un mensaje de advertencia cuando el número de problemas se acerca a este máximo. Cuando se alcanza el máximo, aparece un mensaje de error y no se pueden agregar problemas adicionales al proyecto.</p> <p>Para evitar alcanzar este máximo, mueva los problemas que estén cerrados a otro proyecto designado para problemas cerrados. Es posible que haya que ajustar los informes sobre estos proyectos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Duraciones</p></td> 
   <td> <p>La duración máxima de un proyecto debe ser de 15 años para que Workfront calcule automáticamente su cronología. Aparece un mensaje de advertencia cuando la duración del proyecto se acerca al máximo. Cuando se alcanza el máximo, aparece un mensaje de advertencia y ya no se producen los cálculos automáticos de la cronología.</p> <p>Los cálculos automáticos del calendario se reanudarán tan pronto como la duración de un proyecto se reduzca por debajo de los 15 años, ajustando las fechas de las tareas del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Cálculos de cronología</p></td> 
   <td>Workfront no realiza cálculos de escala de tiempo automáticos para proyectos que no se hayan actualizado en seis meses y no se reanudarán hasta que se realice una actualización.<p>En el caso de los proyectos que no se hayan actualizado en tres meses, Workfront realiza cálculos de escala de tiempo semanalmente en lugar de cada noche.</p><p>Para obtener información sobre el cálculo de la escala de tiempo del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular escalas de tiempo del proyecto</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->