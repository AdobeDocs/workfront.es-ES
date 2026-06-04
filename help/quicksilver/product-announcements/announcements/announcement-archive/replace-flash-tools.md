---
title: Reemplazo de herramientas basadas en Flash en Adobe Workfront
description: Reemplazo de herramientas basadas en Flash en Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ZiRTszrV8GYwr0GIM523WXP7Qk6zfRRsMjVLJ3PZRZg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 2730
ht-degree: 99%

---

# Reemplazo de herramientas basadas en Flash en Adobe Workfront

Hemos eliminado todas las herramientas basadas en Flash de Adobe Workfront Classic.

Las herramientas de reemplazo basadas en los estándares actuales ya están disponibles en Workfront. Estos cambios coinciden con el fin de la compatibilidad con los productos Flash anunciado por Adobe.

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

Para obtener información acerca de las herramientas de reemplazo, consulte [Herramientas heredadas basadas en Flash y sus reemplazos](#legacy-flash-based-tools-and-their-replacements) en este artículo.

### Administración de recursos

* La pestaña Planificación de recursos heredados del área Personas y todas las herramientas que contiene, que incluye lo siguiente:

   * Administrador del presupuesto de recursos
   * Planificador de capacidades
   * Estimaciones de recursos
   * Cuadrícula de recursos\
     Para obtener más información, consulte [Planificación de recursos: índice de artículos](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* El área Estimaciones de recursos heredados en el caso empresarial de un proyecto

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

* La subpestaña Cuadrícula de recursos de la ficha Asignación de personal de un proyecto
* La opción Utilizar nueva área de programación de la subpestaña Programación de la pestaña Asignación de personal de un proyecto que elimina el área de programación heredada o el Generador de equipos. En este caso, la cronología de la programación ahora se muestra de forma predeterminada.
* La pestaña Asignación en el perfil de usuario

### Informes

Se han eliminado las siguientes funciones de creación de informes e informes:

* Funciones de creación de informes eliminadas:

   * La opción Cuadrícula de recursos en un informe de usuario
   * La opción Gantt heredado en un proyecto o un informe de tarea\
     Para obtener más información, consulte [Ver información en el gráfico Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Informes eliminados:

   * El informe del conjunto de recursos heredados
   * El informe Estimaciones de recursos

  >[!NOTE]
  >
  >Todos los campos heredados a los que se accede a través de los informes o a través de la API (Conjunto de recursos heredado, Coste presupuestado heredado, Coste preexistente, Horas presupuestadas heredadas, Coste de mano de obra presupuestado heredado, etc.) se muestran en varios informes, pero no se rellenan con información nueva.

### Gantt anterior

* Todas las vistas de Gantt heredado de las listas de proyectos y tareas, así como las opciones de creación de informes e informes
* Las subpestañas de Gantt heredado en portafolios y programas
* La subpestaña Gantt heredado en una lista de Tareas de plantilla en una Plantilla, la vista Gantt heredado en la pestaña Subtareas de una Tarea de plantilla y en un informe de Tarea de plantilla

### Revisión

El visor de corrección heredado se ha reemplazado con el nuevo visor de corrección web y el visor de corrección de escritorio para la mayoría de los clientes, y se eliminó para todos los clientes en noviembre de 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Para obtener más información, consulte los recursos siguientes:

* [Revisión de pruebas en el visor de corrección web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Revisión de pruebas en el visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

## Herramientas heredadas basadas en Flash y sus reemplazos {#legacy-flash-based-tools-and-their-replacements}

Salvo que se especifique lo contrario, todas las funciones heredadas se han sustituido por otras nuevas, como se muestra en la tabla siguiente.

>[!CAUTION]
>
>Las herramientas heredadas basadas en Flash se han eliminado de todos los entornos.

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
   <td> <p><strong>Conjuntos de recursos heredados</strong> </p> <p>Los conjuntos de recursos heredados eran grupos o colecciones de funciones necesarias al mismo tiempo para la finalización de un proyecto. Los conjuntos de recursos heredados tenían una serie de deficiencias:</p> 
    <ul> 
     <li> Era posible asociar un usuario con un conjunto de recursos heredados, pero esta opción solo se utilizaba para la creación de informes. Dado que los conjuntos de recursos heredados funcionaban con entidades de funciones abstractas, no se tenía en cuenta ninguna de las excepciones de programación y los días libres de los usuarios, lo que daba lugar a datos inexactos sobre la disponibilidad de los recursos. </li> 
    </ul> 
    <ul> 
     <li>Puede especificar solamente un conjunto de recursos heredados por proyecto, lo que resultó en varios conjuntos de recursos heredados que solo admiten el flujo de grupos separados que funcionan de forma independiente entre sí y nunca comparten recursos. En todos los demás casos, se recomendaba mantener un conjunto de recursos heredados que incluyera todos los recursos en el sistema, lo que ocasionaba problemas de rendimiento con grandes cantidades de proyectos y datos.</li> 
    </ul> </td> 
   <td> <p><strong>Conjunto de recursos</strong> </p> <p>Los nuevos conjuntos de recursos son una colección de usuarios que se necesitan al mismo tiempo para completar el proyecto. Workfront también es consciente de que hay casos en los que los usuarios especializados necesitan que se les asigne trabajo por separado. Por este motivo, ahora puede presupuestar usuarios en lugar de funciones. </p> Entre las ventajas del conjunto de recursos con respecto a los conjuntos de recursos heredados se incluyen las siguientes: 
    <ul>
     <li>Dado que los conjuntos de recursos se basan en los usuarios, sus días libres y las excepciones de programación ya se tienen en cuenta para los cálculos de disponibilidad de usuarios y funciones. Esto da como resultado datos precisos y actualizados, lo que permite tomar decisiones presupuestarias correctas y minimizar la probabilidad de cambios cuando el proyecto está en curso.</li>
     <li>Dado que ahora hay más control sobre la disponibilidad de los recursos y la precisión de los datos, Workfront le permite asociar varios conjuntos de recursos con un proyecto. Un usuario también puede pertenecer a más de un conjunto de recursos, en caso de que tenga varias aptitudes que se puedan utilizar en varios proyectos al mismo tiempo. </li>
    </ul><p>Con este control sobre los datos, ya no es necesario tener un conjunto de recursos que incluya todos los recursos para distribuir el presupuesto disponible. De hecho, no se recomienda. En lugar de ello, recomendamos diversificar sus conjuntos de recursos y asociar únicamente los conjuntos de recursos relevantes con los proyectos.</p><p> Para obtener más información sobre los conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Información general sobre los conjuntos de recursos </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Administrador del presupuesto de recursos</strong> </p> <p>Puede utilizar el Administrador del presupuesto de recursos para especificar la disponibilidad de los recursos de funciones en varios conjuntos de recursos. Sin embargo, debido a las deficiencias del conjunto de recursos heredados, esta funcionalidad rara vez se utilizaba. Cuando se utilizaba, obligaba a los usuarios a introducir manualmente la disponibilidad de las funciones para hacer que la presupuestación fuera más precisa. No se tuvieron en cuenta las excepciones de programación ni los días libres de los usuarios.</p> </td> 
   <td> <p>Con el cálculo automático de la disponibilidad basado en los usuarios de los conjuntos de recursos, el Administrador del presupuesto de recursos ya no es necesario. Se ha eliminado la herramienta, junto con todo el trabajo manual, para calcular la disponibilidad.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimaciones de recursos</strong> </p> <p>La ficha Estimaciones de recursos de cada conjunto de recursos heredados tenía el mismo propósito que el Administrador de presupuesto de recursos, solo que en el contexto de un conjunto de recursos heredados. Esta herramienta presentaba las mismas limitaciones que el Administrador de presupuesto de recursos y los Conjuntos de recursos heredados: datos inexactos e introducción manual de disponibilidad. </p> </td> 
   <td> <p>Con el cálculo automático de la disponibilidad de los usuarios, las estimaciones de recursos han quedado obsoletas y se han eliminado.</p> <p>La herramienta se elimina en los conjuntos de recursos de legado y en las estimaciones de recursos de legado en el caso empresarial de un proyecto.
   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     -->
     </p> </td>
  </tr> 
  <tr> 
   <td> <p><strong>Planificador de capacidades</strong> </p> <p>El Planificador de capacidades era una herramienta de Workfront para presupuestar recursos y priorizar proyectos dentro de un conjunto de recursos heredados, de acuerdo con la disponibilidad de los recursos. Dado que los datos de las estimaciones de recursos y del Administrador de presupuesto de recursos que proporcionaban la información para el Planificador de capacidades eran incompletos, había que verificar dos veces la prioridad de los proyectos en relación con la disponibilidad de los usuarios.</p> <p>El uso de un único conjunto de recursos heredados que incluyera todas las funciones en el sistema era el escenario más común, lo que producía problemas de rendimiento con el Planificador de capacidades al intentar cargar un gran número de proyectos.</p> </td> 
   <td> <p><strong>Vista de proyecto del Planificador de recursos</strong> </p> <p>En la vista basada en proyectos del Planificador de recursos, puede presupuestar recursos y priorizar proyectos de manera similar a como lo hacía en el Planificador de capacidades heredadas. A diferencia de la herramienta heredada, ahora se admiten más datos y la información disponible es más precisa, ya que tiene en cuenta el tiempo libre de los usuarios y las excepciones de programación.</p> <p>La información disponible, planificada y presupuestada se puede consultar de un vistazo para que los administradores de recursos puedan ver si hay suficientes personas para realizar el trabajo y si los planes del proyecto superan las estimaciones presupuestarias iniciales.</p> <p> Para obtener información sobre el uso de la vista de proyecto en el Planificador de recursos, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general sobre el planificador de recursos</a></p> <p><strong>El Planificador de escenarios</strong> </p> <p>Para la planificación de la capacidad a largo plazo, el modelado de escenarios hipotéticos y la priorización, también hemos presentado el Planificador de escenarios de Workfront. </p> <p>El Planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Planificador de escenarios de Workfront, consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general sobre el Planificador de escenarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimaciones de recursos heredados (caso empresarial)</strong> </p> <p>Puede utilizar el área Estimaciones de recursos heredados del caso empresarial para presupuestar una cierta cantidad de horas de trabajo y costes como parte de la planificación del proyecto y la solicitud de recursos. Esta vista no proporcionó ninguna visibilidad sobre la disponibilidad de recursos, lo que se traducía en solicitudes aproximadas de recursos y en una mayor probabilidad de que se rechazara el trabajo del proyecto.</p> </td> 
   <td> <p><strong>Presupuestación de recursos (caso empresarial)</strong> </p> <p>La sección Presupuestación de recursos del caso empresarial aporta las funciones del Planificador de recursos al caso empresarial, proporcionando visibilidad sobre la disponibilidad de usuarios y funciones, así como la capacidad de realizar presupuestos a nivel de usuario. </p> <p> Para obtener información acerca del área de presupuestación de recursos del caso empresarial, consulte la <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Información general de las áreas del caso empresarial</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Informes de estimación de recursos</strong> </p> <p>Al utilizar las herramientas heredadas para la administración de recursos, podía informar sobre las horas presupuestadas y planificadas desde el caso empresarial. Esto le permitía crear informes de matriz que mostraban el trabajo total presupuestado y planificado para cada función en un lapso de tiempo específico. Este informe no se podía editar ni podía realizarse ningún cambio en el presupuesto de los recursos según los resultados del informe. </p> </td> 
   <td> <p><strong>Informe de utilización</strong> </p> <p>El informe de Utilización integrado muestra en paralelo las horas planificadas, las presupuestadas y las reales, los costes y los ingresos. </p> <p>Para obtener información acerca del uso del informe Utilización, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información sobre utilización de recursos </a>. </p> 
    <div> 
     <p><strong>Horas presupuestadas notificables</strong> </p> 
     <p>Cree un informe de horas presupuestadas para revisar las horas presupuestadas en el Planificador de recursos en un formulario de informe. </p> 
     <p>Para obtener información sobre las horas presupuestadas, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glosario de terminología de Adobe Workfront</a>.</p> 
     <p>Para obtener información sobre cómo crear un informe, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> 
    </div> <p><strong>La vista de función del Planificador de recursos</strong> </p> <p>Las horas presupuestadas y planificadas del caso empresarial en las herramientas de administración de recursos heredadas están ahora disponibles en una nueva vista nativa: la vista basada en funciones del Planificador de recursos. Esta vista proporciona información rápida sobre las horas disponibles, planificadas y presupuestadas, y le permite controlar y cambiar las horas presupuestadas en el mismo lugar. Esto garantiza una mejor toma de decisiones durante la planificación de funciones de alto nivel. </p> <p> Para obtener información acerca de cómo presupuestar recursos en la vista de función del Planificador de recursos, consulte la sección <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Usar las vistas de proyecto y función para presupuestar recursos </a> en <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del Planificador de recursos</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Cuadrícula de recursos</strong> </p> <p>La cuadrícula de recursos le da visibilidad en cuanto a asignación de usuarios específicos a medida que un proyecto alcanza sus etapas finales. </p> <p>Por ejemplo, podía ver fácilmente cuándo alguien del equipo del proyecto terminaba su trabajo temprano y cuándo alguien se retrasaba, así como si se le asignó demasiado o no lo suficiente para un lapso de tiempo específico. </p> <p>Por desgracia, no podía actuar sobre la información en la misma vista. Para corregir los problemas de sobreasignación tenía que ir a los proyectos y ajustar manualmente la información allí sin visibilidad sobre resultado de sus acciones.</p> </td> 
   <td> <p>La cuadrícula de recursos se ha reemplazado por dos nuevas herramientas. Puede utilizar las siguientes herramientas, en función de la fase de planificación de recursos en la que se encuentre:</p> 
    <ul> 
     <li> <p><strong>Para la fase analítica:</strong> </p> 
      <ul> 
       <li> <p><strong>Distribuidor de cargas de trabajo</strong>: use el Distribuidor de cargas de trabajo para ver la carga de trabajo de los usuarios a un nivel más granular. Al utilizar el Distribuidor de cargas de trabajo, puede ver qué usuarios tienen disponibilidad en su carga de trabajo para así completar la tarea a tiempo. Esto incluye los detalles de sus días libres y excepciones de horario. </p> <p>Para obtener información sobre el Distribuidor de cargas de trabajo, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Información general del Distribuidor de cargas de trabajo</a>.</p> </li> 
       <li> <p><strong>La vista de usuario del Planificador de recursos</strong><strong>:</strong> Al intentar comprender en un nivel superior a qué proyectos están asignados los usuarios, use la vista de usuario del Planificador de recursos. Esto le permite ver en qué están trabajando los usuarios, así como su asignación excesiva o insuficiente para un lapso de tiempo específico. El Planificador de recursos también proporciona una visualización de la asignación general de los usuarios en su conjunto, así como visibilidad de las horas reales registradas, lo cual resulta útil para analizar el progreso del trabajo realizado. </p> <p>Para obtener información sobre el uso de la vista de usuario en el Planificador de recursos, consulte la sección <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Usar la vista de usuario para ver las horas disponibles, planificadas y reales o FTE </a> en <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del Planificador de recursos</a></p> </li> 
      </ul> </li> 
     <li><strong>Para la fase táctica:</strong> 
      <ul> 
       <li><strong>Distribuidor de cargas de trabajo</strong> Mediante el Distribuidor de cargas de trabajo, podrá hacer lo siguiente: 
        <ul>
         <li>Asignar trabajo a los usuarios.</li>
         <li>Administrar las asignaciones de usuarios a elementos de trabajo. </li>
         <li>Compartir el Distribuidor de cargas de trabajo con otros usuarios que podrían no tener visibilidad en el área de personas. Utilice la funcionalidad de vínculo compartido para compartir un vínculo al Distribuidor de cargas de trabajo e incrustarlo en paneles de control personalizados. Cualquier usuario con acceso a Ver usuarios puede ver estos paneles de control cuando usted los comparta.</li>
        </ul><p>El Distribuidor de cargas de trabajo está disponible en el área de personas. </p><p>Para obtener información sobre el Distribuidor de cargas de trabajo, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Información general del Distribuidor de cargas de trabajo</a>.</p></li> 
      </ul>
      <!--
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
      -->
      </li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gráfico Gantt heredado, lista de tareas</strong> </p> <p> El gráfico Gantt heredado de la lista de tareas permitía a los usuarios visualizar la cronología del proyecto y realizar la planificación de escenarios hipotéticos sin confirmar los cambios en la base de datos. El gráfico Gantt heredado se basaba en la tecnología Flash, la cual presentaba riesgos para la seguridad. </p> </td> 
   <td> <p><strong>Gráfico Gantt,</strong> <strong>Lista de tareas</strong></p> <p> El nuevo gráfico Gantt basado en HTML tiene el mismo propósito que el gráfico Gantt heredado. Los usuarios pueden visualizar la cronología del proyecto y realizar la planificación de escenarios hipotéticos sin confirmar los cambios en la base de datos, cambiando a la opción Guardar de forma manual en la barra de herramientas de la lista de tareas. </p> <p>El nuevo gráfico Gantt es interactivo cuando se utiliza la opción de guardado automático, la cual puede utilizar cuando desee guardar automáticamente los cambios a medida que se producen. </p> <p>El nuevo gráfico Gantt de la lista de tareas se basa en la tecnología más reciente y es fiable. Este nuevo gráfico Gantt se encuentra directamente en la lista de tareas y se accede fácilmente a él mientras trabaja en la lista de tareas sin cambiar de pestaña ni de vista. </p> <p>Aunque el nuevo gráfico Gantt ofrece la misma funcionalidad que el diagrama anterior, hay algunas diferencias en las características en comparación con el Gantt heredado. </p> <p> La subpestaña Gantt heredado de una lista de tareas de plantilla de una plantilla, la vista de Gantt heredado de la pestaña Subtareas de una tarea de plantilla y el gráfico Gantt heredado de un informe de tareas de plantilla también se han sustituido por el gráfico Gantt basado en HTML. </p> <p>Si utiliza el gráfico Gantt heredado principalmente para la vista simple y las ediciones rápidas y no utiliza el gráfico real, la nueva opción Planificación de la cronología le permite realizar cambios rápidos en los campos de planificación clave. Puede seleccionar la Planificación de la cronología en lugar de Guardar automáticamente en la barra de herramientas de la lista de tareas.</p> <p>Para obtener más información acerca de cómo guardar una lista de tareas con la opción Planificación de la cronología, consulte la sección “Guardar cambios en una lista de tareas manualmente al seleccionar la opción Planificación de la cronología” en el artículo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tareas en una lista</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gráfico Gantt heredado para una lista de proyectos</strong> </p> <p>El gráfico Gantt heredado de la lista de proyectos permitía a los usuarios ver los proyectos y sus tareas en una sola vista. Sin salir del contexto de la lista de proyectos, los usuarios podían ver detalles sobre las tareas de un proyecto, así como las dependencias entre los proyectos. El gráfico Gantt heredado de la lista de proyectos se basaba en la tecnología Flash, que entrañaba riesgos para la seguridad. </p> </td> 
   <td> <p><strong>Gráfico Gantt, lista de proyectos</strong> </p> <p>El gráfico Gantt basado en HTML sirve para el mismo propósito que el gráfico Gantt heredado. Los usuarios pueden ver los proyectos y sus tareas en una vista para identificar visualmente las dependencias entre proyectos y tareas. El gráfico Gantt de la lista de proyectos se encuentra directamente en la lista de proyectos. El nuevo gráfico Gantt tiene una interfaz moderna y se basa en la tecnología más reciente.</p> <p>Para obtener información acerca del gráfico Gantt de la lista de proyectos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Ver información en el gráfico Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Compartir cuadros de diálogo para informes, calendarios y documentos</strong> </p> <p>Al compartir informes, calendarios y documentos, los cuadros de diálogo que se utilizaban se basaban en la tecnología Flash.</p> </td> 
   <td> <p>La experiencia al compartir informes, calendarios y documentos en Workfront no ha cambiado. Sin embargo, la experiencia ya no depende de Flash.</p> <p>Para obtener más información acerca de cómo compartir estos elementos, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido en objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visor de corrección heredado</strong> </p> <p>El visor de corrección heredado era un visor de corrección basado en web que proporcionaba funciones de revisión para pruebas estáticas, de vídeo e interactivas.</p> </td> 
   <td> <p><strong>Visor de corrección web y visor de corrección de escritorio</strong> </p> <p>El visor de corrección web proporciona funciones de revisión para pruebas estáticas y de vídeo.</p> <p>El visor de corrección de escritorio proporciona funciones de corrección para revisiones interactivas, además de compatibilidad total con revisiones estáticas y de vídeo.</p> <p>El formato de archivo SWF ya no es compatible con ninguno de los proveedores principales y se ha sustituido por banners HTML 5 para las revisiones. </p> <p>Para obtener información más detallada acerca de las diferencias entre los visores de corrección disponibles, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Diferencias entre el visor de corrección web y el visor de corrección de escritorio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
