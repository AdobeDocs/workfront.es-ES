---
title: Información general sobre los límites del proyecto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront tiene límites para la cantidad de objetos que se pueden asociar a un proyecto. Los límites del proyecto están establecidos para mejorar el rendimiento del producto y mejorar su experiencia con Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 809f1c3629c343a55305c0c617f4974dc05439bf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Información general sobre los límites del proyecto

Adobe Workfront tiene límites para la cantidad de objetos que se pueden asociar a un proyecto. Los límites del proyecto están establecidos para mejorar el rendimiento del producto y mejorar su experiencia con Workfront.

Los siguientes objetos asociados a proyectos tienen los límites siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tareas</p></td> 
   <td>  <p>El número máximo de tareas por proyecto es de 5.000. Aparece un mensaje de advertencia cuando el número de tareas se acerca a este máximo. Cuando se alcanza el máximo, aparece un mensaje de error y no se pueden agregar tareas adicionales al proyecto.</p> <p>Para evitar alcanzar este máximo, mueva las tareas que estén cerradas a otro proyecto designado para tareas cerradas. Puede que sea necesario ajustar los informes sobre estos proyectos.</p>

<b>IMPORTANTE</b>

Para los proyectos en los que las tareas tienen muchas dependencias, recomendamos que el número de tareas en los proyectos sea mucho menor que el máximo permitido de 5000 tareas.

Algunos ejemplos de dependencias de tareas que pueden influir o evitar volver a calcular la cronología del proyecto son:

<ul><li>Número de elementos secundarios</li>
   <li>Múltiples niveles de sangría de tareas</li>
   <li>Número de predecesores</li>
   <li>Múltiples asignaciones</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemas</p></td> 
   <td>  <p>El número máximo de problemas por proyecto es de 10.000. Aparece un mensaje de advertencia cuando el número de problemas se acerca a este máximo. Cuando se alcanza el máximo, aparece un mensaje de error y no se pueden agregar problemas adicionales al proyecto.</p> <p>Para evitar alcanzar este máximo, traslade los problemas que están cerrados a otro proyecto designado para problemas cerrados. Puede que sea necesario ajustar los informes sobre estos proyectos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Duraciones</p></td> 
   <td> <p>La duración máxima de un proyecto debe ser de 15 años para que Workfront calcule automáticamente su cronología. Aparece un mensaje de advertencia cuando la duración del proyecto se acerca al máximo. Cuando se alcanza el máximo, aparece un mensaje de advertencia y ya no se realizan los cálculos automáticos de la cronología.</p> <p>Los cálculos automáticos de la cronología se reanudarán en cuanto la duración de un proyecto se reduzca por debajo de 15 años ajustando las fechas de las tareas del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Cálculos de línea de tiempo</p></td> 
   <td>Workfront no realiza cálculos automáticos de cronología para proyectos que no se hayan actualizado en 6 meses y no se reanudarán hasta que se realice una actualización.<p>Para los proyectos que no se han actualizado en 3 meses, Workfront realiza cálculos de cronología semanalmente en lugar de por la noche.</p><p>Para obtener información sobre el cálculo de la cronología del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Volver a calcular las líneas de tiempo del proyecto</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->