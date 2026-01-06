---
title: Información general sobre la condición y el tipo de condición del proyecto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: La condición del proyecto es una representación visual del progreso del proyecto. Es una variable notificable determinada por la relación entre las fechas planificadas, proyectadas y estimadas del proyecto.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 100%

---

# Información general sobre la condición y el tipo de condición del proyecto

<!-- Audited: 12/2023 -->

La condición del proyecto es una representación visual del progreso del proyecto. Es una variable notificable determinada por la relación entre las fechas planificadas, proyectadas y estimadas del proyecto.

## Información general sobre la condición del proyecto

Tenga en cuenta lo siguiente para comprender la condición de un proyecto:

* Como propietario del proyecto, puede decidir si la condición de un proyecto se establece de forma manual o automática. La condición de un proyecto se puede establecer de las siguientes maneras:

   * De forma manual, por usuarios que tengan acceso a Administrar el proyecto y cuando el Tipo de condición del proyecto se establezca en Manual.
   * Automáticamente, por parte de Workfront, cuando el tipo de condición del proyecto se establece en Estado de progreso. El estado del progreso del proyecto viene determinado por el progreso de las tareas del proyecto. Para obtener información sobre el estado de progreso del proyecto, consulte [Información general sobre el estado de progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Para obtener información sobre cómo actualizar el tipo de condición del proyecto, consulte [Establecer el tipo de condición de un proyecto](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Al permitir que Workfront calcule la condición del proyecto automáticamente, le recomendamos que utilice predecesoras en las tareas para que el progreso de la tarea se refleje en el progreso real y en el estado de progreso del proyecto.
* Como propietario de un proyecto, puede cambiar el proyecto para que utilice un tipo de condición manual en lugar de utilizar el estado de progreso cambiando el tipo de condición de estado de progreso a manual.

  >[!NOTE]
  >
  >Los proyectos que se encuentran en cualquiera de los siguientes estados siempre se marcan como Bien encaminado, independientemente de las fechas de las tareas y de su progreso:
  >
  >* Idea
  >* Solicitud
  >* Aprobado
  >* Rechazado

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Cómo actualizar Workfront la condición del proyecto en función del estado de progreso

Cuando el tipo de condición del proyecto se establece en Manual, puede determinar cuál es la condición del proyecto de forma independiente del estado de progreso del proyecto.

No obstante, Workfront recomienda establecer el tipo de condición en Estado de progreso para que tenga una indicación clara del progreso real del proyecto, en función del progreso de las tareas. Para obtener información sobre cómo calcula Workfront el estado de progreso de los proyectos, consulte [Información general sobre el estado de progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

En este caso, la condición del proyecto puede ser la siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Condición del proyecto</strong></td> 
   <td><strong>Estado de progreso del proyecto</strong></td> 
   <td><strong>Indicador de condición de Workfront</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bien encaminado</td> 
   <td>Cuando el estado del progreso del proyecto sea A tiempo, la condición del proyecto será <strong>Bien encaminado</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>En riesgo</td> 
   <td>Cuando el estado del progreso del proyecto es <strong>Rezagado</strong> o <strong>En riesgo</strong>, la condición del proyecto es <strong>En riesgo</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Con problemas</td> 
   <td>Cuando el estado del progreso del proyecto es <strong>Retrasado</strong>, la condición del proyecto es <strong>Con problemas</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las condiciones pueden ser diferentes a los enumerados anteriormente. Para obtener información sobre las condiciones de personalización, consulte el artículo [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Informe sobre la condición del proyecto, la actualización de la condición del proyecto y la última nota de condición

En la vista de un informe de proyecto, puede mostrar los siguientes campos relacionados con la condición del proyecto:

* **Condición del proyecto:** muestra la condición actual del proyecto.
* **Actualización de la condición del proyecto**: muestra la actualización más reciente proporcionada por el propietario del proyecto en el flujo de actualización del proyecto, junto con la nueva condición.\
  Los comentarios realizados en las actualizaciones de condición no se muestran en la columna **Actualización de la condición**; solo se muestra la actualización principal.

* **Última nota de condición**: muestra la última actualización introducida en un objeto por el propietario del objeto. Este campo es útil para mostrar la actividad o interacción más reciente del propietario sobre un objeto.\
  La columna **Última nota de condición** está vacía si se ha eliminado el texto de nota de la última nota de un objeto. Cuando se introduce una nota nueva sobre el objeto, se convierte en la última nota y se vuelve a mostrar en la columna.

Para obtener información sobre cómo crear un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
