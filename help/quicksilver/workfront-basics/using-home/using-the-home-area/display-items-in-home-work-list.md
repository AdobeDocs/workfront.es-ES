---
product-area: projects
navigation-topic: use-the-home-area
title: Mostrar elementos en la [!UICONTROL Lista de trabajos] del área de Inicio
description: La [!UICONTROL Lista de trabajos] en el área [!UICONTROL Inicio] muestra todos los elementos de trabajo que se le han asignado. Puede controlar qué elementos se muestran en su [!UICONTROL Lista de trabajos] mediante filtros y agrupando y ordenando los elementos de trabajo.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1840'
ht-degree: 0%

---

# Mostrar elementos en la [!UICONTROL Lista de trabajos] en el área [!UICONTROL Inicio]

<!-- Audited: 1/2024 -->


La [!UICONTROL Lista de trabajos] en el área [!UICONTROL Inicio] muestra todos los elementos de trabajo que se le han asignado. Puede controlar qué elementos se muestran en su [!UICONTROL Lista de trabajos] mediante filtros y agrupando y ordenando los elementos de trabajo.

>[!NOTE]
>
>* Al convertir un problema en una tarea o un proyecto, el problema se elimina del área de Inicio del usuario asignado al problema.
>
>* Al convertir una tarea en un proyecto, la tarea se elimina y esta se elimina del área de Inicio del usuario asignado a la tarea.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> <p>Nuevo:</p><ul><li>[!UICONTROL Contributor] solo para aprobaciones</li> <li>[!UICONTROL Standard] o superior para todos los demás objetos</li> <p>O</p> 
  </ul><p>Actual:</p><ul><li>[!UICONTROL Review] solo para aprobaciones</li> <li>[!UICONTROL Work] o superior para todos los demás objetos</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos, Tareas, Problemas y Documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de Contribute o superiores para las tareas y problemas en los que debe trabajar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar [!UICONTROL Lista de trabajos]

Puede filtrar elementos en la [!UICONTROL Lista de trabajos] para ver solamente tipos de elementos específicos. Por ejemplo, puede filtrar [!UICONTROL Work List] para mostrar solo los problemas o las solicitudes.

