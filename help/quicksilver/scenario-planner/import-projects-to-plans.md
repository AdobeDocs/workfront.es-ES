---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importar proyectos a planes en el planificador de escenarios
description: Puede importar proyectos existentes en un plan. Los proyectos importados se convierten en iniciativas y puede administrarlos dentro del plan, ya que administraría una nueva iniciativa. El proyecto original sigue vinculado a la nueva iniciativa.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# Importar proyectos a planes en el [!DNL Scenario Planner]

Puede importar proyectos existentes en un plan. Los proyectos importados se convierten en iniciativas y puede administrarlos dentro del plan, ya que administraría una nueva iniciativa. El proyecto original sigue vinculado a la nueva iniciativa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licencia*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en el planificador de escenarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Consideraciones sobre la importación de proyectos a planes como nuevas iniciativas

* Debe crear proyectos para poder importarlos en un plan como iniciativas nuevas.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Debe tener al menos [!UICONTROL Ver] permisos para los proyectos para poder importarlos a un plan como nueva iniciativa.
* Puede importar el mismo proyecto en varios planes.
* Los proyectos que desea importar deben tener fechas incluidas en el lapso de tiempo del plan. No se pueden importar proyectos con un [!UICONTROL Fecha de finalización planeada] antes del inicio del plan o [!UICONTROL Fecha de inicio planeada] más tarde del final del plan.
* No se pueden importar más de 100 proyectos a la vez.
* Parte de la información del proyecto también se importa en el plan y se convierte en información sobre la iniciativa. Para obtener información sobre qué información del proyecto se importa en el plan y se convierte en información de iniciativa, consulte la [Información del proyecto importada en el plan](#project-information-imported-into-the-plan) en este artículo.
* Los cambios que se producen en los proyectos vinculados no afectan a las iniciativas del plan.
* Los cambios que se producen en las iniciativas del plan no afectan automáticamente a los proyectos vinculados Los cambios de la Iniciativa afectan a los proyectos vinculados solo cuando se publica la iniciativa desde el plan. Para obtener información sobre cómo las iniciativas de publicación afectan a los proyectos vinculados, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* Al eliminar una iniciativa que se ha creado mediante la importación de un proyecto, este no se elimina.
* Al eliminar un proyecto vinculado a una iniciativa, esta no se elimina.

## Información del proyecto importada en el plan {#project-information-imported-into-the-plan}

Al importar un proyecto en un plan, también se importa parte de la información del proyecto en el plan, que se convierte en información de la iniciativa. La tabla siguiente muestra qué información del proyecto se convierte en información de iniciativa al importar un proyecto en un plan:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Información del proyecto</td> 
   <td>Información sobre la iniciativa </td> 
  </tr> 
  <tr> 
   <td>Nombre del proyecto</td> 
   <td>Nombre de la iniciativa</td> 
  </tr> 
  <tr> 
   <td>Fechas planificadas del proyecto</td> 
   <td> <p>Los meses de inicio y fin de la iniciativa.</p> <p>Si un proyecto comienza o finaliza a mediados de un mes, las fechas importadas se amplían para cubrir un mes completo del plan. Por ejemplo, si las fechas previstas para el proyecto son del 20 de marzo al 5 de mayo de 2020, las fechas de la iniciativa importada serán marzo a mayo de 2020.</p> <p>Si la fecha de inicio o finalización planeada está más allá de la duración del plan, existe una indicación visual de que la iniciativa importada comienza antes o finaliza después del plan. </p> </td> 
  </tr> 
  <tr> 
   <td>Funciones de trabajo asignadas a tareas y problemas</td> 
   <td> <p>Funciones del puesto de la iniciativa. </p> <p>Nota:   <p>Si un usuario cambia de función durante la vida del proyecto, las funciones que se importan dependen del estado de la asignación al importar el proyecto. Existen los siguientes escenarios:</p> 
     <ul> 
      <li> <p>Si un usuario asignado a una tarea o un problema ha cambiado su función después de marcar su asignación como [!UICONTROL Listo], [!DNL Workfront] importa a la iniciativa la función que el usuario cumplió antes de marcar la asignación como [!UICONTROL Listo].</p> </li> 
      <li> <p>Si un usuario asignado a una tarea o problema ha cambiado la función durante la vida del proyecto, pero su asignación en la tarea o el problema no está marcada como [!UICONTROL Listo] al importar el proyecto, [!DNL Workfront] importa solo la función actual del usuario asignado. </p> </li> 
     </ul> <p>Para obtener información sobre el estado de una asignación, consulte "Estado de asignación" en <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glosario de Adobes [!DNL Workfront] terminología</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto [!UICONTROL Horario planificado] asociado con funciones de trabajo asignadas a tareas o problemas</td> 
   <td> <p><span>Dependiendo de si el plan está configurado para utilizar FTE u horas, las [!UICONTROL Horario planificado] de las tareas del proyecto se convierten en:</span> [!UICONTROL FTEs requeridos] <span>o [!UICONTROL Horas requeridas] en el plan</span>. </p> <p>Para obtener información sobre la configuración de un plan para utilizar FTE u horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Cree y edite planes en el [!DNL Scenario Planner]</a>. </p> <p>Tenga en cuenta lo siguiente:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] utiliza las funciones de trabajo asignadas a tareas y problemas o las funciones de trabajo con las que los usuarios asignados a tareas o problemas están asociados en el proyecto y las transfiere a la nueva iniciativa como Funciones de Trabajo Requeridas. </p> </li> 
     <li> <p>Cuando se configura el plan para utilizar FTE, las horas planificadas asociadas con las funciones de trabajo en las tareas y problemas del proyecto se convierten primero a FTE. A continuación, se asigna a este ETC la función de trabajo de la iniciativa. <span>Las horas planificadas se distribuyen de forma equitativa en [!DNL Workfront]. Si una tarea o un problema abarca varios meses, la cantidad de horas programadas para cada mes de duración de la iniciativa se convierte en FTE mensuales y se transfiere a cada mes de la iniciativa.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><span>Por ejemplo, si se asigna una tarea a una función de trabajo durante 80 horas programadas en septiembre, la función de trabajo importada mostrará 0,5 horas al día para la iniciativa en septiembre.</span> </p> </li> 
     <li> <p>[!DNL Workfront] calcula el FTE de las funciones de trabajo requeridas asociadas con la iniciativa mediante la fórmula siguiente:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Sugerencia: La variable [!DNL Scenario Planner] supone que hay 160 horas de trabajo al mes.</p> <p>Por ejemplo, si un proyecto tiene una duración de 1200 minutos y una función de trabajo en el proyecto está asociada con 600 minutos de horas planificadas, su tiempo de espera es de 0,5. Al importar el proyecto, el tiempo de espera necesario para la función de trabajo de la iniciativa recién creada es de 0,5 para cada mes de la iniciativa. </p> </li> 
     <li>Cuando se asigna una función de trabajo a una tarea del proyecto con cero horas planificadas, el FTE requerido para la función de trabajo de la iniciativa es cero de forma predeterminada. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Cuando se asigna una función de trabajo a una tarea del proyecto con una [!UICONTROL Duration] cero, se llama a FTE requerido <span>o horas</span> para la función de trabajo de la iniciativa es cero de forma predeterminada, aunque la tarea tenga Horario planificado. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Importar proyectos en un plan

