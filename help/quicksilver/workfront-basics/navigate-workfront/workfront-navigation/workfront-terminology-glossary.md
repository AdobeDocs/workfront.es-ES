---
content-type: reference
navigation-topic: workfront-navigation
title: Glosario de [!DNL Adobe Workfront] terminología
description: La variable [!DNL Adobe Workfront] el glosario enumera los términos más utilizados en Adobe Workfront.
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '19387'
ht-degree: 0%

---

# Glosario de [!DNL Adobe Workfront] terminología

>[!IMPORTANT]
>
>Este artículo debe utilizarse como referencia para comprender los términos que puede encontrar en la variable [!DNL Adobe Workfront] en el [!DNL Workfront] o cuando se habla generalmente de planificación y administración del trabajo. Actualmente estamos actualizando esta información, por lo que es posible que esta tabla no esté completa. Eliminaremos esta exención de responsabilidad cuando consideremos que esta información es exhaustiva.

La siguiente tabla es una lista de los términos más utilizados en Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nombre de objeto</strong></th> 
   <th><strong>Descripción</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nivel de acceso]</td> 
   <td>Un perfil de usuario que determina cómo un usuario puede interactuar con diferentes objetos y herramientas dentro de Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea activa]</td> 
   <td>Una tarea incompleta en un proyecto actual que no se impide que una tarea predecesora trabaje en ella y que no tiene una restricción de tarea con una fecha de inicio planificada futura. En otras palabras, hoy se puede trabajar en él.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Actividad]</td> 
   <td>En [!DNL Workfront Goals], una actividad es un indicador de progreso para un objetivo. Puede ser una barra de progreso que actualice manualmente o un proyecto que esté asociado con el objetivo. No puede mostrar las actividades en un informe y no puede acceder a ellas a través del [!DNL Workfront] API. Para obtener información sobre las actividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introducción a resultados y actividades en objetivos de Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo real]</td> 
   <td> <p>Para tareas y problemas, este es el coste asociado con las horas reales registradas en relación con la tasa Costo por hora del recurso asignado a la tarea o problema. Para los proyectos, esto es un total de todos los [!UICONTROL Costes reales] de tareas y problemas en el proyecto. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo real de gastos]</td> 
   <td> <p>La suma de las [!UICONTROL Cantidades reales] para todos los gastos registrados para un proyecto o una tarea.</p> <b>EJEMPLO </b>
   <p>Si crea un gasto para la Tarea 1 e introduce 600,00 $ en el campo [!UICONTROL Importe Real], el [!UICONTROL Costo Real] para esta tarea es 600,00 $. </p> 
   <p>Para un proyecto, [!DNL Workfront] utiliza la fórmula siguiente para calcular [!UICONTROL Costo real de gastos]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas reales]</td> 
   <td> <p>En un informe de proyecto, tarea o problema, [!UICONTROL Horario real] es la suma de todas las horas registradas en el proyecto, la tarea o el problema.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span> Si en la ficha [!UICONTROL Actualizaciones] para la tarea 1, hace clic en "Tiempo de registro" e introduce 25 horas, las horas reales de la tarea 1 = 25 horas. </p> <p>[!DNL Workfront] calcula [!UICONTROL horas reales] para tareas o proyectos principales mediante las siguientes fórmulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo real de trabajo]</td> 
   <td> <p>El [!UICONTROL Costo real] asociado con la mano de obra invertida en una tarea o proyecto. </p> <p>Para una tarea, [!DNL Workfront] calcula el [!UICONTROL costo laboral real] mediante la fórmula siguiente:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Si la tarea tiene un [!UICONTROL Cost Type] de [!UICONTROL User Hourly], [!DNL Workfront] utiliza la tasa de usuario. Si la tarea tiene un [!UICONTROL Cost Type] de [!UICONTROL Role Hourly], [!DNL Workfront] utiliza la tasa de función del trabajo para calcular el [!UICONTROL costo laboral real]. </p> <p>Para un proyecto, [!DNL Workfront] utiliza la fórmula siguiente para calcular el [!UICONTROL costo laboral real]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Por ejemplo, si un usuario registra 5 horas para una tarea con un [!UICONTROL User Hourly] [!UICONTROL Cost Type] y su tasa horaria es de 100 dólares, el [!UICONTROL Real Labor Cost] es de 500 dólares.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ingresos reales] </td> 
   <td> <p>Los [!UICONTROL ingresos reales] de un proyecto o una tarea son la cantidad de dinero asociada con las [!UICONTROL horas reales] del proyecto o la tarea. </p> <p>Para obtener información sobre el seguimiento de ingresos en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Inicio real]</td> 
   <td>Marca de tiempo cuando un usuario cambia un objeto en curso en el trabajo que se le ha asignado.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>Metodología de [!UICONTROL Agile]</td> 
   <td>Tipo de metodología basada en la evolución colaborativa de las necesidades y soluciones con equipos interfuncionales. Fomenta la flexibilidad y el cambio en función de un calendario fijo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Difiere del equipo tradicional porque toma su trabajo potencial de un trabajo atrasado y trabaja en él dentro de un período de tiempo establecido que se denomina [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Todos mis equipos]</td> 
   <td> <p>Cuando se hace referencia a esto en [!UICONTROL filters], este campo muestra los usuarios que pertenecen a cualquiera de los equipos a los que pertenece el usuario que ha iniciado sesión o los elementos de trabajo asignados a cualquiera de los equipos a los que pertenece el usuario que ha iniciado sesión. </p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, puede crear solo un informe que muestre información diferente en función de quién inicie sesión para verla, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de asignación]</td> 
   <td> <p>Puede encontrar este campo en los siguientes tipos de informes:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (datos financieros)</li> 
     <li>[!UICONTROL Hora presupuestada]</li> 
    </ul> <p>Para un<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->Informe [!UICONTROL Project (Financial Data)]: </p> 
    <ul> 
     <li>Genere este informe al intentar comprender <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> la cantidad de [!UICONTROL Horario planificado] que se asigna a sus recursos.</li> 
     <li> <p>[!UICONTROL Allocation Date] es el primer día (domingo) de una semana en el que se inicia la asignación de una función de trabajo [!UICONTROL Job] a una tarea. Un recurso ([!UICONTROL Job Role]) puede tener tantas [!UICONTROL Allocation Dates] como semanas durante la [!UICONTROL Duration] de las tareas asignadas. Si las tareas abarcan varios meses, el primer día de un mes también puede convertirse en una [!UICONTROL Fecha de asignación], si se encuentra dentro de la [!UICONTROL Duración] de la tarea.</p> <p>Por ejemplo, puede tener un [!UICONTROL Job Role] asignado a una tarea que dure más de 3 semanas y tenga 90 [!UICONTROL Planned Hours]. Estas horas se distribuyen uniformemente durante la duración de la tarea, lo que hace que cada día asigne 6 [!UICONTROL Horario planificado] a su función de trabajo:</p> <p><em> [!UICONTROL Horario planificado diario] = [!UICONTROL Horario total planificado]/ Número de [!UICONTROL Días laborables] durante la [!UICONTROL Duración] de la tarea </em> </p> <p>Como resultado, hay tres [!UICONTROL Fechas de asignación], una para cada domingo de cada semana durante la [!UICONTROL Duración] de la tarea, cada uno con un determinado número de [!UICONTROL Horario planificado] asociado a ellas.<br>Si la tarea comienza a mediados de la última semana de un mes y finaliza dos semanas después del comienzo de un nuevo mes, la tarea tendrá cuatro [!UICONTROL Fechas de asignación]: uno para cada domingo de cada semana durante la [!UICONTROL Duration] de la tarea y otro para el primer día del nuevo mes.</p> <p>Para aprovechar al máximo esta información, le recomendamos que cree un <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Informe de proyecto (datos financieros) y agregue una agrupación de matriz para [!UICONTROL Fecha de asignación]. A continuación, agrupe los resultados semanalmente, mensualmente, trimestralmente o anualmente para los datos más precisos.<br>Para obtener información sobre la creación de una agrupación de matriz, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Crear un informe de matriz</a>.</p> </li> 
    </ul> <p>La información financiera se rellena en los informes de [!UICONTROL Project (Financial Data)] únicamente cuando los datos asociados a él tienen menos de 5 años. Por ejemplo, si una función de trabajo se asignó a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como [!UICONTROL Allocation Date] para la función de trabajo no se rellena en el informe [!UICONTROL Project (Financial Data)]. </p> 
    <div> 
     <p>Para un informe de [!UICONTROL Hora presupuestada]:</p> 
     <ul> 
      <li>Genere este informe al intentar comprender la cantidad de [!UICONTROL Horario presupuestado] que se asigna a sus recursos o a sus proyectos en el Planificador de recursos.</li> 
      <li> <p>El [!UICONTROL Fecha de asignación] es el primer día (domingo) de la semana para el que se presupuestaron las horas en el [!UICONTROL Resource Planner]. </p> <p>Sugerencia:   <p>Si una semana abarca dos meses, se generarán dos filas en el informe: una correspondiente al primer día de la semana (domingo de la primera semana, que es durante el primer mes) y la segunda fila muestra el primer día del segundo mes. </p> <p>Por ejemplo, si se presupuestan 8 horas para un usuario para la semana del 30 de junio (domingo) al 6 de julio (sábado), las dos filas muestran un [!UICONTROL Fecha de asignación] del 30 de junio y un 1 de julio. </p> </p> <p>Para obtener información sobre la presupuestación de los recursos en la [!DNL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Los recursos presupuestarios de [!DNL Resource Planner] uso de las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>.</p> <p>Para obtener información sobre la creación de un informe de [!UICONTROL Hora presupuestada], consulte <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Informe: Hora presupuestada</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anuncios]</td> 
   <td> <p>Una forma de comunicar a los usuarios información dentro del sistema. Esta información suele proceder de [!DNL Workfront] al administrador o del administrador al usuario. </p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar anuncios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>Normalmente, una aplicación representa un conector de una aplicación de software, pero también puede representar funciones especiales que manipulan los datos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisión del aprobador]</td> 
   <td> <p>En el informe [!UICONTROL Proof Approval], este campo muestra las decisiones de aprobación de pruebas para las pruebas que ya no están activas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fase del aprobador]</td> 
   <td>En el [!UICONTROL Proof Approval report], este campo muestra información sobre una fase actual de pruebas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Un elemento de trabajo determinado, como una tarea, un documento o un parte de horas, puede requerir que un supervisor u otro usuario cierre la sesión en el elemento de trabajo. Este proceso de desactivación se denomina aprobación. </p> <p>Para obtener más información, consulte <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Información general del proceso de aprobación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de aprobación]</td> 
   <td>En el informe [!UICONTROL Proof Approval], este campo muestra la fecha en la que se aprobó una prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprobador]</td> 
   <td>Un rol de usuario o de trabajo que debe cerrar la sesión en un elemento de trabajo determinado, o el usuario que aprueba entradas de hora en hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignado A]</td> 
   <td> <p>En un informe de [!UICONTROL Task or Issue], este campo muestra el propietario de la tarea o del problema, o el [!UICONTROL Primary Assignee]. También puede filtrar o agrupar por este campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Usuario, función de trabajo o equipo asignado a un problema o una tarea. Los proyectos, portafolios o programas no pueden tener asignaciones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignaciones]</td> 
   <td> <p>En un informe de [!UICONTROL Task] o [!UICONTROL Issue], este campo muestra una lista de todas las entidades (usuarios, funciones de trabajo, equipos) asignadas a la tarea o al problema. Puede filtrar por este campo utilizando los campos [!UICONTROL Assignment Users] y [!UICONTROL Assignment roles]. Puede filtrar por el equipo asignado a la tarea o al problema mediante el campo Equipo . No se puede agrupar un informe por este campo.</p> <p>Los elementos de trabajo que se hayan colocado en la [!UICONTROL Papelera de reciclaje] seguirán mostrándose en algunos informes que hacen referencia al objeto [!UICONTROL Assignment] donde se muestra un [!DNL OR] se utiliza el modificador de filtro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Funciones de asignación]</td> 
   <td>
   <p>En un informe [!UICONTROL Task] o [!UICONTROL Issue], este campo muestra información sobre las funciones de trabajo asignadas a las tareas o los problemas. Este campo muestra [!UICONTROL Primary Owners], así como otras funciones de trabajo asignadas a tareas o problemas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado de asignación]</td> 
   <td> <p>En un informe de asignación, tarea o problema, el [!UICONTROL Estado de asignación] muestra si los usuarios asignados a un elemento de trabajo han hecho clic en el botón [!UICONTROL Work On It] o [!UICONTROL Done] para aceptar o completar el trabajo. Existen los siguientes [!UICONTROL Estados de asignación]:</p> 
    <ul> 
     <li><b>[!UICONTROL solicitado]</b>: se ha asignado al usuario la tarea o el problema, pero aún no han hecho clic en el botón [!UICONTROL Work On It] para comenzar a trabajar en él.</li> 
     <li><b>[!UICONTROL funciona]</b>: el usuario ha hecho clic en el botón [!UICONTROL Work On It] y está trabajando en el elemento. </li> 
     <li><b>[!UICONTROL Listo]</b>: el usuario ha hecho clic en el botón [!UICONTROL Listo] y ha completado su trabajo en el elemento. </li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Información general sobre los botones [!UICONTROL Work On It] y [!UICONTROL Done]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipos de asignación]</td> 
   <td>
   <p>En un informe [!UICONTROL task] o [!UICONTROL issue] , este campo muestra información sobre los equipos asignados a las tareas o problemas. El campo muestra [!UICONTROL Primary Owners], así como otros equipos asignados a tareas o problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuarios de asignación]</td> 
   <td>
   <p>En un informe [!UICONTROL Task] o [!UICONTROL Issue], este campo muestra información sobre los usuarios asignados a las tareas o problemas. Este campo muestra [!UICONTROL Primary Owners], así como otros usuarios asignados a tareas o problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Un atributo es un rasgo de un [!DNL Workfront] objeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Área de auditoría]</td> 
   <td> <p>Las auditorías son mensajes del sistema que registran una acción que se ha producido en Workfront. Se registran los siguientes tipos de auditoría:</p> 
    <ul> 
     <li>[!UICONTROL Cambio de ámbito]</li> 
     <li>[!UICONTROL Acción de datos adjuntos]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Cambio de estado]</li> 
     <li>[!UICONTROL Nota]</li> 
     <li>[!UICONTROL Entrada combinada]</li> 
     <li>[!UICONTROL Entrada de error]</li> 
     <li>[!UICONTROL Cambio de estado]</li> 
     <li>[!UICONTROL Cambio de suscripción]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pista de auditoría]</td> 
   <td>Recopilación de notas generadas automáticamente por eventos que se rastrean a través de los cambios registrados ([!UICONTROL Áreas de auditoría]). Cada nota registra quién hizo la acción, qué hicieron y cuándo lo hicieron.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automático Y En Cambio]</td> 
   <td> <p>Uno de los tipos [!UICONTROL Project Update]. De este modo, se recalcularán los plazos proyectados y planeados del proyecto cuando se ejecute el proceso de cálculo nocturno y cuando se realice cualquier actualización del proyecto o de las tareas dentro del proyecto. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilidad</p></td> 
   <td> <p>Este término se utiliza en relación con la "disponibilidad del usuario" o la "disponibilidad de recursos" e ilustra la cantidad de tiempo que el recurso (función de usuario o de trabajo) está disponible para funcionar. </p> 
   <p>Workfront calcula la disponibilidad de los usuarios mediante varios campos y según la configuración de las preferencias de Gestión de recursos de su sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a>. </p>
   <p>Para obtener más información sobre la disponibilidad de recursos, consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introducción a la administración de recursos</a></p>
   Alternativamente, la "capacidad" también se utiliza para hacer referencia a la disponibilidad de recursos. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automático solamente]</td> 
   <td> <p>Uno de los tipos [!UICONTROL Project Update]. De este modo, se recalcularán las líneas de tiempo proyectadas y planificadas cuando se ejecute el proceso de cálculo por la noche.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Trabajo "como de costumbre" que contribuye a ejecutar los objetivos principales del negocio cotidiano.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>El área en un entorno ágil donde se mantienen nuevas cuestiones hasta que estén listas para ser trabajadas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Línea de base]</td> 
   <td>Fuente de datos para medir iteraciones en un entorno ágil.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Registro de facturación]</td> 
   <td> <p>Registra los ingresos, horas o gastos que se pueden facturar. Esta información se puede utilizar para crear facturas en un sistema de contabilidad externo.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Crear registros de facturación</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Estado de registro de facturación</td> 
   <td> <p>En un informe Registro de facturación o Hora, el estado de un registro de facturación indica si el registro de facturación se ha facturado o no se ha facturado. No puede eliminar un proyecto ni editar la hora asociada a un registro de facturación facturado. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crear registros de facturación</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td>El proceso de personalización [!DNL Workfront] para dar a la interfaz un aspecto que refleje su empresa utilizando sus colores y logotipos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rutas de exploración]</td> 
   <td> <p>Área en la parte superior de la página que muestra la ubicación jerárquica de donde se encuentra el usuario en la aplicación.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obtener más información, consulte <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Información general sobre rutas de exploración</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado del presupuesto]</td> 
   <td> <p>Se trata de un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado y el campo no se puede actualizar. </p> <p>Este campo muestra si el proyecto se agregó al [!UICONTROL Capacity Planner] y si el cálculo del presupuesto se ha completado para él. El [!UICONTROL Capacity Planner] se ha eliminado de [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización presupuestada]</td> 
   <td> <p>Se trata de un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado. Este campo no se puede actualizar. </p>
   <p> Este campo sigue visible en los informes y listas de [!UICONTROL project] y [!UICONTROL tasks].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo presupuestado]</td>

