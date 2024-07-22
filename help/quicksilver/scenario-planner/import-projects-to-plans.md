---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importar proyectos a planes en el Scenario Planner
description: Puede importar proyectos existentes en un plan. Los proyectos importados se convierten en iniciativas y puede administrarlos dentro del plan como lo haría con una nueva iniciativa. El proyecto original sigue estando vinculado a la nueva iniciativa.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '1670'
ht-degree: 0%

---

# Importar proyectos a planes en [!DNL Scenario Planner]

Puede importar proyectos existentes en un plan. Los proyectos importados se convierten en iniciativas y puede administrarlos dentro del plan como lo haría con una nueva iniciativa. El proyecto original sigue estando vinculado a la nueva iniciativa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Actual: [!UICONTROL Empresa] o superior</p>
   <p>Nuevo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>Nuevo: claro o superior</p> 
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Producto* </td> 
   <td> 
   <p>Para los planes actuales de Workfront: </p>
   <p>Debe adquirir una licencia adicional para la funcionalidad [!DNL Adobe Workfront Scenario Planner] de acceso descrita en este artículo.</p> <p>Para obtener información acerca del acceso y los permisos para [!DNL Workfront Scenario Planner], vea <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nivel de acceso </td> 
   <td> <p>Acceso de [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la importación de proyectos en planes como nuevas iniciativas

* Debe crear proyectos antes de poder importarlos en un plan como nuevas iniciativas.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Debe tener al menos [!UICONTROL Ver] permisos en los proyectos para poder importarlos a un plan como nueva iniciativa.
* Puede importar el mismo proyecto en varios planes.
* Los proyectos que desea importar deben tener fechas incluidas en el lapso de tiempo del plan. No puede importar proyectos con una [!UICONTROL Fecha planificada de finalización] anterior al inicio del plan o con una [!UICONTROL Fecha planificada de inicio] posterior al final del plan.
* No se pueden importar más de 100 proyectos al mismo tiempo.
* Parte de la información del proyecto también se importa al plan y se convierte en información de la iniciativa. Para obtener información sobre qué información del proyecto se importa al plan y se convierte en información de iniciativa, consulte la sección [Información del proyecto importada al plan](#project-information-imported-into-the-plan) en este artículo.
* Los cambios que se producen en los proyectos vinculados no afectan a las iniciativas del plan.
* Los cambios que se producen en las iniciativas del plan no afectan automáticamente a los proyectos vinculados. Los cambios de la iniciativa afectan a los proyectos vinculados solo cuando publica la iniciativa del plan. Para obtener información acerca de cómo la publicación de iniciativas afecta a los proyectos vinculados, vea [Actualizar o crear proyectos mediante la publicación de iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* Al eliminar una iniciativa creada mediante la importación de un proyecto, no se elimina el proyecto.
* Al eliminar un proyecto vinculado a una iniciativa, no se elimina la iniciativa.

## Información del proyecto importada en el plan {#project-information-imported-into-the-plan}

Al importar un proyecto en un plan, parte de la información del proyecto también se importa en el plan y se convierte en información de la iniciativa. En la tabla siguiente se muestra qué información de proyecto se convierte en información de iniciativa al importar un proyecto a un plan:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Información del proyecto</td> 
   <td>Información de iniciativa </td> 
  </tr> 
  <tr> 
   <td>Nombre del proyecto</td> 
   <td>Nombre de iniciativa</td> 
  </tr> 
  <tr> 
   <td>Fechas planificadas del proyecto</td> 
   <td> <p>Meses de inicio y finalización de la iniciativa.</p> <p>Si un proyecto comienza o finaliza a mitad de mes, las fechas importadas se amplían para abarcar un mes completo del plan. Por ejemplo, si las fechas planificadas del proyecto son del 20 de marzo al 5 de mayo de 2020, las fechas de la iniciativa importada serán de marzo a mayo de 2020.</p> <p>Si la fecha planificada de inicio o finalización supera la duración del plan, existe una indicación visual de que la iniciativa importada se inicia antes o finaliza después del plan. </p> </td> 
  </tr> 
  <tr> 
   <td>Funciones del puesto asignadas a tareas y problemas</td> 
   <td> <p>Funciones del puesto de la iniciativa. </p> <p>Nota:   <p>Si un usuario cambia de función durante la duración del proyecto, las funciones que se importan dependen del estado de la asignación al importar el proyecto. Existen los siguientes escenarios:</p> 
     <ul> 
      <li> <p>Si un usuario asignado a una tarea o un problema cambió su rol después de marcar su asignación como [!UICONTROL Listo], [!DNL Workfront] importa a la iniciativa el rol que el usuario cumplió antes de marcar la asignación como [!UICONTROL Listo].</p> </li> 
      <li> <p>Si un usuario asignado a una tarea o un problema cambió el rol durante la duración del proyecto pero su asignación en la tarea o el problema no se marca como [!UICONTROL Listo] al importar el proyecto, [!DNL Workfront] importa solamente el rol actual del usuario asignado. </p> </li> 
     </ul> <p>Para obtener información acerca del estado de una asignación, vea "Estado de asignación" en <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glosario de terminología del Adobe [!DNL Workfront]</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto [!UICONTROL Horas planificadas] asociado con roles asignados a tareas o problemas</td> 
   <td> <p><span>Dependiendo de si el plan está configurado para usar FTE u horas, las [!UICONTROL Horas planificadas] de las tareas del proyecto se convierten en </span> [!UICONTROL FTE requeridos] <span>u [!UICONTROL Horas requeridas] en el plan</span>. </p> <p>Para obtener información acerca de cómo configurar un plan para usar jornadas completas u horas, vea <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en [!DNL Scenario Planner]</a>. </p> <p>Tenga en cuenta lo siguiente:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] utiliza los roles asignados a tareas y problemas o los roles de trabajo con los que están asociados los usuarios asignados a tareas o problemas en el proyecto y los transfiere a la nueva iniciativa como Roles de Trabajo Necesarios. </p> </li> 
     <li> <p>Cuando el plan está configurado para utilizar FTE, las horas planificadas asociadas con los roles en las tareas y problemas del proyecto se convierten primero a FTE. A continuación, se asigna a este ETC la función de trabajo de la iniciativa. <span>Las horas planificadas se distribuyen equitativamente en [!DNL Workfront]. Si una tarea o un problema abarca varios meses, la cantidad de horas planificadas para cada mes en la duración de la iniciativa se convierte en ETC mensuales y se transfiere a cada mes de la iniciativa.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><span>Por ejemplo, si se asigna una tarea a un rol durante 80 horas planificadas en septiembre, el rol importado mostrará 0,5 FTE para la iniciativa en septiembre.</span> </p> </li> 
     <li> <p>[!DNL Workfront] calcula el valor de FTE de los roles de trabajo requeridos asociados a la iniciativa mediante la fórmula siguiente:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Sugerencia: [!DNL Scenario Planner] supone que hay 160 horas laborables en un mes.</p> <p>Por ejemplo, si un proyecto tiene una duración de 1200 minutos y un rol en el proyecto está asociado con 600 minutos de horas planificadas, su valor de FTE es 0,5. Al importar el proyecto, el valor de FTE de rol requerido en la iniciativa recién creada es de 0,5 por cada mes de la iniciativa. </p> </li> 
     <li>Cuando se asigna un rol a una tarea en el proyecto con cero horas planificadas, el valor de FTE requerido para el rol de trabajo de la iniciativa es cero de forma predeterminada. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Cuando se asigna un rol a una tarea en el proyecto con una [!UICONTROL Duración] cero, el valor de FTE requerido <span> u horas</span> para el rol de la iniciativa es cero de forma predeterminada, incluso si la tarea tiene horas planificadas. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Importar proyectos en un plan

>[!IMPORTANT]
>
>Después de importar proyectos en un plan, se convierten en iniciativas del plan. Aunque los dos elementos están vinculados, existen como entidades independientes y no se afectan automáticamente cuando se actualizan.
>
>Ocurren lo siguiente:
>
>* Los cambios en el proyecto nunca afectan a la iniciativa después de importar el proyecto al plan. Estos cambios incluyen cambios en las asignaciones de roles.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Los cambios que se realicen en la iniciativa afectan a la información del área [!DNL Scenario Planner] del proyecto únicamente cuando se publica la iniciativa en el proyecto correspondiente. De lo contrario, no afectarán la información de [!UICONTROL Horas planificadas] para las tareas y problemas del proyecto.
>
>  Para obtener información acerca de cómo la publicación de iniciativas afecta a los proyectos vinculados, vea [Actualizar o crear proyectos mediante la publicación de iniciativas en el Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).
>

{{step1-to-scenario-planner}}

1. Haga clic en el nombre de un plan en el que desee importar proyectos.
1. Haga clic en **[!UICONTROL Nueva iniciativa]** y luego haga clic en **[!UICONTROL Importar proyectos]**.

   Se muestra el cuadro [!UICONTROL Importar proyectos]. Los proyectos que tienen fechas incluidas en el lapso de tiempo del plan se muestran en una lista.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Los proyectos de cualquier estado se muestran en la lista.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Opcional) Haga clic en el icono **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png)y seleccione un filtro disponible en la lista para reducir la cantidad de proyectos que hay en ella. De forma predeterminada, la lista de proyectos se filtra mediante el filtro de proyectos seleccionado actualmente por el usuario en una lista de proyectos.

