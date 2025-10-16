---
title: Crear y personalizar prioridades
description: Puede controlar las prioridades de los proyectos, tareas y problemas en el área de Configuración de Workfront. Las prioridades otorgan importancia a sus proyectos, tareas o problemas en Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: b0b9b80b4eb718e3e131ee0cd022f54cb906f187
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 44%

---

# Crear y personalizar prioridades

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Puede controlar las prioridades de los proyectos, tareas y problemas en el área de Configuración de Workfront. Las prioridades otorgan importancia a sus proyectos, tareas o problemas en Adobe Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalización de las prioridades existentes

Como administrador de Workfront, puede realizar las siguientes modificaciones en las prioridades predeterminadas proporcionadas en Workfront:

* Cambiar el nombre de las prioridades.
* Reordenar las prioridades.

  Para obtener más información sobre cómo reordenar las prioridades, vea [Crear una prioridad para un proyecto, tarea o problema](#create-a-priority-for-a-project-task-or-issue).

* Cambiar la prioridad predeterminada.

  Para obtener más información sobre la funcionalidad de cambiar la prioridad predeterminada, vea [Crear una prioridad para un proyecto, tarea o problema](#create-a-priority-for-a-project-task-or-issue).

* Editar la descripción de las prioridades.
* Establecer un color para cada prioridad. 

  El color de la prioridad se usa en los informes de gráficos cuando se agrupan los resultados por la **Prioridad**.

  Para obtener más información sobre los informes de gráficos, consulte [Añadir un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Eliminar las prioridades.

  Al eliminar una prioridad existente, debe seleccionar una de reemplazo.

* Ocultar las prioridades.

  Para obtener más información sobre la funcionalidad de ocultar prioridades, vea [Crear una prioridad para un proyecto, tarea o problema](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Debe tener al menos una prioridad en la cuenta de Workfront para cada objeto.

Las prioridades proporcionadas de forma predeterminada para cada tipo de objeto (proyecto, tarea y problema) son idénticas:

* Ninguno
* Bajo
* Normal
* Alto
* Urgente

## Crear una prioridad para un proyecto, tarea o problema {#create-a-priority-for-a-project-task-or-issue}

Además de las prioridades predeterminadas proporcionadas en Workfront, puede añadir sus propias prioridades para reflejar las necesidades de su organización.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Prioridades**.

1. Haga clic en la pestaña del tipo de objeto para el que desea crear una prioridad para (**Proyecto**, **Tarea** o **Problema**).
1. Haga clic en <span class="preview">**Nueva fila** en la parte inferior de la tabla</span> o en **Agregar nueva prioridad**.
1. Configure las siguientes opciones para la prioridad:

   * **Nombre de prioridad**: escriba un nombre para la prioridad.
   * **Importancia**: Al agregar una nueva prioridad, se le asigna un número de forma predeterminada. Edite este número si no coincide con sus necesidades.

     El número de Importancia de cada prioridad debe ser único. El número de la prioridad refleja la importancia del proyecto, la tarea o el problema: el número más alto corresponde a la prioridad más alta.

     No puede editar este número después de guardar la prioridad.

   * **Color**: elige un color para la prioridad.

     El color de la prioridad se utiliza en los informes de gráficos y en la configuración del Equipo ágil. Para obtener información sobre los informes de gráficos, consulte [Agregar un gráfico a un informe](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). Para obtener información sobre la configuración de Agile Team, consulte [Crear un equipo Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Prioridad predeterminada**: seleccione la prioridad que desea que Workfront aplique automáticamente a todos los proyectos, tareas o problemas recién creados.

     **Normal** es la prioridad predeterminada para todos los objetos de Workfront.

     No se puede convertir una prioridad oculta en la predeterminada.

     <div class="preview">

     La prioridad predeterminada se indica con un icono ![Icono de prioridad predeterminado](assets/default-icon.png). Para elegir un nuevo valor predeterminado, siga uno de estos procedimientos:

      * Seleccione la casilla de verificación situada junto al nombre de la prioridad y seleccione **Establecer como predeterminado** en la barra de acciones de la parte inferior de la pantalla.
      * Pase el ratón sobre el nombre de prioridad y haga clic en el menú **Más** que aparece. A continuación, seleccione **Establecer como predeterminado**.

        La nueva prioridad predeterminada se etiqueta con el icono.

     </div>

   * **Descripción**: escriba una descripción para la prioridad para explicar su función.
   * <span class="preview">**Ocultar opción**</span> o **Ocultar**: <span class="preview">Seleccione **Sí**</span> o active la casilla de verificación para ocultar una prioridad que ya no sea necesaria.

     Una prioridad oculta no se muestra en ninguna parte de Workfront, por lo que los usuarios no pueden elegirla para sus proyectos, tareas o problemas.

     >[!IMPORTANT]
     >
     >En lugar de eliminar prioridades que ya no desee utilizar, le sugerimos que las oculte. De este modo, se conservan todos los datos históricos de los objetos ya completados con la prioridad, a la vez que se impide que las personas utilicen la prioridad en el futuro.

1. (Opcional) Para cambiar el orden de listado de sus prioridades, arrastre y suelte las prioridades en el orden que desee.

   Esto cambia el orden en que se muestran para los proyectos, las tareas o los problemas. No cambia el número **Importancia**.

1. Haga clic en **Guardar**.

Para obtener instrucciones sobre cómo aplicar prioridades a proyectos, tareas y problemas, consulte los siguientes artículos:

* [Comprensión y actualización de las prioridades del proyecto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Actualización de la prioridad de la tarea](../../../manage-work/tasks/task-information/task-priority.md)
* [Actualizar prioridad del problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