<td> <p>Este es el costo asociado con la presupuestación de recursos para un proyecto. </p>
   <p>El campo se muestra en las siguientes áreas de [!DNL Workfront] con los nombres siguientes:</p>
   <ul>
   <li><strong>[!UICONTROL Costo presupuestado]</strong>: en el panel [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Cost]</strong>: en las áreas [!UICONTROL Utilization] al visualizar información por [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Costo presupuestado del proyecto]</strong>: en listas e informes</li>
   </ul>   
    <p>El [!UICONTROL Costo presupuestado] del proyecto se calcula mediante la fórmula siguiente:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Para obtener más información sobre el cálculo de [!UICONTROL Coste presupuestado] y para comprender los distintos nombres de este concepto en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular costo presupuestado del proyecto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas presupuestadas]</td> 
   <td> <p>Horas presupuestadas para los recursos para el trabajo que necesitan completar en los proyectos. Este campo hace referencia a las horas presupuestadas en el área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] (o en el [!UICONTROL Resource Planner]) para el proyecto o para los recursos del proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender [!UICONTROL Costo de trabajo presupuestado] y [!UICONTROL Horario presupuestado] para proyectos</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Para obtener información sobre cómo presupuestar usuarios en la variable [!DNL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Los recursos presupuestarios de [!DNL Resource Planner] uso de las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>. </p> 
    <p>Las horas presupuestadas en el área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] o del [!UICONTROL Resource Planner] se muestran en las siguientes áreas de [!DNL Workfront] y con los nombres siguientes:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nombre para mostrar de [!UICONTROL Horas presupuestadas]</strong></td> 
        <td><strong>Áreas de [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas]</td> 
        <td>Área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] visualizado por [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas presupuestadas]</td> 
        <td> <p>Vista del informe de uso [!UICONTROL Hours]</p> <p>Para obtener más información sobre el informe [!UICONTROL Utilization], consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Descripción general del informe [!UICONTROL Resource Utilization]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Horas]</td> 
        <td> <p>Informe de [!UICONTROL BudHour]</p><p>El objeto [!UICONTROL Budgeted Hour] del informe de horas presupuestadas hace referencia a información relacionada con una herramienta de administración de recursos obsoleta. Solo el "[!UICONTROL Bud. El campo Horas]" de este informe hace referencia a las horas presupuestadas en el [!UICONTROL Resource Planner] o el área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] del proyecto. </p> <p>Para obtener más información sobre la creación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Horas Presupuestadas] </td> 
        <td> <p>Se encuentra en los siguientes informes:</p>
        <ul>
        <li>Informe [!UICONTROL Project]
        <li>Informe [!UICONTROL Project (Financial Data)]
        <li>Informe [!UICONTROL Task]
        <li>Informe [!UICONTROL Problema]
        <li>Informe de [!UICONTROL BudHour]</li>
        </ul>
         <p>Para obtener más información sobre la creación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Cualquier otra mención de [!UICONTROL Horario presupuestado] en [!DNL Adobe Workfront] hace referencia a las horas presupuestadas utilizando funciones obsoletas que se han eliminado de Workfront . Son campos de solo vista y no se actualizan con la información actual cuando se utilizan herramientas de presupuestación de recursos actuales. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coste de trabajo presupuestado]</td> 
   <td> <p>Este es el coste asociado con las horas que usted, como gestor de recursos, presupuesta para sus funciones de trabajo para el trabajo que necesitan completar en proyectos. </p> <p>El [!UICONTROL Costo de mano de obra presupuestado] de un informe de proyecto se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Este campo puede hacer referencia a lo siguiente:</p> 
    <ul> 
     <li> <p>Costes de mano de obra mostrados en el área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] o en el [!UICONTROL Resource Planner] que están asociados al coste de las funciones de trabajo en un proyecto. Para obtener información sobre el cálculo del [!UICONTROL Costo de mano de obra presupuestado], consulte el artículo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Comprender el coste laboral presupuestado] y [!UICONTROL Horas presupuestadas] para proyectos</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Costes laborales que se muestran en el área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] que reflejan los [!UICONTROL People Costs] estimados en una iniciativa vinculada al proyecto desde el [!DNL Scenario Planner] cuando use el planificador de escenarios para presupuestar los recursos del proyecto. Para obtener información sobre iniciativas, consulte <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Información general sobre las iniciativas en el planificador de escenarios</a>. </p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">La variable [!DNL Scenario Planner] información general</a>. </p> </li> 
     <p>Se muestra en las siguientes áreas de bajo los nombres siguientes:</p>
   <ul>
   <li><strong>[!UICONTROL Coste de trabajo presupuestado]</strong>: en el área [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Costo presupuestado]</strong>: en la vista [!UICONTROL Utilization] report [!UICONTROL Cost]
   <p>Para obtener más información, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información de utilización de recursos </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: en el [!DNL Resource Planner] Proyecto o [!DNL Role] vistas, al ver por coste
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: en los siguientes informes: 
   <ul>
    <li>Informe [!UICONTROL Project]</li>
    <li>Informe [!UICONTROL Project (Financial Data)]</li>
    <li>Informe [!UICONTROL Task]</li>
    <li>Informe [!UICONTROL Problema]</li>
    <li>Informe de [!UICONTROL BudHour]</li> 
    </ul>
    <p>Para obtener más información sobre la creación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Fecha de inicio presupuestada]</td> 
  <td> <p>Se trata de un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado. Este campo no se puede actualizar.</p>
  <p>Estas áreas se han eliminado de [!DNL Workfront]. </p> 
  <p>El campo sigue visible en los informes y listas de [!UICONTROL project] y [!UICONTROL task].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>Gráfico de líneas que proporciona una representación visual del trabajo completado y restante.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Caso empresarial]</td> 
   <td> <p>Herramienta utilizada para evaluar si un proyecto debe moverse hacia delante del estado [!UICONTROL Idea] al estado [!UICONTROL Planning]. En otras palabras, un [!UICONTROL business case] ayuda a la organización a decidir si vale la pena iniciar y completar el proyecto o no, especialmente al comparar proyectos con otros de un portafolio.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Crear un [!UICONTROL Business Case] para un proyecto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Caso de negocio: horas presupuestadas]</td> 
   <td> <p>Se trata de un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado. Este campo no se puede actualizar.</p> <p>Este campo sigue visible en las listas de proyectos y [!UICONTROL task] e informes. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignación calculada]</td> 
   <td> <p>Uno de los tipos de tarea [!UICONTROL Duration]. Esto calculará el porcentaje de un día laboral de 8 horas que el usuario asignado a la tarea se asignará a la tarea, según la [!UICONTROL Duration] de la tarea y el [!UICONTROL Work Required].</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Duration] y [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabajo calculado]</td> 
   <td> <p>Una de las tareas [!UICONTROL Duration Types]. Esto calculará el [!UICONTROL Work Required] en una tarea, dados los porcentajes [!UICONTROL Duration] y [!UICONTROL Assignment] del usuario (que se basan en un día laboral de 8 horas).</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Duration] y [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendario]</td> 
   <td> <p>Existen dos tipos de calendarios en [!DNL Workfront]: los informes [!UICONTROL Home Calendar] y calendario .</p> <p>El [!UICONTROL Home Calendar] es un calendario personal que permite al usuario administrar su carga de trabajo en relación con las horas disponibles en [!DNL Workfront]. El usuario también puede integrar su [!UICONTROL Home Calendar] con [!DNL Outlook] ([!DNL Google] y [!DNL Microsoft] integración próximamente). </p> <p>Para obtener más información sobre el [!UICONTROL Home Calendar], consulte <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">Vista del [!UICONTROL Home Calendar]</a>.</p> <p>Un informe de calendario es un informe dinámico en el que los usuarios pueden ver la fecha y otros detalles importantes de un evento, incluida la fecha de vencimiento, el estado del trabajo y el usuario al que se asigna el evento.</p> <p> Para obtener más información sobre los informes de calendario, consulte <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Información general sobre los informes del calendario</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Puede Iniciar]</td> 
   <td> <p>Este campo indica si una tarea está lista para empezar a trabajar en ella. Si el inicio está listo para trabajar en el campo [!UICONTROL Can Start] de la tarea se establece en [!UICONTROL True]. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Descripción general de "[!UICONTROL Can Start]" para tareas</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Capacidad</p> </td> 
   <td> <p>El tiempo disponible de un recurso cuando se puede asignar para que funcione. Consulte "Disponibilidad". </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Categoría]</p> </td> 
   <td> <p>Una categoría es un formulario personalizado. Puede crear informes para este objeto y mostrarlos también en otros informes de objeto. No todos los objetos pueden tener un formulario personalizado o una categoría. Los siguientes objetos pueden tener un formulario personalizado: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL Usuario]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteración]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de categoría]</td> 
   <td> <p>Cuando se agrega como columna a la vista de cualquiera de los siguientes objetos, muestra una lista de todos los formularios personalizados asociados a estos objetos:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Problema]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL Usuario]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteración]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestión de cambios]</td> 
   <td>Un área de prácticas se centró en definir, comprender y adaptar el trabajo planificado a los cambios en el alcance, el programa, el costo y los factores de recurso.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cambiar orden]</td> 
   <td>Tipo de cuestión planteada a un proyecto que describe un cambio solicitado en el alcance acordado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambiar solo]</td> 
   <td>Uno de los [!UICONTROL Update Types] del proyecto. Solo actualiza las líneas de tiempo [!UICONTROL Project Projected] y [!UICONTROL Planned] cuando se realizan actualizaciones en Tareas o ediciones en el proyecto o tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambiar orden]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Problema], que normalmente indica que se debe realizar una cantidad de trabajo no planificada antes de que se pueda completar el proyecto.</p> <p>Para obtener más información sobre los tipos de [!UICONTROL Problema], consulte la sección "Tipos de problemas predeterminados" en el artículo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalización de tipos de problemas predeterminados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea secundaria]</td> 
   <td>Una tarea que es una [!UICONTROL Subtask] de una [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>La colección de [!UICONTROL Subtasks] a [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] y [!UICONTROL Training]</td> 
   <td>Módulos de aprendizaje, certificaciones, estándares o una comunidad de prácticas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Una herramienta de comunicación para que los usuarios establezcan expectativas con respecto a los envíos de tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de confirmación]</td> 
   <td>Una herramienta de comunicación para que el usuario establezca expectativas en torno a los envíos de tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] y [!UICONTROL Reporting]</td> 
   <td>Normas para revisar las excepciones y el estado de un proyecto, programa o portafolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Una [!UICONTROL Company] es una unidad organizativa de [!DNL Workfront]. </p> 
   <p> Puede asociar un usuario o un proyecto con una empresa. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Crear y editar empresas</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización]</td> 
   <td> <p>La fecha en la que se ha definido para completarse un proyecto, tarea o problema. Existen varios tipos de [!UICONTROL Fechas de finalización] en [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Fecha real de finalización]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Descripción general del proyecto [!UICONTROL Fecha real de finalización] </a>.</li> 
     <li>[!UICONTROL Fecha de finalización planeada]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establezca el proyecto [!UICONTROL Fecha de finalización planeada]</a> y <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Fecha de finalización prevista]</a>.</li> 
     <li>[!UICONTROL Fecha de finalización prevista]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre [!UICONTROL Fecha de finalización prevista] para proyectos, tareas y problemas</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Día de finalización]</td> 
   <td>El día, relativo al inicio de la [!UICONTROL Template], en el que se supone que se debe completar una [!UICONTROL Template Task] o una [!UICONTROL Template].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de finalización]</td> 
   <td> <p>Esto indica cómo se marcará un proyecto como [!UICONTROL Complete]. Puede tener dos valores:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: Un usuario debe cambiar el estado del proyecto a [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automático]: El estado del proyecto cambiará automáticamente a [!UICONTROL Complete] cuando todas las tareas del proyecto se hayan completado al 100% y se hayan cerrado todos los problemas.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Es una representación visual del progreso de una tarea, problema o proyecto.</p> <p>Para los proyectos, el propietario del proyecto puede configurar manualmente la condición o automáticamente [!DNL Workfront], en función del estado de progreso del proyecto. </p> <p>Los valores posibles para la condición del proyecto son:</p> 
    <ul> 
     <li>[!UICONTROL En Target]</li> 
     <li>[!UICONTROL En Riesgo]</li> 
     <li>[!UICONTROL En Problemas]</li> 
    </ul> <p>Para obtener más información sobre la condición del proyecto, consulte el artículo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Información general sobre [!UICONTROL Project Condition] y [!UICONTROL Condition Type]</a>.</p>
     <p>Puede asociar tareas y condiciones de problema con un número que se pueda mostrar en los informes. Las listas siguientes muestran los nombres y números predeterminados para las condiciones de problema y tarea. El administrador del sistema puede actualizar los nombres de las condiciones y pueden agregar nuevas condiciones con números diferentes. Una vez asociado un número a una condición, no se puede editar.  </p> 
     <p>Para las tareas, el propietario de la tarea establece manualmente la condición. Los valores posibles para la condición de tarea son:</p> 
    <ul> 
     <li>[!UICONTROL Suavemente] (0)<br></li> 
     <li> [!UICONTROL Algunas preocupaciones] (1)<br></li> 
     <li>[!UICONTROL Principales Bloques de Carretera] (2)</li> 
    </ul> <p>Para obtener más información sobre la condición de tarea, consulte el artículo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Actualizar [!UICONTROL Condition] para tareas y problemas</a>.</p> <p>Para los problemas, el propietario del problema establece manualmente la condición. Los valores posibles para la condición del problema son:<br></p> 
    <ul> 
     <li>[!UICONTROL Suavemente] (0)<br></li> 
     <li>[!UICONTROL Algunas preocupaciones] (1)<br></li> 
     <li>[!UICONTROL Principales Bloques de Carretera] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Cuando se realiza el seguimiento del campo [!UICONTROL Condition] en los informes [!UICONTROL Journal Entry], los [!UICONTROL New] y [!UICONTROL Old Number Values] muestran el número asociado a la condición en lugar de su nombre. Si una condición no está definida originalmente para una tarea o un problema y más adelante la actualiza, la entrada del historial que captura la actualización mostrará el [!UICONTROL Valor de número antiguo] del campo [!UICONTROL Condición] como -2.147.483.648. Consulte también "[!UICONTROL Nuevo valor de número]", "[!UICONTROL Valor de número antiguo]" y "[!UICONTROL Entrada de diario]" en este artículo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Este campo muestra la condición actual de las tareas, los proyectos o los problemas. Esta opción muestra las actualizaciones más recientes que los propietarios de tareas, proyectos o problemas han proporcionado en el campo [!UICONTROL Update Status], junto con la nueva condición.</p> <p>Los comentarios realizados en las actualizaciones de condiciones no se muestran en la columna [!UICONTROL Condition Update]; solo se muestra la actualización principal.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de restricción]</td> 
   <td> <p>Si utiliza una [!UICONTROL Task Constraint] vinculada a una fecha específica, como [!UICONTROL Must Start On], esa fecha específica pasa a ser la [!UICONTROL Constraint Date] de la tarea.</p> <p>Las siguientes restricciones de tareas actualizan el campo [!UICONTROL Fecha de restricción]:</p> 
    <ul> 
     <li>[!UICONTROL Debe Iniciar En]</li> 
     <li>[!UICONTROL Debe Finalizar El]</li> 
     <li>[!UICONTROL Iniciar No Más Tarde Que]</li> 
     <li>[!UICONTROL Inicio no anterior a]</li> 
    </ul> <p>Sugerencia:   
     <ul> 
      <li> <p>Una tarea con una [!UICONTROL Constraint] de [!UICONTROL Fechas fijas] no tiene ninguna [!UICONTROL Fecha de restricción]. </p> </li> 
      <li> <p> [!UICONTROL Fecha de restricción] solo se puede ver en un informe o en una vista personalizada.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Día de restricción]</td> 
   <td> <p>Si está utilizando una restricción de tarea en una tarea de plantilla vinculada a un día específico, como Debe comenzar el, ese día específico se convierte en el Día de restricción de la tarea de plantilla.</p> <p>Las siguientes restricciones de tarea actualizan el campo [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Debe Iniciar En]</li> 
     <li>[!UICONTROL Debe Finalizar El]</li> 
     <li>[!UICONTROL Iniciar No Más Tarde Que]</li> 
     <li>[!UICONTROL Inicio no anterior a]</li> 
    </ul> <p>Sugerencia: [!UICONTROL Días de restricción] solo se puede ver en un informe o en una vista personalizada. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de restricción]</td> 
   <td> <p>Tendencia de programación de una tarea. Por ejemplo, [!UICONTROL Tan pronto como sea posible] programará una tarea para que comience lo antes posible y [!UICONTROL Finalizar no más tarde de] programará una tarea para que finalice por [!UICONTROL Constraint Date] y no más tarde.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre [!UICONTROL Task Constraint]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menú contextual]</td> 
   <td>Menú situado en la parte izquierda de la pantalla, en el que los elementos cambian para correlacionarse con el contenido activo. Por ejemplo, cuando un usuario está viendo un proyecto, el [!UICONTROL Contextual Menu] mostrará vínculos a información y herramientas relacionadas con el proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Creador de problemas convertidos]</td> 
   <td>Campo de un informe de proyecto o tarea que muestra información sobre el usuario que es el [!UICONTROL contacto principal] de un problema cuando el problema se convierte en un proyecto o una tarea. El campo también se muestra en la sección [!UICONTROL Project Details] donde se muestra el nombre del [!UICONTROL Primary Contact] del problema convertido. Consulte también "[!UICONTROL Primary Contact]" en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Cantidad monetaria que debe gastar al completar un proyecto, una tarea o un problema. </p> <p>Puede realizar el seguimiento de varios tipos de costes de mano de obra, gastos y riesgos relacionados con el proyecto. Para obtener información sobre el seguimiento de costes en [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/track-costs.md">Seguimiento de costes</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de coste]</td> 
   <td>Para una tarea, el [!UICONTROL Cost Type] determina cómo acumulará los costes la tarea. Algunos ejemplos son [!UICONTROL Fijo por hora], [!UICONTROL Usuario por hora] y [!UICONTROL Usuario por hora más Fijo]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependencias entre proyectos]</td> 
   <td> <p>Una tarea de un proyecto depende de una tarea de otro proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Crear predecesores entre proyectos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Datos personalizados]</td> 
   <td> <p>Datos exclusivos de una organización. Las organizaciones pueden personalizar el [!DNL Workfront] al crear formularios personalizados y campos personalizados. Esta información personalizada puede generar informes para KPI, auditoría y combinación de demanda. </p> <p>[!UICONTROL Datos personalizados] puede estar vinculado a:</p> 
    <ul> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Usuarios]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de datos personalizado]</td> 
   <td>La opción para especificar si un campo de [!UICONTROL Personalizar datos] está almacenado en la base de datos como Texto, Fecha, Número o Moneda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de visualización personalizado]</td> 
   <td>El campo muestra el tipo de campo personalizado. Algunos ejemplos son [!UICONTROL Desplegable], [!UICONTROL Campo de texto], [!UICONTROL Área de texto], [!UICONTROL Botones de radio], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo personalizado]</td> 
   <td>Para los datos personalizados que permiten al usuario seleccionar entre varias opciones, estos son los valores que puede seleccionar un usuario. Las opciones personalizadas solo son válidas en las casillas de verificación [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop Down], [!UICONTROL Radio Button] y [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Etiqueta de formulario personalizada]</td> 
   <td>Cuando se utiliza un tipo de visualización personalizado con opciones personalizadas, este es el texto de la interfaz de usuario que se mostrará en el menú desplegable, las casillas de verificación o los botones de opción de esa opción personalizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor personalizado]</td> 
   <td>Cuando se utiliza un campo personalizado con opciones personalizadas, este es el valor que se almacenará en la base de datos para una opción determinada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vista personalizada]</td> 
   <td>Definición de los campos de datos, o columnas, que se muestran para cada objeto de una lista.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Organización que utiliza una instancia de Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Tableros]</td> 
   <td> <p> Puede agregar este campo en un informe o en una lista del objeto de informe para mostrar los tableros en los que se enumera el informe en una lista. </p> <p> Puede utilizar este campo para filtrar también los informes que aparecen en un tablero específico. </p> <p> Para obtener más información sobre cómo incluir información de tablero en informes de objetos de informe, consulte la sección "Explicación de los informes que se enumeran en tableros" del artículo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Acceso y organización de informes</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de datos]</td> 
   <td>Consulte "[!UICONTROL Tipo de datos personalizado]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Días tarde]</td> 
   <td> <p>Este campo muestra una diferencia de fecha entre [!UICONTROL Planned Start] y [!UICONTROL Today] si falta la [!UICONTROL Actual Completion Date].</p> <p>También muestra una diferencia de fecha entre [!UICONTROL Real Completion] y [!UICONTROL Planned Completion], cuando existe una [!UICONTROL Real Completion Date].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Programación predeterminada]</td> 
   <td> <p>Horas de trabajo predeterminadas personalizables que se asignarán a usuarios y proyectos dentro de una organización. </p> <p>Las programaciones se utilizan para calcular las fechas de planificación, inicio y finalización de las tareas asignadas a los usuarios.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Bienes o servicios cuantificables que deben prestarse al término de un proyecto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Administración de la demanda]</td> 
   <td>Puntuación y priorización de los procesos de admisión.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Objetivos del Departamento]</td> 
   <td>Objetivos exclusivos de un departamento específico que se centran en mejorar las métricas operacionales dentro del departamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>El vínculo entre dos tareas que requieren que una tarea cambie de estado antes de que la otra tarea también pueda cambiar de estado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de dependencia]</td> 
   <td> <p>Tipo de relación de programación entre una tarea y sus predecesores. Un ejemplo es [!UICONTROL Finish-Start], que requiere que la primera tarea debe finalizar antes de que la segunda tarea pueda comenzar.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Descripción general de los tipos de dependencia de tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Cualquier archivo adjunto a un objeto dentro de [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Cada vez que se carga el mismo documento en el mismo objeto, se le asigna un número de versión. Los usuarios pueden ver y cambiar varias opciones para una versión anterior de un documento.</p> <p>Para obtener más información, consulte <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Administrar versiones de documentos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duración]</td> 
   <td> <p>Período de tiempo asignado para la finalización de un problema de tarea o proyecto (determinado por el número de días entre el [!UICONTROL Planned Start] y la finalización planificada).</p> 
    <ul> 
     <li>Para las tareas, la Duración es un campo editable si el Tipo de duración de la tarea no es Simple. Si el tipo de duración de la tarea es simple o si la restricción de tareas es Fechas fijas, la duración es un cálculo realizado por Workfront.</li> 
     <li>Para los problemas, la Duración es siempre un campo editable y debe representar una estimación de un número de días que requerirían que se resolviera el problema.</li> 
     <li>Para los proyectos, Duración es un cálculo realizado por [!DNL Workfront] y representa la diferencia en días entre el Inicio planificado de la tarea más temprana y la [!UICONTROL Finalización planificada] de la tarea más reciente del proyecto.</li> 
    </ul> <p>Para obtener más información sobre la diferencia entre [!UICONTROL Duration] y [!UICONTROL Planned Duration] para las tareas, consulte el artículo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Diferencia entre [!UICONTROL Duración planificada] y [!UICONTROL Duración] para tareas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duración en minutos]</td> 
   <td>Este campo muestra la misma información que el campo [!UICONTROL Duration] en minutos en lugar de días. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duración por incidencia]</td> 
   <td> <p>Esto se muestra en los cuadros [!UICONTROL Task Details] y [!UICONTROL Edit Task] de un elemento principal de las tareas recurrentes. Muestra la duración de cada tarea recurrente. Para obtener información sobre la creación de tareas recurrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> <p> <span>Las duraciones modificadas en tareas recurrentes individuales no muestran el valor indicado en este campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo de duración]</td> 
   <td> <p>Campo de tarea que indica cómo se asigna el trabajo necesario para completar la tarea a los destinatarios asignados a lo largo de la duración de la tarea. Representa la relación entre la [!UICONTROL Duration] de la tarea, el [!UICONTROL Work Required] y la cantidad de tiempo, o [!UICONTROL Allocation], que los recursos asignados deben invertir en la tarea para completarla. </p> <p>Este campo aparece en la pestaña [!UICONTROL Details] de una tarea. </p> <p>Las opciones son:</p> 
    <ul> 
     <li>[!UICONTROL Asignación calculada]</li> 
     <li>[!UICONTROL Trabajo calculado]</li> 
     <li>[!UICONTROL Esfuerzo conducido]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Duration] y [!UICONTROL Duration Type]</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unidad de duración]</td> 
   <td>Unidad que se utiliza para medir el tiempo en una búsqueda de energía.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esfuerzo conducido]</td> 
   <td>Relación entre el número de usuarios y la cantidad de tiempo que tardará la tarea en completarse. A medida que agrega más usuarios, el tiempo total programado para que la tarea se complete disminuye, pero la duración de la tarea permanece igual. Por ejemplo, si una tarea está bombardeando un barril de maníes, añadir más personas reducirá el tiempo programado, pero la duración en días-persona seguirá siendo la misma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo transcurrido]</td> 
   <td> <p>[!UICONTROL Tiempo transcurrido] es una unidad de tiempo para la [!UICONTROL Duración] de una tarea. Es la hora entre la [!UICONTROL Fecha de inicio planeada] y la [!UICONTROL Fecha de finalización planeada] de una tarea que incluye festivos, fines de semana y tiempo libre. En otras palabras, el tiempo transcurrido es el paso de días naturales. </p> <p>[!DNL Workfront] admite las siguientes unidades de tiempo transcurrido para la duración de la tarea:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minutos transcurridos]</p> </li> 
     <li> <p>[!UICONTROL Horas transcurridas]</p> </li> 
     <li> <p>[!UICONTROL Días transcurridos]</p> </li> 
     <li> <p>[!UICONTROL Semanas Transcurridas]</p> </li> 
     <li> <p>[!UICONTROL Meses transcurridos]</p> </li> 
    </ul> <p>Para obtener más información sobre la duración de la tarea, incluido el tiempo transcurrido, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Duration] y [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización]</td> 
   <td> <p> En un informe de [!UICONTROL Rate], es la fecha en la que finaliza una nueva tasa de facturación de una función de trabajo a nivel de proyecto. Las horas asociadas al proyecto que son anteriores a esta fecha se multiplican por esta tasa de facturación para calcular los ingresos del proyecto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Participación]</td> 
   <td>El [!UICONTROL Work Performance Indicator] (WPI) que indica cuándo está disminuyendo el compromiso y la fe en la tarea, el proyecto, el equipo o la organización. Esto indica que debe actuar para revivir esa creencia y ese compromiso. La WPI se mediría haciendo preguntas sencillas: "¿Entendiste lo que se esperaba de ti? ¿El trabajo que le asignaron marcó una diferencia para la organización? ¿Hiciste el trabajo bueno?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Objetivos empresariales]</td> 
   <td>Objetivos interfuncionales que contribuyen a las métricas de los objetivos de la empresa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Cualquier cambio en un proyecto o tarea.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Tareas automatizadas que se producen cuando se producen eventos. Un ejemplo común es una notificación automática por correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>Correo electrónico generado a partir de un controlador de eventos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>Coste no laboral en tareas o proyectos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externo]</td> 
   <td> <p>Normalmente, un tipo de licencia, o un usuario con dicha licencia, que solo tiene la capacidad de revisar la información en el sistema.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] información general sobre licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sistema externo]</td> 
   <td>Cualquier servicio o software que esté almacenado y regido fuera del sistema de registro designado.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Cualquier objeto de Workfront o la información asociada a él, tal como aparece en la base de datos. </p>
   <p>Por ejemplo, "proyecto", "usuario", "hora" son objetos de Workfront y campos. "Nombre", "estado", "propietario", "fecha de inicio" son campos de Workfront asociados a los objetos anteriores. </p>