1. (Opcional) Haga clic en el **[!UICONTROL icono de búsqueda]** ![](assets/search-icon.png) y agregue una palabra clave que se muestre en cualquier campo de la pantalla. Los elementos que contienen la palabra de búsqueda se muestran automáticamente en la lista y todos los elementos están ocultos.

1. (Condicional) Haga clic en el icono **[!UICONTROL X]** para quitar la búsqueda y mostrar todos los proyectos.
1. Seleccione hasta 100 proyectos y haga clic en **[!UICONTROL Importar]**.

   Los proyectos se importan como nuevas iniciativas.

   Observe lo siguiente:

   * Aparece un icono de proyecto ![](assets/project-icon-sp.png) a la derecha del nombre de la iniciativa.
   * Si la cronología del proyecto supera la duración del plan, la barra de la iniciativa finaliza con un margen apuntado a la izquierda (cuando la fecha de inicio es anterior a la fecha del plan) o a la derecha (cuando la fecha de finalización es posterior a la fecha del plan).

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * El número de meses y las funciones del puesto se han actualizado para que coincidan con las del proyecto.

   >[!TIP]
   >
   >Los costes asociados con las funciones del puesto se actualizan en el nivel de iniciativa y no se importan desde el proyecto.

1. Haga clic en la barra que representa la nueva iniciativa para abrir el panel de detalles de la iniciativa a la derecha.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   En el área **[!UICONTROL Duración de la iniciativa]**, revise la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duración de la iniciativa]</td> 
      <td>Esta es la duración de la iniciativa en meses. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Iniciativa]</td> 
      <td>Las fechas de inicio y finalización de la iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Proyecto]</td> 
      <td> <p>[!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fechas de finalización] del proyecto vinculado.</p> <p>Sugerencia: si falta la información de [!UICONTROL Project], se ha eliminado el proyecto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Edite el nombre de la iniciativa. De forma predeterminada, coincide con el nombre del proyecto.
1. (Opcional) Realice una de las siguientes acciones:

   * Actualizar los roles en la sección **[!UICONTROL Roles requeridos]**
   * Actualizar **[!UICONTROL costos fijos]** en la sección **[!UICONTROL costos]**

   * Haga clic en **[!UICONTROL Actualizar los puestos disponibles]** o en **[!UICONTROL Actualizar el presupuesto disponible]** para resolver los conflictos entre la nueva iniciativa y otras iniciativas del plan.

1. (Condicional) Haga clic en **[!UICONTROL Aplicar]** para guardar los cambios realizados en la iniciativa.
1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios realizados en su plan.
1. (Opcional) Para actualizar los cambios realizados en la iniciativa al proyecto desde el que se importó, publique el proyecto desde el plan. Para obtener información acerca de los planes de publicación, vea [Actualizar o crear proyectos mediante iniciativas de publicación en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Opcional) Haga clic en el icono del proyecto para acceder al proyecto vinculado.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