>[!IMPORTANT]
>
>Después de importar proyectos a un plan, se convierten en iniciativas sobre el plan. Aunque los dos elementos están vinculados, existen como entidades independientes y no se afectan entre sí automáticamente cuando se actualizan.
>
>Se produce lo siguiente:
>
>* Los cambios en el proyecto no afectan a la iniciativa después de importarlo al plan. Estos cambios incluyen cambios en las asignaciones de funciones de trabajo.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Los cambios en la iniciativa afectan a la información de la [!DNL Scenario Planner] solo cuando publica la iniciativa en el proyecto correspondiente. De lo contrario, no afectan a la variable [!UICONTROL Horas planificadas] información sobre las tareas y los problemas del proyecto.
>
>  Para obtener información sobre cómo las iniciativas de publicación afectan a los proyectos vinculados, consulte  [Actualizar o crear proyectos publicando iniciativas en el Planificador de escenarios](../scenario-planner/publish-scenarios-update-projects.md).

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en [!DNL Scenarios] para acceder a la [!DNL Scenario Planner].

1. Haga clic en el nombre de un plan en el que desea importar proyectos.
1. Haga clic en **[!UICONTROL Nueva Iniciativa]** y haga clic en **[!UICONTROL Importar proyectos]**.

   La variable [!UICONTROL Importar proyectos] se muestra. Los proyectos que tienen fechas incluidas en el lapso de tiempo del plan se muestran en una lista.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Los proyectos con cualquier estado se muestran en la lista.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Opcional) Haga clic en el **[!UICONTROL Icono de filtro]** ![](assets/filter-nwepng.png)y seleccione un filtro disponible en la lista para reducir la cantidad de proyectos que hay en la lista. De forma predeterminada, la lista de proyectos se filtra mediante el filtro de proyecto seleccionado actualmente por el usuario en una lista de proyectos.

