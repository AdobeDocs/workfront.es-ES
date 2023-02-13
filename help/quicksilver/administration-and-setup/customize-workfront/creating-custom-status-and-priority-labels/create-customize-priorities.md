---
title: Crear y personalizar prioridades
description: Puede controlar las prioridades de los proyectos, tareas y problemas en el área de configuración de Workfront. Las prioridades dan importancia a sus proyectos, tareas o problemas en Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Crear y personalizar prioridades

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Puede controlar las prioridades de los proyectos, tareas y problemas en el área de configuración de Workfront. Las prioridades dan importancia a sus proyectos, tareas o problemas en Adobe Workfront.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalización de prioridades existentes

Como administrador de Workfront, puede realizar las siguientes modificaciones en las prioridades predeterminadas que se proporcionan en Workfront:

* Cambie el nombre de las prioridades.
* Reordenar las prioridades.

   Para obtener más información sobre cómo reordenar las prioridades, consulte [Crear una prioridad para una tarea de proyecto o un problema](#create-a-priority-for-a-project-task-or-issue).

* Cambie la prioridad predeterminada.

   Para obtener más información sobre la funcionalidad de cambiar la prioridad predeterminada, consulte [Crear una prioridad para una tarea de proyecto o un problema](#create-a-priority-for-a-project-task-or-issue).

* Edite la descripción de las prioridades.
* Establezca un color para cada prioridad.

   El color de la prioridad se utiliza en los informes de gráficos, cuando se agrupan los resultados por **Prioridad**.

   Para obtener más información sobre los informes de gráficos, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Eliminar prioridades.

   Cuando elimine una prioridad existente, debe seleccionar una que la sustituya.

* Ocultar prioridades.

   Para obtener más información sobre la funcionalidad de ocultar prioridades, consulte [Crear una prioridad para una tarea de proyecto o un problema](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >Debe tener al menos una prioridad en la cuenta de Workfront para cada objeto.

Las prioridades proporcionadas de forma predeterminada para cada tipo de objeto (proyecto, tarea y problema) son idénticas:

* Ninguno
* Bajo
* Normal
* Alto
* Urgente

## Crear una prioridad para una tarea de proyecto o un problema {#create-a-priority-for-a-project-task-or-issue}

Además de las prioridades predeterminadas que se proporcionan en Workfront, puede agregar sus propias prioridades para reflejar las necesidades de su organización.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Prioridades**.

1. Haga clic en la pestaña del tipo de objeto para el que desea crear una prioridad (**Proyecto**, **Tarea** o **Problema**).
1. Haga clic en **Añadir una nueva prioridad**.
1. Especifique la siguiente información para la nueva prioridad:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de prioridad</td> 
      <td>Escriba un nombre para la prioridad.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importancia</td> 
      <td> <p>Al añadir una nueva prioridad, se le asigna un número de forma predeterminada. Edite este número si no se ajusta a sus necesidades.</p> <p>La variable <strong>Importancia</strong> para cada prioridad debe ser único para el objeto seleccionado.<br>El número de la prioridad refleja la importancia del proyecto, la tarea o el problema: el número más alto corresponde a la prioridad más alta.</p> <p><b>NOTA</b>: Después de guardar la prioridad, no se puede editar el número de importancia. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Elija un color para la prioridad.</p> <p>El color de la prioridad se utiliza en los informes de gráficos y en la configuración del equipo de Agile. Para obtener más información sobre los informes de gráficos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> <p>Para obtener más información sobre la configuración de Agile Team, consulte en .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioridad predeterminada</td> 
      <td> <p>Decida si esta debería ser una prioridad predeterminada o no, seleccionando el botón de opción .</p> <p>Si se designa una prioridad como la variable <strong>Prioridad predeterminada</strong>, se selecciona automáticamente para todos los proyectos, tareas o problemas de Workfront. <strong>Normal</strong> es la prioridad predeterminada para todos los objetos de Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Añada una descripción para la prioridad para explicar su función.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> <p>Seleccione este cuadro si desea ocultar la prioridad.</p><p>Al seleccionar la variable <b>Ocultar</b> , la prioridad no se muestra en ninguna parte de Workfront y los usuarios no pueden elegirla para sus proyectos, tareas y problemas.</p> 
      <p><b>IMPORTANTE</b>: Le recomendamos que oculte las prioridades que ya no desea utilizar, en lugar de eliminarlas. Al ocultarlas, se conservarán todos los datos históricos, de los objetos que se hayan completado con esta prioridad, a la vez que se evita que las personas elijan esta prioridad en el futuro. </p>
      <p>De forma opcional, puede cambiar el orden de las prioridades arrastrándolas y soltándolas en el orden deseado. Esto cambia el orden en que se muestran para los proyectos, las tareas y los problemas. Esto no cambia la variable <b>Importancia</b> número. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

Para obtener instrucciones sobre la aplicación de prioridades a proyectos, tareas y problemas, consulte los siguientes artículos:

* [Comprender y actualizar las prioridades del proyecto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Actualizar prioridad de tareas](../../../manage-work/tasks/task-information/task-priority.md)
* [Actualizar prioridad del problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
