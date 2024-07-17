---
title: Reemplazo de herramientas basadas en Flash en Adobe Workfront
description: Reemplazo de herramientas basadas en Flash en Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '2701'
ht-degree: 0%

---

# Reemplazo de herramientas basadas en Flash en Adobe Workfront

Hemos eliminado todas las herramientas basadas en Flash de Adobe Workfront Classic.

Las herramientas de reemplazo basadas en los estándares actuales ya están disponibles en Workfront. Estos cambios se alinean con el fin de la compatibilidad con los productos de Flash según lo anunciado por el Adobe.

## Fechas importantes

Las siguientes fechas son importantes para el proceso de eliminación de todas las herramientas basadas en Flash en Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 de noviembre de 2020**: se han eliminado todas las herramientas basadas en Flash de todos los productos de Workfront.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Herramientas heredadas basadas en Flash

Las herramientas enumeradas en las secciones siguientes se han eliminado del sistema de Workfront y se han sustituido por nuevas soluciones.

Para obtener información acerca de las herramientas de reemplazo, vea [Herramientas heredadas basadas en Flash y sus reemplazos](#legacy-flash-based-tools-and-their-replacements) en este artículo.

### Administración de recursos

* La pestaña Planificación de recursos de legado del área Personas y todas las herramientas que contiene, que incluye lo siguiente:

   * Administrador de presupuesto de recursos
   * Planificador de capacidades
   * Estimaciones de recursos
   * Cuadrícula de recursos\
     Para obtener más información, vea [Planificación de recursos: índice de artículo](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* El área Estimaciones de recursos de legado en el caso comercial de un proyecto

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

* La subpestaña Cuadrícula de recursos de la pestaña Asignación de personal de un proyecto
* La opción Utilizar nueva área de programación de la subpestaña Programación de la pestaña Asignación de personal de un proyecto que elimina el área de programación heredada o el Generador de equipos. En este caso, la cronología de programación ahora se muestra de forma predeterminada.
* La pestaña Asignación en el perfil de usuario

### Informes

Se han eliminado las siguientes funciones e informes de informes:

* Funciones de sistema de informes eliminadas:

   * La opción Cuadrícula de recursos en un informe de usuario
   * La opción Gantt anterior en un informe de proyecto o tarea\
     Para obtener más información, vea [Ver información en el diagrama de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Informes eliminados:

   * Informe Conjunto de recursos de legado
   * El informe Estimaciones de recursos

  >[!NOTE]
  >
  >Todos los campos heredados a los que se accede a través de los informes o a través de la API (Conjunto de recursos heredado, Costo presupuestado heredado, Costo preexistente, Horas presupuestadas heredadas, Costo de mano de obra presupuestado heredado, etc.) se muestran en varios informes, pero no se rellenan con información nueva.

### Gantt anterior

* Todas las vistas Gantt heredadas de las listas de proyectos y tareas, así como las opciones de informes e informes
* Las subpestañas de Gantt heredadas en Portfolio y programas
* La subpestaña Gantt heredado en una lista de Tareas de plantilla en una Plantilla, la vista Gantt heredado en la pestaña Subtareas de una Tarea de plantilla y en un informe de Tarea de plantilla

### Revisión

El visor de revisión heredado se ha reemplazado con el nuevo Visor de revisión web y el Visor de revisión de escritorio para la mayoría de los clientes, y se eliminó para todos los clientes en noviembre de 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Para obtener más información, consulte los siguientes recursos:

* [Revisar pruebas en el Visor de revisiones web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Revisar pruebas en el Visor de revisiones de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

## Herramientas heredadas basadas en Flashes y sus sustitutos {#legacy-flash-based-tools-and-their-replacements}

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
   <td> <p><strong>Conjuntos de recursos de legado</strong> </p> <p>Los conjuntos de recursos de legado eran grupos o colecciones de funciones de trabajo necesarias al mismo tiempo para la finalización de un proyecto. Los Conjuntos de recursos de legado tenían una serie de deficiencias:</p> 
    <ul> 
     <li> Puede asociar un usuario con un conjunto de recursos heredados, pero solo se utilizó para la creación de informes. Dado que los conjuntos de recursos de legado funcionaban con entidades de funciones abstractas, no se tuvieron en cuenta las excepciones de horario y los días libres de los usuarios, lo que resultó en datos inexactos sobre la disponibilidad de los recursos. </li> 
    </ul> 
    <ul> 
     <li>Puede especificar solamente un conjunto de recursos de legado por proyecto, lo que resultó en varios conjuntos de recursos de legado que solo admiten el flujo de grupos separados que trabajan de forma independiente entre sí y nunca comparten recursos. En todos los demás casos, se recomendó mantener un conjunto de recursos de legado que incluyera todos los recursos en el sistema, lo que ocasionaba problemas de rendimiento con grandes cantidades de proyectos y datos.</li> 
    </ul> </td> 
   <td> <p><strong>Conjunto de recursos</strong> </p> <p>Los nuevos conjuntos de recursos son una colección de usuarios que se necesitan al mismo tiempo para completar el proyecto. Workfront también es consciente de que hay casos en los que los usuarios especializados necesitan que les asignen trabajo por separado. Por este motivo, ahora puede presupuestar usuarios en lugar de funciones del puesto. </p> Entre las ventajas del conjunto de recursos con respecto a los conjuntos de recursos de legado se incluyen las siguientes: 
    <ul>
     <li>Dado que los conjuntos de recursos se basan en los usuarios, su tiempo libre y las excepciones de horario ya se tienen en cuenta para los cálculos de disponibilidad de usuarios y funciones. Esto da como resultado datos precisos y actualizados, lo que permite tomar decisiones presupuestarias correctas y minimizar la probabilidad de cambios cuando el proyecto está en marcha.</li>
     <li>Dado que ahora hay más control sobre la disponibilidad de los recursos y la precisión de los datos, Workfront le permite asociar varios conjuntos de recursos con un proyecto. Un usuario también puede pertenecer a más de un conjunto de recursos, en caso de que tenga varias aptitudes que se puedan utilizar en varios proyectos al mismo tiempo. </li>
    </ul><p>Con este control sobre los datos, ya no es necesario tener un conjunto de recursos que incluya todos los recursos para distribuir el presupuesto disponible. De hecho, no se recomienda. En su lugar, recomendamos diversificar sus conjuntos de recursos y asociar únicamente los conjuntos de recursos relevantes con los proyectos.</p><p> Para obtener más información sobre los conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Información general sobre los conjuntos de recursos </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Administrador de presupuesto de recursos</strong> </p> <p>Puede utilizar el Administrador de presupuesto de recursos para especificar la disponibilidad de los recursos de funciones en varios conjuntos de recursos. Sin embargo, debido a las deficiencias del Conjunto de recursos de legado, esta funcionalidad rara vez se utilizaba. Cuando se utilizaba, obligaba a los usuarios a introducir manualmente la disponibilidad de las funciones del puesto para hacer que la presupuestación fuera más precisa. No se tuvieron en cuenta las excepciones de horario ni el tiempo libre de los usuarios.</p> </td> 
   <td> <p>Con el cálculo automático de la disponibilidad basado en los usuarios de los conjuntos de recursos, el Administrador de presupuesto de recursos ya no es necesario. Se ha eliminado la herramienta, junto con todo el trabajo manual para calcular la disponibilidad.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimaciones de recursos</strong> </p> <p>La pestaña Estimaciones de recursos de cada conjunto de recursos de legado tenía el mismo propósito que el Administrador de presupuesto de recursos, solo en el contexto de un conjunto de recursos de legado. Esta herramienta presentaba las mismas limitaciones que el Administrador de presupuesto de recursos y los Conjuntos de recursos de legado: datos inexactos y entrada manual de disponibilidad. </p> </td> 
   <td> <p>Con el cálculo automático de la disponibilidad de los usuarios, las estimaciones de recursos han quedado obsoletas y se han eliminado.</p> <p>La herramienta se elimina en los conjuntos de recursos de legado y en las estimaciones de recursos de legado en el caso empresarial de un proyecto. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Planificador de capacidades</strong> </p> <p>El Planificador de capacidades era una herramienta de Workfront para presupuestar recursos y priorizar proyectos dentro de un Conjunto de recursos heredados, de acuerdo con la disponibilidad de los recursos. Dado que los datos de las estimaciones de recursos y del Administrador del presupuesto de recursos que proporcionaban la información para el Planificador de capacidades eran incompletos, había que verificar dos veces la prioridad de los proyectos en relación con la disponibilidad de los usuarios.</p> <p>El uso de un único conjunto de recursos de legado que incluyera todas las funciones del puesto en el sistema era el escenario más común, lo que producía problemas de rendimiento con el Planificador de capacidades al intentar cargar un gran número de proyectos.</p> </td> 
   <td> <p><strong>Vista de proyecto del Planificador de recursos</strong> </p> <p>En la vista basada en proyectos del Planificador de recursos, puede presupuestar recursos y priorizar proyectos de manera similar a como lo hacía en el Planificador de capacidades de legado. A diferencia de la herramienta heredada, ahora se admiten más datos, y la información disponible es más precisa, ya que tiene en cuenta el tiempo libre de los usuarios y las excepciones de programación.</p> <p>La información disponible, planificada y presupuestada se puede ver de un vistazo para que los administradores de recursos puedan ver si hay suficientes personas para realizar el trabajo y si los planes del proyecto superan las estimaciones presupuestarias iniciales.</p> <p> Para obtener información sobre el uso de la vista de proyecto en el Planificador de recursos, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resumen del planificador de recursos</a></p> <p><strong>Planificador de escenarios</strong> </p> <p>Para la planificación de la capacidad a largo plazo, el modelado de escenarios hipotéticos y la priorización, también hemos presentado Workfront Scenario Planner . </p> <p>El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general sobre el Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimaciones de recursos de legado (caso comercial)</strong> </p> <p>Puede utilizar el área Estimaciones de recursos de legado del caso empresarial para presupuestar una cierta cantidad de horas de trabajo y costos como parte de la planificación del proyecto y la solicitud de recursos. Esta vista no proporcionó ninguna visibilidad sobre la disponibilidad de recursos, lo que resultó en solicitudes aproximadas de recursos y una mayor oportunidad de trabajo de proyecto rechazado.</p> </td> 
   <td> <p><strong>Presupuesto de recursos (caso comercial)</strong> </p> <p>La sección Presupuestación de recursos del caso empresarial aporta las funciones del Planificador de recursos al caso empresarial, proporcionando visibilidad sobre la disponibilidad de usuarios y funciones, así como la capacidad de realizar presupuestos a nivel de usuario. </p> <p> Para obtener información acerca del área de presupuesto de recursos del caso comercial, vea <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Descripción general de las áreas del caso comercial</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Informes de estimación de recursos</strong> </p> <p>Al utilizar las herramientas heredadas para la Administración de recursos, puede informar sobre las horas presupuestadas y planificadas a partir del caso empresarial. Esto le permitía crear informes en matriz que mostraban el trabajo total presupuestado y planificado para cada rol en un lapso de tiempo específico. Este informe no se podía editar y no se podía realizar ningún cambio en el presupuesto de los recursos según los resultados del informe. </p> </td> 
   <td> <p><strong>Informe de utilización</strong> </p> <p>El informe integrado Utilización muestra en paralelo las horas planificadas, las presupuestadas y las reales, los costes y los ingresos. </p> <p>Para obtener información acerca del uso del informe Utilización, vea <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información de utilización de recursos </a>. </p> 
    <div> 
     <p><strong>Horas presupuestadas reportables</strong> </p> 
     <p>Cree un informe de horas presupuestadas para revisar las horas presupuestadas en el Planificador de recursos en un formulario de informe. </p> 
     <p>Para obtener información sobre las horas presupuestadas, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glosario de terminología de Adobe Workfront</a>.</p> 
     <p>Para obtener información sobre cómo crear un informe, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> 
    </div> <p><strong>La vista de rol del Planificador de recursos</strong> </p> <p>Las horas presupuestadas y planificadas del caso empresarial en las herramientas de Administración de recursos de legado ahora están disponibles en una nueva vista nativa: la vista basada en roles del Planificador de recursos. Esta vista proporciona información rápida sobre las horas disponibles, planificadas y presupuestadas y le permite controlar y cambiar las horas presupuestadas en el mismo lugar. Esto garantiza una mejor toma de decisiones durante la planificación de funciones de alto nivel. </p> <p> Para obtener información acerca de cómo presupuestar recursos en la vista de rol del Planificador de recursos, vea la sección <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Usar las vistas de proyecto y rol para presupuestar recursos </a> en <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del Planificador de recursos</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuadrícula de recursos</strong> </p> <p>La cuadrícula de recursos le da visibilidad de la asignación de usuarios específicos a medida que un proyecto progresa hacia la finalización. </p> <p>Por ejemplo, podría ver fácilmente cuándo alguien del equipo del proyecto terminó su trabajo temprano y cuándo alguien se retrasó, así como si se le asignó demasiado o menos de lo necesario para un período de tiempo específico. </p> <p>Desafortunadamente, no ha podido modificar la información de la misma vista. Para corregir los problemas de sobreasignación tenía que ir a los proyectos y ajustar manualmente la información allí sin ninguna visibilidad del resultado de sus acciones.</p> </td> 
   <td> <p>La cuadrícula de recursos se ha reemplazado con dos nuevas herramientas. Puede utilizar las siguientes herramientas, en función de la fase de planificación de recursos en la que se encuentre:</p> 
    <ul> 
     <li> <p><strong>Para la fase analítica:</strong> </p> 
      <ul> 
       <li> <p><strong>Distribuidor de cargas de trabajo</strong>: use el Distribuidor de cargas de trabajo para ver la carga de trabajo de los usuarios en un nivel más granular. Al utilizar el Distribuidor de cargas de trabajo, puede ver qué usuarios tienen disponibilidad en su carga de trabajo para completar la tarea a tiempo. Esto incluye los detalles de sus días libres y excepciones de horario. </p> <p>Para obtener información sobre el Distribuidor de cargas de trabajo, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Resumen del Distribuidor de cargas de trabajo</a>.</p> </li> 
       <li> <p><strong>La vista de usuario del Planificador de recursos</strong><strong>:</strong> Al intentar comprender en un nivel superior a qué proyectos están asignados los usuarios, use la vista de usuario del Planificador de recursos. Esto le permite ver en qué están trabajando los usuarios, así como su asignación excesiva o insuficiente para un lapso de tiempo específico. El Planificador de recursos también proporciona una visualización de la asignación general de los usuarios en su conjunto, así como visibilidad de las horas reales registradas, lo cual resulta útil para analizar el progreso del trabajo realizado. </p> <p>Para obtener información sobre el uso de la vista de usuario en el Planificador de recursos, vea la sección <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Usar la vista de usuario para ver las horas disponibles, planificadas y reales o las jornadas completas </a> en <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del Planificador de recursos</a></p> </li> 
      </ul> </li> 
     <li><strong>Para la fase táctica:</strong> 
      <ul> 
       <li><strong>Distribuidor de cargas de trabajo</strong> Puede hacer lo siguiente mediante el Distribuidor de cargas de trabajo: 
        <ul>
         <li>Asignar trabajo a los usuarios.</li>
         <li>Administrar asignaciones de usuarios a elementos de trabajo. </li>
         <li>Comparta el Distribuidor de cargas de trabajo con otros usuarios que pueden no tener visibilidad del área de Personas. Utilice la funcionalidad de vínculo compartido para compartir un vínculo al Distribuidor de cargas de trabajo e incrustarlo en paneles personalizados. Los usuarios con acceso a Ver usuarios pueden ver estos paneles cuando los comparta.</li>
        </ul><p>El Distribuidor de cargas de trabajo está disponible en el área Personas. </p><p>Para obtener información sobre el Distribuidor de cargas de trabajo, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Resumen del Distribuidor de cargas de trabajo</a>.</p></li> 
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
   <td> <p><strong>Gráfico Gantt heredado, lista de tareas</strong> </p> <p> El diagrama de Gantt heredado de la lista de tareas permite a los usuarios ver visualmente la cronología del proyecto y realizar la planificación de escenarios hipotéticos sin confirmar los cambios en la base de datos. El gráfico Gantt anterior se basaba en la tecnología de Flash, que presentaba riesgos para la seguridad. </p> </td> 
   <td> <p><strong>Gráfico Gantt,</strong> <strong>Lista de tareas</strong></p> <p> El nuevo diagrama de Gantt basado en el HTML sirve para el mismo propósito que el diagrama de Gantt heredado. Los usuarios pueden visualizar la cronología del proyecto y realizar la planificación de escenarios hipotéticos sin confirmar los cambios en la base de datos cambiando a la opción Guardar de forma manual en la barra de herramientas de la lista de tareas. </p> <p>El nuevo gráfico Gantt es interactivo cuando se utiliza la opción de guardado automático, que puede utilizar cuando desee guardar automáticamente los cambios a medida que se producen. </p> <p>El nuevo gráfico Gantt de lista de tareas se basa en la tecnología más reciente y es fiable. Este nuevo gráfico Gantt se encuentra directamente en la lista de tareas y se accede fácilmente a él mientras trabaja en la lista de tareas sin cambiar de pestaña ni cambiar de vista. </p> <p>Aunque el nuevo gráfico Gantt ofrece la misma funcionalidad que el anterior, hay algunas diferencias en las características en comparación con el Gantt anterior. </p> <p> La subpestaña Gantt heredado de una lista de tareas de plantilla de una plantilla, la vista Gantt heredado de la pestaña Subtareas de una tarea de plantilla y el diagrama de Gantt heredado de un informe de tareas de plantilla también se han sustituido por el diagrama de Gantt basado en el HTML. </p> <p>Si utiliza el diagrama de Gantt heredado principalmente para la vista simple y las ediciones rápidas y no utiliza el diagrama real, la nueva opción Planificación de cronología le permite realizar cambios rápidos en los campos de planificación clave. Puede seleccionar Planificación de cronología en lugar de Guardar automáticamente en la barra de herramientas de la lista de tareas.</p> <p>Para obtener más información acerca de cómo guardar una lista de tareas con la opción Planificación de escala de tiempo, vea la sección "Guardar cambios en una lista de tareas manualmente al seleccionar la opción Planificación de escala de tiempo" en el artículo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tareas en una lista</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gráfico Gantt heredado para una lista de proyectos</strong> </p> <p>El gráfico Gantt anterior de la lista de proyectos permitía a los usuarios ver los proyectos y sus tareas en una sola vista. Sin salir del contexto de la lista de proyectos, los usuarios podían ver detalles sobre las tareas de un proyecto, así como las dependencias entre los proyectos. El gráfico Gantt anterior de la lista de proyectos se basaba en la tecnología de Flash, que presentaba riesgos para la seguridad. </p> </td> 
   <td> <p><strong>Gráfico Gantt, lista de proyectos</strong> </p> <p>El diagrama de Gantt basado en el HTML sirve para el mismo propósito que el diagrama de Gantt heredado. Los usuarios pueden ver los proyectos y sus tareas en una vista para identificar visualmente las dependencias entre proyectos y tareas. El gráfico Gantt de lista de proyectos se encuentra directamente en la lista de proyectos. El nuevo gráfico Gantt tiene una interfaz moderna y se basa en la tecnología más reciente.</p> <p>Para obtener información acerca del gráfico Gantt de lista de proyectos, vea <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Ver información en el gráfico Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Compartir cuadros de diálogo para informes, calendarios y documentos</strong> </p> <p>Al compartir informes, calendarios y documentos, los cuadros de diálogo que se utilizaban se basaban en la tecnología de Flash.</p> </td> 
   <td> <p>La experiencia al compartir informes, calendarios y documentos en Workfront no ha cambiado. Sin embargo, la experiencia ya no depende del Flash.</p> <p>Para obtener más información acerca de cómo compartir estos elementos, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido en objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visor de revisiones heredado</strong> </p> <p>El visualizador de pruebas heredado era un visualizador de pruebas basado en la web que proporcionaba funciones de prueba para pruebas estáticas, de vídeo e interactivas.</p> </td> 
   <td> <p><strong>Visor de corrección web y Visor de corrección de escritorio</strong> </p> <p>El Visor de revisión web proporciona funciones de revisión para pruebas estáticas y de vídeo.</p> <p>El Visor de corrección de escritorio proporciona funciones de corrección para pruebas interactivas, además de compatibilidad total con pruebas estáticas y de vídeo.</p> <p>El formato de archivo SWF ya no es compatible con ninguno de los proveedores principales y se ha sustituido por titulares HTML 5 para las pruebas. </p> <p>Para obtener información más detallada acerca de las diferencias entre los visores de revisión disponibles, vea <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Diferencias entre el Visor de revisión web y el Visor de revisión de escritorio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
