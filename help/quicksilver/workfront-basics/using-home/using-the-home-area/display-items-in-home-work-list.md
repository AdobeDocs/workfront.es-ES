---
product-area: projects
navigation-topic: use-the-home-area
title: Mostrar los elementos en la [!UICONTROL Lista de trabajo] en el área de inicio
description: La variable [!UICONTROL Lista de trabajo] en el [!UICONTROL Página principal] muestra todos los elementos de trabajo que están asignados a usted. Puede controlar qué elementos se muestran en la variable [!UICONTROL Trabajo] Haga una lista como se describe a continuación.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# Mostrar los elementos en la [!UICONTROL Lista de trabajo] en el área de inicio

La variable [!UICONTROL Lista de trabajo] en el [!UICONTROL Página principal] muestra todos los elementos de trabajo que están asignados a usted. Puede controlar qué elementos se muestran en la variable [!UICONTROL Trabajo] Haga una lista como se describe a continuación.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Review] solo para aprobaciones</p> <p>[!UICONTROL Work] o superior para todos los demás objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a proyectos, tareas, problemas y documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de Contribute o superior a las tareas y problemas en los que debe trabajar</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Filtre el [!UICONTROL Lista de trabajo]

Puede filtrar elementos en la variable [!UICONTROL Lista de trabajo] para ver solo tipos específicos de elementos. Por ejemplo, puede filtrar el [!UICONTROL Lista de trabajo] para mostrar solo problemas o solicitudes.

>[!NOTE]
>
>Las opciones de filtro se almacenan en el explorador. Si utiliza el mismo explorador de forma consistente en el mismo equipo (y no borra los datos del sitio), los filtros seleccionados no cambiarán. Si cambia de explorador o equipo, los filtros vuelven a la opción predeterminada, que es con todos los filtros desseleccionados.

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Página principal]**.
1. Haga clic en el **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png) menú desplegable.
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
      <td role="rowheader"><strong>[!UICONTROL Tareas En Las Que Se Trabaja]</strong></td> 
      <td> <p>Muestra solo las tareas en las que está trabajando activamente. Estas son tareas asignadas para las que ha hecho clic en el botón [!UICONTROL Work On It].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tareas listas para empezar]</strong></td> 
      <td> 
       <div> 
        <p>Muestra únicamente las tareas que están listas para su inicio. Las dos afirmaciones siguientes deben ser verdaderas:</p> 
        <ul> 
         <li> <p>Las tareas y sus padres no tienen predecesores ni limitaciones de tareas que les impidan trabajar en ellas.</p> </li> 
         <li> <p>La [!UICONTROL Fecha de inicio planeada] de las tareas se encuentra en el pasado o hasta dos semanas en el futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tareas no listas]</strong></td> 
      <td> 
       <div> 
        <p>Muestra solo las tareas que aún no están listas para iniciarse. Cualquiera de las siguientes afirmaciones debe ser verdadera:</p> 
        <ul> 
         <li> <p>Las tareas y sus padres pueden tener predecesores o restricciones de tareas que les impidan trabajar en ellas.</p> </li> 
         <li> <p>Las tareas tienen un [!UICONTROL Fecha de inicio planeada] que dura más de dos semanas en el futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas En Los Que Se Trabaja]</strong></td> 
      <td> <p>Muestra solo los problemas en los que está trabajando activamente. Estos son problemas asignados a usted para los que ha hecho clic en el botón [!UICONTROL Work On It].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas solicitados]</strong></td> 
      <td>Muestra solo los problemas que tiene asignados pero para los que no ha hecho clic en el botón [!UICONTROL Work On It].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personal</strong></td> 
      <td>Muestra solo las tareas personales. Estas son tareas que se crean como tarea de [!UICONTROL To Do], tal como se describe en la sección <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Crear una tarea personal</a> en el artículo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Crear elementos de trabajo desde el área [!UICONTROL Home]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aprobaciones]</strong></td> 
      <td> 
       <div> 
        <p>Muestra únicamente las aprobaciones asignadas o delegadas a usted y las aprobaciones que ha enviado. Las aprobaciones incluyen aprobaciones de elementos de trabajo (proyectos, tareas y problemas) y aprobaciones de documentos, pruebas, solicitudes de acceso y partes de horas. Para obtener más información sobre las aprobaciones, consulte los siguientes artículos:</p> 
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
      <td role="rowheader"><strong>[!UICONTROL Completado]</strong></td> 
      <td> <p>Muestra solo las tareas completadas, los problemas y las tareas personales. El trabajo completado se muestra para las dos semanas anteriores y se agrupa en la lista de trabajo según la semana en que se completaron. No se incluyen las aprobaciones.</p> <p>El trabajo completado está oculto en la [!UICONTROL Work List] a menos que seleccione este filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Las opciones de filtro se basan en objetos (tareas, problemas, aprobaciones, tareas personales).
   >* Las tareas y los problemas se filtran aún más por su estado en relación con nuestra disposición a trabajar en ellos ([!UICONTROL Trabajar con], [!UICONTROL Listo para empezar], [!UICONTROL No está listo] para tareas y [!UICONTROL Trabajar con] y [!UICONTROL Solicitado] para problemas). Puede seleccionar para mostrar tareas o problemas en un estado específico o hacer clic en Tareas o Problemas para seleccionar y mostrar todos los estados.
   >* Hay un filtro independiente para los elementos completados que incluye tanto tareas como problemas. Esto no incluye aprobaciones. La variable [!UICONTROL Completado] incluye tareas personales.
   >* Solo puede seleccionar un estado a la vez. Por ejemplo, solo puede mostrar [!UICONTROL Trabajar con] tareas y solo [!UICONTROL Solicitado] problemas.
   >* No puede aplicar filtros a los elementos asignados a uno de sus equipos y no se incluyen en los elementos que están asignados directamente a usted.



