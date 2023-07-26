---
product-area: projects
navigation-topic: use-the-home-area
title: Mostrar elementos en [!UICONTROL Lista de trabajos] en el área de Inicio
description: El [!UICONTROL Lista de trabajos] en el [!UICONTROL Inicio] muestra todos los elementos de trabajo que tiene asignados. Puede controlar qué elementos se muestran en la [!UICONTROL Trabajo] Enumere como se describe a continuación.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 0%

---

# Mostrar elementos en [!UICONTROL Lista de trabajos] en el área de Inicio

El [!UICONTROL Lista de trabajos] en el [!UICONTROL Inicio] muestra todos los elementos de trabajo que tiene asignados. Puede controlar qué elementos se muestran en la [!UICONTROL Trabajo] Enumere como se describe a continuación.

>[!NOTE]
>
>Al convertir un problema en una tarea o un proyecto, el problema se elimina del área de Inicio del usuario asignado al problema.
>
>Al convertir una tarea en un proyecto, la tarea se elimina y esta se elimina del área de Inicio del usuario asignado a la tarea.


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
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos, Tareas, Problemas y Documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Aportar permisos o superiores a las tareas y problemas en los que necesita trabajar</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Filtrar el [!UICONTROL Lista de trabajos]

Puede filtrar elementos en la variable [!UICONTROL Lista de trabajos] para ver sólo tipos específicos de elementos. Por ejemplo, puede filtrar la variable [!UICONTROL Lista de trabajos] para mostrar solo problemas o solicitudes.

>[!NOTE]
>
>Las opciones de filtro se almacenan en el explorador. Si utiliza el mismo explorador de forma constante en el mismo equipo (y no borra los datos del sitio), los filtros seleccionados no cambian. Si cambia de navegador o de ordenador, los filtros vuelven a la opción predeterminada, que es la que no está seleccionada para todos los filtros.

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en **[!UICONTROL Filtrar]** ![](assets/filter-nwepng.png) menú desplegable.
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
      <td role="rowheader"><strong>Tareas de [!UICONTROL en curso]</strong></td> 
      <td> <p>Muestra únicamente las tareas en las que está trabajando activamente. Son tareas asignadas para las que ha hecho clic en el botón [!UICONTROL Trabajar en ello].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tareas listas para iniciarse]</strong></td> 
      <td> 
       <div> 
        <p>Muestra sólo las tareas que están listas para iniciarse. Las dos afirmaciones siguientes deben ser verdaderas:</p> 
        <ul> 
         <li> <p>Las tareas y sus tareas principales no tienen predecesoras ni restricciones de tarea que impidan trabajar con ellas.</p> </li> 
         <li> <p>La [!UICONTROL Fecha planificada de inicio] de las tareas se encuentra en las últimas o hasta dos semanas en el futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tareas no listas]</strong></td> 
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
      <td role="rowheader"><strong>[!UICONTROL Problemas en funcionamiento]</strong></td> 
      <td> <p>Muestra únicamente los problemas en los que está trabajando activamente. Estos son problemas asignados a usted para los que ha hecho clic en el botón [!UICONTROL Trabajar en ello].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas solicitados]</strong></td> 
      <td>Muestra sólo los problemas que tiene asignados pero para los que no ha hecho clic en el botón [!UICONTROL Trabajar en ello].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personal</strong></td> 
      <td>Muestra sólo las tareas personales. Son tareas que se crean como una tarea de [!UICONTROL Tareas pendientes], tal como se describe en la sección <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Crear una tarea personal</a> en el artículo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Crear elementos de trabajo desde el área de [!UICONTROL Home]</a>.</td> 
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
      <td role="rowheader"><strong>[!UICONTROL completado]</strong></td> 
      <td> <p>Muestra sólo las tareas, problemas y tareas personales completados. El trabajo completado se muestra durante las dos semanas anteriores y se agrupa en la Lista de trabajos según la semana en que se completaron. No se incluyen las aprobaciones.</p> <p>El trabajo completado está oculto en la Lista de trabajos de [!UICONTROL] a menos que seleccione este filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Las opciones de filtro se basan en objetos (tareas, problemas, aprobaciones, tareas personales).
   >* Las tareas y los problemas se filtran aún más por su estado en relación con nuestra disposición a trabajar en ellos ([!UICONTROL Trabajando en], [!UICONTROL Listo para empezar], [!UICONTROL No está listo] para tareas, y [!UICONTROL Trabajando en] y [!UICONTROL Solicitado] para problemas). Puede seleccionar mostrar tareas o problemas en un estado específico o hacer clic en Tareas o Problemas para seleccionar y mostrar todos los estados.
   >* Hay un filtro independiente para los elementos completados que incluye tareas y problemas. Esto no incluye las aprobaciones. El [!UICONTROL Completado] El filtro incluye las tareas personales.
   >* Solo se puede seleccionar un estado a la vez. Por ejemplo, solo puede mostrar [!UICONTROL Trabajando en] tareas y solo [!UICONTROL Solicitado] problemas.
   >* No puede aplicar filtros a los elementos asignados a uno de sus equipos y no se incluyen en los elementos que se le han asignado directamente.


