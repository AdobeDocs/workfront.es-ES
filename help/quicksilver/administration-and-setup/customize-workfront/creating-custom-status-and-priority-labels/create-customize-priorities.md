---
title: Crear y personalizar prioridades
description: Puede controlar las prioridades de los proyectos, tareas y problemas en el área de Configuración de Workfront. Las prioridades otorgan importancia a sus proyectos, tareas o problemas en Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 2%

---

# Crear y personalizar prioridades

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Puede controlar las prioridades de los proyectos, tareas y problemas en el área de Configuración de Workfront. Las prioridades otorgan importancia a sus proyectos, tareas o problemas en Adobe Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td>
     <p>Nuevo: estándar</p>
     <p>o</p>
     <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar las prioridades existentes

Como administrador de Workfront, puede realizar las siguientes modificaciones en las prioridades predeterminadas proporcionadas en Workfront:

* Cambie el nombre de prioridades.
* Reordene las prioridades.

  Para obtener más información sobre cómo reordenar las prioridades, vea [Crear una prioridad para una tarea o un problema de proyecto](#create-a-priority-for-a-project-task-or-issue).

* Cambie la prioridad predeterminada.

  Para obtener más información sobre la funcionalidad de cambiar la prioridad predeterminada, vea [Crear una prioridad para una tarea de proyecto o un problema](#create-a-priority-for-a-project-task-or-issue).

* Edite la descripción de las prioridades.
* Defina un color para cada prioridad.

  El color de la prioridad se usa en los informes de gráficos cuando se agrupan los resultados por **Prioridad**.

  Para obtener más información sobre los informes de gráficos, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Eliminar prioridades.

  Al eliminar una prioridad existente, debe seleccionar una de reemplazo.

* Ocultar prioridades.

  Para obtener más información sobre la funcionalidad de ocultar prioridades, vea [Crear una prioridad para una tarea de proyecto o un problema](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Debe tener al menos una prioridad en la cuenta de Workfront para cada objeto.

Las prioridades proporcionadas de forma predeterminada para cada tipo de objeto (proyecto, tarea y problema) son idénticas:

* Ninguno
* Bajo
* Normal
* Alto
* Urgente

## Crear una prioridad para una tarea o un problema de proyecto {#create-a-priority-for-a-project-task-or-issue}

Además de las prioridades predeterminadas proporcionadas en Workfront, puede agregar sus propias prioridades para reflejar las necesidades de su organización.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Prioridades**.

1. Haga clic en la ficha del tipo de objeto para el que desea crear una prioridad (**Proyecto**, **Tarea** o **Problema**).
1. Haga clic en **Agregar nueva prioridad**.
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
      <td> <p>Al agregar una nueva prioridad, se le asigna un número de forma predeterminada. Edite este número si no coincide con sus necesidades.</p> <p>El número <strong>Importance</strong> de cada prioridad debe ser único para el objeto seleccionado.<br>El número de la prioridad refleja la importancia del proyecto, tarea o problema: el número más alto corresponde a la prioridad más alta.</p> <p><b>NOTA</b>: no puede editar el número de importancia después de guardar la prioridad. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Elija un color para su prioridad.</p> <p>El color de la prioridad se utiliza en los informes de gráficos y en la configuración del equipo de Agile. Para obtener más información sobre los informes de gráficos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> <p>Para obtener más información sobre la configuración de Agile Team, consulte en .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioridad predeterminada</td> 
      <td> <p>Decida si debe ser una prioridad predeterminada o no, seleccionando el botón de opción.</p> <p>Si se designa una prioridad como <strong>Prioridad predeterminada</strong>, se selecciona automáticamente para todos los proyectos, tareas o problemas de Workfront. <strong>Normal</strong> es la prioridad predeterminada para todos los objetos de Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Añada una descripción para la prioridad para explicar su función.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> <p>Seleccione esta casilla si desea ocultar la prioridad.</p><p>Al seleccionar la opción <b>Ocultar</b>, la prioridad no se muestra en ninguna parte de Workfront y los usuarios no pueden elegirla para sus proyectos, tareas y problemas.</p> 
      <p><b>IMPORTANTE</b>: Le recomendamos que oculte las prioridades que ya no desee usar, en lugar de eliminarlas. Al ocultarlos, se conservan todos los datos históricos, de los objetos que se han completado con esta prioridad, al tiempo que se impide que las personas elijan esta prioridad en el futuro. </p>
      <p>Si lo desea, puede cambiar el orden de los listados de sus prioridades arrastrándolas y soltándolas en el orden deseado. Esto cambia el orden en que se muestran para los proyectos, las tareas y los problemas. Esto no cambia el número <b>Importance</b>. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

Para obtener instrucciones sobre cómo aplicar prioridades a proyectos, tareas y problemas, consulte los siguientes artículos:

* [Comprender y actualizar las prioridades del proyecto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Actualizar prioridad de tarea](../../../manage-work/tasks/task-information/task-priority.md)
* [Actualizar prioridad del problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