1. (Opcional) Haga clic en el **[!UICONTROL Icono de búsqueda]** ![](assets/search-icon.png) y añada una palabra clave que se muestre en cualquier campo de la pantalla. Los elementos que contienen la palabra de búsqueda se muestran en la lista automáticamente y todos los elementos están ocultos.

1. (Condicional) Haga clic en el **[!UICONTROL Icono X]** para eliminar la búsqueda y mostrar todos los proyectos.
1. Seleccione hasta 100 proyectos y haga clic en **[!UICONTROL Importar]**.

   Los proyectos se importan como nuevas iniciativas.

   Observe lo siguiente:

   * Icono de proyecto ![](assets/project-icon-sp.png) se muestra a la derecha del nombre de la iniciativa.
   * Si la línea de tiempo del proyecto supera la duración del plan, la barra de la iniciativa termina con un margen específico a la izquierda (cuando la fecha de inicio es anterior a la fecha del plan) o a la derecha (cuando la fecha de finalización es posterior a la fecha del plan).

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Se ha actualizado el número de meses y las funciones de trabajo para que coincidan con las del proyecto.
   >[!TIP]
   >
   >Los costes asociados con las funciones de trabajo se actualizan a nivel de iniciativa y no se importan desde el proyecto.

1. Haga clic en la barra que representa la nueva iniciativa para abrir el panel de detalles de la iniciativa a la derecha.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   En el **[!UICONTROL Duración de la iniciativa]** revise la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duración de la iniciativa]</td> 
      <td>Esta es la duración de la iniciativa en meses. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Las fechas de inicio y finalización de la iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>El [!UICONTROL Planned Start] y [!UICONTROL Fechas de finalización] del proyecto vinculado.</p> <p>Sugerencia: Si falta la información de [!UICONTROL Project], se eliminó el proyecto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Edite el nombre de la iniciativa. De forma predeterminada, coincide con el nombre del proyecto.
1. (Opcional) Realice una de las siguientes acciones:

   * Actualizar funciones de trabajo en la variable **[!UICONTROL Funciones de trabajo requeridas]** sección
   * Actualice el **[!UICONTROL Costes fijos]** en el **[!UICONTROL Costes]** sección

   * Haga clic en **[!UICONTROL Actualizar funciones de trabajo disponibles]** o **[!UICONTROL Actualizar el presupuesto disponible]** resolver los conflictos entre la nueva iniciativa y otras iniciativas sobre el plan.

1. (Condicional) Haga clic en **[!UICONTROL Aplicar]** para guardar los cambios en su iniciativa.
1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios en su plan.
1. (Opcional) Para actualizar los cambios realizados en la iniciativa al proyecto desde el que se importó, publique el proyecto desde el plan. Para obtener información sobre los planes de publicación, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Opcional) Haga clic en el icono del proyecto para acceder al proyecto vinculado.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