>[!NOTE]
>
>Las opciones de filtro se almacenan en el explorador. Si utiliza el mismo explorador de forma constante en el mismo equipo (y no borra los datos del sitio), los filtros seleccionados no cambian. Si cambia de navegador o de ordenador, los filtros vuelven a la opción predeterminada, que es la que no está seleccionada para todos los filtros.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en el menú desplegable **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png). Si tiene algún filtro seleccionado, el número de filtros seleccionados se muestra en lugar del icono.
1. Seleccione entre las siguientes opciones de filtro para especificar el tipo de elementos que desea mostrar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Todo]</strong></td> 
      <td>Muestra y selecciona todos los elementos. Esto incluye tareas, problemas, aprobaciones, tareas personales y tareas y problemas completados. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tareas de [!UICONTROL: Trabajando en]</strong></td> 
      <td> <p>Muestra únicamente las tareas en las que está trabajando activamente. Son tareas asignadas para las que ha hecho clic en el botón [!UICONTROL Trabajar en ello].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tareas: Listo para iniciarse]</strong></td> 
      <td> 
       <div> 
        <p>Muestra sólo las tareas que están listas para iniciarse. Las dos afirmaciones siguientes deben ser verdaderas:</p> 
        <ul> 
         <li> <p>Las tareas y sus tareas principales no tienen predecesoras ni restricciones de tarea que impidan trabajar con ellas.</p> </li> 
         <li> <p>Se han completado todas las tareas predecesoras.</p> </li> 
         <li> <p>La [!UICONTROL Fecha planificada de inicio] de las tareas se encuentra en las últimas o hasta dos semanas en el futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tareas: No está listo]</strong></td> 
      <td> 
       <div> 
        <p>Muestra únicamente las tareas que aún no están listas para iniciarse. Cualquiera de las siguientes afirmaciones debe ser verdadera:</p> 
        <ul> 
         <li> <p>Las tareas y sus tareas principales pueden tener predecesoras o restricciones de tareas que impiden que se trabaje con ellas.</p> </li> 
         <li> <p>Las tareas tienen una [!UICONTROL Fecha planificada de inicio] que es más de dos semanas en el futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas: Trabajando en]</strong></td> 
      <td> <p>Muestra únicamente los problemas en los que está trabajando activamente. Estos son problemas asignados a usted para los que ha hecho clic en el botón [!UICONTROL Trabajar en ello].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas: Solicitado]</strong></td> 
      <td>Muestra sólo los problemas que tiene asignados pero para los que no ha hecho clic en el botón [!UICONTROL Trabajar en ello].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personal</strong></td> 
      <td>Muestra sólo las tareas personales. Son tareas que crea como una tarea de [!UICONTROL Tareas pendientes], tal como se describe en la sección <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Crear una tarea personal</a> del artículo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Crear elementos de trabajo a partir del área de [!UICONTROL Inicio]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aprobaciones]</strong></td> 
      <td> 
       <div> 
        <p>Muestra sólo las aprobaciones que se le han asignado o delegado y las que ha enviado. Las aprobaciones incluyen aprobaciones de elementos de trabajo (proyectos, tareas y problemas) y aprobaciones de documentos, pruebas, solicitudes de acceso y hojas de horas. Para obtener más información sobre las aprobaciones, consulte los siguientes artículos:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Ver aprobaciones</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Aprobaciones de trabajo</a> </p> </li> 
        </ul> 
        <p>Nota: Las aprobaciones que ha enviado y en las que también es uno de los aprobadores se cuentan dos veces.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegado: delegado por mí]</strong></td> 
      <td> 
       <div> 
        <p>Muestra sólo los elementos de trabajo que ha delegado a otro usuario.</p> 
        <p>Para obtener más información acerca de la delegación de tareas, vea <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Delegar tareas y problemas</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegado: Delegado a mí]</strong></td> 
      <td> 
       <div> 
        <p>Muestra sólo los elementos de trabajo que le ha delegado temporalmente otro usuario.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL completado]</strong></td> 
      <td> <p>Muestra sólo las tareas, problemas y tareas personales completados. El trabajo completado se muestra durante las dos semanas anteriores y se agrupa en la Lista de trabajos según la semana en que se completaron. No se incluyen las aprobaciones.</p> <p>El trabajo completado está oculto en la Lista de trabajos de [!UICONTROL] a menos que seleccione este filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Las opciones de filtro se basan en objetos (tareas, problemas, aprobaciones, tareas personales).
   >* Las tareas y los problemas se filtran aún más por su estado en relación con nuestra preparación para trabajar con ellos ([!UICONTROL Trabajando en], [!UICONTROL Listo para comenzar], [!UICONTROL No listo] para las tareas y [!UICONTROL Trabajando en] y [!UICONTROL Solicitado] para los problemas). Puede seleccionar mostrar tareas o problemas en un estado específico o hacer clic en Tareas o Problemas para seleccionar y mostrar todos los estados.
   >* Hay un filtro independiente para los elementos completados que incluye tareas y problemas. Esto no incluye las aprobaciones. El filtro [!UICONTROL Completado] incluye tareas personales.
   >* Puede seleccionar mostrar solo un estado a la vez. Por ejemplo, solo puede mostrar [!UICONTROL Trabajando en] tareas y solo [!UICONTROL Solicitado] problemas. También puede seleccionar varios estados a la vez.
   >* No se pueden aplicar filtros a los elementos asignados a uno de los equipos, y las asignaciones de equipo no se incluyen en los elementos que se le han asignado directamente.


