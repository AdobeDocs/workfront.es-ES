---
title: Resumen de límites del proyecto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront tiene límites en cuanto a la cantidad de objetos que pueden asociarse a un proyecto. Existen límites de proyecto para mejorar el rendimiento del producto y la experiencia con Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/t6tfn132hAQe--u8g73CAFAfrJTf2qFi7yOhm4flP58
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 458
ht-degree: 1%

---

# Información general de los límites del proyecto

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
   <td>Workfront no realiza cálculos de escala de tiempo automáticos para proyectos que no se hayan actualizado en seis meses y no se reanudarán hasta que se realice una actualización.<p>En el caso de los proyectos que no se hayan actualizado en tres meses, Workfront realiza cálculos de escala de tiempo semanalmente en lugar de cada noche.</p><p>Para obtener información sobre cómo calcular la escala de tiempo del proyecto, vea <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular escala de tiempo del proyecto</a>. </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader"><p>Convertir objetos </p></td> 
   <td>Workfront tiene un límite de procesamiento de 5 minutos al convertir objetos. Si el objeto tiene un gran número de documentos adjuntos a él, es posible que no se convierta dentro del límite de 5 minutos. Es posible que tenga que eliminar algunos de los documentos e intentarlo de nuevo.</td> 
  </tr> 
 </tbody> 
</table>

<!--
 Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