<p>Al referirse a los objetos, los términos "objetos" y "campos" pueden utilizarse de forma intercambiable.</p>
   <p>En el ámbito de los informes, los "campos" hacen referencia a los objetos o a la información sobre el objeto que desea capturar en el informe.</p>

<p><b>NOTA</b></p>

<p>En los informes de texto adicional, los campos hacen referencia a los objetos o a su información tal como aparece en la base de datos.</p>
   <p>A veces, el nombre que se ve en la interfaz de usuario es diferente del nombre del campo de la base de datos. Por ejemplo, "problema" es el nombre del objeto en la interfaz de Workfront, pero "opTask" es el nombre del objeto (o el campo) en la base de datos de Workfront. </p> 
   <p> Es importante utilizar el campo como aparece en la base de datos al escribir un informe, una vista, un filtro o una agrupación en modo de texto, o al crear un campo calculado.</p>

<p>Para obtener más información, consulte <a href="../../../wf-api/general/api-explorer.md">Explorador de API</a> y <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Información general sobre el modo de texto</a>.</p>

<p>De forma predeterminada, Workfront viene con un conjunto de campos que definen ambos objetos y su información. También puede crear campos personalizados para definir objetos, pero no puede crear objetos personalizados.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Uno de los componentes principales de un informe o un elemento de lista que define qué información se muestra en la pantalla. Para obtener más información sobre los elementos de informes, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de informes: filtros, vistas y agrupaciones</a>.</p> <p>El filtro determina los resultados que se muestran en un informe o en un [!DNL Workfront] listado de paneles, como proyectos, tareas o problemas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Proceso para administrar los datos de costos, gastos e ingresos laborales en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo fijo]</td> 
   <td>Puede definir una cantidad fija de coste para un proyecto. Esto forma parte del [!UICONTROL Costo planeado] del proyecto, que representa la cantidad de dinero necesaria para completar el proyecto. Para obtener información sobre los costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ingresos fijos]</td> 
   <td>Puede definir una cantidad fija de ingresos para un proyecto. Esto forma parte de los [!UICONTROL Ingresos planificados] del proyecto, que representan la cantidad de dinero que podría obtener si completa el proyecto. Para obtener información sobre los ingresos, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Este campo es el mismo que el de [!UICONTROL Status Icons], pero solo está disponible para las siguientes vistas: </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> Para obtener más información, consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en las vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Las carpetas se utilizan para organizar documentos o informes asociados a un objeto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (equivalente a tiempo completo)</td> 
   <td>Este es el equivalente de tiempo completo que indica la cantidad de tiempo que un recurso está disponible para trabajar. 
   El campo [!UICONTROL FTE] se muestra en las siguientes áreas: 
  <ul>
   <li> Perfil del usuario al editar o crear el usuario </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (requiere licencia adicional para Workfront Scenario Planner) </li>
   <li> Listas de usuarios e informes </li> </ul>

<p>El [!UICONTROL FTE] debe ser un número decimal de hasta 1 y no puede ser 0. </p>
   <p> Un [!UICONTROL FTE] de 1 (que es el valor predeterminado del campo [!UICONTROL FTE] de un usuario, tal como se define en su perfil) significa que un recurso (usuario o función) funciona durante todo el número de horas, según la programación que calcula su disponibilidad. </p>
   <p>El administrador de Workfront decide qué programación utilizar para determinar la disponibilidad del usuario.  </p>
   <ul>
   <li> Cuando se utiliza el [!UICONTROL Programación predeterminada], Workfront utiliza el [!UICONTROL FTE] del usuario que se encuentra en su perfil para calcular la disponibilidad. </li>
   <li> Cuando se utiliza la programación del usuario, Workfront utiliza el tiempo de espera del usuario, el valor [!UICONTROL Work Time] y las horas de [!UICONTROL Default Schedule] para calcular el [!UICONTROL FTE] del usuario. </li> </ul>

<p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a>.  </p>
   <p>Para obtener más información sobre la creación de programaciones en [!DNL Workfront], consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear una programación</a>. </p>

