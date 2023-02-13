---
title: Descripción general de la condición y el tipo de condición del proyecto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: La condición del proyecto es una representación visual del progreso del proyecto. Es una variable que se puede incluir en los informes, determinada por la relación entre las fechas previstas, proyectadas y estimadas del proyecto.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Descripción general de la condición y el tipo de condición del proyecto

La condición del proyecto es una representación visual del progreso del proyecto. Es una variable que se puede incluir en los informes, determinada por la relación entre las fechas previstas, proyectadas y estimadas del proyecto.

## Información general sobre la condición del proyecto

Tenga en cuenta lo siguiente para comprender la condición de un proyecto:

* Como propietario del proyecto, puede decidir si la condición de un proyecto se establece de forma manual o automática. La condición de un proyecto se puede establecer de las siguientes maneras:

   * Manualmente, por usuarios que tienen acceso a Administrar el proyecto y cuando el tipo de condición del proyecto está configurado en Manual.
   * Automáticamente, por Adobe Workfront, cuando el tipo de condición del proyecto se establece en Estado de progreso. El estado de progreso del proyecto viene determinado por el progreso de las tareas del proyecto. Para obtener información sobre el estado de progreso del proyecto, consulte [Resumen del estado del progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   Para obtener información sobre cómo actualizar el tipo de condición del proyecto, consulte [Definición del tipo de condición de un proyecto](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Al permitir que Workfront calcule automáticamente la condición del proyecto, le recomendamos que utilice predecesores en sus tareas para que el progreso de la tarea se refleje en el progreso real y en el estado de progreso del proyecto.
* Como propietario de un proyecto, puede cambiar el proyecto para que utilice un tipo de condición manual en lugar de utilizar el estado de progreso cambiando el tipo de condición de estado de progreso a manual.

   >[!NOTE]
   >
   >Los proyectos que tengan cualquiera de los siguientes estados siempre se marcan como En Target, independientemente de las fechas de las tareas y de su progreso:
   >
   >* Idea
   >* Solicitado
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

## Cómo actualiza Workfront la condición del proyecto en función del estado de progreso

Cuando el tipo de condición del proyecto se establece en Manual, puede determinar qué condición del proyecto es independiente del estado de progreso del proyecto.

Sin embargo, le recomendamos que establezca el Tipo de condición del proyecto en Estado de progreso para que pueda tener una indicación clara del verdadero progreso del proyecto, en función del progreso de sus tareas. Para obtener información sobre cómo calcula Workfront el estado de progreso de los proyectos, consulte [Resumen del estado del progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

En este caso, los valores de la condición del proyecto pueden ser:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Condición del proyecto</td> 
   <td>Estado del progreso del proyecto</td> 
   <td>Indicador de condición de Workfront</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bien encaminado</td> 
   <td> <li>Cuando el estado de progreso del proyecto es Tiempo de activación, la condición del proyecto es <strong>En Target</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>En riesgo</td> 
   <td>Cuando el estado de progreso del proyecto es <strong>Detrás</strong> o <strong>En riesgo</strong>, la condición del proyecto es <strong>En riesgo</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Con problemas</td> 
   <td>Cuando el estado de progreso del proyecto es <strong>Late</strong>, la condición del proyecto es <strong>En problemas</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las Condiciones pueden ser diferentes de los indicados arriba. Para obtener información sobre la personalización de condiciones en , consulte el artículo [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Informe sobre las condiciones del proyecto, la actualización de las condiciones del proyecto y la última nota sobre las condiciones del proyecto

En la vista de un informe de proyecto, puede mostrar los siguientes campos relacionados con la condición del proyecto:

* **Condición del proyecto:** Muestra la condición actual del proyecto.
* **Actualización de condición del proyecto**: Muestra la actualización más reciente proporcionada por el propietario del proyecto en el flujo de actualización del proyecto, junto con la nueva condición.\
   Los comentarios realizados en las actualizaciones de Condición no se muestran en la **Actualización de condición** columna; solo se muestra la actualización principal.

* **Última nota de condición**: Muestra la última actualización introducida en un objeto por el propietario del objeto. Este campo es útil para mostrar la actividad o interacción más reciente del propietario en un objeto.\
   La variable **Última nota de condición** está vacía si se ha eliminado el texto de la nota de la última nota de un objeto. Cuando se introduce una nota nueva en el objeto, esta se convierte en la última nota y se muestra de nuevo en la columna .

Para obtener información sobre cómo crear un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