1. (Opcional) Siga organizando las [!UICONTROL Lista de trabajos], tal como se describe en la sección [Agrupar y ordenar por fecha, proyecto y prioridad](#group-and-sort-by-date-project-and-priority) en este artículo.

## Agrupar y ordenar por [!UICONTROL Fecha], [!UICONTROL Proyecto], y [!UICONTROL Prioridad]

Puede agrupar y ordenar las variables [!UICONTROL Lista de trabajos] por [!UICONTROL Fecha planificada de finalización], [!UICONTROL Fecha de confirmación], [!UICONTROL Proyecto], o [!UICONTROL Mi prioridad]. La opción que elija determina cómo se agrupan los elementos en la variable [!UICONTROL Lista de trabajos].

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en **[!UICONTROL Agrupar por]** menú desplegable.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

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
      <td>Los artículos se muestran en el orden que elija. Para obtener más información, consulte <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Priorizar el trabajo en el área de [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>El orden predeterminado es ascendente. Si cambia la ordenación a descendente , las opciones de ordenación seleccionadas se almacenan en el explorador. Si utiliza el mismo explorador de forma constante en el mismo equipo (y no borra los datos del sitio), la ordenación no cambia, pero si cambia de explorador o de equipo, la ordenación cambia a la predeterminada.

## Ver elementos atrasados

[!DNL Adobe Workfront] utiliza las fechas siguientes para determinar si las solicitudes de trabajo están atrasadas:

* **Tareas**: [!UICONTROL Fecha planificada de finalización]
* **Problemas**: [!UICONTROL Fecha planificada de finalización]
* **Documentos**: [!UICONTROL Fecha de envío]
* **Plantillas de horas**: [!UICONTROL Fecha de envío]
* **Aprobaciones**: [!UICONTROL Fecha de envío]
* **Aprobaciones de revisión**: [!UICONTROL Plazo de prueba]

## Busque en [!UICONTROL Lista de trabajos]

Al buscar en [!UICONTROL Lista de trabajos], todos los elementos asignados a usted se devolverán en la búsqueda (incluso los elementos que no estén cargados actualmente en la pantalla). Si la variable [!UICONTROL Mostrar finalizados] está seleccionada, también se devolverán todos los elementos que haya marcado como completados en las últimas dos semanas.

Además, sólo se buscan los nombres de los elementos de trabajo (no se busca información dentro del elemento de trabajo, ni tampoco los nombres de los proyectos en los que reside el elemento de trabajo).

Para buscar en [!UICONTROL Lista de trabajos]:

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Inicio]**.
1. (Opcional) Filtre la variable [!UICONTROL Lista de trabajos], tal como se describe en [Filtrar el [!UICONTROL Lista de trabajos]](#filter-the-work-list) y [Agrupar y ordenar por fecha, proyecto y prioridad](#group-and-sort-by-date-project-and-priority).

1. (Opcional) Si está buscando un elemento de trabajo que ya se ha completado, debe configurar la variable [!UICONTROL Lista de trabajos] para mostrar los elementos completados antes de buscar.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Empiece a escribir el nombre del elemento que está buscando.\
   El [!UICONTROL Lista de trabajos] se filtra automáticamente para incluir elementos con un nombre que coincida.

## Cambiar el tamaño de la Lista de trabajos

Puede cambiar el tamaño de la [!UICONTROL Lista de trabajos] para que consuma entre un cuarto del área de inicio y la mitad del [!UICONTROL Inicio] área.

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Inicio]**.
1. Pase el ratón por encima del borde derecho del [!UICONTROL Lista de trabajos]A continuación, arrastre hacia la izquierda o la derecha hasta que la Lista de trabajos tenga el tamaño deseado.

## Contraer y expandir agrupaciones

Elementos en la [!UICONTROL Lista de trabajos] se muestran dentro de las agrupaciones. Puede contraer y expandir las agrupaciones para controlar cuánta información se muestra en la página en un momento determinado.

Puede contraer y expandir agrupaciones dentro del [!UICONTROL Lista de trabajos] para controlar mejor qué información es visible.\
De forma predeterminada, la variable [!UICONTROL Esta semana] La agrupación se expande y todas las demás agrupaciones se contraen. Cualquier cambio que realice se recordará la próxima vez que acceda al área de Inicio.

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en **[!UICONTROL Expandir]** o **[!UICONTROL Contraer]** junto a cualquier agrupación que desee expandir o contraer.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   O\
   Para expandir o contraer todas las agrupaciones simultáneamente, haga clic en **[!UICONTROL Expandir]** o **[!UICONTROL Contraer]** flecha junto a cualquier agrupación mientras mantiene pulsada la tecla [!UICONTROL Shift] clave.