<p><b>NOTA</b></p>
   <p>Para todos los cálculos del [!UICONTROL Scenario Planner], Workfront utiliza el siguiente valor: 1 [!UICONTROL FTE] = 8 horas.</p>
   <p>Para obtener más información, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introducción al [!UICONTROL Scenario Planner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Diagrama de Gantt]</td> 
   <td> <p>Línea de tiempo visual de las fechas del proyecto en una vista de calendario basada en las fechas planificadas o proyectadas, ya que las tareas del proyecto están programadas actualmente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Hay dos conceptos de objetivos en [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Objetivos del proyecto</b>: Conjunto de objetivos empresariales acordados por los interesados pertinentes de un proyecto. Los objetivos del proyecto forman parte del caso empresarial de un proyecto. </p> <p>No es posible mostrar los objetivos del proyecto en listas o informes, pero puede acceder a ellos a través de la API. </p> <p>Para obtener información sobre los objetivos del proyecto Caso empresarial, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Crear objetivos de caso empresarial </a>. </p> </li> 
     <li> <p><b>Objetivos estratégicos</b>: Un objetivo estratégico es un objetivo que usted crea para planificar su estrategia de trabajo para un período de tiempo específico. Puede crear estos tipos de objetivos utilizando [!DNL Workfront Goals]. Su organización debe adquirir una licencia adicional y debe tener acceso a esta función para poder crear objetivos estratégicos. [!DNL Workfront Goals] solo están disponibles con una licencia adicional.</p> 
     <p>Para obtener más información, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] información general </a>. </p> 
     <p>Puede mostrar los objetivos estratégicos en un informe de objetivo o de proyecto y acceder a ellos a través de la API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Jerarquía de objetivos]</td> 
   <td> <p>En los informes [!UICONTROL Goal] y [!UICONTROL Project], se trata de un campo de recopilación que muestra los objetivos de la jerarquía a la que pertenece un objetivo estratégico cuando se adhiere a otros objetivos. Los objetivos se separan con un delimitador de -. </p> <p>En este campo solo se muestran los elementos primarios del objetivo y del objetivo. Los objetivos secundarios no se muestran. </p> <p>Para obtener información sobre cómo alinear objetivos en [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Información general sobre la alineación de objetivos en [!DNL Workfront Goals]</a>. </p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos, use [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] información general </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Succore Score]</td> 
   <td> En un [!UICONTROL Project report], este campo se utilizaba para hacer referencia a los objetivos de nivel de proyecto asociados con el caso [!UICONTROL Business]. Actualmente, se trata de un campo obsoleto y no está asociado a ninguna funcionalidad.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objetivos] </td> 
   <td> <p>En un informe [!UICONTROL Project], se trata de un campo de recopilación que muestra todos los objetivos estratégicos asociados a un proyecto. Los objetivos están separados por comas.</p> <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos, use [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] información general</a>. Para obtener más información sobre los objetivos estratégicos y los objetivos del proyecto en [!DNL Workfront], consulte "[!UICONTROL Goal]" en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Configuración de interfaz que afecta a todos los usuarios. [!UICONTROL Global Interface Preferences] se puede sobrescribir mediante las [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Colección de usuarios (posiblemente del mismo departamento o unidad de negocio) que tienen acceso a los mismos objetos. Además de los usuarios, los grupos pueden asociarse con portafolios, programas, proyectos,<span> plantillas de proyecto,</span> empresas, equipos, programaciones, plantillas de diseño y perfiles de parte de horas.</p> <p>También puede conceder permisos a los objetos por grupo. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general sobre grupos</a>.</p> <p>En una lista o informe de objetos de uno de los siguientes tipos, puede utilizar el campo [!UICONTROL Group] para enumerar qué objetos de ese tipo están asociados a un grupo en particular: usuario, portafolio, programa, proyecto, <span>plantilla de proyecto</span>, empresa, equipo, programación, plantilla de diseño o perfil de parte de horas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Usuarios que administran los objetos, el acceso y los usuarios de los grupos de usuarios designados.</p> <p> En un informe de [!UICONTROL Group], este campo muestra los nombres de los usuarios designados como [!UICONTROL Group Administradores] en el grupo. Para obtener más información sobre los administradores de grupo, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Grupo con acceso de administración]</td> 
   <td> <p> En un [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile] o [!UICONTROL Schedule report], este campo muestra los grupos a los que los administradores de grupo tienen acceso para modificar la plantilla. También puede filtrar este informe por este campo. </p> <p> Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>Elemento de informe utilizado para categorizar la información de una lista según un criterio común.</p> <p>Para obtener más información, consulte la sección "[!UICONTROL Groupings]" en el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de informes: filtros, vistas y agrupaciones</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de entrega]</td> 
   <td> <p>La fecha en la que una tarea está disponible para el trabajo. La [!UICONTROL Handoff Date] es un cálculo y no se puede configurar manualmente. <br>Para obtener más información sobre la [!UICONTROL Fecha de entrega], consulte el artículo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Información general sobre [!UICONTROL Task Handoff Date]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>La parte de [!DNL Workfront] que contiene todas las colas de problemas. El [!UICONTROL Help Desk] se puede utilizar para procesar solicitudes de soporte al cliente, solicitudes de proyectos, tickets de asistencia técnica, etc. Es igual que el área [!UICONTROL Solicitudes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propietario]</td> 
   <td>En un informe de [!UICONTROL Hour], [!UICONTROL Owner] es el usuario al que se atribuyen las horas. Esto es diferente al usuario que está registrando la hora. Estas dos entidades a veces pueden ser dos usuarios diferentes. <br>Para obtener más información sobre el tiempo de registro de otro usuario, consulte el artículo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tiempo de registro</a>.</td> 
  </tr>

<tr> 
   <td>Estado de hora</td> 
   <td> <p>Atributo establecido por Workfront para las horas reales que los usuarios registran para tareas, problemas o proyectos. </p>

Las entradas de hora pueden tener uno de los siguientes estados en Workfront:
<ul>
   <li><b>Enviado</b>: las horas se han registrado en un proyecto, tarea o problema. Forman parte de un registro de facturación o aún no se han agregado a un registro de facturación.</li>
   <li><b>Aprobado</b>: las horas se han registrado y el propietario del proyecto las ha aprobado. Forman parte de un registro de facturación o aún no se han agregado a un registro de facturación.</li> 
   <li><b>No aprobado</b>: el propietario del proyecto ha registrado y rechazado las horas. Forman parte de un registro de facturación o aún no se han agregado a un registro de facturación.</li>
   <li><b>Facturado</b>: las horas se han registrado, agregado a un registro de facturación y el estado del registro de facturación se ha marcado como Facturado. No era necesario que el propietario del proyecto los aprobara.</li>
   <li><b>Facturado y aprobado</b>: las horas se han registrado, aprobado por el propietario del proyecto y el estado del registro de facturación se ha marcado como Facturado.</li>
   </ul>


<p>Cuando las horas forman parte de un registro de facturación, el estado de la hora indica si se han aprobado las horas o si se ha facturado el registro de facturación al que pertenecen. El estado de la hora de una entrada de hora solo está visible en una lista de horas o en un informe. </p>

<p>Para obtener más información sobre la adición de horas a los registros de facturación, consulte la sección "Añadir horas a los registros de facturación" en el artículo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crear registros de facturación</a>.</p>

<p>Para obtener más información sobre la aprobación del tiempo en los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Requerir tiempo para ser aprobado para un proyecto</a>.</p>

<p><b>SUGERENCIA</b></p>

<p>Las horas generales que no se registran directamente en elementos de trabajo no muestran el estado de la hora. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Tipo de hora]</td> 
   <td> <p>Atributo que se puede configurar para horas reales y que los usuarios registran para tareas, problemas o proyectos. También es un atributo para las horas registradas que no están directamente vinculadas al trabajo, como [!UICONTROL Vacation] y [!UICONTROL Time Off].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Administrar tipos de hora</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>El ID es un indicador alfanumérico asociado a cada objeto de [!DNL Workfront]. Identifica de forma exclusiva cada objeto de la variable [!DNL Workfront] base de datos. Puede ver el ID de cualquier objeto de un informe o una lista para cada objeto. </p> <p>Sugerencia:   <p>También puede ver el ID en la dirección URL de la página del objeto. Por ejemplo, el ID de un proyecto puede tener un aspecto similar al número indicado en la siguiente URL, al acceder a la página [!UICONTROL Detalles del proyecto]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Objetivos individuales]</td> 
   <td>Objetivos individuales que contribuyen a las métricas de los objetivos del equipo, pero no relacionados con el desarrollo personal o profesional.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Acceso heredado]</td> 
   <td>Función de difusión que permite propagar el acceso de un objeto a otro. Por ejemplo, el acceso heredado del usuario del proyecto se define en los registros de programa y de portafolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>En el [!DNL Workfront Scenario Planner], puede dividir un plan en varias iniciativas para facilitar su administración. <span>Puede crear un informe de [!UICONTROL Initiative] y acceder a la información de [!UICONTROL Initiative] en un informe de [!UICONTROL Project].</span></p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">La variable [!DNL Scenario Planner] información general</a>. </p> <p>La variable [!DNL Initiative] El informe no está visible en el [!DNL Workfront] instancia a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia. No puede acceder a [!UICONTROL Initiatives] mediante la API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>El tipo de informe [!UICONTROL Initiative Job Role] muestra información sobre las funciones de trabajo asociadas con una iniciativa de plan en la [!DNL Workfront Scenario Planner].</span> </p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La variable [!DNL Scenario Planner] información general</a>. </p> <p><span>Este tipo de informe no es visible en su [!DNL Workfront] instancia a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Iniciativa Horario de trabajo]</span> </td> 
   <td> <p><span> En un informe [!UICONTROL Initiative Job Role] , se muestra el número de horas asociadas a una función de trabajo en una iniciativa.</span> </p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La variable [!DNL Scenario Planner] información general</a>. </p> <p>Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no están visibles en su [!DNL Workfront] instancia a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>En un informe de [!UICONTROL Initiative Job Role] , se muestra el número de una función de trabajo específica asociada a una iniciativa.</p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La variable [!DNL Scenario Planner] información general</a>. </p> <p>Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no están visibles en su [!DNL Workfront] instancia a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Iniciativa Fecha de la última publicación]</td> 
   <td> <p>Campo de los informes [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] y [!UICONTROL Project] que muestra la fecha en que se publicó por última vez una iniciativa de plan en un proyecto. Puede publicar iniciativas para crear proyectos o actualizar proyectos vinculados a las iniciativas.</p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La variable [!DNL Scenario Planner] información general</a>. </p> <p><span>Para obtener información sobre las iniciativas de publicación, consulte</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publicar escenarios para crear y actualizar proyectos en la variable [!DNL Workfront Scenario Planner]</a>. Este campo no está visible en el [!DNL Workfront] instancia a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Búsqueda en línea]</td> 
   <td>Búsqueda realizada, en el proceso de cumplimentación de un formulario, para encontrar posibles entradas para un campo específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>El área de la aplicación que permite definir Vistas personalizadas, Filtros, Agrupaciones, Controles de lista, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Es Objetivo De La Empresa]</p></td> 
   <td> <p>En [!DNL goal reports], se muestra un valor "[!UICONTROL True]/ [!UICONTROL False]" para cada objetivo estratégico a fin de indicar si su organización está asignada al objetivo como propietario. </p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos, use [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] información general </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema]</td> 
   <td> <p>Elemento de trabajo no planificado que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Se evalúa y evalúa para su ulterior examen del esfuerzo</p> <p>Un [!UICONTROL Problema] también puede ser una solicitud del [!UICONTROL Help Desk]. [!UICONTROL Change Orders], [!UICONTROL Requests] y [!UICONTROL Bugs] también son [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestión de problemas]</td> 
   <td> <p>Proceso y reglas que rigen la definición de tipos de problemas y el proceso de enrutamiento, ensayo o tráfico asociado a cada tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema Propietario]</td> 
   <td>El equipo o los usuarios responsables de probar y completar un problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteración]</td> 
   <td>Período de tiempo en el que un equipo produce un conjunto predefinido de entregables.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Puesto de trabajo]</td> 
   <td> <p>Se utiliza para identificar las funciones y responsabilidades cotidianas de un usuario. Las funciones de trabajo se pueden asignar a elementos de trabajo para identificar la habilidad necesaria para completar un proceso de trabajo sin asignarlo a un usuario específico. </p> <p>Un usuario puede tener más de una función. Algunos ejemplos son Diseñador gráfico o Consultor.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Entrada de diario]</p> </td> 
   <td> <p>Un objeto que se puede incluir en los informes y que proporciona información sobre las actualizaciones del sistema para los campos rastreados que aparecen en el área [!UICONTROL Actualizaciones] de proyectos, tareas, problemas y otros objetos.</p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Informar sobre el área [!UICONTROL Actualizaciones]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>En un informe de [!UICONTROL Task] o de [!UICONTROL Issue], el campo [!UICONTROL Kanban Flag] muestra el estado del indicador que se establece en el artículo del [!UICONTROL Kanban board]. Los valores posibles son [!UICONTROL On Track], [!UICONTROL Ready to Pull] y [!UICONTROL Is Blocked].</p> <p>Para obtener más información sobre la configuración del estado del indicador en artículos del tablero de artículos [!UICONTROL Kanban], consulte el artículo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Usar indicadores en historias en la [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Un valor mensurable que demuestra la eficacia con la que una empresa está alcanzando objetivos clave del negocio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Cantidad de tiempo que debe transcurrir después de que haya pasado el [!UICONTROL Fecha de finalización planeada] de la tarea predecesora hasta que pueda comenzar la tarea dependiente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de registro]</td> 
   <td> <p>Método de cálculo del [!UICONTROL Lag]. Puede ser:</p> 
    <ul> 
     <li>[!UICONTROL Días] (días laborables)</li> 
     <li>[!UICONTROL Calendar Days] (ignorar festivos)</li> 
     <li>[!UICONTROL Porcentaje]</li> 
     <li>[!UICONTROL Día de la semana]</li> 
    </ul> <p>Para obtener más información, consulte la sección "[!UICONTROL Información general sobre los tipos de retraso]" en <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Descripción general de los tipos de retraso</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura grande]</td> 
   <td> <p> En una lista o informe de [!UICONTROL Document], se muestra una vista previa del documento en una miniatura. </p> <p>Select <strong>[!UICONTROL Miniatura grande]</strong> para ver una miniatura de 400 píxeles de ancho en el informe.</p> <p>El tamaño de la miniatura se ajusta cuando se modifica el ancho de la columna en una lista o informe.</p> <p>Consulte también "[!UICONTROL Miniatura]" en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Últimos 10 visualizadores]</td> 
   <td> <p>En una lista de informes, este campo muestra los nombres de hasta 10 usuarios que vieron el informe más recientemente.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última nota de condición]</td> 
   <td> <p>Este campo muestra la última actualización introducida en un objeto por el propietario del objeto. Esta es la actividad o interacción más reciente del propietario en un objeto.</p> <p>La variable [!DNL Last Condition Note] está vacía si se ha eliminado el texto de la nota de la última nota de un objeto. Cuando se introduce una nota nueva en el objeto, esta se convierte en la última nota y se muestra de nuevo en la columna . </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última fecha de actualización de finanzas]</td> 
   <td>En un informe [!UICONTROL project], este campo captura la fecha y la hora en que se calcularon y actualizaron por última vez las finanzas del proyecto. Para obtener información sobre las finanzas de los proyectos, consulte <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Resumen de las finanzas del proyecto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última nota]</td> 
   <td> <p>Este campo muestra la última actualización introducida en un objeto por cualquier usuario. Esta es la actividad o interacción más reciente de un objeto.</p> <p>La columna [!UICONTROL Última nota] está vacía si se ha eliminado el texto de la última nota de un objeto. Cuando se introduce una nota nueva en el objeto, esta se convierte en la última nota y se muestra de nuevo en la columna .</p>
   <p>Cuando este campo se agrega a un informe de [!UICONTROL Task], cualquier actualización que quede en objetos secundarios (como problemas, subtareas, documentos, etc.). — de la tarea no se muestra en esta columna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última visualización por]</td> 
   <td> <p>En una lista de informes, este campo muestra información sobre el usuario que vio el último informe.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última fecha de visualización]</td> 
   <td> <p>En una lista de informes, este campo muestra la fecha en la que se mostró el informe por última vez.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Plantilla de diseño]</td> 
   <td>Definido por el administrador del sistema o el administrador del grupo para identificar las pestañas y los informes que se muestran en el espacio de trabajo de un usuario determinado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de diseño]</td> 
   <td>Junto con [!UICONTROL Vistas personalizadas], el [!UICONTROL Tipo de diseño] especifica el tipo de [!UICONTROL Vista personalizada]. Actualmente, solo Lista está disponible. En el futuro, es posible que [!UICONTROL Detail] (la vista [!UICONTROL Detail] de un objeto) esté disponible.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Library Task]</td> 
   <td>Una plantilla para una sola tarea que se utiliza para proporcionar un nombre coherente de [!UICONTROL Tasks] y [!UICONTROL Template Tasks] en toda la aplicación.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de licencia]</td> 
   <td>Tipo de licencia asignada a un [!UICONTROL Nivel de acceso]. Es [!UICONTROL Usuario completo], [!UICONTROL Usuario limitado] o [!UICONTROL Solicitante].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>En una vista o informe de [!UICONTROL Group], este campo muestra el número máximo de licencias de [!UICONTROL Plan] que se pueden asignar a usuarios que tienen el grupo respectivo designado como su [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Licencia de trabajo - trabajo</td> 
   <td> <p>En una vista o informe de [!UICONTROL Group], este campo muestra el número máximo de licencias de [!UICONTROL Work] que se pueden asignar a usuarios que tienen el grupo respectivo designado como su [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuario limitado]</td> 
   <td>Un tipo de licencia que permite crear una [!DNL Access Level] que contiene privilegios de solo vista, con la capacidad de enviar problemas, introducir notas y cargar documentos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Parte de [!UICONTROL Interface Setup] que permite vincular filtros personalizados, vistas y grupos a usuarios individuales o globalmente a todos los usuarios.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>Uno de los [!UICONTROL Project] de [!UICONTROL Update Types]. Esta configuración permite actualizar las líneas de tiempo [!UICONTROL Project Projected] y [!UICONTROL Planned] solo cuando se hace clic en "[!UICONTROL Cronologías recalculadas]". Los proyectos configurados de esta forma se ignorarán durante el proceso de cálculo ligero y cuando se actualicen el proyecto o la tarea del proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el proyecto [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Esto hace referencia al usuario que ha iniciado sesión en ese momento. </p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, puede crear solo un informe que muestre información diferente en función de quién inicie sesión para verla, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo de usuarios]</td> 
   <td> <p>Se trata de un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado y el campo no se puede actualizar. </p> <p>En versiones anteriores de [!DNL Workfront], puede actualizar este campo al crear o editar una función de trabajo. Se mostraba el número total de usuarios que se pueden asociar a una función en cada proyecto. Un valor de cero permitido para un número ilimitado de usuarios que se pueden asignar en un proyecto. </p>El campo sigue visible en algunos informes y listas, pero la información mostrada no se puede actualizar. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Un marcador que puede asociar con una tarea para indicar que se ha alcanzado un punto clave en el proyecto cuando se completa la tarea. Por lo general, se pueden usar hitos para mostrar un evento significativo, como la finalización de una fase del proyecto o un conjunto de actividades críticas. Los [!UICONTROL Milestones] generalmente están asociados a tareas principales. Debe crear los hitos para poder adjuntarlos a las tareas. Para obtener información sobre hitos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Crear una ruta de hitos</a> y <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Asociar hitos con tareas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Una colección de [!UICONTROL hitos]. [!UICONTROL Milestone Paths] se utilizan en Proyectos para distinguir proyectos con determinados tipos de [!UICONTROL Milestones] de proyectos con un conjunto diferente de [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarea Milestone]</td> 
   <td>Una tarea marcada para indicar un evento que se puede medir.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Un solo paso dentro de un escenario en [!DNL Workfront Fusion] que realiza alguna función basada en la aplicación asociada.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mi Función Principal]</td> 
   <td> <p>Cuando se hace referencia a esto en los filtros, se muestran los usuarios que tienen la misma [!UICONTROL Función principal] que el usuario que ha iniciado sesión, o los elementos de trabajo asignados a la [!UICONTROL Función principal] del usuario que ha iniciado sesión.</p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, puede crear solo un informe que muestre información diferente en función de quién inicie sesión para verla, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mi equipo de casa]</td> 
   <td> <p>Cuando se hace referencia a esto en los filtros, este campo muestra los usuarios que pertenecen al [!UICONTROL Home Team] del usuario que ha iniciado sesión o los elementos de trabajo asignados al [!UICONTROL Home Team] del usuario que ha iniciado sesión. </p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, puede crear solo un informe que muestre información diferente en función de quién inicie sesión para verla, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convención de nomenclatura]</td> 
   <td>Conjunto de reglas de toda la organización que utiliza datos para crear nombres de proyectos, tareas y envíos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Integración nativa]</td> 
   <td>Integración que no requiere codificación manual ni configuración de API. También se denomina integración "predeterminada".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menú de navegación]</td> 
   <td>Panel superior central de la aplicación que tiene vínculos a las áreas principales de [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Nuevo valor numérico]</td> 
   <td>En un informe [!UICONTROL Journal Entry], se muestra el valor actualizado de un campo que reemplaza al [!UICONTROL Old Number Value].
   Para obtener más información, consulte "[!UICONTROL Valor de número antiguo]" en este artículo.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Día no laborable]</td> 
   <td>Un día que no se asigna a la finalización de ninguna asignación. Generalmente es un día de vacaciones, de vacaciones o de fin de semana.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nota]</td> 
   <td>Un comentario o actualización realizados en un [!DNL Workfront] objeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nota Texto]</td> 
   <td> <p>Se muestra el texto de una actualización introducida por un usuario en cualquier objeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Número de objetivos vinculados]</td> 
   <td> <p>En un informe [!UICONTROL Project], es el número de objetivos estratégicos asociados al proyecto. Para obtener información sobre cómo asociar proyectos con objetivos estratégicos, consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Agregar proyectos a objetivos en  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Para obtener información sobre los objetivos estratégicos, consulte también "[!UICONTROL Goal]" en este artículo.</p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos, use [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Agregar proyectos a objetivos en [!UICONTROL Adobe Workfront Objectives]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL (objeto)</td> 
   <td> <p>La información que se muestra en [!DNL Adobe Workfront] se representa mediante objetos almacenados en la variable [!DNL Workfront] base de datos. Los objetos son lo que impulsa la información en Workfront. Algunos ejemplos de objetos son:</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Tableros]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Grupos]</li> 
     <li>[!UICONTROL Equipos]</li> 
     <li>[!UICONTROL Usuarios]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Formularios personalizados]</li>
     <li>[!UICONTROL Campos personalizados]</li>  
     <li>[!UICONTROL Horas]</li> 
     <li>[!UICONTROL Tasas de facturación]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Plantillas]</li>