1. (Opcional) Organice más la [!UICONTROL Lista de trabajo], tal como se describe en la sección [Agrupar y ordenar por fecha, proyecto y prioridad](#group-and-sort-by-date-project-and-priority) en este artículo.

## Agrupar y ordenar por [!UICONTROL Fecha], [!UICONTROL Proyecto]y [!UICONTROL Prioridad]

Puede agrupar y ordenar el [!UICONTROL Lista de trabajo] por [!UICONTROL Fecha de finalización planeada], [!UICONTROL Fecha de confirmación], [!UICONTROL Proyecto]o [!UICONTROL Mi prioridad]. La opción que elija determina cómo se agrupan los elementos en la variable [!UICONTROL Lista de trabajo].

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Página principal]**.
1. Haga clic en el **[!UICONTROL Agrupar por]** menú desplegable.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Finalización planificada]</strong></td> 
      <td> <p> Los elementos se muestran en las siguientes agrupaciones de la [!UICONTROL Work List], en función de su [!UICONTROL Planned Completion Date] (el número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Sin fecha de finalización planificada]</p> </li> 
        <li> <p>[!UICONTROL Esta Semana]</p> <p>Esta agrupación se expande de forma predeterminada.</p> </li> 
        <li> <p>[!UICONTROL Próxima semana]</p> </li> 
        <li> <p>[!UICONTROL Planificado], seguido de varias [!UICONTROL Fechas de finalización previstas] (varias agrupaciones)</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Inicio planificado]</strong></td> 
      <td> <p>Los elementos se muestran en las siguientes agrupaciones de la [!UICONTROL Work List], en función de su [!UICONTROL Planned Start Date] (el número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Esta Semana] </p> <p>Esta agrupación se expande de forma predeterminada.</p> </li> 
        <li> <p>[!UICONTROL Próxima semana]</p> </li> 
        <li> <p>[!UICONTROL Planificado], seguido de varias [!UICONTROL Fechas de inicio planificadas] (varias agrupaciones)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fecha de confirmación]</strong></td> 
      <td> <p>Los elementos se muestran en las siguientes agrupaciones de la [!UICONTROL Work List] (el número de elementos contenidos en cada agrupación se muestra entre paréntesis junto al título del encabezado):</p> 
       <ul> 
        <li> <p>[!UICONTROL Sin fecha de confirmación]</p> </li> 
        <li> <p>[!UICONTROL Se Comprometió La Próxima Semana]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>Los elementos se agrupan según el proyecto y los proyectos aparecen alfabéticamente en la [!UICONTROL Work List]. (El número de elementos contenidos dentro de cada agrupación se muestra entre paréntesis junto al título del encabezado).</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Mi prioridad]</strong></td> 
      <td>Los elementos se muestran en el orden que elija. Para obtener más información, consulte <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Priorizar el trabajo en el área [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>El orden predeterminado es ascendente. Si cambia la ordenación a descendente , las opciones de clasificación seleccionadas se almacenan en el explorador. Si utiliza el mismo explorador de forma consistente en el mismo equipo (y no borra los datos del sitio), la ordenación no cambia, pero si cambia los navegadores o equipos, la clasificación cambia a la ordenación predeterminada.

## Ver elementos atrasados

[!DNL Adobe Workfront] utiliza las fechas siguientes para determinar si las solicitudes de trabajo están atrasadas:

* **Tareas**: [!UICONTROL Fecha de finalización planeada]
* **Problemas**: [!UICONTROL Fecha de finalización planeada]
* **Documentos**: [!UICONTROL Fecha de envío]
* **Hojas de tiempo**: [!UICONTROL Fecha de envío]
* **Aprobaciones**: [!UICONTROL Fecha de envío]
* **Aprobaciones de prueba**: [!UICONTROL Plazo de prueba]

## Busque la variable [!UICONTROL Lista de trabajo]

Al buscar en la variable [!UICONTROL Lista de trabajo], cualquier elemento asignado a usted se devuelve en la búsqueda (incluso los elementos que no están cargados actualmente en la pantalla). Si la variable [!UICONTROL Mostrar completado] está seleccionada, también se devolverán los elementos que haya marcado como completos en las últimas dos semanas.

Además, sólo se buscan los nombres de los elementos de trabajo (no se busca la información dentro del elemento de trabajo, ni tampoco los nombres de los proyectos en los que reside el elemento de trabajo).

Para buscar en el [!UICONTROL Lista de trabajo]:

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Página principal]**.
1. (Opcional) Filtre el [!UICONTROL Lista de trabajo], tal como se describe en [Filtre el [!UICONTROL Lista de trabajo]](#filter-the-work-list) y [Agrupar y ordenar por fecha, proyecto y prioridad](#group-and-sort-by-date-project-and-priority).

1. (Opcional) Si está buscando un elemento de trabajo que ya esté completo, debe configurar la variable [!UICONTROL Lista de trabajo] para mostrar los elementos completados antes de realizar la búsqueda.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Empiece a escribir el nombre del elemento que está buscando.\
   La variable [!UICONTROL Lista de trabajo] se filtra automáticamente para incluir elementos con un nombre coincidente.

## Cambiar el tamaño de la lista de trabajo

Puede cambiar el tamaño de la variable [!UICONTROL Lista de trabajo] para que consuma entre aproximadamente un cuarto del área de inicio y aproximadamente la mitad del [!UICONTROL Página principal] .

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Página principal]**.
1. Pase el ratón sobre el borde derecho del [!UICONTROL Lista de trabajo]y, a continuación, arrastre hacia la izquierda o hacia la derecha hasta que la lista de trabajo tenga el tamaño deseado.

## Contraer y expandir agrupaciones

Los elementos del [!UICONTROL Lista de trabajo] se muestran dentro de agrupaciones. Puede contraer y expandir agrupaciones para controlar la cantidad de información que se muestra en la página en un momento determinado.

Puede contraer y expandir agrupaciones dentro de [!UICONTROL Lista de trabajo] para controlar mejor qué información es visible.\
De forma predeterminada, la variable [!UICONTROL Esta semana] la agrupación se expande y todas las demás agrupaciones se contraen. Los cambios que realice se recordarán la próxima vez que acceda al área principal.

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Página principal]**.
1. Haga clic en el **[!UICONTROL Expandir]** o **[!UICONTROL Contraer]** flecha junto a cualquier agrupación que desee expandir o contraer.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   O\
   Para expandir o contraer todas las agrupaciones simultáneamente, haga clic en el botón **[!UICONTROL Expandir]** o **[!UICONTROL Contraer]** flecha junto a cualquier agrupación mientras mantiene presionada la tecla [!UICONTROL Mayús] clave.