1. (Opcional) Organice aún más la [!UICONTROL Lista de trabajos], tal como se describe en la sección [Agrupar y ordenar por fecha, proyecto y prioridad](#group-and-sort-by-date-project-and-priority) en este artículo.

## Agrupar y ordenar por [!UICONTROL Fecha], [!UICONTROL Proyecto] y [!UICONTROL Prioridad]

Puede agrupar y ordenar la [!UICONTROL Lista de trabajos] por [!UICONTROL Fecha planificada de finalización], [!UICONTROL Fecha de confirmación], [!UICONTROL Proyecto] o [!UICONTROL Mi prioridad]. La opción que elija determina cómo se agrupan los elementos en la [!UICONTROL Lista de trabajos].

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en el menú desplegable **[!UICONTROL Agrupar por]** ![Agrupar por](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png).

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Finalización planificada]</strong></td> 
      <td> <p> Los elementos se muestran en las siguientes agrupaciones de la [!UICONTROL Lista de trabajos], según su [!UICONTROL Fecha planificada de finalización] (el número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Sin fecha planificada de finalización]</p> </li> 
        <li> <p>[!UICONTROL Esta semana]</p> <p>Esta agrupación se expande de forma predeterminada.</p> </li> 
        <li> <p>[!UICONTROL Próxima semana]</p> </li> 
        <li> <p>[!UICONTROL Planificado], seguido de varias [!UICONTROL Fechas planificadas de finalización] (varias agrupaciones)</p> </li> 
        <li> <p>[!UICONTROL Completo]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Inicio planificado]</strong></td> 
      <td> <p>Los elementos se muestran en las siguientes agrupaciones de la [!UICONTROL Lista de trabajos], según su [!UICONTROL Fecha planificada de inicio] (el número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Esta semana] </p> <p>Esta agrupación se expande de forma predeterminada.</p> </li> 
        <li> <p>[!UICONTROL Próxima semana]</p> </li> 
        <li> <p>[!UICONTROL Planificado], seguido de varias [!UICONTROL Fechas planificadas de inicio] (varias agrupaciones)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de confirmación]</strong></td> 
      <td> <p>Los elementos se muestran en las siguientes agrupaciones de la [!UICONTROL Work List] (el número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado):</p> 
       <ul> 
        <li> <p>[!UICONTROL Sin fecha de confirmación]</p> </li> 
        <li> <p>[!UICONTROL Confirmado Para La Próxima Semana]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Proyecto]</strong></td> 
      <td>Los elementos se agrupan según el proyecto y los proyectos aparecen alfabéticamente en la Lista de trabajos de [!UICONTROL]. (El número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Mi prioridad]</strong></td> 
      <td>Los artículos se muestran en el orden que elija. Para obtener más información, vea <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Priorizar el trabajo en el área de [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>El orden predeterminado es ascendente. Si cambia el orden a descendente, las opciones de ordenación seleccionadas se almacenan en el explorador. Si utiliza el mismo explorador de forma constante en el mismo equipo (y no borra los datos del sitio), la ordenación no cambia, pero si cambia de explorador o de equipo, la ordenación cambia a la predeterminada.

## Ver elementos atrasados

[!DNL Adobe Workfront] usa las fechas siguientes para determinar si las solicitudes de trabajo están atrasadas:

* **Tareas**: [!UICONTROL Fecha planificada de finalización]
* **Problemas**: [!UICONTROL Fecha planificada de finalización]
* **Documentos**: [!UICONTROL Fecha de envío]
* **Plantillas de horas**: [!UICONTROL Fecha de envío]
* **Aprobaciones**: [!UICONTROL Fecha de envío]
* **Aprobaciones de revisión**: [!UICONTROL Plazo de revisión]

## Buscar en [!UICONTROL Lista de trabajos]

Al buscar en la [!UICONTROL Lista de trabajos], todos los elementos que se le hayan asignado se devolverán en la búsqueda (incluso los elementos que no estén cargados actualmente en la pantalla). Si se selecciona la opción [!UICONTROL Mostrar completado], también se devolverán todos los elementos que haya marcado como completados en las últimas dos semanas.

Además, sólo se buscan los nombres de los elementos de trabajo (no se busca información dentro del elemento de trabajo ni los nombres de los proyectos en los que reside el elemento de trabajo).

Para buscar en [!UICONTROL Lista de trabajos]:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Opcional) Filtre y agrupe la [!UICONTROL Lista de trabajos], tal como se describe en [Filtre la [!UICONTROL Lista de trabajos]](#filter-the-work-list) y [Agrupe y ordene por fecha, proyecto y prioridad](#group-and-sort-by-date-project-and-priority).

1. (Opcional) Si está buscando un elemento de trabajo que ya se ha completado, debe configurar la [!UICONTROL Lista de trabajos] para que muestre los elementos completados antes de realizar la búsqueda.

1. Haga clic en el icono Buscar ![Buscar](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Empiece a escribir el nombre del elemento que está buscando.\
   La [!UICONTROL Lista de trabajos] se filtra automáticamente para incluir elementos con un nombre que coincida.

## Cambiar el tamaño de la Lista de trabajos

Puede cambiar el tamaño de la [!UICONTROL Lista de trabajos] para que consuma entre un cuarto del área de Inicio y la mitad del área de [!UICONTROL Hogar].

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. Pase el ratón sobre el borde derecho de la [!UICONTROL Lista de trabajos] y luego arrástrela hacia la izquierda o hacia la derecha hasta que la Lista de trabajos tenga el tamaño deseado.

## Contraer y expandir agrupaciones

Los elementos de [!UICONTROL Lista de trabajos] se muestran dentro de las agrupaciones. Puede contraer y expandir las agrupaciones para controlar cuánta información se muestra en la página en un momento determinado.

Puede contraer y expandir agrupaciones dentro de la [!UICONTROL Lista de trabajos] para controlar mejor qué información es visible.\
De manera predeterminada, la agrupación [!UICONTROL This Week] se expande y todas las demás agrupaciones se contraen. Cualquier cambio que realice se recordará la próxima vez que acceda al área de Inicio.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en la flecha **[!UICONTROL Expandir]** o **[!UICONTROL Contraer]** junto a cualquier agrupación que desee expandir o contraer.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   O\
   Para expandir o contraer todas las agrupaciones simultáneamente, haga clic en la flecha **[!UICONTROL Expandir]** o **[!UICONTROL Contraer]** junto a cualquier agrupación mientras mantiene presionada la tecla [!UICONTROL Mayús].