<p><b>NOTA</b></p>
  <p>Esta no es una lista extensa. </p>

</ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de objetos]</td> 
   <td>Si crea un informe o una lista que contenga todos los formularios personalizados, puede utilizar este campo como una vista o un filtro para ver qué tipos de objeto están asociados a cada formulario. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Valor de número antiguo]</td> 
   <td>En un informe [!UICONTROL Journal Entry], se muestra el valor original de un campo antes de actualizarse. Una vez actualizado el valor de un campo, se mostrará como el [!UICONTROL Nuevo valor de número] en un informe [!UICONTROL Journal Entry]. Para obtener más información, consulte también "[!UICONTROL Nuevo valor numérico]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Solo en cambio]</td> 
   <td> <p>Uno de los tipos [!UICONTROL Project Update]. Cuando se selecciona esta opción, las líneas de tiempo [!UICONTROL Project Projected] y [!UICONTROL Planned] se actualizan únicamente cuando se realiza una actualización o cambio en el proyecto o en una tarea del proyecto. No actualiza el proyecto todas las noches.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>El nombre de [!UICONTROL Problema] en la variable [!DNL Workfront] base de datos, se utiliza en los informes de modo de texto o en los datos personalizados calculados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Problema o tarea que no se ha completado, pero en los que se está trabajando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organigrama Chart]</td> 
   <td>Abreviatura del organigrama. Este es un gráfico que muestra la jerarquía de una organización. También se encuentra en la pestaña de la pantalla de detalles [!UICONTROL User] que aparece y permite establecer las relaciones de [!UICONTROL User] y [!UICONTROL Reporting] de [!UICONTROL User].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organization Setup]</td> 
   <td>Define [!UICONTROL Companies], [!UICONTROL Groups] y [!UICONTROL Security Profiles] para su organización.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Otros grupos]</td> 
   <td> <p>En un informe o vista que enumera a los usuarios, este campo muestra todos los grupos a los que pertenece cada usuario. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Anular moneda]</span> </td> 
   <td> 
    <div> 
     <p>En un informe [!UICONTROL Job Role], esta es la moneda asociada a una función de trabajo. Se trata de una anulación de la [!UICONTROL Base Currency] establecida en el área [!UICONTROL Setup] por la variable [!DNL Workfront] administrador. </p> 
     <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Anular Facturación de Moneda/ Hora]</span> </td> 
   <td> 
    <div> 
     <p>En un informe [!UICONTROL Job Role], esta es la tasa de facturación por hora del rol de trabajo utilizando el [!UICONTROL Override Currency] seleccionado en el rol de trabajo.</p> 
     <p> Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Anular costo/hora de moneda]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Job Role], esta es la tasa de coste por hora del rol de trabajo que utiliza el [!UICONTROL Override Currency] seleccionado de la función de trabajo. </p> 
     <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Propietario]</td> 
   <td>Usuario responsable de la finalización del objeto designado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Tipo de propietario]</span> </td> 
   <td> 
    <div> 
     <p>En un informe [!UICONTROL Goal], se muestra el tipo de propietario asignado a un objetivo estratégico. Los siguientes son los tipos de propietarios de objetivos:</p> 
     <ul> 
      <li> <p>[!UICONTROL Usuario]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>No se muestra ningún valor en este campo cuando el propietario del objetivo es su organización. </p> 
     <p>Esto requiere una licencia adicional. Para obtener información sobre [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] información general</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parámetro]</td> 
   <td> <p>Un [!UICONTROL parámetro] es un campo personalizado. Puede crear un informe para todos los parámetros o campos personalizados del sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Principal]</td> 
   <td>En un informe, este campo muestra información sobre el objeto principal. Por ejemplo, en un informe de [!UICONTROL issue] , puede mostrar información sobre la tarea o el proyecto en el que se ha registrado el problema; en un informe de tareas, puede mostrar información sobre la tarea principal directa o sobre el proyecto. Para obtener más información sobre los objetos que pueden tener elementos principales en [!DNL Workfront], consulte la sección "Interdependencia y jerarquía de objetos" en el artículo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos de [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Principal Lag]</td> 
   <td>Cantidad de tiempo que debe transcurrir entre el inicio de [!UICONTROL Parent Task] y el inicio de [!UICONTROL Subtask].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea Principal]</td> 
   <td>También se conoce como [!UICONTROL Summary Task]. Esta es una tarea que tiene Subtareas (también llamadas [!UICONTROL Tareas secundarias]). La [!UICONTROL Duration], [!UICONTROL Work Required] y [!UICONTROL Percent Complete] de la tarea principal se calcula a partir de las subtareas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Recursos a tiempo parcial]</td> 
   <td>Usuario con licencia que tiene menos capacidad que la programación predeterminada definida en el sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Porcentaje completado]</td> 
   <td> <p>Campo de proyecto, tarea o problema que muestra qué porcentaje del trabajo asociado con la tarea, proyecto o problema se completa.</p> <p>Puede actualizar este campo manualmente para problemas y tareas de trabajo. </p> <p>Para los proyectos y las tareas principales, este campo es un resumen de todas las tareas de trabajo y no puede actualizarlo manualmente. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Información general sobre Project [!UICONTROL Percent Complete]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permiso]</td> 
   <td> <p>Derechos que se conceden a un usuario en un objeto, normalmente otorgados para que pueda completar el trabajo en el elemento o ver el elemento. Puede conceder permisos a:</p> 
    <ul> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Tableros]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Forms personalizado]</li> 
     <li>[!UICONTROL Vistas]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre cómo compartir permisos en objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Es un tipo de licencia completo en la variable [!DNL Workfront] sistema. Los usuarios deben tener esto para acceder a todas las funciones de [!DNL Workfront].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] información general sobre licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (en la variable [!DNL Scenario Planner])</td> 
   <td> <p>Un plan es el objeto principal al trabajar con la variable [!DNL Workfront] Planificador de escenario. Puede esbozar la estrategia para el futuro a corto y largo plazo de su empresa, identificar cada resultado de alto nivel y agregarlo como un plan a la [!DNL Workfront] Planificador de escenario. </p> <p>No se puede mostrar [!DNL Scenario Planner] planes de un informe y no puede acceder a ellos a través de la variable [!DNL Workfront] API. </p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La variable [!DNL Scenario Planner] información general</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL planificado]</td> 
   <td> <p>El lapso de tiempo dentro del cual está programado que ocurra algo. Al crear proyectos, tareas o problemas en [!DNL Workfront], se establecen las fechas de inicio y finalización planificadas, así como el periodo planificado durante el cual se producen. Estos valores representan su intención original o estiman cuánto tiempo debe tardar un artículo en completarse. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Beneficio planificado]</td> 
   <td>Se trata de una entrada manual para que el Administrador de proyectos estime si la finalización de un proyecto aportaría algún beneficio económico a la organización. La especificación de este valor puede formar parte de la creación de un [!UICONTROL Business Case] para el proyecto. Debe tener permisos de [!UICONTROL Administrar] en el proyecto para actualizar este valor.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Horario presupuestado planificado]</td> 
   <td> <p>En un informe de [!UICONTROL Hora presupuestada], se muestra la cantidad de horas presupuestadas para Proyectos o [!UICONTROL Funciones de trabajo] en el [!UICONTROL Resource Planner]. </p> <p>Para obtener información sobre la presupuestación de proyectos o funciones en el [!UICONTROL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de presupuesto en [!UICONTROL Resource Planner] utilizando las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>. Para obtener información sobre el informe [!UICONTROL Horario presupuestado], consulte el artículo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Informe: Hora presupuestada</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización prevista]</td> 
   <td> <p>Puede establecer manualmente la [!UICONTROL Fecha de finalización planeada] en una fecha de su elección. Si no define la [!UICONTROL Fecha de finalización prevista], [!DNL Workfront] lo establece automáticamente. Cuando se configura automáticamente, [!UICONTROL Fecha de finalización planeada] es: [!UICONTROL Fecha de inicio planeada] + [!UICONTROL Duración]</p> <p>Para obtener más información, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Fecha de finalización prevista]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establezca el proyecto [!UICONTROL Fecha de finalización planeada]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo planificado]</td> 
   <td> <p>Un total del [!UICONTROL Costo laboral planeado] y el [!UICONTROL Costo de gastos planeado] del proyecto. Esto no incluye el [!UICONTROL Costo de riesgo planeado] en el proyecto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duración planificada]</td> 
   <td> <p>La [!UICONTROL Duración planificada] de una tarea suele ser la misma que la [!UICONTROL Duración] de la tarea. Representa la diferencia en días entre el [!UICONTROL Inicio planeado] y las [!UICONTROL Fechas de finalización planeadas] de la tarea. </p> <p>Cuando la tarea tiene un tipo de [!UICONTROL Duration] de [!UICONTROL Effort Driven], la [!UICONTROL Duración planificada] puede diferir de la [!UICONTROL Duración] de la tarea, en función de cuántos recursos asigne a la tarea. </p> <p>Por ejemplo, si una tarea con un tipo de [!UICONTROL Duration] de [!UICONTROL Effort Driven] tiene una [!UICONTROL Duration] de 3 días y asigna un recurso con una programación de tiempo completo a la tarea, el valor de [!UICONTROL Planned Duration] también es de 3 días. Si asigna tres recursos con una programación de tiempo completo a la misma tarea, la [!UICONTROL Duración] se mantiene en 3 días, pero la [!UICONTROL Duración planificada] se convierte en 1 día. La [!UICONTROL Duración planificada] también cambia las fechas [!UICONTROL Inicio planificado] y [!UICONTROL Finned Completion] de la tarea, para reflejar la nueva [!UICONTROL Duración planificada]. Como resultado, la cronología del proyecto también se ve afectada. </p> <p>Para obtener más información sobre la diferencia entre [!UICONTROL Duration] y [!UICONTROL Planned Duration] para las tareas, consulte el artículo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Diferencia entre [!UICONTROL Duración planificada] y [!UICONTROL Duración] para tareas</a>.</p> <p>Los proyectos y problemas no tienen una [!UICONTROL Duración planificada]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duración planeada minutos]</td> 
   <td> <p>Los [!UICONTROL Minutos de duración planeada] de un proyecto o problema es la [!UICONTROL Duración] del proyecto o problema en minutos. </p> <p>Las tareas no tienen un campo [!UICONTROL Duración planeada minutos]. </p> <p>[!UICONTROL Template Tasks] tienen un campo [!UICONTROL Planned Duration Minutes] que muestra la [!UICONTROL Planned Duration] de la tarea en minutos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de gastos planeado]</td> 
   <td> <p>La suma de las [!UICONTROL Cantidades Planificadas] para todos los gastos registrados para un proyecto o una tarea.</p> <p><b>EJEMPLO</b></p>
   <p>Si crea un gasto para la Tarea 1 e introduce 600,00 $ en el campo [!UICONTROL Importe Planificado], el [!UICONTROL Costo Planificado] para esta tarea es de 600 $. </p> 
   <p>Para un proyecto, [!DNL Workfront] utiliza la fórmula siguiente para calcular [!UICONTROL Costo de gastos planeado]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horario planificado]</td> 
   <td> <p>Este campo aparece en las áreas de [!UICONTROL projects], [!UICONTROL tasks] y problemas, informes para proyectos, tareas o problemas, y herramientas de administración de recursos como [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] y el informe [!UICONTROL Utilization]. </p> <p>Muestra la cantidad de horas que el propietario del proyecto calcula que cada tarea o problema debe tardar en completarse. Para los proyectos, generalmente es un resumen de las [!UICONTROL Horario planificado] de las tareas del proyecto. </p> <p>El campo [!UICONTROL Horario planificado] puede mostrar información diferente en función de su ubicación. Para obtener información sobre las horas planificadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Información general sobre las horas planificadas</a>.</p> <p>Las horas planificadas se almacenan en minutos en la variable [!DNL Workfront] base de datos. Al escribir cálculos con este campo, asegúrese de tener en cuenta el hecho de que las horas se muestran como minutos.<br></p> <p>De forma predeterminada, las horas planificadas se distribuyen de forma equitativa a todos los días dentro de la duración de un elemento de trabajo y también a todos los recursos asignados a la tarea. Los usuarios pueden actualizar la cantidad diaria de horas planificadas para un elemento de trabajo o las horas planificadas individuales para cada usuario asignado.</p> <p>La actualización de este campo difiere en los proyectos, tareas y problemas: </p> 
    <ul> 
     <li> <p>Para problemas, puede actualizar este campo manualmente. Las horas planificadas del problema no se agregan a las horas planificadas del proyecto. </p> <p>Sugerencia: En un informe de problema, uno de los campos [!UICONTROL Planned Hours] se sustituye por el campo [!UICONTROL Work]. El campo muestra el número de horas planificadas sobre el problema. Para obtener más información, consulte los campos "trabajo" o "[!UICONTROL Trabajo]" en esta tabla. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para las tareas, puede actualizar manualmente este campo cuando el [!UICONTROL Duration Type] de la tarea sea [!UICONTROL Calculated Assignment] o [!UICONTROL Simple]. Este campo se calcula mediante [!DNL Workfront] cuando el [!UICONTROL Duration Type] de la tarea es [!UICONTROL Calculated Work] o [!UICONTROL Effort Driven].<br>Para obtener información sobre la [!UICONTROL Task Duration], consulte el artículo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Duration] y [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para proyectos, [!DNL Workfront] calcula las horas planificadas agregando todas las horas planificadas de todas las tareas del proyecto. </p> </li> 
    </ul> <p><b>SUGERENCIA</b></p> <p>También puede mostrar los informes [!UICONTROL Horario planificado] en [!UICONTROL proyecto], [!UICONTROL tarea] o [!UICONTROL problemas] utilizando el modo de texto y haciendo referencia a campos adicionales. Para obtener más información, consulte "<code>work</code>", "[!UICONTROL Work]" y "<code>workRequiredExpression</code>" en esta tabla. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo laboral planificado]</td> 
   <td> 
    <p>Para una tarea, la tasa por hora del usuario o función se multiplica por el número de horas asignadas al usuario o a la función.</p> <p>Para un proyecto, es un total de todas las tareas [!UICONTROL planificado costes laborales].</p> <p>El uso de la tasa del usuario o de la función depende del tipo de coste seleccionado para la tarea determinada. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ingresos planificados]</td> 
   <td> <p>Las tareas y los proyectos pueden mostrar un valor para [!UICONTROL Ingresos planificados] en [!DNL Workfront]. [!UICONTROL Ingresos planificados] representa la cantidad de dinero asociada con las [!UICONTROL Horario planificado] de las tareas del proyecto. Para los proyectos, también puede incluir los [!UICONTROL ingresos fijos] del proyecto. </p> <p>Para las tareas, estos son los ingresos asociados con las [!UICONTROL Horario planificado] de las tareas. Las horas planificadas de todas las tareas se resumen en las horas planificadas del proyecto para contribuir al cálculo del proyecto [!UICONTROL Horario planificado]. </p> 
   <p>[!DNL Workfront] calcula los [!UICONTROL ingresos planificados] para tareas y proyectos mediante las siguientes fórmulas:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>El proyecto [!UICONTROL Ingresos planificados] que se muestra en el área [!UICONTROL Detalles del proyecto] y en los informes de proyecto difiere de los ingresos planificados que se muestran en el informe [!UICONTROL Utilización]. </p> <p>Los [!UICONTROL Ingresos planificados] del área [!UICONTROL Detalles del proyecto] reflejan los ingresos de la tarea, así como los ingresos fijos del proyecto. El [!UICONTROL Planned Revenue] de [!UICONTROL Utilization Report] muestra [!UICONTROL Planned Revenue] asociados únicamente a las tareas del proyecto. </p> 
     <p><b>EJEMPLO</b></p>  
      <p>Si el proyecto tiene una tarea con 10 horas, asignada a un consultor con una tasa de 20 dólares por hora y el proyecto tiene una tasa de [!UICONTROL ingresos fijos] de 100 dólares, el informe [!UICONTROL Utilización] muestra 200 dólares para [!UICONTROL Ingresos planificados] (los [!UICONTROL Ingresos planificados] asociados con las horas de la tarea). La sección [!UICONTROL Detalles del proyecto] muestra 300 $ (los [!UICONTROL Ingresos planificados] de la tarea y los ingresos fijos del proyecto). </p> 
    <p>Para obtener información sobre el seguimiento de ingresos en [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Información general sobre facturación e ingresos</a>. </p> 
    <p>Para obtener información sobre los cálculos [!UICONTROL Planned Revenue] en el [!UICONTROL Utilization report], consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ver información de utilización de recursos </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de riesgo planeado]</td> 
   <td> <p>El total del [!UICONTROL Coste potencial] de todos los riesgos en la factorización del proyecto en su Probabilidad de ocurrir. Esta cantidad no se incluye en el [!UICONTROL Costo planeado] del proyecto.</p> <p>El [!UICONTROL Costo de riesgo planeado] de un proyecto se calcula mediante la fórmula siguiente:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Colección de fichas y secciones del portal definida por el administrador que aparece en la página [!DNL Workfront] Aplicación [!UICONTROL Home] y otros tableros.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Un componente de una ficha en un tablero o una página del portal. Normalmente es un solo informe, gráfico, calendario o lista de información clave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Ficha de un portal o panel que contiene hasta tres secciones del portal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Una colección de proyectos que tienen características unificadoras. Estos proyectos suelen competir por los mismos recursos, presupuesto o periodo de tiempo. Puede dividir los Portfolio en Programas y asociar los proyectos con los Programas antes de añadirlos a un Portfolio.</p> <p>Para obtener más información sobre portafolios, consulte <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">información general del Portfolio en [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Administración de Portfolio]</td> 
   <td>Una esfera de actividad centrada en la gestión de una colección o programas conexos y actividades de proyectos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>A [!DNL Workfront] herramienta para ayudar a evaluar y priorizar los proyectos dentro de una cartera.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Propietario]</td> 
   <td>El responsable de la priorización y el presupuesto de una cartera.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo de riesgo potencial]</td> 
   <td>Se trata de un campo de proyecto que puede encontrar en listas e informes. Muestra el coste potencial de los riesgos asociados con el proyecto, si se producen. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Coste de Riesgo Potencial </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecesor]</td> 
   <td> <p>Tarea que debe completarse antes de que finalice una tarea dependiente. También una tarea que está marcada como una [!UICONTROL Dependency] para otra tarea. Los predecesores permiten al planificador establecer la lógica de dependencia de secuencia, como iniciar una tarea después de que otra tarea finalice.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Descripción general de las predecesoras de tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empresa principal]</td> 
   <td>Empresa a la que pertenece el usuario como se indica en la configuración de usuario. Las empresas también pueden asociarse con Proyectos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contacto Principal]</td> 
   <td><p>El [!UICONTROL Primary Contact] es el creador de un problema y es designado automáticamente por [!DNL Workfront] cuando alguien crea el problema. Puede actualizar manualmente este campo si ha [!DNL Manage] permisos para el problema. Un problema solo puede tener un contacto principal.</p> 
   <p>Si cambia el contacto principal, el usuario designado originalmente como contacto principal seguirá teniendo acceso a [!UICONTROL Administrar] para solucionar el problema.</p>
   <p>Al convertir un problema en una tarea o un proyecto, el usuario designado como [!UICONTROL Primary Contact] de se convierte en el [!UICONTROL Converted Issue Originator] del proyecto o la tarea. Si el [!UICONTROL Primary Contact] del problema se actualiza después de convertir el problema, el [!UICONTROL Converted Issue Originator] se conserva como el [!UICONTROL Primary Contact] del problema en el momento en que se produjo la conversión. Consulte también "[!UICONTROL Creador de problemas convertidos]" en este artículo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Un valor que se puede asignar a una tarea, un problema o un proyecto para designar su importancia. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privado]</td> 
   <td>En una [!UICONTROL Note] o [!UICONTROL Document], esta opción oculta ese objeto a la mayoría de los visualizadores. Para una cola de asistencia técnica privada, solo los usuarios del equipo de cola pueden enviar problemas a esa cola a través del área de [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil]</td> 
   <td>Toda la información sobre una cuenta de usuario.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Un subconjunto dentro de un portafolio, donde proyectos similares pueden agruparse para lograr un beneficio bien definido.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Gestión de dependencias, riesgos, problemas, requisitos y soluciones entre proyectos para mantener el programa en buen estado y lograr los beneficios definidos del programa.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Propietario del programa]</td> 
   <td>El responsable de supervisar y organizar las actividades para garantizar que los objetivos del proyecto se ajusten a los objetivos de la empresa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progreso]</span> </td> 
   <td> <p>En un informe [!UICONTROL Goal], esto muestra el porcentaje de lo cerca que está un objetivo estratégico de completar. El porcentaje de progreso se muestra como un número. Para obtener información sobre los objetivos estratégicos, consulte también "[!UICONTROL Goal]" en esta tabla.</p> <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront] Objetivos. Para obtener información sobre la administración de objetivos estratégicos, use [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Agregar proyectos a objetivos en [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado de progreso]</td> 
   <td> <p>En los informes Proyecto, Tarea y Objetivo, este campo muestra el estado de progreso de los proyectos, tareas u objetivos estratégicos. Para obtener más información, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Resumen del estado del progreso del proyecto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Información general sobre el estado de progreso de la tarea</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Resumen del progreso y la condición del objetivo en [!DNL Adobe Workfront Goals]</a> </p>
     <p>El informe [!UICONTROL Goal] y el [!UICONTROL Progress Status] para [!DNL goals] solo están visibles si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre los objetivos estratégicos en [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] información general</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Una gran cantidad de trabajo que debe completarse dentro de un marco temporal específico y debe utilizar un presupuesto específico y un número de recursos. Para que sea manejable, puede dividir el proyecto en una serie de tareas. La finalización de todas las tareas da como resultado la finalización del proyecto. Para obtener información sobre cómo planificar un proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Información general sobre el plan de un proyecto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignación de proyectos: horas planificadas]</td> 
   <td> <p>En un informe [!UICONTROL Initiative Job Role] , se muestra el número de [!UICONTROL Planned Hours] asociado a una función de trabajo asignada a tareas o problemas en el proyecto. Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no se muestran en la [!DNL Workfront] instancia a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La variable [!DNL Workfront Scenario Planner] información general</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detalles del proyecto]</td> 
   <td>Detalles del estado actual de un proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo presupuestado del proyecto]</td> 
   <td> <p> Este es el [!UICONTROL Costo presupuestado] de un proyecto, tal como se muestra en listas e informes.</p><p>Consulte también "[!UICONTROL Costo presupuestado]" en este artículo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestión de proyectos]</td> 
   <td>Conjunto de políticas que rigen los umbrales para la creación, categorización y asignación de nombres de proyectos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>En un informe de [!UICONTROL Hour], este campo está reservado para información financiera vinculada a las horas registradas con el tipo de hora de [!UICONTROL Project Time]. Los proyectos pueden tener sus propias tasas de facturación y si una hora se registra directamente en un proyecto, esas tasas se utilizarán en los cálculos. En función de la configuración del proyecto, los proyectos también pueden tener distintas monedas y puede haber una conversión de moneda para esas horas. El objeto [!UICONTROL Project Overhead] permite [!DNL Workfront] para obtener esa información.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propietario del proyecto]</td> 
   <td>Usuario responsable de administrar el ámbito, la cronología y las asignaciones de un proyecto. Aprobador predeterminado de pedidos de cambio, cambios financieros y entregables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Procesos para elaborar y mantener el calendario del proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Patrocinador de proyectos]</td> 
   <td>Un perfil de partes interesadas designado al que se debe vincular cada uno de los usuarios. En [!DNL Workfront], se designan como [!UICONTROL Niveles de acceso]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipos de proyectos]</td> 
   <td> <p>Recopilación de usuarios o funciones asignados a un proyecto</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Información general del equipo del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seguimiento de proyectos]</td> 
   <td>Los datos utilizados para medir la salud y el alcance de un proyecto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proyectado]</td> 
   <td> <p>Una estimación de la marca de tiempo de cuándo se completará el trabajo en función de las horas planificadas y el porcentaje completado de una tarea, un problema o un proyecto.</p> <p>Esto hace referencia a fechas o a la [!UICONTROL Duración] de tareas, problemas o proyectos. Por lo general, designa fechas y duraciones que son más fieles a la vida de los elementos de trabajo, después de que algún trabajo ya se haya completado o haya pasado algún tiempo. </p> <p>Por ejemplo, la [!UICONTROL Fecha de finalización prevista] de una tarea es la fecha en la que [!DNL Workfront] calcula que la tarea se completará, en función de cuánto trabajo se haya realizado hasta el momento, cuántas personas se le han asignado y cuánto tiempo ha transcurrido desde la fecha de inicio.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plazo de la prueba]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como los informes [!UICONTROL Document Version] y [!UICONTROL Proof Approval]), este campo muestra el día de la semana, la fecha, la hora del día y el año de la fecha límite de prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof decisions]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el estado de decisión de la prueba (pendiente, cambios necesarios o aprobados)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de prueba]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el nombre de la prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Páginas de prueba]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el número de páginas incluidas en la prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progreso de la prueba]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), muestra el estado de progreso de la prueba ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL decisions Made]).</p> <p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Resumen del progreso de la prueba</a> en <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Resumen del progreso y estado de la prueba</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Proceso de revisión en el que uno o más usuarios marcan y comentan el contenido que debe cambiarse en una imagen, un documento de texto, un vídeo o contenido web interactivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>En una [!UICONTROL Note] o [!UICONTROL Document], esta opción hace que el objeto sea accesible para otros usuarios o incluso para personas de fuera [!DNL Workfront]. Para una [!UICONTROL Help Desk Queue], [!UICONTROL Public] significa que todos los usuarios que pueden enviar Problemas pueden enviar Problemas a través del área de [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Calidad]</td> 
   <td>La percepción de la calidad del trabajo dentro de la organización.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cola]</td> 
   <td>También se denomina [!UICONTROL Cola de asistencia técnica]. Se trata de un proyecto que se ha publicado en el área de [!UICONTROL Help Desk] para permitir a los usuarios enviarles problemas. Normalmente, las colas se crean para temas concretos, como errores, solicitudes de proyectos, etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propiedades de cola]</td> 
   <td>Estos ajustes definen las reglas de envío de problemas para un proyecto que se está publicando en el [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tema de cola]</td> 
   <td> <p>Propiedad de una [!UICONTROL Help Desk Queue] que permite a los usuarios que envían un problema seleccionar un tema. Los temas pueden:</p> 
    <ul> 
     <li>Estar asociado a un formulario de datos personalizado.</li> 
     <li>Asigne el problema automáticamente a un usuario, función o equipo a través del conjunto de reglas de enrutamiento en el tema seleccionado.</li> 
     <li>Mueva el problema a otro proyecto o cola a través del conjunto de reglas de enrutamiento del tema seleccionado.</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crear temas de cola</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>En un informe [!UICONTROL Access Level], puede indicar manualmente una [!UICONTROL Rank] del [!UICONTROL Access Level]. Esto le ayuda a, como [!DNL Workfront] para identificar visualmente el nivel de complejidad asociado a cada nivel de acceso. Por ejemplo, puede dar números inferiores para niveles de acceso más complejos ([!UICONTROL Plan]) y números superiores para niveles de acceso menos complejos ([!UICONTROL Requester]). No puede clasificar los niveles de acceso estándar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Este campo de un informe de tareas indica si una tarea de [!UICONTROL Agile] se ha marcado como [!UICONTROL Ready] en el registro pendiente. Este indicador solo se aplica a las tareas [!UICONTROL Agile], que son tareas asignadas a un equipo [!UICONTROL Agile]. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frecuencia de periodicidad]</td> 
   <td> <p>Campo que se muestra en el cuadro [!UICONTROL Task Details] o [!UICONTROL Edit Task] de un elemento principal de las tareas recurrentes. Es la frecuencia con la que se producen las tareas en la recurrencia. Para obtener información sobre la creación de tareas recurrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de referencia]</td> 
   <td> <p>Los proyectos, las tareas y los problemas se asocian automáticamente a un número de referencia único a medida que se crean. Puede ver el [!UICONTROL Reference Number] en la página [!UICONTROL Details] de proyectos, tareas o problemas, o en una lista o informe. </p> <p><b>SUGERENCIA</b><p><br>Puede diferir a los números de referencia cuando dos elementos tienen el mismo nombre, ya que los números de referencia siempre son únicos. </p> <p>[!DNL Workfront] genera automáticamente un número de referencia secuencial a nivel del sistema. Cada proyecto, tarea o problema obtiene el siguiente número disponible en la secuencia. <br></p> <p>Por ejemplo, si el usuario A crea una tarea, [!DNL Workfront] puede asignar automáticamente la tarea al número de referencia de 100. Si el usuario B crea un problema justo después de esto, [!DNL Workfront] asigna al problema el número de referencia de 101. Los números de referencia no se pueden editar manualmente. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema de rechazo]</td> 
   <td>En un informe de proyecto o tarea, este es el problema que se crea cuando se rechaza la aprobación del proyecto o la tarea. Para obtener información sobre los problemas de rechazo, consulte el artículo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creación de un proceso de aprobación para elementos de trabajo</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de riesgo restante]</td> 
   <td> <p>Campo de proyecto que muestra la diferencia entre el [!UICONTROL Costo de riesgo planeado] de un proyecto y el total de todos los [!UICONTROL Costes reales] de todos los riesgos del proyecto. </p> <p>El [!UICONTROL Costo de riesgo restante] de un proyecto se calcula mediante la fórmula siguiente:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Replanificación]</td> 
   <td>Cambiar las fechas de un proyecto para reparar o superar problemas. Por ejemplo, un proyecto que ha estado suspendido durante varios meses tendría que ser replanificado para reflejar fechas precisas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Un gráfico o tabla que contiene información sobre un [!DNL Workfront] y sus atributos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Tipo de problema que se prueba en una sola cola centralizada y no está relacionado con un esfuerzo de trabajo continuo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Cola de solicitud]</td> 
   <td>El atraso de problemas que se administra mediante un proceso de tráfico y prueba.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>Tiempo total del ciclo de trabajo para la ingesta y completar una solicitud.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Normalmente es un tipo de licencia. Un usuario con una licencia de Solicitante puede enviar solicitudes para que se produzca un nuevo trabajo en el sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo reservado]</td> 
   <td>Días especificados en la hora personal de un usuario, lo que indica que el usuario no estará disponible para trabajar. Consulte "[!UICONTROL Días no laborables]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver problema]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia al problema que resuelve el problema. </p> <p>Para obtener información sobre cómo mostrar la resolución de objetos en los informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información sobre objetos resueltos y resueltos en un informe</a> en <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver proyecto]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia al proyecto que resuelve el problema. </p> <p>Para obtener información sobre cómo mostrar la resolución de objetos en los informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información sobre objetos resueltos y resueltos en un informe</a> en <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver tarea]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia a la tarea que resuelve el problema. </p> <p>Para obtener información sobre cómo mostrar la resolución de objetos en los informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información sobre objetos resueltos y resueltos en un informe</a> en <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso]</td> 
   <td>Usuario(s) y/o Función(s) existentes en el sistema y asignados a equipos y tareas del proyecto.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Gestión de recursos]</td> 
   <td> <p>[!UICONTROL Resource Management] es un conjunto de herramientas empresariales que le permite prever con precisión el uso de sus recursos en función de su disponibilidad, de modo que el trabajo que debe realizarse se complete a tiempo y con presupuesto. </p> <p>Con las herramientas de Gestión de Recursos puede planificar la capacidad a largo plazo y las necesidades de programación a corto plazo de sus recursos. </p> <p>Para obtener información sobre la administración de recursos en [!DNL Workfront], consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introducción a la administración de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager ID]</td> 
   <td><p>En un informe de proyecto, puede utilizar esta opción al crear un filtro para encontrar un gestor de recursos específico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gestores de recursos]</td> 
   <td> <p>En un informe de proyecto o una vista de lista, se trata de un campo informativo que muestra los usuarios designados para realizar actividades de administración de recursos en el proyecto.  Cuando se utiliza "[!UICONTROL Resource Managers]" en un informe, se muestra una lista de gestores de recursos con cada gestor de recursos en el proyecto separado por una coma. Puede designar hasta 30 administradores de recursos en un proyecto determinado.</p> <p>Para obtener más información, consulte el artículo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designar gestores de recursos para un proyecto o plantilla </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Horas Presupuestadas] </td> 
   <td>Las horas presupuestadas para el proyecto y los recursos asociados a él en el [!UICONTROL Resource Planner]. Consulte también "[!UICONTROL Horario presupuestado]" en este artículo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Un [!DNL Workfront] herramienta que permite ver y administrar los recursos entre proyectos, funciones de trabajo o usuarios. Para obtener más información, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Información general del planificador de recursos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Costo presupuestado del trabajo]</td> 
   <td> <p>Estos son los costos asociados con las horas presupuestadas para las funciones de trabajo del proyecto usando el Planificador de recursos. </p> <p>Consulte también "Coste laboral presupuestado" en este artículo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Grupos de recursos]</td> 
   <td> <p>Los grupos de recursos son colecciones de usuarios que se pueden asociar a un proyecto. Los usuarios del mismo grupo de recursos suelen pertenecer al mismo departamento, tienen habilidades similares o complementarias, o están financiados por el mismo presupuesto. Puede asociar varios grupos de recursos a un proyecto o a un usuario. Un grupo de recursos se puede asignar exclusivamente a un proyecto o compartir con varios proyectos.</p> 
   <p>Para obtener más información sobre los grupos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resumen de los grupos de recursos </a>.</p> 
   <p>En los informes de proyecto, los grupos de recursos muestran todos los grupos asociados a un proyecto. Este objeto no se puede utilizar en una agrupación.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Informe que muestra la cantidad de horas disponibles durante un período de tiempo determinado y la cantidad de horas programadas para cada usuario en el informe. Esto también se calcula en [!UICONTROL Average Hours per Day] y un porcentaje de asignación.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Resultado]</td> 
   <td>En [!DNL Workfront Goals], un resultado es un indicador de progreso para un objetivo. Puede ser un número, un valor de porcentaje o una cantidad de moneda que actualice manualmente. No se pueden mostrar resultados en un informe y no se puede acceder a ellos a través de la variable [!DNL Workfront] API. Para obtener información sobre las actividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introducción a resultados y actividades en objetivos de Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ingresos]</td> 
   <td>Cantidad facturable para la tarea o proyecto. La cantidad puede ser por hora, fija o una combinación de ambas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de ingresos]</td> 
   <td>El tipo de ingresos determina cómo acumulará ingresos la tarea. Algunos ejemplos son [!UICONTROL Fijo por hora], [!UICONTROL Rol por hora] y [!UICONTROL Rol por hora con límite]. Para obtener información sobre el seguimiento de ingresos en [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Normalmente es un tipo de licencia. Un usuario con una licencia de [!UICONTROL Reviewer] tiene la capacidad de revisar y aprobar elementos de trabajo en el sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Riesgo]</td> 
   <td> <p>Esto puede hacer referencia a los siguientes conceptos en [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Campo de un proyecto que indica el riesgo que puede suponer un proyecto. Puede priorizar la ejecución de sus proyectos en función del nivel de riesgo. Los proyectos pueden tener los siguientes niveles de riesgo:</p> <p>- [!UICONTROL Muy bajo]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medio]</p> <p>- [!UICONTROL Alto]</p> <p>- [!UICONTROL Muy alto]</p> <p>Los niveles de riesgos que se indican para un proyecto no se pueden personalizar. </p> <p> Para obtener información sobre la actualización del riesgo de un proyecto, consulte la sección "Configuración del proyecto" del artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>. Puede mostrar el campo de riesgo de un proyecto en los informes. </p> </li> 
     <li> <p>Evento que podría ocurrir durante la vida de un proyecto y que identifica un impacto potencial en el costo, el alcance o la programación del proyecto. Puede definir posibles riesgos para un proyecto y asociar una probabilidad de que se produzcan o un coste a medida que crea el caso empresarial del proyecto. Para obtener información sobre cómo añadir riesgos al caso empresarial del proyecto, consulte "Creación y edición de riesgos en proyectos". </p> <p>No se pueden mostrar los riesgos definidos en el [!UICONTROL Business Case] de los informes. Solo se pueden mostrar varios tipos de Costes de riesgo en informes y listas. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo de riesgo]</td> 
   <td> <p>El coste asociado a los riesgos de un proyecto. A continuación se indican los costes de riesgo asociados a los proyectos que se pueden mostrar en los informes:</p> 
    <ul> 
     <li> <p>[!UICONTROL Costo real]: campo de un riesgo que muestra el coste real del riesgo que se ha producido. Además de los informes y listas, puede localizarlos en el cuadro [!UICONTROL Editar riesgo] al editar o crear un riesgo. </p> <p>Para los costes de proyecto, tarea o problema, consulte "[!UICONTROL Coste real]" en este artículo. </p> </li> 
     <li> <p>[!UICONTROL Costo de riesgo planeado]: campo del proyecto que muestra un total de todos los [!UICONTROL Costes de riesgo potenciales] del proyecto. Consulte también "[!UICONTROL Costo de riesgo planeado]" en este artículo. </p> <p>Para obtener información sobre el coste de riesgo potencial, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Coste de Riesgo Potencial </a>. </p> </li> 
     <li> <p>[!UICONTROL Costo de riesgo restante]: campo del proyecto que muestra la diferencia entre el total de los [!UICONTROL Costes reales] de todos los riesgos y el [!UICONTROL Costo de riesgo planeado]. Consulte también "Costo de riesgo restante" en este artículo. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestión de Riesgos]</td> 
   <td>Procesos para identificar, mitigar y monitorear riesgos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rol]</td> 
   <td>Consulte "[!UICONTROL Job Role]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enrutamiento]</td> 
   <td>Asignar o mover automáticamente un problema, normalmente debido a un tema de cola o por ser la ruta predeterminada (regla de enrutamiento) para la cola.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Regla de enrutamiento]</td> 
   <td>Configuración de Proyectos y colas que asigna automáticamente un problema a un usuario, función o equipo, o que movió el problema a otro proyecto o cola. Las reglas de enrutamiento generalmente se utilizan con las colas de asistencia técnica para asignar automáticamente los problemas entrantes.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Búsqueda guardada]</td> 
   <td>Búsqueda en la que se han guardado los criterios de búsqueda. Las búsquedas guardadas facilitan la ejecución de la misma cada una de nuevo sin tener que volver a introducir los criterios de búsqueda.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scene] (en [!DNL Workfront Fusion]) </td> 
   <td> <p>Un escenario consta de una serie de pasos (módulos) que indican cómo se deben transferir y transformar los datos entre aplicaciones y servicios.</p> <p>Para obtener información sobre escenarios en [!DNL Workfront Fusion], consulte <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] información general del escenario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (en la variable [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>En el [!DNL Scenario Planner], un escenario es una copia de un plan. </p> <p>La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">La variable [!DNL Scenario Planner] información general</a>. </p> <p>Para obtener información sobre la creación de escenarios, consulte <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Cree y compare escenarios de plan en la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Programación]</td> 
   <td>El horario de trabajo semanal, incluidos los horarios de trabajo, combinado con días libres (como días festivos) y días de excepción (como un sábado de trabajo). Los programas se pueden aplicar a Proyectos y usuarios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Programar exención]</td> 
   <td>También se conoce como [!UICONTROL Modificfied Shift]. Días programados a diferencia de los tiempos de trabajo semanales normales, tal como se define en la programación. Por ejemplo, un sábado programado para funcionar, cuando el programa está configurado para trabajar solo de lunes a viernes, sería una [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Informe programado]</td> 
   <td> <p>Cuando crea un informe de informes, puede mostrar información sobre las programaciones del informe, si está programado que se envíe utilizando el campo [!UICONTROL Informe programado]. Este campo muestra varios valores, uno para cada programación de cada informe, en una lista con viñetas. Para obtener más información sobre la programación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Resumen del envío de informes</a>.</p> <p>Dado que este campo muestra varios valores, no se puede utilizar en una agrupación. Solo se puede acceder a él desde un filtro o una vista. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambio de ámbito]</td> 
   <td>Una [!UICONTROL Audit Track] que, si está activa, genera una nota cada vez que se realiza un cambio en el ámbito de un proyecto o tarea, como si se cambia una [!UICONTROL Task Duration] o [!UICONTROL Predecesors].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sección]</td> 
   <td>Un área de la pantalla, con su propio encabezado, creada para organizar los datos personalizados con fines de visualización.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salto de sección]</td> 
   <td>Un espacio o borde entre secciones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>La configuración que permite a un usuario interactuar con determinados objetos del sistema y no con otros. Consulte también "[!UICONTROL Niveles de acceso]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Área donde los administradores pueden configurar las configuraciones y preferencias del sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gravedad]</td> 
   <td> <p>[!UICONTROL Gravedad] es una indicación de la probabilidad de que un elemento afecte a la finalización del trabajo. Por ejemplo, un Problema con una gran gravedad de [!UICONTROL] puede bloquear completamente la finalización de una tarea, pero un Problema con una baja gravedad de [!UICONTROL] puede ser meramente cosmético.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Actualizar gravedad del problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Graverities]</td> 
   <td>Consulte "[!UICONTROL Gravedad]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compartir]</td> 
   <td>La acción de permitir que otros usuarios vean o editen un elemento específico en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha Slack]</td> 
   <td>En una vista de tarea o informe, el [!UICONTROL Fecha Slack] muestra la fecha exacta en la que una tarea podría afectar definitivamente a la [!UICONTROL Fecha de finalización] del proyecto. Para obtener información sobre la [!UICONTROL Fecha Slack] de una tarea, consulte <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Información general sobre la fecha del Slack de tareas</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignaciones inteligentes]</td> 
   <td> <p>Al asignar tareas o problemas a los usuarios, [!DNL Workfront] hace recomendaciones ([!UICONTROL Smart Asscriptions]) sobre quiénes son los mejores usuarios para completar el trabajo, en función del tiempo que tengan disponible para completarlo y de su relación con el proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Información general sobre asignaciones inteligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indica el objeto principal de otro objeto. Por ejemplo, un documento adjunto a una tarea tiene el nombre de la tarea en el campo [!UICONTROL Source] de un informe o vista [!UICONTROL Document]; un problema registrado en un proyecto tiene el nombre del proyecto en el campo [!UICONTROL Source] de un informe o vista de problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de inicio]</td> 
   <td> <p>Fecha en la que se define el inicio del trabajo en un elemento. Hay varias fechas de inicio en [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL planificado]</li> 
     <li>[!UICONTROL Real]</li> 
     <li>[!UICONTROL Proyectado] </li> 
    </ul> <p>En un [!UICONTROL Rate report], es la fecha en la que se inicia una nueva tasa de facturación para una función de trabajo a nivel de proyecto. Las horas asociadas al proyecto que siguen a esta fecha se multiplican por esta tasa de facturación para calcular los ingresos del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Un indicador utilizado para indicar la posición de un flujo de trabajo de un elemento de trabajo o de un objetivo estratégico.</p> <p>Para los proyectos, el [!UICONTROL Status] es una configuración del proyecto que indica si el proyecto es:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL En Espera] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL muerto]</li> 
    </ul> <p>Para obtener más información sobre el estado del proyecto, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Acceso a la lista de estados de proyectos del sistema</a>.</p>
    <p>Para las tareas, el [!UICONTROL Status] es una configuración de la tarea que indica si la tarea es:</p> 
    <ul> 
     <li>[!UICONTROL Nuevo]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Para obtener más información sobre el estado de la tarea, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Acceso a la lista de estados de tareas del sistema</a></p> <p>Para Problemas, el [!UICONTROL Status] es una configuración en el Problema que indica si este Problema es:</p> 
    <ul> 
     <li>[!UICONTROL Nuevo]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Espera comentarios]</li> 
     <li>[!UICONTROL En Espera]</li> 
     <li>[!UICONTROL resuelto]</li> 
     <li>[!UICONTROL no resolverá]</li> 
     <li>[!UICONTROL No Se Puede Duplicar]</li> 
     <li>[!UICONTROL Verificado Complete]</li> 
     <li>[!UICONTROL reabierto]</li> 
    </ul> <p>Para obtener más información sobre los estados de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceda a la lista de estados de problemas del sistema</a>.</p> 
    <p>Para objetivos estratégicos, el [!UICONTROL Status] es una configuración en el objetivo que indica si el objetivo es:</p> 
     <ul> 
      <li>[!UICONTROL Activo]</li> 
      <li>[!UICONTROL Borrador]</li> 
      <li>[!UICONTROL Inactivo]</li> 
      <li>[!UICONTROL Cerrado]</li> 
     </ul> 
     <p>Para obtener más información sobre los objetivos estratégicos, consulte también "[!UICONTROL Goal]" o "[!UICONTROL Goal]" en este artículo. </p> 
     <p>Para objetivos estratégicos, este campo solo es visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos, use [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] información general</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambio de estado]</td> 
   <td>Una pista de auditoría [!UICONTROL]. Se genera una nota cuando un usuario cambia el estado del proyecto, la tarea o el problema.</td> 
  </tr> 
  <tr> 
   <td>Iconos de estado</td> 
   <td> <p>Puede añadir el campo integrado [!UICONTROL Status Icons] como columna en las vistas para mejorar la visibilidad de los puntos clave sobre los objetos, como:</p> 
    <ul> 
     <li>Un objeto tiene documentos adjuntos</li> 
     <li>Un objeto está asociado a un proceso de aprobación</li> 
     <li>Un objeto tiene notas adicionales asociadas</li> 
     <li>Un gasto facturable o reembolsable </li> 
     <li>Una tarea está en una ruta crítica</li> 
     <li>Un usuario pertenece a una empresa, a un equipo o está ubicado en un huso horario diferente </li> 
    </ul> <p>Puede añadir el campo [!UICONTROL Status Icons] en las vistas de los siguientes objetos: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tareas de plantilla]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Usuarios]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en las vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>Este campo muestra la última actualización de estado proporcionada por los usuarios en el campo '[!UICONTROL Update Status]'. Los comentarios realizados sobre las actualizaciones de estado no se muestran en la columna [!UICONTROL Status Update] .</p> <p>Para mostrar los estados '[!UICONTROL New]', '[!UICONTROL In Process]' y '[!UICONTROL Complete]', utilice la columna [!UICONTROL Status].</p> <p>Los comentarios realizados sobre las actualizaciones de estado no se muestran en la columna [!UICONTROL Status Update] .</p> <p>Para obtener más información sobre los estados, consulte el artículo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Actualizar estado de tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estados]</td> 
   <td>Consulte "[!UICONTROL Status]" en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Un gráfico que representa el estado de los artículos (tareas en la metodología ágil) y cómo están avanzando hacia su finalización.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Horas del artículo]</td> 
   <td>Métrica utilizada para medir la dificultad o complejidad de un artículo. Los equipos Agile pueden elegir si usar horas o puntos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Métrica utilizada para medir la dificultad o complejidad de un artículo. Los equipos Agile pueden elegir si usar horas o puntos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Estratégico]</td> 
   <td>Trabajo a largo plazo que cambia la organización o cómo funciona la organización.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Alineación estratégica]</td> 
   <td>Medir y alinear los objetivos de la empresa entre portafolios y programas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suscriptores]</td> 
   <td> <p>Usuarios que se suscriben a Proyectos, Tareas o Problemas.</p> <p>Cuando se utiliza este campo en un informe, se muestra una lista de suscriptores con cada suscriptor separado por una coma.</p> <p>Para obtener más información, consulte el artículo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Suscripción a elementos de [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea Resumen]</td> 
   <td>Consulte "[!UICONTROL Principal Task]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtarea]</td> 
   <td>Una tarea secundaria, que se encuentra en una tarea principal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Conjunto de políticas que rigen los cambios y el mantenimiento de un sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>El proceso de vinculación física o funcional de diferentes sistemas informáticos y aplicaciones de software para actuar como un todo coordinado.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Una actividad que debe realizarse como un paso hacia el logro de un objetivo final (completar el proyecto).</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Información general sobre tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo de tarea]</td> 
   <td>Otros campos u objetos asociados a una tarea e indican ciertos detalles sobre la tarea. Algunos ejemplos son [!UICONTROL Planned Completion Date] y [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Consulte "[!UICONTROL Tipo de restricción]" y "[!UICONTROL Fecha de restricción]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>Conjunto de políticas que gobierna los umbrales para la creación, asignación, cierre y visibilidad de tareas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>El equipo o usuario responsable de la estimación del esfuerzo y la finalización de la tarea</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Recopilación de usuarios que trabajan para objetivos similares o objetivos empresariales. Estos usuarios se pueden asignar colectivamente a un elemento de trabajo asignando el equipo al elemento de trabajo.</p> <p>Para obtener más información sobre los equipos, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Información general sobre equipos</a>.</p> <p>Los proyectos pueden tener un [!UICONTROL Project Team], que contiene todos los usuarios o funciones asociados con el trabajo del proyecto.</p> <p>Para obtener más información sobre los equipos de proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Las plantillas de proyecto son descripciones genéricas de los proyectos más repetibles. Al crear una plantilla de proyecto, puede definir tareas, poner en cola temas, formularios personalizados, adjuntar documentos o aprobaciones para ahorrar tiempo en la creación de un nuevo proyecto. </p> <p>Puede adjuntar plantillas a proyectos existentes o utilizarlas para crear nuevos proyectos. Toda la información especificada en la plantilla se transfiere a los proyectos que se crean con ella. </p> <p>Para obtener más información sobre las plantillas, consulte <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Información general sobre la plantilla del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Tarea que forma parte de una plantilla. Las tareas de plantilla se convierten en tareas del proyecto que se crea mediante la plantilla.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subproceso]</td> 
   <td>Una [!UICONTROL Note] y su recopilación de respuestas relacionadas con un tema en particular.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura]</td> 
   <td> <p> En una lista o informe de [!UICONTROL Document], se muestra una vista previa del documento en una miniatura. </p> <p> Select <strong>[!UICONTROL Miniatura]</strong>  para ver una miniatura de entre 33 y 66 píxeles de ancho en el informe. </p> <p>El tamaño de la miniatura se ajusta cuando se modifica el ancho de la columna en una lista o informe.</p> <p>Consulte también "[!UICONTROL Large Thumbnail]" en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Puede crear un informe de [!UICONTROL Time Off] para ver cuándo los usuarios han indicado tiempo de espera en su perfil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de horas]</td> 
   <td> <p>Un historial que permite a los usuarios especificar las horas reales que emplearon trabajando en proyectos, tareas o problemas, o las horas que dedicaron a otras actividades no relacionadas con el trabajo, como reuniones o formación. Además de especificar la cantidad de tiempo que ha invertido trabajando, también puede indicar si el tiempo está relacionado con el trabajo o si equivale a tiempo extra utilizando Tipos de horas para definir las entradas de tiempo. Para obtener información sobre las hojas de horas, consulte <a href="../../../timesheets/timesheets/timesheets-overview.md">Información general sobre las hojas de tiempo</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil de parte de horas]</td> 
   <td> <p>Un [!UICONTROL Perfil de parte de horas] es una plantilla que [!DNL Workfront] utiliza para crear automáticamente partes de horas para los usuarios asociados a ellos. </p> <p>Puede configurar una serie de opciones que se aplicarán a cada parte de horas a medida que se vaya creando. Algunos de estos ajustes son: la frecuencia con la que se debe crear el parte de horas (semanal, cada dos semanas, dos veces al mes o mensual), el día de inicio del parte de horas, los aprobadores de parte de horas, los [!UICONTROL Hour Types] disponibles que los usuarios pueden asociar a las horas registradas.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Principal ID] </td> 
   <td> <p>Este campo permite identificar y filtrar datos sobre un grupo de nivel superior y sus subgrupos en una lista o informe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre principal superior] </td> 
   <td> <p>Este campo permite identificar datos sobre un grupo de nivel superior y sus subgrupos en una [!UICONTROL View] para una lista o informe.</p> <p>También puede hacerlo utilizando el campo [!UICONTROL Top Parent ID] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Horas]</td> 
   <td> <p>En un [!UICONTROL project report], este campo muestra la suma redondeada de todas las horas del proyecto, la última vez que se calcularon las finanzas del proyecto. Las [!UICONTROL horas reales] reflejan las horas exactas registradas en el proyecto. Normalmente, las [!UICONTROL horas reales] deben coincidir con las [!UICONTROL horas totales]. Si el campo [!UICONTROL Total Hours] aparece significativamente diferente al campo [!UICONTROL Real Hours], debe volver a calcular las finanzas del proyecto.</p> <p>Para obtener más información sobre cómo volver a calcular las finanzas del proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Volver a calcular las finanzas del proyecto</a>.</p> <p>En una vista de parte de horas [!UICONTROL Standard], este campo hace referencia al total de horas registradas para los elementos de las fechas mostradas en un parte de horas. El campo [!UICONTROL Total Hours] para las hojas de horas de esta vista integrada hace referencia al campo "[!UICONTROL hoursDuration]" que calcula dinámicamente la diferencia en horas entre las fechas de inicio y finalización del parte de horas. Se utiliza para mostrar la columna [!UICONTROL Total Hours] en rojo si el usuario registra más tiempo que las horas disponibles en el lapso de tiempo del parte de horas. Para obtener más información, consulte <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Ver las horas totales en el parte de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de seguimiento]</td> 
   <td> <p>Un atributo de una tarea. Esto determinaba cómo y luego cómo se actualizarían las líneas de tiempo proyectadas para una tarea. Por ejemplo:</p> 
    <ul> 
     <li>[!UICONTROL El usuario debe actualizar] requiere que una tarea se actualice manualmente. De lo contrario, pasará a ser [!UICONTROL Behind Schedule] y luego [!UICONTROL Late].</li> 
     <li>[!UICONTROL Autocompletar] completará automáticamente una tarea cuando haya pasado la Fecha de vencimiento o [!UICONTROL Fecha de finalización planeada].</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Información general sobre el modo de seguimiento de tareas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Déclencheur]</td> 
   <td>Evento que inicia un escenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task]</td> 
   <td>Una tarea incompleta con una condición de [!UICONTROL Late], [!UICONTROL Behind Schedule] o [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea sin asignar]</td> 
   <td>Tarea que no está asignada a ningún usuario, función o equipo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de actualización]</td> 
   <td> <p>Configuración del proyecto que determina cuándo se recalculará la línea de tiempo proyectada del proyecto. Las opciones son:</p> 
    <ul> 
     <li>[!UICONTROL Automático y en Cambio]</li> 
     <li>[!UICONTROL Automático solamente]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuario]</td> 
   <td>Una cuenta creada en [!DNL Workfront] para permitir que una persona inicie sesión e interactúe con el sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Delegación de usuarios]</p> </td> 
   <td> <p>Un objeto de informe que le dice:</p> 
    <ul> 
     <li>Qué usuarios han delegado aprobaciones de tareas, problemas y proyectos</li> 
     <li>¿Qué usuarios han delegado en ellos tareas, problemas y aprobaciones de proyecto?</li> 
     <li>Cuando esas delegaciones empiecen y terminen</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Creación de un informe de delegación de usuarios</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interfaz de usuario]</td> 
   <td>Todos los aspectos visuales e interactivos del [!DNL Workfront] aplicación.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferencias de interfaz de usuario]</td> 
   <td>[!UICONTROL Configuración de interfaz de usuario]. [!DNL Workfront] los administradores pueden cambiar esta configuración para personalizar aspectos de la interfaz de usuario.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>Disponibilidad de un usuario o función según la programación asignada, el TPO y la carga de trabajo actual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>Búsqueda combinada con un informe que muestra cómo se asignan o sobreasignan los usuarios (recursos). Consulte "[!UICONTROL Resource Utilization]" en este artículo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de objeto</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Una medida del tiempo total del ciclo de trabajo (cuánto tiempo se tarda en completar un trabajo) y la frecuencia con que se realiza el trabajo en el tiempo originalmente comprometido (relación trabajo a comisión).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Las vistas se pueden utilizar para modificar las columnas de un informe o de una lista de proyectos, tareas o problemas, o para indicar el derecho del usuario a ver únicamente información en un nivel de acceso o en un nivel de uso compartido de permisos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ver iconos]</td> 
   <td> <p> Este campo es el mismo que los iconos de estado, pero solo está disponible para las vistas siguientes: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Para obtener más información, consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en las vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas del mes pasado]</td> 
   <td> <p>En una lista de informes, muestra el número de veces que el informe se ha visto durante el último mes.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas del último trimestre]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante el último trimestre.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas del año pasado]</td> 
   <td>En una lista de informes, muestra el número de veces que el informe se ha visto durante el último año.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas este mes]</td> 
   <td> <p>En una lista de informes, muestra el número de veces que se ha visto el informe durante este mes.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas este trimestre]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante este trimestre.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas este año]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante este año.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>En un informe de proyecto, tarea o problema, el uso de la siguiente instrucción en modo de texto muestra las horas planificadas del proyecto, la tarea o el problema:</p>
   <p></p><p></p> 
   <p>Para obtener información sobre el uso del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Información general sobre la sintaxis del modo de texto</a>. </p> 
   <p><b>SUGERENCIA</b> 
   <p>En un informe de problema, al agregar uno de los campos [!UICONTROL Horario planificado] se agrega la variable <code>work </code>al informe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>Uno de los dos tipos de licencia principales. Tiene menos acceso que [!UICONTROL Plan], pero puede crear y realizar actualizaciones en el sistema. Esto tiene más capacidades que los tipos de licencia de [!UICONTROL Externo], [!UICONTROL Reviewer] o [!UICONTROL Requester].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] información general sobre licencias</a>.</p> <p>El trabajo puede hacer referencia al número de [!UICONTROL Horario planificado] para un proyecto, tarea o problema. Para obtener más información, consulte el campo "[!UICONTROL work]" en esta tabla. </p> <p>Sugerencia: En un informe de problema, al agregar uno de los campos [!UICONTROL Horario planificado] se agrega la variable <code>work </code>al informe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estructura de desglose de trabajo]</td> 
   <td>Estructura jerárquica de las tareas que va a ejecutar el equipo del proyecto en función de la relación principal/secundaria.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Esfuerzo de trabajo] </td> 
   <td> 
    <p>Un administrador de proyectos podría decidir utilizar este campo en lugar de [!UICONTROL Horario planificado] para estimar el esfuerzo necesario para completar una tarea. Este campo solo está visible cuando se cumplen las siguientes condiciones:</p> 
     <ul> 
      <li> <p>La tarea tiene un [!UICONTROL Tipo de duración simple]. </p> <p>Sugerencia: Si actualiza la tarea [!UICONTROL Duration Type] a cualquier otro tipo, este campo se oculta. </p> </li> 
      <li>El administrador de proyectos ha habilitado [!UICONTROL Utilizar esfuerzo de trabajo] para calcular automáticamente el campo de tarea [!UICONTROL Horario planificado] en el proyecto. </li> 
     </ul> 
     <p>Para obtener información sobre el uso de [!UICONTROL Work Esfort] en lugar de [!UICONTROL Planned Hours] para estimar el esfuerzo de la tarea, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Información general sobre el esfuerzo de trabajo</a>. </p> 
     <p>Puede mostrar este campo en informes y listas de tareas.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Elemento de trabajo]</td> 
   <td> <p>Este campo hace referencia a tareas o problemas en [!DNL Workfront]. </p> <p>El informe [!UICONTROL Work Item] muestra información sobre tareas y problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Combinación de gestión del trabajo]</td> 
   <td>Un [!UICONTROL Work Performance Indicator] (WPI) de la proporción de trabajo asignado para ejecutar su negocio frente a cambiar su negocio. La Combinar WPI le ayuda a comprender, a nivel organizativo, si su estrategia tiene alguna asignación de trabajo real aplicada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Designación de una persona en el sistema elegible para recibir trabajo o tiempo de seguimiento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Función y responsabilidades de la gestión del trabajo]</td> 
   <td>Definición de los propietarios y las partes interesadas para administrar el ámbito, la ejecución y las aprobaciones del problema, la tarea, el proyecto, el programa o el portafolio designados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>Una métrica cuantificable acordada por todas las partes interesadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Agente de gestión del trabajo]</td> 
   <td>Recopilación de usuarios con un interés adquirido en los resultados de una solicitud de trabajo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Puntos de contacto para la administración del trabajo]</td> 
   <td>Registros digitalizados de la comunicación entre las partes interesadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>Relación de mezcla, capacidad, velocidad, calidad y participación.</p> <p>WPI es un acrónimo común de [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>Método en el que se recibe, se prioriza y se ejecuta el trabajo. La forma de ejecutar el trabajo suele denominarse "flujo de trabajo" o "plan del proyecto" (lista de tareas con fechas, relaciones predecesoras, etc.). </p> <p>Algunos ejemplos de un proceso de trabajo pueden ser la producción de un único recurso o la entrega de una campaña de varios recursos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>En el informe [!UICONTROL Proof Approval], este campo muestra todas las plantillas de flujo de trabajo adjuntas a una prueba. Si no hay plantillas adjuntas, la columna está en blanco.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tiempo de trabajo]</td> 
   <td>

