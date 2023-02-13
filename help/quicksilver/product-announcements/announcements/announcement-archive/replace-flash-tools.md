---
title: Sustitución de herramientas basadas en Flash en Adobe Workfront
description: Sustitución de herramientas basadas en Flash en Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 1%

---

# Sustitución de herramientas basadas en Flash en Adobe Workfront

Hemos eliminado todas las herramientas basadas en Flash de Adobe Workfront Classic.

Las herramientas de reemplazo basadas en los estándares actuales ya están disponibles en Workfront. Estos cambios coinciden con el final de la compatibilidad con los productos de Flash, tal como anunció el Adobe.

## Fechas importantes

Las siguientes fechas son importantes para el proceso de eliminación de todas las herramientas basadas en Flash de Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 de noviembre de 2020**: Todas las herramientas basadas en Flashes se han eliminado de todos los productos de Workfront.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Herramientas heredadas basadas en Flashes

Las herramientas enumeradas en las secciones siguientes se han eliminado del sistema Workfront y se han sustituido por nuevas soluciones.

Para obtener información sobre herramientas de reemplazo, consulte [Herramientas heredadas basadas en Flashes y sus reemplazos](#legacy-flash-based-tools-and-their-replacements) en este artículo.

### Administración de recursos

* La ficha Planificación de recursos heredados del área Personas y todas las herramientas que contiene la pestaña , que incluye lo siguiente:

   * Administrador de presupuesto de recursos
   * Planificador de capacidades
   * Estimaciones de recursos
   * Cuadrícula de recursos\
      Para obtener más información, consulte [Planificación de recursos en Adobe Workfront](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* Área Estimaciones de Recursos Heredadas en el Caso de Negocio de un proyecto

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

   .

* Subficha Cuadrícula de recursos de la ficha Dotación de personal de un proyecto
* La opción Usar nuevo área de programación de la subficha Programación de la ficha Dotación de un proyecto que elimina el área de programación heredada o el Generador de equipos. En este caso, la cronología de programación ahora se muestra de forma predeterminada.
* La pestaña Asignación en el perfil de usuario

### Informes

Se han eliminado las siguientes funciones e informes de informes:

* Se han eliminado las funciones de informes:

   * La opción Cuadrícula de recursos en un informe de usuario
   * La opción Gantt heredado de un informe de proyecto o tarea\
      Para obtener más información, consulte [Ver información en el diagrama de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Se han eliminado informes:

   * El informe Agrupamiento de recursos heredados
   * El informe Estimaciones de Recursos

   >[!NOTE]
   >
   >Todos los campos heredados a los que se accede mediante informes o a través de la API (grupo de recursos heredados, coste presupuestado heredado, coste preexistente, horas presupuestadas heredadas, coste laboral presupuestado heredado, etc.) se muestran en varios informes, pero no se rellenan con información nueva.

### Gantt anterior

* Todas las vistas de Gantt heredadas de listas de proyectos y tareas, así como las opciones de informes y informes
* Las subfichas Gantt heredadas en Portfolio y programas
* La subficha Gantt heredado de una lista de tareas de plantilla de una plantilla, la vista Gantt heredado de la ficha Subtareas de una tarea de plantilla y de un informe Tarea de plantilla

### Prueba

El visor de pruebas heredadas se ha sustituido por el nuevo visor de pruebas web y visor de pruebas de escritorio para la mayoría de los clientes, y se ha eliminado para todos los clientes en noviembre de 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Para obtener más información, consulte los siguientes recursos:

* [Revisar pruebas en el visor de pruebas web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Revise las pruebas en el Visor de pruebas de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## Herramientas heredadas basadas en Flashes y sus reemplazos {#legacy-flash-based-tools-and-their-replacements}

Salvo que se especifique lo contrario, todas las funciones heredadas se han sustituido por otras nuevas, como se muestra en la tabla siguiente.

>[!CAUTION]
>
>Las herramientas heredadas basadas en Flashes se han eliminado de todos los entornos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Herramientas heredadas</strong> </p> </th> 
   <th> <p><strong>Nuevas herramientas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Conjuntos de recursos de legado</strong> </p> <p>Los grupos de recursos heredados eran grupos o conjuntos de funciones de trabajo necesarias al mismo tiempo para la finalización de un proyecto. Las agrupaciones de recursos heredadas tenían varias deficiencias:</p> 
    <ul> 
     <li> Puede asociar un usuario con un grupo de recursos heredado, pero solo se utilizó para generar informes. Dado que los grupos de recursos heredados funcionaban con entidades de funciones de trabajo abstractas, no se tuvieron en cuenta las excepciones de programación de los usuarios ni el tiempo libre, lo que arrojó datos inexactos sobre la disponibilidad de recursos. </li> 
    </ul> 
    <ul> 
     <li>Solo puede especificar un grupo de recursos heredado por proyecto, lo que hace que varios grupos de recursos heredados admitan solo el flujo de grupos separados que trabajan de forma independiente entre sí y nunca comparten recursos. En todos los demás casos, se recomendó mantener un grupo de recursos heredado que incluyera todos los recursos del sistema, lo que provocó problemas de rendimiento con grandes cantidades de proyectos y datos.</li> 
    </ul> </td> 
   <td> <p><strong>Conjunto de recursos</strong> </p> <p>Los nuevos grupos de recursos son una colección de usuarios que se necesitan al mismo tiempo para completar el proyecto. Workfront también es consciente de que hay casos en los que los usuarios especializados necesitan que su trabajo se les asigne por separado. Por este motivo, ahora puede presupuestar usuarios en lugar de funciones de trabajo. </p> Las ventajas del grupo de recursos sobre los grupos de recursos heredados incluyen las siguientes: 
    <ul>
     <li>Debido a que los grupos de recursos se basan en los usuarios, su tiempo de espera y las excepciones de programación ya se tienen en cuenta para los cálculos de disponibilidad del usuario y de la función. Esto da lugar a datos precisos y actualizados, lo que permite tomar decisiones presupuestarias correctas y minimizar la probabilidad de cambios cuando el proyecto está en marcha.</li>
     <li>Dado que ahora hay más control sobre la disponibilidad de los recursos y la precisión de los datos, Workfront le permite asociar varios grupos de recursos con un proyecto. Un usuario también puede pertenecer a más de un grupo de recursos, en caso de que tenga varias habilidades que se puedan usar en varios proyectos al mismo tiempo. </li>
    </ul><p>Con este control sobre los datos, ya no es necesario tener un grupo de recursos que incluya todos los recursos para distribuir el presupuesto disponible. De hecho, no recomendamos esto. En su lugar, recomendamos diversificar los grupos de recursos y asociar solo los grupos de recursos relevantes con los proyectos.</p><p> Para obtener más información sobre los grupos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resumen de los grupos de recursos </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Administrador de presupuesto de recursos</strong> </p> <p>Puede utilizar el Administrador de presupuesto de recursos para especificar la disponibilidad de los recursos de funciones de trabajo en varios grupos de recursos. Sin embargo, debido a las deficiencias del grupo de recursos heredado, esta funcionalidad rara vez se utilizaba. Cuando se utiliza, obliga a los usuarios a introducir manualmente la disponibilidad de las funciones de trabajo para que la presupuestación sea más precisa. No se tuvieron en cuenta las excepciones de programación ni el tiempo libre de los usuarios.</p> </td> 
   <td> <p>Con el cálculo automático de la disponibilidad basado en los usuarios de los grupos de recursos, el Administrador de presupuesto de recursos ya no es necesario. La herramienta se ha eliminado, junto con todo el trabajo manual para calcular la disponibilidad.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimaciones de recursos</strong> </p> <p>La pestaña Estimaciones de Recursos de cada grupo de recursos heredados tenía el mismo propósito que el Administrador de presupuestos de recursos, solo en el contexto de un grupo de recursos heredado. Esta herramienta presentaba las mismas limitaciones que el Administrador de presupuesto de recursos y los grupos de recursos heredados: datos inexactos y entrada manual de disponibilidad. </p> </td> 
   <td> <p>Con el cálculo automático de la disponibilidad del usuario, las estimaciones de recursos han quedado obsoletas y se han eliminado.</p> <p>La herramienta se elimina en los grupos de recursos heredados y en las estimaciones de recursos heredados en el caso empresarial de un proyecto. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Planificador de capacidades</strong> </p> <p>El Planificador de Capacidad es un instrumento de Workfront para presupuestar recursos y priorizar proyectos dentro de un grupo de recursos heredado, según la disponibilidad de los recursos. Habida cuenta de la inexhaustividad de los datos procedentes de las estimaciones de recursos y del Administrador del presupuesto de recursos, que proporcionaban la información para el planificador de capacidad, era preciso comprobar la prioridad de los proyectos en relación con la disponibilidad de los usuarios.</p> <p>El uso de un único grupo de recursos heredado que incluía todas las funciones de trabajo en el sistema era el escenario más común, lo que llevaba a problemas de rendimiento con el planificador de capacidad tratando de cargar un gran número de proyectos.</p> </td> 
   <td> <p><strong>La vista de proyecto del planificador de recursos</strong> </p> <p>En la vista Basada en proyectos del planificador de recursos, puede presupuestar recursos y priorizar proyectos de manera similar a como lo hacía en el Planificador de capacidad heredado. A diferencia de la herramienta heredada, ahora se admiten más datos, y la información disponible es más precisa teniendo en cuenta tanto el tiempo libre de los usuarios como las excepciones de programación.</p> <p>La información disponible, planificada y presupuestada es visible de un vistazo, de modo que los gestores de recursos puedan ver si hay suficiente gente para hacer el trabajo y si los planes del proyecto exceden las estimaciones presupuestarias iniciales.</p> <p> Para obtener información sobre el uso de la vista de proyecto en el planificador de recursos, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del planificador de recursos</a></p> <p><strong>Planificador de escenario</strong> </p> <p>Para la planificación de la capacidad a largo plazo, el modelado de hipótesis alternativas y la priorización, también hemos presentado Workfront Scenario Planner . </p> <p>El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general del planificador de escenarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimaciones de recursos heredadas (caso empresarial)</strong> </p> <p>Puede utilizar el área Estimaciones de Recursos Heredadas del Caso de Negocio para presupuestar una cierta cantidad de horas de trabajo y costos como parte de la planificación del proyecto y la solicitud de recursos. Esta vista no ofrecía ninguna visibilidad sobre la disponibilidad de los recursos, lo que daba como resultado solicitudes aproximadas de recursos y un aumento de las posibilidades de trabajos de proyectos rechazados.</p> </td> 
   <td> <p><strong>Presupuesto de recursos (Caso empresarial)</strong> </p> <p>La sección Presupuestación de Recursos en el Caso de Negocio aporta capacidades de Planificador de Recursos al Caso de Negocio, lo que proporciona visibilidad sobre la disponibilidad de usuarios y funciones, así como la capacidad de presupuestar a nivel de usuario. </p> <p> Para obtener información sobre el área de Presupuestación de Recursos del caso empresarial, consulte <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Información general sobre las áreas del caso empresarial</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Informes de estimación de recursos</strong> </p> <p>Al utilizar las herramientas heredadas para la gestión de recursos, puede crear informes sobre las horas presupuestadas y planificadas desde el caso empresarial. Esto le permitía crear informes de matriz que mostrasen el trabajo total presupuestado y planeado para cada función de trabajo en un lapso de tiempo específico. Este informe no era editable y no se pudo realizar ningún cambio en la presupuestación de los recursos en función de las conclusiones del informe. </p> </td> 
   <td> <p><strong>Informe de uso</strong> </p> <p>El informe de utilización integrado muestra en paralelo Horario, Costo e Ingresos planeados, presupuestados y reales. </p> <p>Para obtener información sobre el uso del informe de utilización, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información de utilización de recursos </a>. </p> 
    <div> 
     <p><strong>Horas presupuestadas notificadas</strong> </p> 
     <p>Cree un informe de horas presupuestadas para revisar las horas presupuestadas en el Planificador de recursos en un formulario de informe. </p> 
     <p>Para obtener información sobre las horas presupuestadas, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glosario de terminología de Adobe Workfront</a>.</p> 
     <p>Para obtener información sobre cómo crear un informe, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> 
    </div> <p><strong>La vista de funciones del planificador de recursos</strong> </p> <p>Las horas presupuestadas y planificadas a partir del caso de negocio en las herramientas de administración de recursos heredadas ya están disponibles en una nueva vista nativa: la vista basada en roles del planificador de recursos. Esta vista proporciona información de horas disponibles, planificadas y presupuestadas de un vistazo y le permite controlar y cambiar la presupuestación en el mismo lugar. Esto garantiza una mejor toma de decisiones durante la planificación de funciones de alto nivel. </p> <p> Para obtener información sobre la presupuestación de recursos en la vista de funciones del planificador de recursos, consulte la <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Uso de las vistas Proyecto y Función para presupuestar recursos </a> en <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del planificador de recursos</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuadrícula de recursos</strong> </p> <p>La cuadrícula de recursos le da visibilidad sobre la asignación de usuarios específicos a medida que un proyecto avanza hacia su finalización. </p> <p>Por ejemplo, podría ver fácilmente cuándo alguien del equipo del proyecto hizo su trabajo antes de tiempo y cuándo alguien se quedó atrás, así como si estaban sobreasignados o subasignados durante un período de tiempo específico. </p> <p>Desafortunadamente, no se pudo actuar sobre la información en la misma vista. Para rectificar los problemas de sobreasignación, tuvo que ir a los proyectos y ajustar manualmente la información sin ninguna visibilidad del resultado de sus acciones.</p> </td> 
   <td> <p>La cuadrícula de recursos se ha sustituido por dos nuevas herramientas. Puede utilizar las siguientes herramientas, en función de la fase de planificación de recursos en la que se encuentre:</p> 
    <ul> 
     <li> <p><strong>Para la fase analítica:</strong> </p> 
      <ul> 
       <li> <p><strong>El equilibrador de carga de trabajo</strong>: Utilice el equilibrador de carga de trabajo para ver la carga de trabajo de los usuarios a un nivel más granular. Al utilizar el equilibrador de carga de trabajo, puede ver qué usuarios tienen disponibilidad en su carga de trabajo para completar la tarea a tiempo. Esto incluye su tiempo libre y los detalles de las excepciones de programación. </p> <p>Para obtener información sobre el equilibrador de carga de trabajo, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Información general del equilibrador de carga de trabajo</a>.</p> </li> 
       <li> <p><strong>La vista de usuario del planificador de recursos</strong><strong>:</strong> Cuando intente comprender en un nivel superior a qué proyectos están asignados sus usuarios, utilice la Vista de usuario del planificador de recursos. Esto le permite ver en qué están trabajando los usuarios, así como su sobreasignación y subasignación para un lapso de tiempo específico. El planificador de recursos también proporciona una visualización de la asignación general de usuarios en su conjunto, así como una visibilidad de las horas reales registradas, lo que resulta útil para analizar el progreso del trabajo realizado. </p> <p>Para obtener información sobre el uso de la Vista de usuario en el Planificador de recursos, consulte la <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Utilice la vista de usuario para ver las horas disponibles, planificadas y reales o FTE </a> en <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del planificador de recursos</a></p> </li> 
      </ul> </li> 
     <li><strong>Para la fase táctica:</strong> 
      <ul> 
       <li><strong>El equilibrador de carga de trabajo</strong> Puede hacer lo siguiente mediante el equilibrador de carga de trabajo: 
        <ul>
         <li>Asignar trabajo a los usuarios.</li>
         <li>Administre las asignaciones de los usuarios a los elementos de trabajo. </li>
         <li>Comparta el equilibrador de carga de trabajo con otros usuarios que pueden no tener visibilidad del área Personas. Utilice la funcionalidad de vínculo compartible para compartir un vínculo con el equilibrador de carga de trabajo e incrustarlo en paneles personalizados. Cualquier usuario con acceso a Ver usuarios puede ver estos tableros cuando los comparta.</li>
        </ul><p>El equilibrador de carga de trabajo está disponible en el área Personas. </p><p>Para obtener información sobre el equilibrador de carga de trabajo, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Información general del equilibrador de carga de trabajo</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Diagrama de Gantt heredado, Lista de tareas</strong> </p> <p> El diagrama de Gantt heredado de la lista de tareas permitía a los usuarios ver la cronología del proyecto y realizar la planificación del escenario de alternativas sin comprometer cambios en la base de datos. El diagrama de Gantt heredado se basaba en la tecnología de Flash, que presentaba riesgos de seguridad. </p> </td> 
   <td> <p><strong>Diagrama de Gantt,</strong> <strong>Lista de tareas</strong></p> <p> El nuevo diagrama de Gantt basado en HTML tiene el mismo propósito que el Gantt heredado. Los usuarios pueden visualizar la línea de tiempo del proyecto y realizar la planificación del escenario de alternativas sin comprometer cambios en la base de datos cambiando a la opción Guardar manual de la barra de herramientas de la lista de tareas. </p> <p>El nuevo diagrama de Gantt es interactivo cuando se utiliza la opción Autoguardar, que puede utilizar cuando desee guardar automáticamente los cambios a medida que se producen. </p> <p>El nuevo diagrama de Gantt de Lista de Tareas se basa en la tecnología más reciente y es fiable. Este nuevo diagrama de Gantt se encuentra directamente en la lista de tareas y es fácil acceder a él mientras trabaja en la lista de tareas sin cambiar las pestañas o cambiar la vista. </p> <p>Aunque el nuevo diagrama de Gantt ofrece la misma funcionalidad que el gráfico anterior, hay algunas diferencias en las características en comparación con el Gantt heredado. </p> <p> La subficha Gantt heredado de una lista de Tareas de plantilla en una plantilla, la vista Gantt heredado de la ficha Subtareas de una tarea de plantilla y el diagrama de Gantt heredado de un informe Tarea de plantilla también se han sustituido por el diagrama de Gantt basado en el HTML. </p> <p>Si utiliza el Diagrama de Gantt heredado principalmente para la vista simple y las ediciones rápidas y no utiliza el gráfico real, la nueva opción Planificación de línea de tiempo le permite realizar cambios rápidos en los campos de planificación clave. Puede seleccionar Planificación de línea de tiempo en lugar de Autoguardar en la barra de herramientas de la lista de tareas.</p> <p>Para obtener más información sobre cómo guardar una lista de tareas mediante la opción Planificación de línea de tiempo, consulte la sección "Guardar cambios en una lista de tareas manualmente al seleccionar la opción Planificación de línea de tiempo" en el artículo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tareas en una lista</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Diagrama de Gantt heredado para una lista de proyectos</strong> </p> <p>El diagrama de Gantt heredado de la lista de proyectos permite a los usuarios ver los proyectos y sus tareas en una sola vista. Sin abandonar el contexto de la lista de proyectos, los usuarios podían ver detalles sobre las tareas de un proyecto, así como las dependencias entre los proyectos. El diagrama de Gantt heredado de la lista de proyectos se basaba en la tecnología de Flash, que presentaba riesgos de seguridad. </p> </td> 
   <td> <p><strong>Diagrama de Gantt, Lista de proyectos</strong> </p> <p>El diagrama de Gantt basado en HTML tiene el mismo propósito que el diagrama de Gantt heredado. Los usuarios pueden ver los proyectos y sus tareas en una vista para identificar visualmente las dependencias entre los proyectos y las tareas. El diagrama de Gantt Lista de proyectos se encuentra directamente en la lista de proyectos. El nuevo diagrama de Gantt tiene una interfaz moderna y se basa en la tecnología más reciente.</p> <p>Para obtener información sobre el diagrama de Gantt de la lista de proyectos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Ver información en el diagrama de Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuadros de diálogo compartidos para informes, calendarios y documentos</strong> </p> <p>Al compartir informes, calendarios y documentos, los cuadros de diálogo utilizados se basaban en la tecnología de Flash.</p> </td> 
   <td> <p>La experiencia al compartir informes, calendarios y documentos en Workfront no ha cambiado. Sin embargo, la experiencia ya no depende del Flash.</p> <p>Para obtener más información sobre cómo compartir estos elementos, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre cómo compartir permisos en objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visor de pruebas heredado</strong> </p> <p>El visor de pruebas heredadas era un visor de pruebas basado en la web que proporcionaba funciones de prueba para pruebas estáticas, de vídeo y de interacción.</p> </td> 
   <td> <p><strong>Visor de pruebas web y Visor de pruebas de escritorio</strong> </p> <p>El visor de pruebas web proporciona funciones de prueba para pruebas estáticas y de vídeo.</p> <p>El Visor de prueba de escritorio proporciona funciones de prueba para pruebas interactivas, además de ofrecer compatibilidad total con pruebas estáticas y de vídeo.</p> <p>El formato del archivo SWF ya no es compatible con ninguno de los principales proveedores y se ha sustituido por banners HTML5 para pruebas. </p> <p>Para obtener información más detallada sobre las diferencias entre los visualizadores de pruebas disponibles, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Diferencias entre el visor de pruebas web y el visor de pruebas de escritorio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