<p>Representa el porcentaje del tiempo equivalente a tiempo completo ([!UICONTROL FTE]) que el usuario está disponible para el trabajo real, sin incluir la sobrecarga. [!UICONTROL Tiempo de trabajo] debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, un 20% de disponibilidad para el trabajo real sería 0,2.</p>
   </p>El valor predeterminado del campo es 1, lo que indica que un usuario gasta todo su [!UICONTROL FTE] en trabajo real relacionado con el proyecto.  </p>
   <p>El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto. </p>
   <p> Las excepciones de programación y el tiempo de espera también pueden afectar a la capacidad del usuario. </p>
   <p>Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear una programación</a>. </p>
    <p>Workfront calcula la disponibilidad de un usuario según las preferencias de Gestión de recursos del área [!UICONTROL Setup]. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurar las preferencias de Administración de recursos</a>. </p> 
   <p>Puede actualizar el [!UICONTROL Work Time] de un usuario al editarlo o crearlo. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Edición del perfil de un usuario</a></p> 
   <b>SUGERENCIA</b> 
   <p>Establezca el valor [!UICONTROL Work Time] en 1 para indicar que el usuario está disponible para trabajos relacionados con proyectos con todo su equivalente a tiempo completo.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo de trabajo]</td> 
   <td>En la documentación de Workfront, este término se utiliza para describir el tiempo asignado al trabajo, según una programación.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>En un informe de proyecto, tarea o problema, el uso de la siguiente instrucción en modo de texto muestra el número de horas planificadas del proyecto, la tarea o el problema seguido de la palabra "horas":</p>
   <p></p><p></p>
    <p>Para obtener información sobre el uso del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Información general sobre la sintaxis del modo de texto</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
