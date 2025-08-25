---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glosario de terminología de  [!DNL Adobe Workfront] '
description: El [!DNL Adobe Workfront] glosario enumera términos de uso común en [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] interfaz, informes, o intenta comprender el significado de los  [!DNL Workfront] conceptos definidos en la [!DNL Workfront]  documentación.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 6d02397a15b0b06c3c60fb5d71dfeb3cb0b0a30d
workflow-type: tm+mt
source-wordcount: '21167'
ht-degree: 96%

---


# Glosario de terminología de [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Este artículo debe utilizarse como referencia para entender los términos que puede encontrar en la aplicación [!DNL Adobe Workfront], en la documentación [!DNL Workfront] o cuando hable en general sobre planificación y gestión del trabajo. Actualmente, estamos actualizando esta información, por lo que es posible que esta tabla no esté completa. Eliminaremos esta advertencia cuando consideremos que la información es exhaustiva.

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
   <td>[!UICONTROL Access Level]</td> 
   <td>Un perfil de usuario que determina cómo un usuario puede interactuar con diferentes objetos y herramientas dentro de Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>Una tarea incompleta en un proyecto actual que no está impedida de ser trabajada por una tarea predecesora y no tiene una restricción de tarea con una futura fecha de inicio planificada. En otras palabras, está disponible para trabajar en ello.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>En [!DNL Workfront Goals], una actividad es un indicador de progreso de una meta. Puede ser una barra de progreso que se actualiza manualmente o un proyecto asociado a la meta. No se pueden mostrar actividades en un informe y no se puede acceder a ellas a través de la API de [!DNL Workfront]. Para obtener información sobre las actividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introducción a los resultados y actividades en Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>En el caso de tareas y problemas, se trata del coste asociado a las horas reales registradas en relación con la tarifa coste por hora del recurso asignado a la tarea o al problema. En el caso de los proyectos, se trata de un total de todos los [!UICONTROL Actual Costs] de las tareas y problemas del proyecto. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p>

<p>Los cálculos de [!UICONTROL Costo real] tienen en cuenta las [!UICONTROL Horas reales heredadas]. Para obtener más información, consulte "[!UICONTROL Horas reales]" o "[!UICONTROL Horas reales heredadas]" en esta tabla. </p>   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>La suma de los [!UICONTROL Actual Amounts] de todos los gastos registrados para un proyecto o una tarea.</p> <b>EJEMPLO </b>
   <p>Si crea un gasto para la Tarea 1 e introduce 600,00 $ en el campo [!UICONTROL Actual Amount], el [!UICONTROL Actual Expense Cost] para esta tarea será de 600,00 $. </p> 
   <p>Para un proyecto, [!DNL Workfront] utiliza la siguiente fórmula para calcular [!UICONTROL Actual Expense Cost]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>En un informe de proyecto, tarea o problema, [!UICONTROL Horas reales] es la suma de todas las horas registradas en el proyecto, tarea o problema después de mayo de 2021.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span> Si desde la pestaña [!UICONTROL Updates] de la Tarea 1, haga clic en “Tiempo de registro” e introduce 25 horas, las Horas reales de la Tarea 1 = 25 horas. </p> <p>[!DNL Workfront] calcula [!UICONTROL Actual Hours] para tareas o proyectos principales mediante las siguientes fórmulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Consulte también <strong>[!UICONTROL Horas reales heredadas]</strong>.
    <p>Para obtener más información, vea <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Ver horas reales</a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>El [!UICONTROL Actual Cost] asociado a la mano de obra invertida en una tarea o un proyecto. </p> <p>Para una tarea, [!DNL Workfront] calcula el [!UICONTROL Actual Labor Cost] utilizando la siguiente fórmula:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Si la tarea tiene un [!UICONTROL Cost Type] de [!UICONTROL User Hourly], [!DNL Workfront] utiliza la tarifa de usuario. Si la tarea tiene un [!UICONTROL Cost Type] de [!UICONTROL Role Hourly], [!DNL Workfront] utiliza la tarifa de la función para calcular el [!UICONTROL Actual Labor Cost]. </p> <p>Para un proyecto, [!DNL Workfront] usa la fórmula siguiente para calcular el [!UICONTROL Actual Labor Cost]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Por ejemplo, si un usuario registra 5 horas para una tarea con un [!UICONTROL User Hourly] [!UICONTROL Cost Type] y su tarifa por hora es de 100$, el [!UICONTROL Actual Labor Cost] es de 500$.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>Los [!UICONTROL Actual Revenue] de un proyecto o una tarea son la cantidad de dinero asociada con las [!UICONTROL Actual Hours] del proyecto o la tarea. </p> <p>Para obtener información acerca del seguimiento de los ingresos en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general de facturación e ingresos</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Start]</td> 
   <td>El momento en que un usuario realiza un cambio en un objeto en progreso en el trabajo que se le ha asignado.</td> 
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
   <td>Un tipo de metodología basada en la evolución colaborativa de necesidades y soluciones con equipos interfuncionales. Fomenta la flexibilidad y el cambio en función de un calendario fijo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Se diferencia de un equipo tradicional porque obtiene su trabajo prospectivo de un registro de asuntos pendientes y trabaja en él durante un período de tiempo establecido que se denomina [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>Cuando se hace referencia a este campo [!UICONTROL filters], muestra los usuarios que pertenecen a cualquiera de los equipos a los que pertenece el usuario que ha iniciado sesión o los elementos de trabajo asignados a cualquiera de los equipos a los que pertenece el usuario que ha iniciado la sesión. </p> <p>Le recomendamos utilizar este campo en un filtro para que los informes sean más genéricos a la hora de compartirlos con otros usuarios. De este modo, puede generar solamente un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>Puede encontrar este campo en los siguientes tipos de informes:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Datos financieros)</li> 
     <li>[!UICONTROL Budgeted Hour]</li> 
    </ul> <p>Para un informe de <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)]: </p> 
    <ul> 
     <li>Genere este informe cuando intente conocer <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> la cantidad de [!UICONTROL Planned Hours] que se asignan a sus recursos.</li> 
     <li> <p>La [!UICONTROL Allocation Date] es el primer día (domingo) de una semana en que comienza la asignación de una [!UICONTROL Job Role] a una tarea. Una ([!UICONTROL Job Role]) de un recurso puede tener tantas [!UICONTROL Allocation Dates] como semanas durante la [!UICONTROL Duration] de las tareas a las que está asignado. Si las tareas abarcan varios meses, el primer día de un mes también puede convertirse en una [!UICONTROL Allocation Date], si se encuentra dentro de la [!UICONTROL Duration] de la tarea.</p> <p>Por ejemplo, puede tener una [!UICONTROL Job Role] asignada a una tarea que dure más de 3 semanas y tenga 90 [!UICONTROL Planned Hours]. Estas horas se distribuyen uniformemente durante la duración de la tarea, lo que hace que cada día se asignen 6 [!UICONTROL Planned Hours] a su función:</p> <p><em>[!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ Número de [!UICONTROL Work Days] durante la [!UICONTROL Duration] de la tarea </em> </p> <p>Como resultado, hay tres [!UICONTROL Allocation Dates], una para cada domingo de cada semana durante la [!UICONTROL Duration] de la tarea, cada una con un determinado número de [!UICONTROL Planned Hours] asociadas a ellas.<br>Si la tarea comienza a mediados de la última semana de un mes y finaliza dos semanas después del comienzo de un nuevo mes, la tarea tendrá cuatro [!UICONTROL Allocation Dates] una para cada domingo de cada semana durante la [!UICONTROL Duration] de la tarea y otra para el primer día del nuevo mes.</p> <p>Para aprovechar al máximo esta información, le recomendamos que genere un informe de <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Proyecto (Datos financieros) y añada una agrupación de matriz para la [!UICONTROL Allocation Date]. Después, agrupe los resultados semanalmente, mensualmente, trimestralmente o anualmente para obtener datos más precisos.<br>Para obtener información sobre cómo crear una agrupación de matriz, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Crear un informe de matriz</a>.</p> </li> 
    </ul> <p>La información financiera se rellena en los informes de [!UICONTROL Project (Financial Data)] solo cuando los datos asociados a ella tienen menos de 5 años. Por ejemplo, si se asignó una función a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como la [!UICONTROL Allocation Date] para la función no se rellena en el informe de [!UICONTROL Project (Financial Data)] </p> 
    <div> 
     <p>Para un informe de [!UICONTROL Budgeted Hour]:</p> 
     <ul> 
      <li>Genere este informe cuando trate de conocer la cantidad de [!UICONTROL Budgeted Hours] que se asignan a sus recursos o a sus proyectos en el Planificador de recursos.</li> 
      <li> <p>La [!UICONTROL Allocation Date] es el primer día (un domingo) de la semana para la que se presupuestaron las horas en el [!UICONTROL Resource Planner]. </p> <p><b>Sugerencia</b></p> <p>Si una semana abarca dos meses, se generan dos filas en el informe: una correspondiente al primer día de la semana (domingo de la primera semana, que es durante el primer mes) y la segunda fila muestra el primer día del segundo mes. </p> <p>Por ejemplo, si asigna un presupuesto de 8 horas a un usuario para la semana del 30 de junio (domingo) al 6 de julio (sábado), las dos filas mostrarán una [!UICONTROL Allocation Date] del 30 de junio y del 1 de julio. </p> </p> <p>Para obtener información sobre el presupuesto de recursos en [!DNL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Presupuesto de recursos en el [!DNL Resource Planner] mediante las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>.</p> <p>Para obtener información sobre cómo generar un informe de [!UICONTROL Budgeted Hour], consulte <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Informe: Hora presupuestada</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>Una forma de comunicar a los usuarios información dentro del sistema. Esta información suele provenir de [!DNL Workfront] al administrador o del administrador al usuario. </p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar anuncios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>Una aplicación representa normalmente un conector en una aplicación de software, pero también puede representar funciones especiales que manipulan datos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>En el informe de [!UICONTROL Proof Approval], este campo muestra las decisiones de aprobación de revisión para revisiones que ya no están activas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>En el informe [!UICONTROL Proof Approval report], este campo muestra información sobre una fase actual de revisiones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Un elemento de trabajo determinado, como una tarea, un documento o una plantilla de horas, puede requerir que un supervisor u otro usuario firme el elemento de trabajo. Este proceso de firma se denomina aprobación. </p> <p>Para más información, consulte <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Información general sobre el proceso de aprobación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>En el informe [!UICONTROL Proof Approval], este campo muestra la fecha de aprobación de una revisión.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>Un usuario o definición que debe firmar un elemento de trabajo determinado o el usuario que aprueba las entradas de horas en las plantillas de horas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>En un informe de [!UICONTROL Task or Issue], este campo muestra al Propietario de la tarea o del problema, o al [!UICONTROL Primary Assignee]. También puede filtrar o agrupar por este campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Usuario, función o equipo asignado a un problema o tarea. Los proyectos, portafolios o programas no pueden tener asignaciones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>En un informe de [!UICONTROL Task] o [!UICONTROL Issue], este campo muestra una lista de todas las entidades (usuarios, funciones, equipos) asignadas a la tarea o al problema. Puede filtrar por este campo utilizando los campos [!UICONTROL Assignment Users] y [!UICONTROL Assignment Roles]. Puede filtrar por el equipo asignado a la tarea o al problema mediante el campo Equipo. No puede agrupar un informe por este campo.</p> <p>Los elementos de trabajo que se hayan colocado en la [!UICONTROL Recycle Bin] seguirán mostrándose en algunos informes que hacen referencia al objeto [!UICONTROL Assignment] donde se utiliza un modificador de filtro [!DNL OR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>En un informe de [!UICONTROL Task] o [!UICONTROL Issue], este campo muestra información sobre las funciones asignadas a las tareas o problemas. Este campo muestra [!UICONTROL Primary Owners], así como otras funciones asignadas a tareas o problemas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>En un informe de asignación, tarea o problema, [!UICONTROL Assignment Status] muestra si los usuarios asignados a un elemento de trabajo han hecho clic en el botón [!UICONTROL Work On It] o en el botón [!UICONTROL Done] para aceptar o completar el trabajo. Existen los siguientes [!UICONTROL Assignment Statuses]:</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>: el usuario ha sido asignado a la tarea o al problema, pero no ha hecho clic en el botón [!UICONTROL Work On It] para comenzar a trabajar en él todavía.</li> 
     <li><b>[!UICONTROL Working]</b>: el usuario ha hecho clic en el botón [!UICONTROL Work On It] y está trabajando en el elemento. </li> 
     <li><b>[!UICONTROL Done]</b>: el usuario ha hecho clic en el botón [!UICONTROL Done] y ha completado su trabajo en el elemento. </li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Información general sobre los botones [!UICONTROL Work On It] y [!UICONTROL Done]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>En un informe de [!UICONTROL task] o [!UICONTROL issue], este campo muestra información sobre los equipos asignados a las tareas o problemas. El campo muestra [!UICONTROL Primary Owners], así como otros equipos asignados a tareas o problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>En un informe de [!UICONTROL Task] o [!UICONTROL Issue], este campo muestra información sobre los usuarios asignados a las tareas o problemas. Este campo muestra [!UICONTROL Primary Owners], así como otros usuarios asignados a tareas o problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Un atributo es un rasgo de un objeto de [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>Las auditorías son mensajes del sistema que registran una acción que se produjo en Workfront. Se registran los siguientes tipos de auditoría:</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>La colección de notas generadas automáticamente por eventos cuyo seguimiento se realiza a través de los cambios registrados ([!UICONTROL Audit Areas]). Cada nota registra quién realizó la acción, qué hizo y cuándo lo hizo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Project Update]. Esto recalculará las cronologías de Proyectado y Planificado del proyecto cuando se ejecute el proceso de recálculo nocturno y cuando se realice cualquier actualización del proyecto o de las tareas incluidas en el proyecto. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccionar el tipo de actualización del proyecto</a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilidad</p></td> 
   <td> <p>Este término se utiliza en relación con la “disponibilidad de usuarios” o la “disponibilidad de recursos” y muestra la cantidad de tiempo que el recurso (usuario o función) está disponible para trabajar. </p> 
   <p>Workfront calcula la disponibilidad de los usuarios utilizando varios campos y dependiendo de cuál sea la configuración de las preferencias de Administración de recursos en su sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a>. </p>
   <p>Para obtener más información sobre la disponibilidad de los recursos, consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introducción a la Administración de recursos</a></p>
   Alternativamente, “capacidad” también se utiliza para hacer referencia a la disponibilidad de recursos. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Project Update]. Esto recalculará las cronologías proyectadas y planificadas cuando se ejecute el proceso de recálculo nocturno.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccionar el tipo de actualización del proyecto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Trabajo "habitual" que contribuye a la consecución de los principales objetivos empresariales diarios.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>El área en un entorno ágil donde se guardan las nuevas cuestiones hasta que están listas para trabajar en ellas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Una fuente de datos para medir las iteraciones en un entorno ágil.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billable Expense]</td> 
   <td> <p>Gasto que se marca como facturable al cliente. Puede ser un gasto planificado o un gasto real.</p> <p>Los campos Coste de gastos facturables previsto y Coste de gastos facturables real están disponibles para que los añada a vistas e informes. No aparecen en las páginas de detalles del proyecto o de la tarea.</p>
   <p>Puede encontrar estos campos en los siguientes tipos de informes:</p>
   <ul>
   <li>Línea base</li>
   <li>Plantilla</li>
   <li>Proyecto (Datos financieros)</li>
   </ul>
   <p>Para obtener más información sobre cómo marcar un gasto como facturable, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Administrar gastos del proyecto</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>Registra los ingresos, horas o gastos que se pueden facturar. Esta información puede utilizarse para crear facturas en un sistema contable externo.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Crear registros de facturación</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Estado del registro de facturación</td> 
   <td> <p>En un informe registro de facturación u hora, el estado de un registro de facturación indica si el registro de facturación se ha facturado o no. No se puede eliminar un proyecto ni editar el tiempo asociado a un registro de facturación facturado. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crear registros de facturación</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>El proceso de personalizar [!DNL Workfront] para dar a la interfaz una apariencia que refleje su empresa utilizando sus colores y logotipos.</p><p><strong>NOTA</strong><br>Si su organización se ha incorporado a [!DNL Adobe Experience Cloud], la marca no está disponible.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Área en la parte superior de la página que muestra la ubicación jerárquica del usuario en la aplicación.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obtener más información, consulte <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Descripción general de las rutas de exploración</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>Este campo está obsoleto. Cualquier información que pueda mostrar este campo está relacionada con una función que [!DNL Workfront] ha eliminado y el campo no se puede actualizar. </p> <p>Este campo muestra si el proyecto se ha añadido al [!UICONTROL Capacity Planner] y si se ha completado el cálculo del presupuesto para el mismo. El [!UICONTROL Capacity Planner] se ha eliminado de [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL Desglose]</td> 
   <td> <p>En Workfront Planning, puede mostrar los registros conectados en la vista de escala de tiempo de un registro mediante la función Desglose. </p>
   <p>El desglose de registros por sus conexiones le permite ver las escalas de tiempo de otros registros conectados y comprender cómo pueden afectar al rendimiento y a los plazos de los registros. </p>
   <p>Los registros conectados se muestran anidados en su registro respectivo. </p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md">Administrar la vista de línea de tiempo</a>. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>Este campo está obsoleto. Cualquier información que pueda mostrar este campo está relacionada con una función que [!DNL Workfront] ha eliminado. Este campo no puede actualizarse. </p>
   <p> Este campo sigue siendo visible en los informes y listas del [!UICONTROL project].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>Es el coste asociado a la presupuestación de recursos para un proyecto. </p>
   <p>El campo se muestra en las siguientes áreas de [!DNL Workfront] con los siguientes nombres:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: en el panel de [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Cost]</strong>: en las áreas de [!UICONTROL Utilization] al ver información de [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>: en listas e informes</li>
   </ul>   
    <p>El [!UICONTROL Budgeted Cost] del proyecto se calcula mediante la fórmula siguiente:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Para obtener más información acerca del cálculo de [!UICONTROL Budgeted Cost] y comprender los distintos nombres de este concepto en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular el coste presupuestado del proyecto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>Las horas presupuestadas para los recursos del trabajo que necesitan para completar los proyectos. Este campo hace referencia a las horas presupuestadas en el área de [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] o en el [!UICONTROL Resource Planner]) del proyecto o de los recursos del proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender [!UICONTROL Budgeted Labor Cost] y [!UICONTROL Budgeted Hours] para los proyectos</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Para obtener información acerca de cómo presupuestar usuarios en [!DNL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Presupuestar recursos en el [!DNL Resource Planner] mediante las vistas [!UICONTROL Project] y [!UICONTROL Role] </a>. </p> 
    <p>Las horas presupuestadas en el área de [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] o del [!UICONTROL Resource Planner] se muestran en las siguientes áreas de [!DNL Workfront] y con los siguientes nombres:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nombre para mostrar de [!UICONTROL Budgeted Hours]</strong></td> 
        <td><strong>Áreas de [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>Área de [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] visto por [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgeted Hours]</td> 
        <td> <p>Vista del informe de utilización de [!UICONTROL Hours]</p> <p>Para obtener más información acerca del informe de [!UICONTROL Utilization], consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Información general sobre el informe de [!UICONTROL Resource Utilization]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>Informe de [!UICONTROL Budgeted Hour]</p><p>El objeto [!UICONTROL Budgeted Hour] del informe de Hora presupuestada hace referencia a información relacionada con una herramienta de administración de recursos obsoleta. Solo el campo "[!UICONTROL . Hours]" en este informe hace referencia a las horas presupuestadas en el área de [!UICONTROL Resource Planner] o [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] del proyecto. </p> <p>Para obtener más información acerca de cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>Se ha encontrado en los siguientes informes:</p>
        <ul>
        <li>Informe de [!UICONTROL Project]
        <li>Informe de [!UICONTROL Project (Financial Data)]
        <li>Informe de [!UICONTROL Task]
        <li>Informe de [!UICONTROL Issue]
        <li>Informe de [!UICONTROL Budgeted Hour]</li>
        </ul>
         <p>Para obtener más información acerca de cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Cualquier otra mención a [!UICONTROL Budgeted Hours] en [!DNL Adobe Workfront] hace referencia a horas presupuestadas mediante funciones obsoletas que se han eliminado de Workfront Son campos de solo consulta y no se actualizan con la información actual cuando se utilizan las herramientas de presupuestación de recursos actuales. </p>
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
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>Es el coste asociado con las horas que usted, como gerente de recursos, presupueste para sus funciones para el trabajo que necesitan completar en los proyectos. </p> <p>El [!UICONTROL Budgeted Labor Cost] de un informe de proyecto se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Este campo puede hacer referencia a lo siguiente:</p> 
    <ul> 
     <li> <p>Costes de mano de obra mostrados en el área de [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] o en el [!UICONTROL Resource Planner] que están asociados con el coste de las funciones de un proyecto. Para obtener información acerca del cálculo de [!UICONTROL Budgeted Labor Cost], consulte el artículo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Understand Budgeted Labor Cost] y [!UICONTROL Budgeted Hours] para los proyectos</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Costes de mano de obra mostrados en el área de [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case] que reflejan los [!UICONTROL People Costs] estimados en una iniciativa vinculada al proyecto del [!DNL Scenario Planner] cuando se usa el Planificador de escenarios para presupuestar los recursos del proyecto. Para obtener información acerca de las iniciativas, consulte <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Información general sobre iniciativas en el Planificador de escenarios</a>. </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general sobre [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Se muestra en las siguientes áreas debajo los nombres siguientes:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong>: en el área de [!UICONTROL Resource Budgeting] del [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: en la vista [!UICONTROL Cost] del informe [!UICONTROL Utilization]
   <p>Para obtener más información, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información sobre la utilización de recursos </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: en el proyecto [!DNL Resource Planner] o las vistas [!DNL Role], al consultarse por coste
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: en los siguientes informes: 
   <ul>
    <li>Informe de [!UICONTROL Project]</li>
    <li>Informe de [!UICONTROL Project (Financial Data)]</li>
    <li>Informe de [!UICONTROL Task]</li>
    <li>Informe de [!UICONTROL Issue]</li>
    <li>Informe de [!UICONTROL Budgeted Hour]</li> 
    </ul>
    <p>Para obtener más información acerca de la creación de un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p>
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
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>Este campo está obsoleto. Cualquier información que pueda mostrar este campo está relacionada con una función que [!DNL Workfront] ha eliminado. Este campo no puede actualizarse.</p>
  <p>Estas áreas se han quitado de [!DNL Workfront]. </p> 
  <p>El campo sigue visible en los informes y listas del [!UICONTROL project].</p>
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
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Herramienta utilizada para evaluar si un proyecto debe pasar del estado [!UICONTROL Idea] al estado [!UICONTROL Planning]. En otras palabras, un [!UICONTROL business case] ayuda a la organización a decidir si merece la pena iniciar y completar el proyecto o no, especialmente cuando se comparan proyectos con otros de un portafolio.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Crear un [!UICONTROL Business Case] para un proyecto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>Este campo está obsoleto. Cualquier información que pueda mostrar este campo está relacionada con una función que [!DNL Workfront] ha eliminado. Este campo no puede actualizarse.</p> <p>Este campo sigue visible en el proyecto y en las listas e informes de [!UICONTROL task]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>Uno de los [!UICONTROL Duration Types] de la tarea. Se calculará el porcentaje de un día laborable de 8 horas en el que el usuario asignado a la tarea se asignará a la tarea, según la [!UICONTROL Duration] de la tarea y el [!UICONTROL Work Required].</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la [!UICONTROL Duration] y el [!UICONTROL Duration Type] de la tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>Uno de los [!UICONTROL Duration Types] de la tarea. Se calculará el [!UICONTROL Work Required] de una tarea, dados los porcentajes de [!UICONTROL Duration] y de [!UICONTROL Assignment] del usuario (que se basan en un día laborable de 8 horas).</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la [!UICONTROL Duration] y el [!UICONTROL Duration Type] de la tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>En Workfront, un informe de calendario es un informe dinámico en el que los usuarios pueden ver la fecha y otros detalles importantes de un evento, como la fecha de vencimiento, el estado del trabajo y el usuario al que se ha asignado el evento.</p> <p> Para obtener más información acerca de los informes de calendario, consulte <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Información general sobre los informes de calendario</a>.</p>
   <p> En Workfront Planning, una vista Calendario es un tipo de vista para un tipo de registro que muestra registros en un calendario. Debe tener una licencia adicional para acceder a Workfront Planning. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>Este campo indica si una tarea está lista para iniciarse. Si está lista para iniciarse, el campo [!UICONTROL Can Start] de la tarea se establece en [!UICONTROL True]. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Información general sobre “[!UICONTROL Can Start]” para las tareas</a>.</p> 
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
   <td> <p>Tiempo disponible de un recurso cuando se le puede asignar al trabajo. Consulte “Disponibilidad” </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>Una categoría es un formulario personalizado. Se pueden generar informes para este objeto y mostrarlos en otros informes de objetos. No todos los objetos pueden tener un formulario o una categoría personalizados. Los siguientes objetos pueden tener un formulario personalizado: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>Cuando se añade como una columna a la vista de cualquiera de los siguientes objetos, se muestra una lista de todos los formularios personalizados asociados a estos objetos:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Área de práctica centrada en definir, comprender y adaptar el trabajo planificado a los cambios en los factores de ámbito, programación, costes y recursos.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>Tipo de problema planteado en un proyecto que describe un cambio solicitado en el ámbito acordado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>Uno de los [!UICONTROL Update Types] del proyecto. Solo actualiza las cronologías del proyecto [!UICONTROL Project Projected] and [!UICONTROL Planned] cuando se realizan actualizaciones en las tareas o ediciones en el proyecto o tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Issue], que normalmente indica que se debe realizar una cantidad de trabajo no planificada antes de completar el proyecto.</p> <p>Para obtener más información acerca de los tipos de [!UICONTROL Issue] , vea la sección “Tipos de problemas predeterminados” en el artículo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizar tipos de problemas predeterminados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>Una tarea que es una [!UICONTROL Subtask] de una [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>Colección de [!UICONTROL Subtasks] en una [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] y [!UICONTROL Training]</td> 
   <td>Módulos de aprendizaje, certificaciones, estándares o una comunidad de prácticas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Una herramienta de comunicación para que los usuarios establezcan expectativas sobre las entregas de las tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>Una herramienta de comunicación para que el usuario establezca expectativas en torno a las entregas de las tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] y [!UICONTROL Reporting]</td> 
   <td>Estándares para revisar las excepciones y el estado de un proyecto, programa o portafolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Una [!UICONTROL Company] es una unidad organizativa de [!DNL Workfront]. </p> 
   <p> Puede asociar un usuario o un proyecto con una compañía. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Crear y editar compañías</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>La fecha establecida para que un proyecto, tarea o problema se haya completado. Existen varios tipos de [!UICONTROL Completion dates] en [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. Para obtener más información, vea <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Información general sobre la [!UICONTROL Actual Completion Date] del proyecto</a>.</li> 
     <li>[!UICONTROL Planned Completion Date]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establecer la [!UICONTROL Planned Completion Date] del proyecto</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Información general de la [!UICONTROL Planned Completion Date] de la tarea</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre la [!UICONTROL Projected Completion Date] para proyectos, tareas y problemas</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>El día, relativo al inicio de la [!UICONTROL Template], en el que se supone que debe haberse completado una [!UICONTROL Template Task] o una [!UICONTROL Template].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>Esto indica cómo se marcará un proyecto como [!UICONTROL Complete]. Puede tener dos valores:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: un usuario debe cambiar el estado del proyecto a [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic]: el estado del proyecto cambiará automáticamente a [!UICONTROL Complete] cuando el estado de todas las tareas del proyecto sea del 100% completado y todos los problemas estén cerrados.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Esto es una representación visual del progreso de una tarea, problema o proyecto.</p> <p>En los proyectos, el propietario del proyecto puede establecer manualmente la condición o [!DNL Workfront] la puede establecer automáticamente en función del estado de progreso del proyecto. </p> <p>Los valores posibles para la condición del proyecto son:</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Para obtener más información sobre las condiciones del proyecto, consulte el artículo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Información general sobre [!UICONTROL Project Condition] y [!UICONTROL Condition Type]</a>.</p>
     <p>Puede asociar condiciones de tarea y problema con un número que se puede mostrar en los informes. Las siguientes listas muestran los nombres y números predeterminados para las condiciones de tarea y problema. El administrador del sistema puede actualizar los nombres de las condiciones y puede añadir nuevas condiciones con números diferentes. Una vez que un número está asociado con una condición, no se puede editar.  </p> 
     <p>En el caso de las tareas, el propietario de la tarea establece manualmente la condición. Los valores posibles para la condición de tarea son:</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>Para obtener más información sobre las condiciones de las tareas, consulte el artículo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Actualizar [!UICONTROL Condition] para tareas y problemas</a>.</p> <p>En el caso de los problemas, el propietario del problema establece manualmente la condición. Los valores posibles para la condición de problema son:<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Cuando se realiza el seguimiento del campo [!UICONTROL Condition] en los informes de [!UICONTROL Journal Entry], [!UICONTROL New] y [!UICONTROL Old Number Values] muestran el número asociado con la condición en lugar de su nombre. Si una condición no está definida originalmente para una tarea o un problema y posteriormente la actualiza, la entrada de cuaderno que captura la actualización mostrará el [!UICONTROL Old Number Value] del campo [!UICONTROL Condition] como -2.147.483.648. Consulte también “[!UICONTROL New Number Value]”, “[!UICONTROL Old Number Value]” y “[!UICONTROL Journal Entry]” en este artículo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Este campo muestra la condición actual de tareas, proyectos o problemas. Esta opción muestra las actualizaciones más recientes que los propietarios de tareas, proyectos o problemas han proporcionado en el campo [!UICONTROL Update Status], junto con la nueva condición.</p> <p>Los comentarios realizados en las actualizaciones de condición no se muestran en la columna [!UICONTROL Condition Update]; solo se muestra la actualización principal.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tipos de registros conectados]</td> 
   <td> <p>En Workfront Planning, puede crear una conexión entre una de las siguientes opciones: </p>
   <ul>
   <li>Dos tipos de registro</li>
   <li>Un tipo de registro y un tipo de objeto de Workfront</li>
   <li>Tipo de registro y recurso de Adobe Experience Manager</li></ul>
   <p>La conexión de tipos de registro permite mostrar información de un registro o tipo de objeto en otro tipo de registro.</p>
   <p>Para obtener más información, vea <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Información general sobre los tipos de registros conectados</a>  </p>
  <p>Workfront Planning requiere una licencia adicional. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Registros conectados]</td> 
   <td> <p>En Workfront Planning, después de conectar dos tipos de registros, puede conectar dos registros individuales de esos tipos entre sí.  </p>
   <p>La conexión de registros permite mostrar información de un registro u objeto de otra aplicación en otro registro.</p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/records/connected-records-overview.md">Información general sobre registros conectados</a>. </p>

<p>Workfront Planning requiere una licencia adicional. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Conexiones]</td> 
   <td> <p>En Workfront Planning, las conexiones pueden hacer referencia a tipos de registros conectados o a registros conectados. Workfront Planning requiere una licencia adicional.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>Si utiliza una [!UICONTROL Task Constraint] vinculada a una fecha específica, como [!UICONTROL Must Start On], esa fecha específica se convierte en la [!UICONTROL Constraint Date] de la tarea.</p> <p>Las siguientes limitaciones de tareas actualizan el campo [!UICONTROL Constraint Date]:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>Sugerencia</b></p>   
     <ul> 
      <li> <p>Una tarea con una [!UICONTROL Constraint] de [!UICONTROL Fixed Dates] no tiene [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] solo se puede ver en un informe o vista personalizados.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Si utiliza una restricción de tarea en una tarea de plantilla vinculada a un día específico, como Must Start On, ese día específico se convierte en el día de restricción de la tarea de plantilla.</p> <p>Las siguientes restricciones de tarea actualizan el campo [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>Sugerencia</b></p> <p>  [!UICONTROL Constraint Day] solo se puede ver en un informe o vista personalizados. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>Tendencia de programación de una tarea. Por ejemplo, [!UICONTROL As Soon as Possible] programará una tarea para que comience lo antes posible y [!UICONTROL Finish No Later Than] programará una tarea para que finalice en la fecha de restricción [!UICONTROL Constraint Date] y no más tarde.</p> <p>Para obtener más información, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] información general</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>Menú situado en la parte izquierda de la pantalla en el que los elementos cambian para correlacionarse con el contenido activo. Por ejemplo, cuando un usuario está viendo un proyecto, el [!UICONTROL Contextual Menu] mostrará vínculos a información y herramientas relacionadas con el proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Campo de un informe de proyecto o tarea que muestra información sobre el usuario que es el [!UICONTROL Primary Contact] de un problema cuando el problema se convierte en un proyecto o tarea. El campo también aparece en la sección [!UICONTROL Project Details], donde muestra el nombre del [!UICONTROL Primary Contact] del problema convertido. Consulte también “[!UICONTROL Primary Contact]” en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>La cantidad monetaria que debe gastar al completar un proyecto, tarea o problema. </p> <p>Puede realizar el seguimiento de varios tipos de costes de mano de obra, gastos y riesgos relacionados con el proyecto. Para obtener información sobre el seguimiento de costes en [!DNL Workfront], vea <a href="../../../manage-work/projects/project-finances/track-costs.md">Seguimiento de costes</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>Para una tarea, el [!UICONTROL Cost Type] determina cómo acumulará costes la tarea. Algunos ejemplos son [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly] y [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>Una tarea de un proyecto depende de una tarea de un proyecto diferente.</p> <p>Para obtener más información, vea <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Crear predecesoras de varios proyectos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Datos que son únicos para una organización. Las organizaciones pueden personalizar la aplicación [!DNL Workfront] creando formularios y campos personalizados. Esta información personalizada puede impulsar la creación de informes para KPI, auditoría y combinación de demanda. </p> <p>[!UICONTROL Custom Data] se puede vincular a:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>La opción para especificar si un campo [!UICONTROL Custom Data] está almacenado en la base de datos como texto, fecha, número o moneda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>El tipo de visualización de campo de un campo personalizado. Algunos ejemplos son [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>Para los datos personalizados que permiten al usuario seleccionar entre varias opciones, estos son los valores entre los que puede seleccionar un usuario. Las opciones personalizadas solo son válidas en [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons] y [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>Al utilizar un tipo de visualización personalizada con opciones personalizadas, este es el texto de la interfaz de usuario que se mostrará en el menú desplegable, las casillas de verificación o los botones de opción de esa opción personalizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>Al utilizar un campo personalizado con opciones personalizadas, este es el valor que se almacenará en la base de datos para una opción en particular.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>La definición de los campos de datos o columnas que se muestran para cada objeto de una lista.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Una organización que utiliza una instancia de Workfront.</td> 
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
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> Puede añadir este campo en un informe o en una vista del objeto Informe para mostrar los paneles de control en los que el informe aparece en una lista. </p> <p> Puede utilizar este campo para filtrar por informes que también se enumeran en un panel de control específico. </p> <p> Para obtener más información sobre cómo incluir la información del panel de control en los informes de objetos del informe, consulte la sección “Explicación de los informes que se enumeran en los paneles de control” en el artículo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Acceso y organización de informes</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Consulte “[!UICONTROL Custom Data Type]”.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>Este campo muestra una diferencia de fecha entre [!UICONTROL Planned Start] y [!UICONTROL Today], si falta la [!UICONTROL Actual Completion Date].</p> <p>También muestra una diferencia de fecha entre [!UICONTROL Actual Completion] y [!UICONTROL Planned Completion], cuando hay una [!UICONTROL Actual Completion Date].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Horas laborables predeterminadas personalizables que se asignarán a usuarios y proyectos de una organización. </p> <p>Las programaciones se utilizan para calcular las fechas planificadas, de inicio y de finalización de las tareas asignadas a los usuarios.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Bienes o servicios cuantificables que deben proporcionarse al finalizar un proyecto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Puntuación y prioridad de los procesos de admisión.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>Metas exclusivas de un departamento específico que se centran en mejorar las métricas operativas dentro del departamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>El vínculo entre dos tareas que requieren que una tarea cambie de estado antes de que la otra tarea también pueda cambiar de estado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>El tipo de relación de programación entre una tarea y sus predecesoras. Un ejemplo es [!UICONTROL Finish-Start], que requiere que la primera tarea deba Finalizar antes de que la segunda tarea se pueda Iniciar.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Información general sobre los tipos de dependencia de las tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Cualquier archivo que esté adjunto a un objeto dentro de [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Cada vez que se carga el mismo documento en el mismo objeto, se le asigna un número de versión. Los usuarios pueden ver y cambiar varias opciones de una versión anterior de un documento.</p> <p>Para obtener más información, consulte <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Administrar versiones de documentos</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p>La fecha en la que se debe completar una tarea o un problema. La fecha de vencimiento de una tarea o problema es la misma fecha que la fecha planificada de finalización.</p>
    <p>La Fecha de vencimiento de la tarea y el problema se puede ver en las listas y los informes de tareas y problemas.</p> 
    <p>Consulte también Fecha planificada de finalización en esta tabla. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>Ventana de tiempo asignado para la finalización de una tarea, problema o proyecto (determinado por el número de días entre el [!UICONTROL Planned Start] y la finalización planificada).</p> 
    <ul> 
     <li>Para las tareas, la duración es un campo editable si el tipo de duración de la tarea no es simple. Si el tipo de duración de la tarea es simple o si la restricción de tarea es Fechas fijas, la duración es un cálculo que realiza Workfront.</li> 
     <li>En el caso de los problemas, la duración siempre es un campo editable y debe representar una estimación de un número de días que necesitaría el problema para resolverse.</li> 
     <li>En los proyectos, la Duración es un cálculo que realiza [!DNL Workfront] y representa la diferencia en días entre el inicio planificado de la tarea más temprana y la [!UICONTROL Planned Completion] de la última tarea del proyecto.</li> 
    </ul> <p>Para obtener más información acerca de la diferencia entre [!UICONTROL Duration] y [!UICONTROL Planned Duration] para las tareas, consulte el artículo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Diferencia entre [!UICONTROL Planned Duration] y [!UICONTROL Duration] para las tareas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>Este campo muestra la misma información que el campo [!UICONTROL Duration] en minutos en lugar de días. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>Esto aparece en los cuadros [!UICONTROL Task Details] y [!UICONTROL Edit Task] de un elemento principal de tareas recurrentes. Muestra la duración de cada tarea recurrente. Para obtener información acerca de la creación de tareas recurrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> <p> <span>Las duraciones modificadas en las tareas recurrentes individuales no muestran el valor indicado en este campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Campo de tarea que indica cómo se asigna el trabajo necesario para completar la tarea a los asignados a lo largo de la duración de la tarea. Representa la relación entre la [!UICONTROL Duration] de la tarea, el [!UICONTROL Work Required] y la cantidad de tiempo o [!UICONTROL Allocation] que los recursos asignados deben dedicar a la tarea para completarla. </p> <p>Este campo aparece en la pestaña [!UICONTROL Details] de una tarea. </p> <p>Las opciones para el tipo de duración de una tarea son:</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la [!UICONTROL Duration] de una tarea y [!UICONTROL Duration Type]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>La unidad que se utiliza para medir el tiempo en una búsqueda de energía.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>Relación entre la cantidad de usuarios y el tiempo que tardará la tarea en completarse. A medida que añade más usuarios, el tiempo total programado para que se complete la tarea disminuye, pero la duración de la tarea permanece igual. Por ejemplo, si una tarea consiste en pelar un barril de cacahuetes, al añadir más personas disminuirá el tiempo programado, pero la duración en días-persona seguirá siendo la misma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time] es una unidad de tiempo de la [!UICONTROL Duration] de una tarea. Es el tiempo entre la [!UICONTROL Planned Start Date] y la [!UICONTROL Planned Completion Date] de una tarea que incluye días festivos, fines de semana y días libres. En otras palabras, el tiempo transcurrido es el paso de los días del calendario. </p> <p>[!DNL Workfront] admite las siguientes unidades de tiempo transcurrido para la duración de la tarea:</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>Para obtener más información sobre la duración de una tarea, incluido el tiempo transcurrido, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la [!UICONTROL Duration] y [!UICONTROL Duration Type] de una tarea</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> En un informe de [!UICONTROL Rate], es la fecha en la que finaliza una nueva tarifa de facturación para una función de nivel de proyecto. Las horas asociadas con el proyecto que son anteriores a esta fecha se multiplican por esta tarifa de facturación para calcular los ingresos del proyecto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>El [!UICONTROL Work Performance Indicator] (ICR) que indica cuándo disminuye el compromiso y la confianza en la tarea, proyecto, equipo u organización. Esto indica que es necesario actuar para revivir dicha confianza y dicho compromiso. WPI se mediría haciendo preguntas sencillas como: “¿Ha entendido lo que se esperaba de usted? ¿Ha supuesto el trabajo que se le había asignado alguna diferencia en la organización? ¿Ha realizado usted un gran trabajo?”</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Metas interdepartamentales que contribuyen a las métricas de los metas de la compañía.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Cualquier cambio en un proyecto o tarea.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Tareas automatizadas que se producen cuando tienen lugar los eventos. Un ejemplo común es una notificación automática por correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>Correo electrónico que se genera desde un controlador de eventos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>Un coste no laboral en tareas o proyectos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>Normalmente, es un tipo de licencia, o un usuario con dicha licencia. Un usuario con un tipo de licencia de este tipo solo tiene la capacidad de revisar la información en el sistema. No pueden participar activamente en el trabajo.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]Información general sobre licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>Cualquier servicio o software que esté almacenado y regido fuera del sistema de registro designado.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Cualquier objeto Workfront o la información asociada con él, tal como aparece en la base de datos. </p>
   <p>Por ejemplo, “proyecto”, “usuario”, “hora” son tanto objetos de Workfront como campos. “Nombre”, “Estado”, “Propietario”, “Fecha de inicio” son campos de Workfront asociados con los objetos anteriores. </p>

<p>Cuando se hace referencia a objetos, los términos “objetos” y “campos” se pueden utilizar indistintamente.</p>
   <p>En el ámbito de la creación de informes, los “campos” hacen referencia a los objetos o a la información sobre el objeto que desea capturar en el informe.</p>

<p><b>NOTA</b></p>

<p>En la creación de informes en modo de texto, los campos hacen referencia a los objetos o a su información tal como aparece en la base de datos.</p>
   <p>A veces, el nombre que se ve en la interfaz de usuario es diferente del nombre del campo en la base de datos. Por ejemplo, “issue” es el nombre del objeto en la interfaz de Workfront, pero “opTask” es el nombre del objeto (o el campo) en la base de datos de Workfront. </p> 
   <p> Es importante utilizar el campo tal como aparece en la base de datos al escribir un informe en modo de texto, ver, filtrar o agrupar, o al crear un campo calculado.</p>

<p>Para obtener más información, consulte <a href="../../../wf-api/general/api-explorer.md">Explorador de API</a> e <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Información general sobre el modo de texto</a>.</p>

<p>De forma predeterminada, Workfront incluye un conjunto de campos que definen tanto los objetos como su información. También puede crear campos personalizados para definir objetos, pero no puede crear objetos personalizados.</p>

<p>En Workfront Planning, puede crear campos personalizados para todos los tipos de registros. Los tipos de registros de Workfront incluyen un número muy limitado de campos. Debe crear todos los campos desde cero y asociarlos a tipos de registro. Para obtener más información, consulte <a href="/help/quicksilver/planning/fields/fields-overview.md">Información general del campo</a>. </p> <p>Workfront Planning requiere una licencia adicional. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Uno de los principales componentes de un informe o un elemento de lista que define la información que se muestra en la pantalla. Para obtener más información sobre los elementos de creación de informes, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de creación de informes: filtros, vistas y agrupaciones</a>.</p> <p>El filtro determina los resultados que se muestran en un informe o en una lista del panel de [!DNL Workfront], como proyectos, tareas o problemas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Proceso para administrar los datos de coste de mano de obra, gastos e ingresos en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>Puede definir una cantidad fija de coste para un proyecto. Esto es parte del [!UICONTROL Planned Cost] del proyecto que representa la cantidad de dinero que se necesita para completar el proyecto. Para obtener información sobre los costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>Puede definir una cantidad fija de ingresos para un proyecto. Esto es parte de los [!UICONTROL Planned Revenue] del proyecto que representa la cantidad de dinero que se podría obtener si se completa el proyecto. Para obtener información sobre los ingresos, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Es el mismo campo que [!UICONTROL Status Icons], pero solo está disponible para las vistas siguientes: </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> Para obtener más información, consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en las vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Las carpetas se utilizan para organizar documentos o informes asociados a un objeto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Full Time Equivalent)</td> 
   <td>El equivalente a jornada completa indica la cantidad de tiempo que un recurso está disponible para trabajar. 
   El campo [!UICONTROL FTE] se muestra en las áreas siguientes: 
  <ul>
   <li> Perfil del usuario, al editar o crear el usuario </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (se requiere una licencia adicional para Workfront Scenario Planner) </li>
   <li> Listas de usuarios e informes </li> </ul>

<p>[!UICONTROL FTE] debe ser un número decimal de hasta 1 y no puede ser 0. </p>
   <p> Un [!UICONTROL FTE] de 1 (que es el valor predeterminado para el campo [!UICONTROL FTE] de un usuario, tal como se define en su perfil) significa que un recurso (usuario o función) funciona todas las horas, según la programación que calcula su disponibilidad. </p>
   <p>El administrador de Workfront decide qué horario utilizar para determinar la disponibilidad del usuario.  </p>
   <ul>
   <li> Cuando se utiliza el horario predeterminado de [!UICONTROL Default Schedule], Workfront utiliza el [!UICONTROL FTE] del usuario que se encuentra en su perfil para calcular la disponibilidad. </li>
   <li> Cuando se usa la programación del usuario, Workfront usa el tiempo libre del usuario, el valor de [!UICONTROL Work Time] y las horas de [!UICONTROL Default Schedule] para calcular el [!UICONTROL FTE] del usuario. </li> </ul>

<p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a>.  </p>
   <p>Para obtener más información acerca de la creación de programaciones en [!DNL Workfront], vea <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear una programación</a>. </p>

<p><b>NOTA</b></p>
   <p>Para todos los cálculos del [!UICONTROL Scenario Planner], Workfront utiliza el siguiente valor: 1 [!UICONTROL FTE] = 8 Horas.</p>
   <p>Para obtener más información, vea <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introducción al [!UICONTROL Scenario Planner]</a>. </p>
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
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Una línea de tiempo visual de las fechas del proyecto en una vista de calendario basada en las fechas planificadas o proyectadas a medida que las tareas del proyecto están programadas actualmente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Hay dos conceptos de metas en [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Metas del proyecto</b>: un conjunto de metas empresariales acordadas por las partes interesadas relevantes de un proyecto. Las metas del proyecto forman parte del caso empresarial de un proyecto. </p> <p>No puede mostrar las metas del proyecto en listas o informes, pero puede acceder a ellos a través de la API. </p> <p>Para obtener información acerca de las metas del proyecto de caso empresarial, vea <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Crear metas de caso empresarial </a>. </p> </li> 
     <li> <p><b>Metas estratégicas</b>: Una meta estratégica es una meta que se crea para planificar la estrategia de trabajo para un período de tiempo específico. Puede crear estos tipos de metas usando [!DNL Workfront Goals]. Su organización debe comprar una licencia adicional y debe tener acceso a esta función para poder crear metas estratégicas. [!DNL Workfront Goals] solo están disponibles con una licencia adicional.</p> 
     <p>Para obtener más información, vea <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] información general </a>. </p> 
     <p>Puede mostrar metas estratégicas en una meta o en un informe de proyecto y acceder a ellas a través de la API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>En los informes de [!UICONTROL Goal] y [!UICONTROL Project], se trata de un campo de colección que muestra las metas de la jerarquía a la que pertenece una meta estratégica cuando se alinea con otras metas. Las metas se separan con un delimitador ▸. </p> <p>En este campo solo se muestran los elementos principales de la meta y la meta. Las metas secundarias no se muestran. </p> <p>Para obtener información acerca de cómo alinear metas en [!DNL Workfront Goals], vea <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Información general de la alineación de metas en [!DNL Workfront Goals]</a>. </p> 
   <p>Este campo solo está visible si su organización ha comprado [!DNL Workfront Goals]. Para obtener información acerca de la administración de metas estratégicas mediante [!DNL Workfront Goals], vea <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] información general </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> En un [!UICONTROL Project report], este campo se usa para hacer referencia a las metas de nivel de proyecto asociadas con el caso de [!UICONTROL Business]. Actualmente, este es un campo obsoleto y no está asociado con ninguna funcionalidad.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>En un informe de [!UICONTROL Project], se trata de un campo de colección que muestra todas las metas estratégicas asociadas a un proyecto. Las metas se separan con comas.</p> <p>Este campo solo está visible si su organización ha comprado [!DNL Workfront Goals]. Para obtener información acerca de la administración de metas estratégicas mediante [!DNL Workfront Goals], vea <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] Información general</a>. Para obtener más información acerca de las metas estratégicas y las metas del proyecto en [!DNL Workfront], vea “[!UICONTROL Goal]” en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Configuración de la interfaz que afecta a todos los usuarios. [!UICONTROL Global Interface Preferences] se puede sobrescribir con [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Colección de usuarios (posiblemente del mismo departamento o unidad de negocio) que tienen acceso a los mismos objetos. Además de los usuarios, los grupos pueden asociarse con portafolios, programas, proyectos, <span> plantillas de proyecto, </span> compañías, equipos, programaciones, plantillas de diseño y perfiles de plantilla de horas.</p> <p>También puede conceder permisos a objetos por grupo. Para más información, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general de grupos</a>.</p> <p>En una lista o informe de objetos de uno de los tipos siguientes, puede utilizar el campo [!UICONTROL Group] para enumerar qué objetos de ese tipo están asociados a un grupo determinado: usuario, portafolio, programa, proyecto, <span>plantilla de proyecto</span>, compañía, equipo, programación, plantilla de diseño o perfil de plantilla de horas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Usuarios que administran los objetos, accesos y usuarios de grupos de usuarios designados.</p> <p> En un informe de [!UICONTROL Group], este campo muestra los nombres de los usuarios designados como [!UICONTROL Group Administrators] en el grupo. Para obtener más información sobre los administradores de grupo, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> En una [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile] o [!UICONTROL Schedule report], este campo muestra los grupos a los que tienen acceso los administradores del grupo para modificar la plantilla. También puede filtrar este informe por este campo. </p> <p> Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Crear y administrar plantillas de diseño</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>Elemento de informe que se utiliza para categorizar la información de una lista según un criterio común.</p> <p>Para obtener más información, consulte la sección “[!UICONTROL Groupings]” en el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de creación de informes: filtros, vistas y agrupaciones</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>La fecha en la que una tarea está disponible para trabajar en ella. [!UICONTROL Handoff Date] es un cálculo y no se puede establecer manualmente. <br>Para obtener más información acerca de [!UICONTROL Handoff Date], consulte el artículo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref"> Información general de [!UICONTROL Task Handoff Date]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Un nombre alternativo para describir el área de [!UICONTROL Requests] de [!DNL Workfront]. Puede usar el área de [!UICONTROL Requests] para procesar tickets de asistencia al cliente, solicitudes de proyectos, tickets de servicio de asistencia, etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>En un informe de [!UICONTROL Hour], el [!UICONTROL Owner] es el usuario al que se le atribuyen las horas. Es diferente del usuario que realmente registra la hora. Estas dos entidades pueden ser a veces dos usuarios diferentes. <br>Para obtener más información acerca de cómo registrar tiempo para otro usuario, consulte el artículo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrar tiempo</a>.</td> 
  </tr>

<tr> 
   <td>Estado de hora</td> 
   <td> <p>Atributo establecido por Workfront para las horas reales que los usuarios registran para tareas, problemas o proyectos. </p>

Las entradas de horas pueden tener uno de los siguientes estados en Workfront:
<ul>
   <li><b>Enviado</b>: las horas se han registrado en un proyecto, tarea o problema. Forman parte de un registro de facturación o aún no se han añadido a un registro de facturación.</li>
   <li><b>Aprobado</b>: las horas se han registrado y el propietario del proyecto las ha aprobado. Forman parte de un registro de facturación o aún no se han añadido a un registro de facturación.</li> 
   <li><b>No aprobado</b>: el propietario del proyecto ha registrado y rechazado las horas. Forman parte de un registro de facturación o aún no se han añadido a un registro de facturación.</li>
   <li><b>Facturado</b>: las horas se han registrado, se han añadido a un registro de facturación y el estado del registro de facturación se ha marcado como Facturado. No es necesario que el propietario del proyecto las apruebe.</li>
   <li><b>Facturado y aprobado</b>: las horas se han registrado, el propietario del proyecto las ha aprobado y el estado del registro de facturación se ha marcado como Facturado.</li>
   </ul>

<p>Cuando las horas forman parte de un registro de facturación, el Estado de hora indica si las horas se han aprobado o si se ha facturado el Registro de facturación al que pertenecen. El estado de hora de una entrada de hora solo es visible en una lista de horas o un informe. </p>

<p>Para obtener más información acerca de cómo añadir horas a los registros de facturación, consulte la sección “Añadir horas a los registros de facturación” en el artículo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crear registros de facturación</a>.</p>

<p>Para obtener más información acerca de la hora de aprobación de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Requerir tiempo de aprobación de un proyecto</a>.</p>

<p><b>Sugerencia</b></p>

<p>Las horas generales que no se registran directamente en los elementos de trabajo no muestran un estado de hora. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>Atributo que se puede establecer para Horas reales que los usuarios registran para tareas, problemas o proyectos. También es un atributo para las horas registradas que no están directamente vinculadas al trabajo, como [!UICONTROL Vacation] y [!UICONTROL Time Off].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Administrar tipos de hora</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>El identificador es un indicador alfanumérico asociado con cada objeto en [!DNL Workfront]. Identifica de forma exclusiva cada objeto de la base de datos de [!DNL Workfront]. Puede ver el identificador de cualquier objeto en un informe o una lista para cada objeto. </p> <p><b>Sugerencia</b></p>   <p>También puede ver el identificador en la URL de la página del objeto. Por ejemplo, el identificador de un proyecto puede parecerse al número indicado en la siguiente URL, al acceder a la página [!UICONTROL Project Details]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Sistema Identity Management. Adobe IMS requiere que inicie sesión en Workfront a través de Adobe en lugar de usar su nombre de usuario y contraseña de Workfront.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Metas individuales que contribuyen a las métricas de las metas del equipo, pero que no están relacionadas con el desarrollo personal o profesional.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>Función de uso compartido que permite propagar el acceso de un objeto a otro. Por ejemplo, el acceso heredado del usuario del proyecto definido en los registros del programa y del portafolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>En [!DNL Workfront Scenario Planner], puede dividir un plan en varias iniciativas para facilitar su administración. <span>Puede generar un informe de [!UICONTROL Initiative] y tener acceso a la información de [!UICONTROL Initiative] en un informe de [!UICONTROL Project].</span></p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general sobre [!DNL Scenario Planner]</a>. </p> <p>El informe [!DNL Initiative] no está visible en su instancia de [!DNL Workfront] a menos que su compañía haya adquirido una licencia del [!DNL Workfront Scenario Planner]. No puede tener acceso a [!UICONTROL Initiatives] mediante la API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>El tipo de informe de [!UICONTROL Initiative Job Role] muestra información sobre las funciones asociadas con una iniciativa de plan en el [!DNL Workfront Scenario Planner].</span> </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Información general sobre [!DNL Scenario Planner]</a>. </p> <p><span>Este tipo de informe no es visible en su instancia de [!DNL Workfront] a menos que su compañía haya adquirido una licencia del [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> En un informe de [!UICONTROL Initiative Job Role], se muestra el número de horas asociadas con una función en una iniciativa.</span> </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Información general sobre [!DNL Scenario Planner]</a>. </p> <p>Este tipo de informe y el tipo de informe del [!UICONTROL Initiative Job Role] no es visible en su instancia de [!DNL Workfront] a menos que su compañía haya adquirido una licencia del [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>En un informe de [!UICONTROL Initiative Job Role], se muestra el número de funciones específicas asociadas a una iniciativa.</p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Información general sobre [!DNL Scenario Planner]</a>. </p> <p>Este tipo de informe y el tipo de informe del [!UICONTROL Initiative Job Role] no es visible en su instancia de [!DNL Workfront] a menos que su compañía haya adquirido una licencia del [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Campo de un informe de [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] y [!UICONTROL Project] que muestra la última fecha de publicación de una iniciativa de plan en un proyecto. Puede publicar iniciativas para crear proyectos o actualizar proyectos vinculados a las iniciativas.</p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Información general sobre [!DNL Scenario Planner]</a>. </p> <p><span>Para obtener información sobre las iniciativas de publicación, consulte</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publicar escenarios para crear y actualizar proyectos en [!DNL Workfront Scenario Planner]</a>. Este campo no está visible en su instancia de [!DNL Workfront] a menos que su compañía haya adquirido una licencia de [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>Búsqueda realizada, durante el proceso de cumplimentación de un formulario, para encontrar posibles entradas para un campo específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>El área de la aplicación que permite definir vistas personalizadas, filtros, agrupaciones, controles de lista, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>En [!DNL goal reports], esto muestra un valor “[!UICONTROL True]/[!UICONTROL False]” para cada meta estratégica a fin de indicar si su organización está asignada a la meta como propietario. </p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de metas estratégicas mediante [!DNL Workfront Goals], consulte Información general de <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>Elemento de trabajo no planificado que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Se evalúa y determina su prioridad para considerar el esfuerzo de trabajo adicional</p> <p>Un [!UICONTROL Issue] también puede ser una solicitud de [!UICONTROL Help Desk]. [!UICONTROL Change Orders], [!UICONTROL Requests] y [!UICONTROL Bugs] también son [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>Proceso y reglas que rigen la definición de los tipos de problemas y el proceso de enrutamiento, prioridad o tráfico asociado con cada tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>El equipo o usuarios responsables de determinar la prioridad y completar un problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Período de tiempo en el que un equipo produce un conjunto predefinido de entregas.</td> 
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
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>Se utiliza para identificar las funciones y responsabilidades diarias de un usuario. Las funciones se pueden asignar a elementos de trabajo para identificar la aptitud necesaria para completar un proceso de trabajo sin su asignación a un usuario específico. </p> <p>Un usuario puede tener más de una función. Algunos ejemplos son Diseñador gráfico o Consultor.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Objeto notificable que proporciona información acerca de las actualizaciones del sistema para los campos de seguimiento que aparecen en el área [!UICONTROL Updates] de proyectos, tareas, problemas y otros objetos.</p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Informe sobre el área de actualizaciones con un informe de entrada de diario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>En un informe de [!UICONTROL Task] o de [!UICONTROL Issue], el campo [!UICONTROL Kanban Flag] muestra el estado del indicador que se ha establecido en la historia del [!UICONTROL Kanban board]. Los valores posibles son [!UICONTROL On Track], [!UICONTROL Ready to Pull] y [!UICONTROL Is Blocked].</p> <p>Para obtener más información sobre cómo establecer el estado del indicador en las historias del [!UICONTROL Kanban story board], consulte el artículo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Usar indicadores en las historias del [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Un valor mensurable que demuestra la eficacia con la que una compañía logra sus objetivos empresariales clave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Cantidad de tiempo que debe transcurrir después de que la [!UICONTROL Planned Completion Date] de la tarea predecesora haya pasado hasta que pueda comenzar la tarea dependiente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>Método de cálculo del [!UICONTROL Lag]. Puede ser:</p> 
    <ul> 
     <li>[!UICONTROL Days] (días laborables)</li> 
     <li>[!UICONTROL Calendar Days] (omitir festivos)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Informe general de tipos de retardo</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> En una lista o informe de [!UICONTROL Document], muestra una vista previa del documento en una miniatura. </p> <p>Seleccione <strong>[!UICONTROL Large Thumbnail]</strong> para ver una miniatura de 400 píxeles de ancho en el informe.</p> <p>El tamaño de la miniatura se ajusta al modificar el ancho de la columna en una lista o informe.</p> <p>Consulte también “[!UICONTROL Thumbnail]” en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>En una lista de informes, este campo muestra los nombres de hasta 10 usuarios que han visto el informe más recientemente.<br>Para obtener más información acerca de la información de uso en las listas del informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver el uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>Este campo muestra la última actualización introducida en un objeto por el propietario del objeto. Se trata de la actividad o interacción más reciente del propietario con un objeto.</p> <p>La columna [!DNL Last Condition Note] está vacía si se ha eliminado el texto de la nota de la última nota de un objeto. Cuando se introduce una nota nueva sobre el objeto, se convierte en la última nota y se vuelve a mostrar en la columna. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>En un informe de [!UICONTROL project], este campo registra la fecha y hora a las que se calculado y actualizado por última vez las finanzas del proyecto. Para obtener información sobre finanzas del proyecto, consulte <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Información general sobre las finanzas del proyecto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>Este campo muestra la última actualización introducida en un objeto por cualquier usuario. Esta es la actividad o interacción más reciente con un objeto.</p> <p>La columna [!UICONTROL Last Note] está vacía si se ha eliminado el texto de la última nota de un objeto. Cuando se introduce una nota nueva sobre el objeto, se convierte en la última nota y se vuelve a mostrar en la columna.</p>
   <p>Cuando este campo se añade a un informe de [!UICONTROL Task], las actualizaciones que queden en los objetos secundarios, como problemas, subtareas, documentos, etc. de la tarea, no se muestran en esta columna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>En una lista de informes, este campo muestra información sobre el usuario que ha visto el informe por última vez.<br>Para obtener más información acerca de la información de uso en las listas del informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver el uso del informe</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>En una lista de informes, este campo muestra la fecha en la que se ha visto el informe por última vez.<br>Para obtener más información acerca de la información de uso en las listas del informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver el uso del informe</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>La define el administrador del sistema o de grupos para identificar las pestañas e informes que se muestran en el espacio de trabajo de un usuario determinado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>Junto con [!UICONTROL Custom Views], el [!UICONTROL Layout Type] especifica el tipo de [!UICONTROL Custom View].  Actualmente, solo está disponible Lista. En el futuro, puede estar disponible [!UICONTROL Detail] (la vista de un objeto [!UICONTROL Detail].</td> 
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
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas reales heredadas]</td> 
   <td> <p>En un informe de proyecto, tarea o problema, las [!UICONTROL Horas reales heredadas] son la suma de todas las horas registradas en el proyecto, tarea o problema en cualquier momento, incluso antes de mayo de 2021.</p>  
   <p>Las horas reales heredadas se muestran como horas reales en el área de detalles de un proyecto, tarea o problema. </p>
   <p>Ver también <strong>Horas reales</strong>.
    <p>Para obtener más información, vea <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Ver horas reales</a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Tipo de licencia asignada a un [!UICONTROL Access Level].  Es [!UICONTROL Full User], [!UICONTROL Limited User] o [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>En una vista o informe de [!UICONTROL Group], este campo muestra el número máximo de licencias de [!UICONTROL Plan] que se pueden asignar a usuarios que tienen el grupo respectivo designado como su [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>En una vista o informe de [!UICONTROL Group], este campo muestra el número máximo de licencias de [!UICONTROL Work] que se pueden asignar a usuarios que tienen el grupo respectivo designado como su [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>Tipo de licencia que permite crear un [!DNL Access Level] que contenga privilegios de solo lectura, con la posibilidad de enviar problemas, introducir notas y cargar documentos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Parte de [!UICONTROL Interface Setup] que permite vincular filtros, vistas y agrupaciones personalizados a usuarios individuales o globalmente a todos los usuarios.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Campos de búsqueda]</td> 
   <td> <p>En Workfront Planning, después de establecer la conexión entre dos tipos de registros y de vincular registros individuales, puede hacer referencia a los campos de los registros vinculados en el registro desde el que se conecta.</p>
   <p>Por ejemplo, si conecta un tipo de registro de campaña con un tipo de objeto de proyecto de Workfront, puede mostrar el campo Presupuesto de los proyectos conectados en los registros de campaña. El campo Proyecto de presupuesto es un campo de búsqueda de proyectos en una campaña.</p> <p>Los valores de los campos de búsqueda se rellenan automáticamente en los registros desde los que están conectados.</p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/records/connected-records-overview.md">Información general sobre registros conectados</a>.</p>
   <p>Workfront Planning requiere una licencia adicional.</p>
    </td> 
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
   <td> <p>Uno de los [!UICONTROL Update Types] de [!UICONTROL Project]. Esta configuración permite actualizar las líneas de tiempo de [!UICONTROL Project Projected] y [!UICONTROL Planned] solo cuando se hace clic en “[!UICONTROL Recalculated Timelines]”. Los proyectos configurados de esta manera se omitirán durante el proceso de cálculo nocturno y cuando se actualicen el proyecto o las tareas del proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccionar el [!UICONTROL Update Type] del proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Hace referencia al usuario que ha iniciado sesión actualmente. </p> <p>Le recomendamos utilizar este campo en un filtro para que los informes sean más genéricos a la hora de compartirlos con otros usuarios. De este modo, puede generar solamente un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Este campo está obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una característica que [!DNL Workfront] ha quitado y el campo no se puede actualizar. </p> <p>En versiones anteriores de [!DNL Workfront], se podía actualizar este campo al crear o editar una función. Muestra el número total de usuarios que se pueden asociar a una función en cada proyecto. Un valor de cero permitido para un número ilimitado de usuarios que se pueden asignar en un proyecto. </p>El campo sigue visible en algunos informes y listas, pero la información mostrada no se puede actualizar. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Un marcador que se puede asociar a una tarea para indicar que se ha alcanzado un punto clave del proyecto cuando se completa la tarea. Por lo general, puede utilizar hitos para mostrar un evento significativo, como la finalización de una fase del proyecto o un conjunto de actividades críticas. [!UICONTROL Milestones] suelen estar asociados a tareas principales. Debe crear los hitos para poder adjuntarlos a las tareas. Para obtener información acerca de los hitos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Crear una ruta de hitos</a> y <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Asociar hitos con tareas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Colección de [!UICONTROL milestones]. [!UICONTROL Milestone Paths] se utilizan en proyectos para distinguir proyectos con ciertos tipos de [!UICONTROL Milestones] de proyectos con un conjunto diferente de [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>Una tarea marcada para indicar un evento notificable que hay que medir.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Un solo paso en un escenario en [!DNL Workfront Fusion] que realiza alguna función basada en la aplicación asociada.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>Cuando se hace referencia a esto en los filtros, se muestran los usuarios que tienen la misma [!UICONTROL Primary Role] que el usuario que ha iniciado sesión o los elementos de trabajo asignados a la [!UICONTROL Primary Role] del usuario que ha iniciado sesión.</p> <p>Le recomendamos utilizar este campo en un filtro para que los informes sean más genéricos a la hora de compartirlos con otros usuarios. De este modo, puede generar solamente un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Cuando se hace referencia a esto en los filtros, este campo muestra los usuarios que pertenecen al [!UICONTROL Home Team] del usuario que ha iniciado sesión o los elementos de trabajo asignados al [!UICONTROL Home Team] del usuario que ha iniciado sesión. </p> <p>Le recomendamos utilizar este campo en un filtro para que los informes sean más genéricos a la hora de compartirlos con otros usuarios. De este modo, puede generar solamente un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>Conjunto de reglas de toda la organización que utilizan datos para crear nombres de proyectos, tareas y entregas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Integración que no requiere codificación manual ni configuración de la API. También se denomina integración “predeterminada”.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>Panel superior central de la aplicación que tiene vínculos a las áreas principales de [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>En un informe de [!UICONTROL Journal Entry], se muestra el valor actualizado de un campo que reemplaza a [!UICONTROL Old Number Value].
 Para obtener más información, consulte “[!UICONTROL Old Number Value]” en este artículo.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Non-Billable Expense]</td> 
   <td> <p>Un gasto que no está marcado como facturable al cliente. Puede ser un gasto planificado o un gasto real.</p> <p>Los campos Coste de gastos planificados no facturables y Coste de gastos reales no facturables están disponibles para que los añada a las vistas e informes. No aparecen en las páginas de detalles del proyecto o de la tarea.</p>
   <p>Puede encontrar estos campos en los siguientes tipos de informes:</p>
   <ul>
   <li>Línea base</li>
   <li>Plantilla</li>
   <li>Proyecto (Datos financieros)</li>
   </ul>
   <p>Para obtener más información sobre cómo marcar un gasto como facturable, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Administrar gastos del proyecto</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>Un día que no está asignado a la finalización de ninguna asignación. Generalmente es un día de vacaciones, un día festivo o un fin de semana. El término se muestra en el explorador de la API. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>Comentario o actualización realizada en un objeto de [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>Muestra el texto de una actualización introducida por un usuario en cualquier objeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>En un informe de [!UICONTROL Project], es el número de objetivos estratégicos asociados al proyecto. Para obtener información acerca de cómo asociar proyectos con metas estratégicas, consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Añadir proyectos a metas en [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Para obtener información acerca de los objetivos estratégicos, consulte también “[!UICONTROL Goal]” en este artículo.</p> 
   <p>Este campo solo está visible si su organización ha comprado [!DNL Workfront Goals]. Para obtener información acerca de cómo administrar metas estratégicas con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Añadir proyectos a metas en [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>La información que se muestra en [!DNL Adobe Workfront] está representada por objetos almacenados en la base de datos de [!DNL Workfront]. Los objetos son lo que impulsa la información en Workfront. Algunos ejemplos de objetos son los siguientes:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Template tasks]</li>

<p><b>NOTA</b></p>
  <p>Esta no es una lista exhaustiva. </p>

</ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprender los objetos en [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>Si crea un informe o una lista que contiene todos los formularios personalizados, puede utilizar este campo como vista o filtro para ver qué tipos de objetos están asociados con cada formulario. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>En un informe de [!UICONTROL Journal Entry], se muestra el valor original de un campo antes de que se actualizara. Una vez actualizado el valor de un campo, se mostrará como [!UICONTROL New Number Value] en un informe de [!UICONTROL Journal Entry]. Para obtener más información, consulte “[!UICONTROL New Number Value]”.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Project Update]. Si se selecciona esta opción, las cronologías de [!UICONTROL Project Projected] y [!UICONTROL Planned] solo se actualizan cuando se realiza una actualización o un cambio en el proyecto o en una tarea del proyecto. No se actualiza el proyecto todas las noches.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccionar el tipo de actualización del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>Nombre de [!UICONTROL Issue] en la base de datos [!DNL Workfront], que se utiliza en los informes de modo de texto o en los datos personalizados calculados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Problema o tarea que no se ha completado, pero se está trabajando en ello.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Abreviatura de Organigrama. Se trata de un gráfico que muestra la jerarquía de una organización. También aparece en la ficha de la pantalla de detalles de [!UICONTROL User] que muestra y permite establecer las relaciones de [!UICONTROL Company] de [!UICONTROL User] y [!UICONTROL Reporting]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>Define [!UICONTROL Companies], [!UICONTROL Groups] y [!UICONTROL Security Profiles] para su organización.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>En un informe o vista que enumera los usuarios, este campo muestra todos los grupos de los que es miembro cada usuario. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>En un informe [!UICONTROL Job Role], esta es la moneda asociada a una función. Es una anulación de la [!UICONTROL Base Currency] tal como la estableció el administrador de [!DNL Workfront] en el área [!UICONTROL Setup]. </p> 
     <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Job Role], esta es la tarifa por hora de facturación de la función que utiliza la [!UICONTROL Override Currency] seleccionada de la función.</p> 
     <p> Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Job Role], es la tarifa de coste por hora de la función utilizando la [!UICONTROL Override Currency] seleccionada de la función. </p> 
     <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>El usuario responsable de la finalización del objeto designado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Goal], se muestra el tipo de propietario asignado a una meta estratégica. Los siguientes son los tipos de propietario de metas:</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>No se muestra ningún valor en este campo cuando el propietario de la meta es su organización. </p> 
     <p>Se requiere una licencia adicional. Para obtener información acerca de [!DNL Workfront Goals], vea <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] Información general</a>. </p> 
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
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>Un [!UICONTROL parameter] es un campo personalizado. Puede crear un informe para todos los parámetros o campos personalizados del sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>En un informe, este campo muestra información sobre el objeto principal del objeto. Por ejemplo, en un informe de [!UICONTROL issue], puede mostrar información sobre la tarea o el proyecto en el que se ha registrado el problema; en un informe de tareas, puede mostrar información sobre la tarea principal directa o sobre el proyecto. Para obtener más información acerca de los objetos que podrían tener elementos primarios en [!DNL Workfront], consulte la sección "Interdependencia y jerarquía de objetos" en el artículo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprender los objetos en [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>Cantidad de tiempo que debe transcurrir entre el inicio de la [!UICONTROL Parent Task] y el inicio de la [!UICONTROL Subtask].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>También se conoce como [!UICONTROL Summary Task]. Esta es una tarea que tiene Subtareas (también denominadas [!UICONTROL Children Tasks]). La [!UICONTROL Duration], [!UICONTROL Work Required], y [!UICONTROL Percent Complete] de la tarea principal se calcula a partir de las subtareas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>Un usuario con licencia que tiene menos capacidad que el horario predeterminado definido en el sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Campo de proyecto, tarea o problema que muestra qué porcentaje del trabajo asociado con la tarea, el proyecto o el problema se ha completado.</p> <p>Puede actualizar este campo manualmente para problemas y tareas de trabajo. </p> <p>Para los proyectos y las tareas principales, este campo es un resumen de todas las tareas de trabajo y no se puede actualizar de forma manual. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Información general del proyecto [!UICONTROL Percent Complete]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Derechos que se conceden a un usuario sobre un objeto, normalmente otorgados para que pueda completar el trabajo en el elemento o verlo. Puede conceder permisos a:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Para obtener más información, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido en objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Es un tipo de licencia completa en el sistema [!DNL Workfront]. Los usuarios deben tener esto para tener acceso a todas las características de [!DNL Workfront].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]Información general sobre licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (en [!DNL Scenario Planner])</td> 
   <td> <p>Un plan es el objeto principal cuando se trabaja con el Planificador de escenarios [!DNL Workfront]. Puede esbozar la estrategia para el futuro a corto y largo plazo de su empresa, identificar cada resultado de alto nivel y agregarlo como plan al Planificador de escenarios [!DNL Workfront]. </p> <p>No puede mostrar [!DNL Scenario Planner] planes en un informe y no puede acceder a ellos a través de la API [!DNL Workfront]. </p> <p>[!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca de [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">La descripción general de [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>El lapso de tiempo en el que está programado que ocurra algo. Cuando crea proyectos, tareas o problemas en [!DNL Workfront], establece las fechas de inicio y finalización planificadas, así como el período de tiempo planificado durante el cual se producen. Estos valores representan su intención original o estiman el tiempo que un elemento debería tardar en completarse. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Se trata de una entrada manual para que el administrador del proyecto calcule si la finalización de un proyecto reportaría algún beneficio monetario a la organización. Especificar este valor puede formar parte de la creación de un [!UICONTROL Business Case] para el proyecto. Debe tener permisos de [!UICONTROL Manage] en el proyecto para actualizar este valor.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>En un informe de [!UICONTROL Budgeted Hour], se muestra el número de horas presupuestadas para proyectos o [!UICONTROL Job Roles] en el [!UICONTROL Resource Planner]. </p> <p>Para obtener información acerca de cómo presupuestar proyectos o funciones en [!UICONTROL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Presupuestar recursos en el [!UICONTROL Resource Planner] mediante las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>. Para obtener información acerca del informe de [!UICONTROL Budgeted Hours], consulte el artículo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Informe: hora presupuestada</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>Puede establecer manualmente la [!UICONTROL Planned Completion Date] de una tarea, proyecto o problema en una fecha de su elección. Si no establece la [!UICONTROL Planned Completion Date], [!DNL Workfront] la establece automáticamente. Cuando se establece automáticamente, la [!UICONTROL Planned Completion Date] es: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Para obtener más información, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Información general sobre la tarea [!UICONTROL Planned Completion Date]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establecer la [!UICONTROL Planned Completion Date] del proyecto</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>Total del [!UICONTROL Planned Labor Cost] y el [!UICONTROL Planned Expense Cost] del proyecto. Esto no incluye el [!UICONTROL Planned Risk Cost] en el proyecto.  </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Planned Date Alignment]</td> 
   <td> <p>Este es un indicador automático de que Workfront asigna proyectos, tareas y problemas para mostrar cuándo se completará un elemento en relación con su fecha planificada de finalización. </p>
   <p>Los siguientes son valores posibles para el indicador Alineación de fechas planificada: </p>
<ul>
<li>Se terminará en la fecha planificada de finalización</li>
<li>Se terminará antes de la fecha planificada de finalización</li>
<li>Se terminará después de la fecha planificada de finalización</li></ul>
<p>La alineación de fechas planificada es visible en las listas de proyectos, tareas y problemas y en los informes. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>La [!UICONTROL Planned Duration] de una tarea suele ser la misma que la [!UICONTROL Duration] de la tarea. Representa la diferencia en días entre el [!UICONTROL Planned Start] y las [!UICONTROL Planned Completion Dates] de la tarea. </p> <p>Cuando la tarea tiene un tipo de [!UICONTROL Duration] de [!UICONTROL Effort Driven], la [!UICONTROL Planned Duration] puede diferir de la [!UICONTROL Duration] de la tarea, en función de cuántos recursos le asigne. </p> <p>Por ejemplo, si una tarea con un tipo de [!UICONTROL Duration] de [!UICONTROL Effort Driven] tiene una [!UICONTROL Duration] de 3 días y asigna un recurso con una programación a tiempo completo sobre la tarea, la [!UICONTROL Planned Duration] también será de 3 días. Si asigna tres recursos con una programación a tiempo completo sobre la misma tarea, la [!UICONTROL Duration] sigue siendo de 3 días, pero la [!UICONTROL Planned Duration] pasa a ser de 1 día. La [!UICONTROL Planned Duration] también cambia las fechas de [!UICONTROL Planned Start] y [!UICONTROL Planned Completion] de la tarea para reflejar la nueva [!UICONTROL Planned Duration].  Como resultado, la línea de tiempo del proyecto también se ve afectada. </p> <p>Para obtener más información acerca de la diferencia entre [!UICONTROL Duration] y [!UICONTROL Planned Duration] para tareas, consulte el artículo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Diferencia entre [!UICONTROL Planned Duration] y [!UICONTROL Duration] para tareas</a>.</p> <p>Los proyectos y problemas no tienen una [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>La [!UICONTROL Planned Duration Minutes] de un proyecto o un problema es la [!UICONTROL Duration] del proyecto o problema en minutos. </p> <p>Las tareas no tienen un campo de [!UICONTROL Planned Duration Minutes] </p> <p>Las [!UICONTROL Template Tasks] tienen un campo de [!UICONTROL Planned Duration Minutes] que muestra la [!UICONTROL Planned Duration] de la tarea en minutos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>Suma de [!UICONTROL Planned Amounts] para todos los gastos registrados de un proyecto o tarea.</p> <p><b>Ejemplo</b></p>
   <p>Si crea un gasto para la Tarea 1 y escribe 600 USD en el campo [!UICONTROL Planned Amount], el [!UICONTROL Planned Expense Cost] para esta tarea es de 600 USD. </p> 
   <p>Para un proyecto, [!DNL Workfront] usa la fórmula siguiente para calcular el [!UICONTROL Planned Expense Cost]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>Este campo aparece en las áreas de [!UICONTROL projects], [!UICONTROL tasks] y problemas, informes de proyectos, tareas o problemas y herramientas de administración de recursos como [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] y el informe de [!UICONTROL Utilization]. </p> <p>Muestra el número de horas que el propietario del proyecto estima que cada tarea o problema debería tardar en completarse. En los proyectos, suele ser un resumen de las [!UICONTROL Planned Hours] de las tareas del proyecto. </p> <p>El campo [!UICONTROL Planned Hours] puede mostrar información diferente según el lugar desde el que se vea. Para obtener información sobre las horas planificadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Información general de las horas planificadas</a>.</p> <p>Las horas planificadas se almacenan en minutos en la base de datos de [!DNL Workfront]. Cuando escriba cálculos utilizando este campo, asegúrese de que tiene en cuenta el hecho de que las horas se muestran como minutos.<br></p> <p>De forma predeterminada, las horas planificadas se distribuyen de forma equitativa para todos los días dentro de la duración de un elemento de trabajo y también de forma equitativa para todos los recursos asignados a la tarea. Los usuarios pueden actualizar el número diario de horas planificadas para un elemento de trabajo o las horas planificadas individuales para cada asignado.</p> <p>La actualización de este campo es diferente para los proyectos, las tareas y los problemas: </p> 
    <ul> 
     <li> <p>Para los problemas, puede actualizar manualmente este campo.Las horas planificadas de problemas no se añaden a las horas planificadas de los proyectos. </p> <p><b>Sugerencia</b></p> <p>En un informe de problemas, uno de los campos [!UICONTROL Planned Hours] se reemplaza por el campo [!UICONTROL Work].El campo muestra la cantidad de horas planificadas en el problema. Para obtener más información, consulte los campos "trabajo" o "[!UICONTROL Work]" en esta tabla. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para las tareas, puede actualizar manualmente este campo cuando el [!UICONTROL Duration Type] de la tarea sea [!UICONTROL Calculated Assignment] o [!UICONTROL Simple]. Este campo lo calcula [!DNL Workfront] cuando el [!UICONTROL Duration Type] de la tarea es [!UICONTROL Calculated Work] o [!UICONTROL Effort Driven].<br>Para obtener información sobre la [!UICONTROL Task Duration], consulte el artículo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la [!UICONTROL Duration] y el [!UICONTROL Duration Type] de la tarea</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>En los proyectos, [!DNL Workfront] calcula las horas planificadas añadiendo todas las horas planificadas de todas las tareas del proyecto. </p> </li> 
    </ul> <p><b>Sugerencia</b></p> <p>También puede mostrar las [!UICONTROL Planned Hours] en los informes de [!UICONTROL project], [!UICONTROL task] o [!UICONTROL issues] utilizando el modo de texto y haciendo referencia a campos adicionales. Para obtener más información, consulte los campos "<code>work</code>", "[!UICONTROL Work]" y "<code>workRequiredExpression</code>" de esta tabla. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>Para una tarea, la tarifa por hora del usuario o función multiplicada por el número de horas asignadas al usuario o o a la función.</p> <p>Para un proyecto, es un total de todos los [!UICONTROL Planned Labor Costs] de todas las tareas.</p> <p>La utilización de la tarifa del usuario o función depende del tipo de coste seleccionado para la tarea especificada. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Las tareas y los proyectos pueden mostrar un valor para los [!UICONTROL Planned Revenue] en [!DNL Workfront].  Los [!UICONTROL Planned Revenue] representan la cantidad de dinero asociado a las [!UICONTROL Planned Hours] de las tareas del proyecto. Para los proyectos, también puede incluir los [!UICONTROL Fixed Revenue] del proyecto. </p> <p>En el caso de las tareas, son los ingresos asociados a las [!UICONTROL Planned Hours] de las tareas. Las horas planificadas de todas las tareas se suman a las horas planificadas del proyecto para contribuir al cálculo de las [!UICONTROL Planned Hours] del proyecto. </p> 
   <p>[!DNL Workfront] calcula los [!UICONTROL Planned Revenue] de tareas y proyectos mediante las fórmulas siguientes:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Los [!UICONTROL Planned Revenue] del proyecto que se muestran en el área [!UICONTROL Project Details] y en los informes de proyecto son diferentes de los ingresos planificados que se muestran en el informe de [!UICONTROL Utilization]. </p> <p>Los [!UICONTROL Planned Revenue] del área [!UICONTROL Project Details] reflejan los ingresos de la tarea así como los ingresos fijos del proyecto. Los [!UICONTROL Planned Revenue] del [!UICONTROL Utilization Report] muestran los [!UICONTROL Planned Revenue] asociados únicamente a las tareas del proyecto. </p> 
     <p><b>Ejemplo</b></p>  
      <p>Si el proyecto tiene 1 tarea con 10 horas, asignada a un consultor con una tarifa por hora de 20 $ y el proyecto tiene 100 $ de [!UICONTROL Fixed Revenue], el informe de [!UICONTROL Utilization] muestra 200 $ de [!UICONTROL Planned Revenue] (los [!UICONTROL Planned Revenue] asociados a las horas de la tarea).  La sección [!UICONTROL Project Details] muestra 300 $ (los [!UICONTROL Planned Revenue] de la tarea y los ingresos fijos del proyecto). </p> 
    <p>Para obtener información sobre el seguimiento de los ingresos en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Información general sobre facturación e ingresos</a>. </p> 
    <p>Para obtener información sobre los cálculos de [!UICONTROL Planned Revenue] en el informe de [!UICONTROL Utilization report], consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ver información sobre la utilización de recursos</a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>El total del [!UICONTROL Potential Cost] de todos los riesgos del proyecto teniendo en cuenta su probabilidad de que ocurran. Esta cantidad no se incluye en el [!UICONTROL Planned Cost] del proyecto.</p> <p>El [!UICONTROL Planned Risk Cost] de un proyecto se calcula mediante la siguiente fórmula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Colección definida por el administrador de fichas y secciones que se muestra en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Un componente de una Pestaña en un panel de control o página de Portal. Generalmente, un solo informe, gráfico, calendario o lista de información clave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Pestaña de un portal o panel de control que contiene hasta tres secciones de portal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Colección de proyectos con características comunes. Estos proyectos suelen competir por los mismos recursos, presupuesto o franja horaria. Puede dividir Portafolio en Programas y asociar los proyectos con los Programas antes de añadirlos a un Portafolio.</p> <p>Para obtener más información sobre portafolios, consulte <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Información general al portafolio en [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Área de práctica centrada en administrar una colección o programas y esfuerzos de proyectos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Una herramienta de [!DNL Workfront] para ayudar a evaluar y priorizar proyectos dentro de un portafolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>El responsable de departamento de la priorización y el presupuesto de un portafolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>Este es un campo del proyecto que se puede encontrar en listas e informes. Muestra el coste potencial de los riesgos asociados con el proyecto, en caso de que se produzcan. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular el coste potencial de riesgos</a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Tarea que debe completarse antes de que finalice una tarea dependiente. También es una tarea que está marcada como [!UICONTROL Dependency] para otra tarea. Las predecesoras permiten al planificador establecer una lógica de dependencia de secuencias, como iniciar una tarea una vez finalizada otra.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Información general sobre las predecesoras de tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>Compañía a la que pertenece el usuario según lo designado en su configuración de usuario. Las compañías también pueden asociarse con proyectos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>El [!UICONTROL Primary Contact] es el creador de un problema y [!DNL Workfront] lo designa automáticamente cuando alguien lo crea. Puede actualizar manualmente este campo si tiene permisos de [!DNL Manage] del problema. Un problema solo puede tener un contacto principal.</p> 
   <p>Si cambia el Contacto principal, el usuario designado originalmente como contacto principal seguirá teniendo acceso de [!UICONTROL Manage] al problema.</p>
   <p>Al convertir un problema en una tarea o un proyecto, el usuario designado como [!UICONTROL Primary Contact] del problema se convierte en el [!UICONTROL Converted Issue Originator] del proyecto o tarea. Si el [!UICONTROL Primary Contact] del problema se actualiza después de convertirlo, el [!UICONTROL Converted Issue Originator] se conservará como el [!UICONTROL Primary Contact] del problema en el momento en el que se produjo la conversión. Consulte también “[!UICONTROL Converted Issue Originator]” en este artículo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Un valor que se puede asignar a una tarea, problema o proyecto para designar la importancia que tiene. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>En un [!UICONTROL Note] o [!UICONTROL Document], esta opción oculta ese objeto a la mayoría de los visualizadores. Para una cola de solicitudes de ayuda privada, solo los usuarios del equipo del proyecto pueden enviar problemas a esa cola (o proyecto) a través del área de [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Toda la información sobre una cuenta de usuario.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Un subconjunto dentro de un portafolio, donde proyectos similares pueden agruparse para lograr un beneficio bien definido.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Administración de dependencias, riesgos, problemas, requisitos y soluciones entre proyectos para mantener el programa en buen estado y lograr el beneficio definido del programa.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>El responsable del departamento de supervisar y organizar las actividades para garantizar que las metas del proyecto se ajusten a los objetivos de la compañía.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>En un informe de [!UICONTROL Goal], muestra el porcentaje de proximidad a la consecución de una meta estratégica. El porcentaje del progreso se muestra como un número. Para obtener información acerca de las metas estratégicas, consulte “[!UICONTROL Goal]” en esta tabla.</p> <p>Este campo solo es visible si su organización ha adquirido [!DNL Workfront] Goals. Para obtener información acerca de la administración de metas estratégicas mediante [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Añadir proyectos a metas en [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>En un informe de proyecto, tarea y meta, este campo muestra el estado de progreso de los proyectos, tareas o metas estratégicas. Para obtener más información, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Información general sobre el estado de progreso del proyecto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Información general sobre el estado de progreso de la tarea</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Información general sobre el progreso y la condición de la meta en [!DNL Adobe Workfront Goals]</a> </p>
     <p>El informe [!UICONTROL Goal] y el informe [!UICONTROL Progress Status] para el campo [!DNL goals] solo son visibles si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información acerca de las metas estratégicas de [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] información general</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Una gran cantidad de trabajo que debe completarse en un plazo determinado y debe utilizar un presupuesto y un número de recursos específicos. Para hacerlo manejable, divide el proyecto en una serie de tareas. La realización de todas las tareas da como resultado la finalización del proyecto. Para obtener información sobre cómo planificar un proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Información general sobre cómo planificar un proyecto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>En un informe de [!UICONTROL Initiative Job Role], se muestra el número de [!UICONTROL Planned Hours] asociadas con una función asignada a tareas o problemas del proyecto. Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no se muestran en la instancia de [!DNL Workfront] a menos que su empresa haya adquirido una licencia de [!DNL Workfront Scenario Planner]. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Información general sobre [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>Los detalles del estado actual de un proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> Es el [!UICONTROL Budgeted Cost] de un proyecto tal como se muestra en listas e informes.</p><p>Consulte también “[!UICONTROL Budgeted Cost]” en este artículo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Conjunto de políticas que rige los umbrales para la creación, categorización y denominación de proyectos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>En un informe de [!UICONTROL Hour], este campo se reserva para la información financiera vinculada a las horas registradas con el tipo de hora de [!UICONTROL Project Time]. Los proyectos pueden tener sus propias Tarifas de facturación y si se registra una hora directamente en un proyecto, dichas tarifas se utilizarán en los cálculos. En función de la configuración del proyecto, los proyectos también pueden tener distintas monedas y puede haber una conversión de moneda para esas horas. El objeto [!UICONTROL Project Overhead] permite que [!DNL Workfront] obtenga dicha información.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>Usuario responsable de administrar el ámbito, la línea de tiempo y las asignaciones de un proyecto. Aprobador predeterminado para cambiar pedidos, cambios financieros y entregas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Procesos para desarrollar y mantener la programación del proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>Un perfil de responsable del departamento designado con el que debe relacionarse cada uno de sus usuarios. En [!DNL Workfront], se designan como [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>Colección de usuarios o funciones asignados a un proyecto</p> <p>Para más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Información general del equipo del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>Los datos utilizados para medir el estado y el alcance de un proyecto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>Una estimación de la marca de tiempo del momento en que se completará el trabajo en función de las horas planificadas y el porcentaje completado de una tarea, problema o proyecto.</p> <p>Hace referencia a fechas o a la [!UICONTROL Duration] de las tareas, problemas o proyectos. Normalmente, designa fechas y duraciones que se ajustan más a la vida útil de los elementos de trabajo, después de que ya se haya completado algún trabajo o haya transcurrido algún tiempo. </p> <p>Por ejemplo, la [!UICONTROL Projected Completion Date] de una tarea es la fecha en la que [!DNL Workfront] calcula que la tarea se completará, en función de cuánto trabajo se haya realizado en ella hasta el momento, cuántas personas están asignadas a ella y cuánto tiempo ha pasado desde la fecha de inicio.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe de [!UICONTROL Document Version] y un informe de [!UICONTROL Proof Approval]), este campo muestra el día de la semana, la fecha, la hora del día y el año de la fecha límite de la revisión.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe de [!UICONTROL Document Version]) y un informe de [!UICONTROL Proof Approval]), este campo muestra el estado de decisión de la revisión (pendiente, cambios necesarios o aprobado)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe de [!UICONTROL Document Version] y un informe de [!UICONTROL Proof Approval]), este campo muestra el nombre de la revisión.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe de [!UICONTROL Document Version] y un informe de [!UICONTROL Proof Approval]), este campo muestra el número de páginas incluidas en la prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe de [!UICONTROL Document Version] y un informe de [!UICONTROL Proof Approval]), muestra el estado de progreso de la revisión ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented] o [!UICONTROL Decision Made]).</p> <p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Información general sobre el progreso de la revisión</a> en <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Información general sobre el progreso y el estado de la revisión</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Proceso de revisión en el que uno o varios usuarios marcan y comentan contenido que debe cambiarse en una imagen, documento de texto, vídeo o contenido web interactivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>En una [!UICONTROL Note] o un [!UICONTROL Document], esta opción hace accesible ese objeto para otros usuarios o incluso para personas de fuera de [!DNL Workfront]. En el caso de una [!UICONTROL Help Request Queue], [!UICONTROL Public] significa que todos los usuarios que pueden enviar problemas a un proyecto pueden hacerlo a través del área [!UICONTROL Requests].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>La percepción de la calidad del trabajo dentro de la organización.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>También se denomina cola del servicio de asistencia [!UICONTROL Help Request Queue]. Este es un proyecto que se ha publicado en el área de [!UICONTROL Requests], a la que los usuarios pueden enviar problemas. Normalmente, las colas se crean para temas concretos, como [!UICONTROL Bugs], [!UICONTROL Project Requests], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>Esta configuración define las reglas de envío de problemas para un proyecto que se publica en el área de [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>Propiedad de una [!UICONTROL Help Request Queue] que permite a los usuarios que envían un problema seleccionar un tema. Los temas pueden:</p> 
    <ul> 
     <li>Asociarse a un formulario de datos personalizados.</li> 
     <li>Asignar el problema automáticamente a un usuario, una función o un equipo a través de la regla de enrutamiento establecida en el tema seleccionado.</li> 
     <li>Mover el problema a otro proyecto o cola a través de la regla de enrutamiento establecida en el tema seleccionado.</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crear temas de colas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>En un informe de [!UICONTROL Access Level] puede indicar manualmente un [!UICONTROL Rank] del [!UICONTROL Access Level]. Esto le ayuda, como administrador de [!DNL Workfront], a identificar visualmente el nivel de complejidad asociado a cada nivel de acceso. Por ejemplo, puede dar números más bajos para niveles de acceso más complejos (nivel de [!UICONTROL Plan]) y números más altos para niveles de acceso menos complejos (nivel de [!UICONTROL Requester]). No pueden clasificarse los niveles de acceso estándar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Este campo de un informe de tareas indica si una tarea de [!UICONTROL Agile] se ha marcado como [!UICONTROL Ready] en el registro de asuntos pendientes. Este indicador solo se aplica a las tareas de [!UICONTROL Agile], que son las tareas asignadas a un equipo de [!UICONTROL Agile]. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p>En Workfront Planning, un registro es una instancia única de un tipo de registro.</p>
<p>Después de añadir un tipo de registro a un espacio de trabajo, podrá empezar a añadir registros de ese tipo a la página del tipo de registro.</p>
<p>Por ejemplo, "Campaña" puede ser un tipo de registro y "Campaña de verano para EMEA" es un registro del tipo de registro Campaña.</p>
<p>Para obtener información sobre cómo crear registros, vea <a href="/help/quicksilver/planning/records/create-records.md">Crear registros</a>. </p> <p>Workfront Planning requiere una licencia adicional. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Record type]</td> 
   <td> <p>Tipo de objeto de Workfront Planning.</p>
<p>A diferencia de Workfront, donde los tipos de objeto están predefinidos, en Workfront Planning puede crear sus propios tipos de objeto. Los tipos de objeto de Workfront Planning se denominan tipos de registro.</p>
<p>Por ejemplo, en Workfront, los tipos de objeto Programa, Portafolios, Proyecto, Tarea o Problema ya están creados.</p>
<p>En Workfront Planning es posible crear cualquier tipo de registro que cumpla con los flujos de trabajo de la organización. Posteriormente, defina cómo se relacionarán los tipos de registro entre sí o las dependencias de formularios.</p> Para obtener información acerca de cómo crear tipos de registros, consulte <a href="/help/quicksilver/planning/architecture/create-record-types.md">Creación de tipos de registro</a>. </p> <p>Workfront Planning requiere una licencia adicional. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>Campo que se muestra en los [!UICONTROL Task Details] o la [!UICONTROL Edit Task] de un principal de tareas recurrentes. Es la frecuencia con la que se producen las tareas en la periodicidad. Para obtener información acerca de la creación de tareas recurrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Los proyectos, las tareas y los problemas se asocian automáticamente a un número de referencia único a medida que se crean. Puede ver el [!UICONTROL Reference Number] en la página de [!UICONTROL Details] de los proyectos, tareas o problemas, o en una lista o informe. </p> <p><b>Sugerencia</b><p><br>Se puede recurrir a los números de referencia cuando dos elementos tengan el mismo nombre, ya que los números de referencia son siempre únicos. </p> <p>[!DNL Workfront] genera automáticamente números de referencia secuenciales en el nivel de sistema. Cada proyecto, tarea o problema obtiene el siguiente número disponible en la secuencia. <br></p> <p>Por ejemplo, si el usuario A crea una tarea, [!DNL Workfront] podría asignar automáticamente a la tarea el número de referencia 100. Si el usuario B crea una incidencia justo después, [!DNL Workfront] asigna a la incidencia el número de referencia 101. No es posible editar manualmente los números de referencia. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>En un informe de proyecto o de tarea, es la incidencia que se crea cuando se rechaza la aprobación del proyecto o de la tarea. Para obtener información sobre problemas de rechazo, consulte el artículo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Crear un proceso de aprobación para los elementos de trabajo</a>. </td> 
  </tr>

<tr>
  <td>Tipos de relación</td>
  <td><p>Los objetos de Workfront siempre están conectados entre sí mediante uno de los siguientes tipos de relación:</p>

<ul><li> <b>Uno a varios</b>: en esta relación, un objeto se puede conectar a varios objetos de otros tipos. Por ejemplo, un proyecto puede tener varias tareas. La relación Proyecto-Tareas es una relación de uno a varios. No se puede mostrar esta relación en un informe mediante la interfaz estándar. Debe utilizar los informes de modo de texto para ver una o varias relaciones.</li>
  <li><b>Uno a uno</b>: en esta relación, un objeto solo puede conectarse a otro objeto de un tipo diferente. Por ejemplo, un proyecto solo puede tener un grupo. La relación Proyecto-Grupo es una relación uno a uno. En un informe estándar se pueden mostrar relaciones individualizadas entre objetos.</li>
  <li><b>Varios a uno</b>: en esta relación, varios objetos sólo se pueden conectar a otros objetos de otro tipo. Por ejemplo, se pueden conectar varias tareas al mismo proyecto. La relación entre tareas y proyectos es una relación de varios a uno. En un informe estándar se pueden mostrar las relaciones de varios a uno entre los objetos. </li>
  <li><b>Varios a varios</b>: en esta relación, se pueden conectar varios objetos del mismo tipo a varios objetos de un tipo diferente. Por ejemplo, varios usuarios pueden pertenecer a varios otros equipos y los equipos pueden pertenecer a varios usuarios. No se puede mostrar esta relación en un informe mediante la interfaz estándar. Debe utilizar los informes de modo de texto para ver de muchas a muchas relaciones. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>Campo del proyecto que muestra la diferencia entre el [!UICONTROL Planned Risk Cost] de un proyecto y el total de todos los [!UICONTROL Actual Costs] de todos los riesgos del proyecto. </p> <p>El [!UICONTROL Remaining Risk Cost] de un proyecto se calcula mediante la siguiente fórmula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>Cambiar las fechas de un proyecto para reparar o superar problemas. Por ejemplo, un proyecto que ha estado en espera durante varios meses tendría que volver a planificarse para reflejar las fechas precisas. Es una operación manual de ajustar las fechas del proyecto o las de las tareas. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Gráfico o tabla que contiene información sobre un determinado [!DNL Workfront] objeto y sus atributos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Tipo de incidencia que se clasifica en una cola única centralizada y no está relacionada con un trabajo en curso.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>La acumulación de problemas que se gestiona mediante un proceso de tráfico y triaje.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>Tiempo total del ciclo de trabajo para ingerir y completar una solicitud.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Normalmente es un tipo de licencia. Un usuario con una licencia de solicitante puede enviar solicitudes para que se produzcan nuevos trabajos en el sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>Días especificados en el horario personal de un usuario, lo que indica que el usuario no estará disponible para trabajar. Consulte "[!UICONTROL Non Work Days]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia al problema que resuelve el problema. </p> <p>Para obtener información sobre la visualización de objetos resolubles en informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información de objetos resolubles y resolubles en un informe</a> en <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Descripción general de objetos resolubles y resolubles </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia al proyecto que resuelve el problema. </p> <p>Para obtener información sobre cómo mostrar objetos de resolución en los informes, vea <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información sobre objetos que se pueden resolver y sobre cómo resolver información de un objeto en un informe</a> en <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre cómo resolver y resolver objetos que se pueden resolver </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia a la tarea que resuelve el problema. </p> <p>Para obtener información sobre cómo mostrar objetos de resolución en los informes, vea <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información sobre objetos que se pueden resolver y sobre cómo resolver información de un objeto en un informe</a> en <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre cómo resolver y resolver objetos que se pueden resolver </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Usuarios o funciones que existen en [!DNL Workfront] y que se han asignado a equipos, tareas y problemas del proyecto. Son responsables de completar el trabajo asociado con proyectos, tareas o problemas. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] es un conjunto de herramientas empresariales que le permite prever con precisión el uso de los recursos en función de su disponibilidad, de modo que el trabajo que debe realizarse se complete a tiempo y según el presupuesto. </p> <p>Con las herramientas de administración de recursos, puede planificar las necesidades de capacidad a largo plazo y de programación a corto plazo de sus recursos. </p> <p>Para obtener información acerca de la administración de recursos en [!DNL Workfront], vea <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introducción a la administración de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>En un informe de proyecto, puede utilizar esta opción al crear un filtro para buscar un administrador de recursos específico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>En un informe de proyecto o vista de lista, se trata de un campo informativo que muestra los usuarios designados para realizar actividades de administración de recursos en el proyecto.  Cuando se usa “[!UICONTROL Resource Managers]” en un informe, se muestra una lista de administradores de recursos, con cada uno de los administradores de recursos del proyecto separados con comas. Puede designar hasta 30 administradores de recursos en un proyecto determinado.</p> <p>Para obtener más información, vea el artículo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designar administradores de recursos para un proyecto o plantilla </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>Horas presupuestadas para el proyecto y recursos asociados con él en [!UICONTROL Resource Planner]. Consulte también “[!UICONTROL Budgeted Hours]” en este artículo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Herramienta avanzada [!DNL Workfront] que le permite ver y administrar recursos entre proyectos, funciones o usuarios. Para obtener más información, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resumen del Planificador de recursos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>Es el coste asociado con las horas presupuestadas para las funciones del proyecto que se usan en el Planificador de recursos. </p> <p>Consulte también “Coste laboral presupuestado” en este artículo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Los conjuntos de recursos son colecciones de usuarios que se pueden asociar a un proyecto. Los usuarios del mismo conjunto de recursos suelen pertenecer al mismo departamento, tener aptitudes similares o complementarias o estar financiados con cargo al mismo presupuesto. Puede asociar varios conjuntos de recursos a un proyecto o a un usuario. Un conjunto de recursos se puede asignar exclusivamente a un proyecto o compartir en varios proyectos.</p> 
   <p>Para obtener más información sobre los conjuntos de recursos, vea <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Información general sobre los conjuntos de recursos </a>.</p> 
   <p>En los informes de proyecto, los conjuntos de recursos muestran todos los conjuntos asociados a un proyecto. Este objeto no se puede utilizar en una agrupación.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Informe que muestra la cantidad de horas disponibles durante un período de tiempo determinado y la cantidad de horas programadas para cada usuario en el informe. Esto también se calcula en [!UICONTROL Average Hours Per Day] y un porcentaje de asignación.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>En [!DNL Workfront Goals], un resultado es un indicador de progreso para una meta. Puede ser un número, un valor porcentual o una cantidad de moneda que se actualiza manualmente. No puede mostrar los resultados en un informe y no puede acceder a ellos a través de la API [!DNL Workfront]. Para obtener información sobre las actividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introducción a los resultados y las actividades en Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Un importe facturable por la tarea o el proyecto. La cantidad puede ser por hora, fija o una combinación de ambas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>El tipo de ingresos determina cómo devengará ingresos la tarea. Algunos ejemplos son [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly], y [!UICONTROL Role Hourly w/Cap]. Para obtener información sobre el seguimiento de los ingresos en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Normalmente es un tipo de licencia. Un usuario con una licencia [!UICONTROL Reviewer] tiene la capacidad de revisar y aprobar elementos de trabajo en el sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Esto puede hacer referencia a los siguientes conceptos en [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Campo de un proyecto que indica lo riesgoso que puede ser un proyecto. Puede priorizar la ejecución de sus proyectos en función del nivel de riesgo. Los proyectos pueden tener los siguientes niveles de riesgo:</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>Los niveles de riesgo que indique para un proyecto no pueden personalizarse. </p> <p> Para obtener información sobre cómo actualizar el Riesgo de un proyecto, consulte la sección “Configuración del proyecto” del artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>. Puede visualizar el campo de riesgo de un proyecto en los informes. </p> </li> 
     <li> <p>Acontecimiento que puede producirse durante la vida de un proyecto y que identifica un impacto potencial en el coste, el alcance o el calendario del proyecto. Defina los riesgos potenciales para un proyecto y asocie una probabilidad de que se produzcan o un coste a medida que crea el caso comercial del proyecto. Para obtener información sobre cómo añadir riesgos al caso empresarial del proyecto, consulte "Crear y editar riesgos en proyectos". </p> <p>No se pueden mostrar los riesgos definidos en [!UICONTROL Business Case] en los informes. Solamente se pueden mostrar varios tipos de costos de riesgo en informes y listas. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>Coste asociado con los riesgos de un proyecto. A continuación se indican los costes de riesgo asociados a los proyectos que pueden visualizarse en los informes:</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]: campo de un riesgo que muestra el coste real del riesgo que se ha producido. Además de en informes y listas, puede localizarlo en el cuadro [!UICONTROL Edit Risk] al editar o crear un riesgo. </p> <p>Para los costes de proyectos, tareas o problemas, consulte “[!UICONTROL Actual Cost]” en este artículo. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: campo del proyecto que muestra un total de todos los [!UICONTROL Potential Risk Costs] del proyecto. Consulte también “[!UICONTROL Planned Risk Cost]” en este artículo. </p> <p>Para obtener información acerca del Costo de riesgo potencial, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular el coste potencial de riesgos </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]: campo del proyecto que muestra la diferencia entre el total de [!UICONTROL Actual Costs] de todos los riesgos y el [!UICONTROL Planned Risk Cost]. Consulte también “Coste restante de riesgos” en este artículo. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Procesos para identificar, mitigar y controlar los riesgos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Consulte “[!UICONTROL Job Role]” en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Asignar o mover automáticamente una incidencia, normalmente debido a un tema de cola o por ser la ruta predeterminada (regla de enrutamiento) de la cola.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>Un ajuste en proyectos y temas en cola que asigna automáticamente un problema a un usuario, rol o equipo, o mueve el problema a otro proyecto o tema en cola. Las reglas de enrutamiento se utilizan generalmente con colas de solicitudes de ayuda para asignar automáticamente problemas entrantes.</td> 
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
   <td>[!UICONTROL Saved Search]</td> 
   <td>Una búsqueda para la que se han guardado los criterios de búsqueda. Las búsquedas guardadas facilitan la ejecución de cada una de ellas sin tener que volver a introducir los criterios de búsqueda.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (en [!DNL Workfront Fusion]) </td> 
   <td> <p>Un escenario consiste en una serie de pasos (módulos) que indican cómo se deben transferir y transformar los datos entre aplicaciones y servicios.</p> <p>Para obtener información acerca de los escenarios de [!DNL Workfront Fusion], consulte Información general sobre escenarios de <a href="https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (en el [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>En [!DNL Scenario Planner], un escenario es una copia de un plan. </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca del [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general sobre [!DNL Scenario Planner]</a>. </p> <p>Para obtener información acerca de cómo crear escenarios, consulte <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Crear y comparar escenarios de plan en [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>El horario de trabajo semanal, incluidos los tiempos de trabajo, combinado con los días libres (tales como días festivos) y los días de excepción (tales como un día laborable sábado). Puede asociar programaciones con proyectos y usuarios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>También se conoce como [!UICONTROL Modified Shift]. Días programados, en contraste con los tiempos de trabajo semanales normales definidos por la programación. Por ejemplo, un sábado programado para trabajar, cuando la programación está configurada para trabajar únicamente de lunes a viernes, sería una [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>Cuando se genera un informe de informes, se puede mostrar información sobre las programaciones del informe, si está programado para su envío, utilizando el campo [!UICONTROL Scheduled Report]. Este campo muestra varios valores, uno para cada programación de cada informe, en una lista con viñetas. Para obtener más información sobre la programación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Información general sobre la entrega de informes</a>.</p> <p>Dado que este campo muestra varios valores, no se puede utilizar en una agrupación. Solo puede acceder a él en un filtro o una vista. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>Un [!UICONTROL Audit Trail] que, si está activo, genera una nota cada vez que se realiza un cambio en el ámbito de un proyecto o tarea, como si se cambia una [!UICONTROL Task Duration] o los [!UICONTROL Predecessors].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Área de la pantalla, con su propio encabezado, creada para organizar los datos personalizados con fines de visualización.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>Un hueco o borde entre secciones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>Configuración que permite al usuario interactuar con determinados objetos del sistema y no con otros. Consulte también “[!UICONTROL Access Levels]” en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Área en la que los administradores pueden definir las configuraciones y preferencias del sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] es una indicación de la probabilidad de que un elemento afecte a la finalización del trabajo. Por ejemplo, un problema con una [!UICONTROL Severity] alta puede bloquear por completo la finalización de una tarea, pero un problema con una [!UICONTROL Severity] baja puede ser meramente superficial.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Actualizar gravedad del problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Consulte “[!UICONTROL Severity]” en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Acción de permitir que otros usuarios vean o editen un elemento específico en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>En una vista de tareas o informe, [!UICONTROL Slack Date] muestra la fecha exacta en la que una tarea podría afectar definitivamente a la [!UICONTROL Completion Date] del proyecto. Para obtener información acerca de la [!UICONTROL Slack Date] de una tarea, consulte <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Información general sobre la fecha de margen de demora de una tarea</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>Al asignar tareas o problemas a los usuarios, [!DNL Workfront] hace recomendaciones ([!UICONTROL Smart Assignments]) sobre quiénes son los mejores usuarios para completar el trabajo, en función del tiempo que tengan disponible para completarlo y de su relación con el proyecto.</p> <p>Para más información, consulte <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Información general sobre las asignaciones inteligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indica el objeto principal de otro objeto. Por ejemplo, un documento adjunto a una tarea tiene el nombre de la tarea en el campo [!UICONTROL Source] de un informe o vista de [!UICONTROL Document]; un problema registrado en un proyecto tiene el nombre del proyecto en el campo [!UICONTROL Source] de un informe o vista del problema. </p> 
   <p>Los siguientes informes muestran una columna Source en la que puede ver información sobre el objeto principal:</p>
  <ul><li>Informes de problema</li>
    <li>Informes por hora</li>
    <li>Informes de documentos </li>
    </ul>
   <p>Si los usuarios no tienen permisos para el objeto principal de un problema, hora o documento, la columna Source del informe se muestra vacía, incluso cuando el informe está configurado para mostrarse o para entregarse con los derechos de acceso de otro usuario. </p>
   <p> Para mostrar información sobre el objeto principal en el informe, se recomienda añadir una columna para el objeto principal en la que se pueda mostrar el nombre del objeto principal. </p>
    <p>Por ejemplo, puede añadir cualquiera de las siguientes opciones a un informe con una columna Source: </p>
    <ul><li>Las columnas Nombre del proyecto, Nombre de tarea o Nombre del problema a un documento o informe de horas.</li>
    <li>Las columnas Nombre del proyecto o Nombre de tarea a un informe de problemas. </li> </ul>
    Para obtener más información, vea <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Ejecutar y enviar un informe con los derechos de acceso de otro usuario</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>La fecha en la que está establecido el inicio del trabajo en un elemento. Hay varias fechas de inicio en [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>En un [!UICONTROL Rate report], esta es la fecha en la que se inicia una nueva tasa de facturación para una función en el nivel de proyecto. Las horas asociadas con el proyecto que son posteriores a esta fecha se multiplican por esta tarifa de facturación para calcular los ingresos del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Indicador utilizado para indicar la posición del flujo de trabajo de un elemento de trabajo o de una meta estratégica.</p> <p>Para los proyectos, [!UICONTROL Status] es una configuración del proyecto que indica si el proyecto está:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Para obtener más información sobre el estado de un proyecto, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Acceso a la lista de estados de proyectos del sistema</a>.</p>
    <p>Para las tareas, [!UICONTROL Status] es una configuración de la tarea que indica si la tarea es:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Para obtener más información sobre el estado de la tarea, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Acceso a la lista de estados de tareas del sistema</a></p> <p>En el caso de los problemas, [!UICONTROL Status] es una configuración del problema que indica si este problema está:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>Para obtener más información sobre los estados de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceso a la lista de estados de problemas del sistema</a>.</p> 
    <p>Para las metas estratégicas, el [!UICONTROL Status] es una configuración de la meta que indica si la meta está:</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>Para obtener más información acerca de las metas estratégicas, consulte “[!UICONTROL Goal]” o “[!UICONTROL Goals]” en este artículo. </p> 
     <p>Para las metas estratégicas, este campo solo está visible si su organización ha comprado [!DNL Workfront Goals]. Para obtener información acerca de la administración de metas estratégicas mediante [!DNL Workfront Goals], vea <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]Información general</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>Un [!UICONTROL Audit Trail]. Se genera una nota cuando un usuario cambia el estado del proyecto, tarea o problema.</td> 
  </tr> 
  <tr> 
   <td>Iconos de estado</td> 
   <td> <p>Puede añadir el campo integrado [!UICONTROL Status Icons] como una columna en las vistas para mejorar la visibilidad de los puntos clave sobre los objetos, como:</p> 
    <ul> 
     <li>Un objeto tiene documentos adjuntos</li> 
     <li>Un objeto está asociado a un proceso de aprobación</li> 
     <li>Un objeto tiene notas adicionales asociadas</li> 
     <li>Un gasto es facturable o reembolsable </li> 
     <li>Una tarea se encuentra en una ruta crítica</li> 
     <li>Un usuario pertenece a una empresa, a un equipo o está ubicado en una zona horaria diferente </li> 
    </ul> <p>Puede añadir el campo [!UICONTROL Status Icons] en las vistas de los objetos siguientes: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en las vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>En un informe de proyecto, tarea o problema, este campo muestra la actualización de estado más reciente que los propietarios de objetos han proporcionado en el área “[!UICONTROL Updates]”. En el caso de los proyectos, esto significa que los comentarios realizados por el Propietario del proyecto, así como las tareas y problemas, significan que los comentarios realizados por los usuarios asignados.</p> 
   <p> Los comentarios realizados al actualizar el estado de un objeto no se muestran en la columna [!UICONTROL Status Update].</p> <p>Para mostrar los estados “[!UICONTROL New]”, “[!UICONTROL In Process]” y “[!UICONTROL Complete]”, utilice la columna “[!UICONTROL Status]”.</p> <p>Para obtener más información sobre los estados, consulte el artículo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Actualizar el estado de una tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Consulte “[!UICONTROL Status]” en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Un gráfico que representa el estado de las historias (tareas en la metodología ágil) y cómo progresan hacia su finalización.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Métrica utilizada para medir la dificultad o complejidad de una historia. Los equipos ágiles pueden elegir si desean utilizar horas o puntos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Métrica utilizada para medir la dificultad o complejidad de una historia. Los equipos ágiles pueden elegir si desean utilizar horas o puntos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Un trabajo a largo plazo que cambia la organización o cómo funciona la organización.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>Medir y alinear las metas de la compañía en portafolios y programas.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Se utiliza en las columnas del informe al utilizar la interfaz de modo de texto. </p>
   <p>El <code>[!UICONTROL stretch]</code> se utiliza para identificar qué columnas ocupan espacio extra que no necesita la vista. La anchura de la interfaz de usuario del espacio de trabajo de un usuario típico es de unos 850 píxeles. Esto significa que si tiene una vista con cuatro
  columnas (150 píxeles cada una) que la vista ocupa 600 de 850 píxeles. Hay 250 píxeles adicionales en la interfaz de usuario que se añadirán a las columnas que tengan un porcentaje de ampliación proporcionado. </p>
   <p>La ampliación de una columna se impone cuando se utiliza la línea de código adicional: <code>[!UICONTROL usewidths=true]</code> para al menos una de las columnas de la vista. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Usuarios que se suscriben a proyectos, tareas o problemas.</p> <p>Cuando se utiliza este campo en un informe, se muestra una lista de suscriptores, cada uno de los cuales está separado por una coma.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Suscribirse a elementos en [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>Consulte “[!UICONTROL Parent Task]” en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>Una tarea secundaria, que se encuentra debajo de una tarea principal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Conjunto de directivas que rigen los cambios y el mantenimiento de un sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>Proceso de conexión física o funcional de diferentes sistemas informáticos y aplicaciones de software para que actúen como un todo coordinado.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Una actividad que debe realizarse como paso hacia el logro de un objetivo final (completar el proyecto).</p>

<p>Las tareas son unidades de trabajo más pequeñas que finalmente completan un proyecto, lo que representa una unidad de trabajo más grande.</p>
   <p>Las tareas nunca pueden existir de forma independiente. Siempre son parte de un proyecto. </p>
   <p>Para obtener más información acerca de las tareas, vea <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Información general sobre tareas</a>.</p> 
   <p>Para obtener información acerca de cómo crear tareas, vea <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md">Crear tareas en un proyecto</a>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Otros campos u objetos asociados a una tarea e indican determinados detalles sobre la tarea. Algunos ejemplos son[!UICONTROL Planned Completion Date] y [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Consulte “[!UICONTROL Constraint Type]” y “[!UICONTROL Constraint Date]”.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>Conjunto de políticas que rigen los umbrales de creación, asignación, cierre y visibilidad de tareas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>El equipo o usuario responsable de la estimación del esfuerzo y la finalización de la tarea</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Una colección de usuarios que trabajan para lograr metas u objetivos comerciales similares. Estos usuarios se pueden asignar colectivamente a un elemento de trabajo asignando al equipo dicho elemento de trabajo.</p> <p>Para obtener más información sobre Teams, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Información general sobre Teams</a>.</p> <p>Los proyectos pueden tener un [!UICONTROL Project Team], que contiene todos los usuarios o roles asociados con el trabajo en el proyecto.</p> <p>Para obtener más información sobre los equipos del proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Las plantillas de proyecto son descripciones genéricas de los proyectos más repetibles. Puede definir tareas, temas de colas, formularios personalizados, adjuntar documentos o aprobaciones cuando cree una plantilla de proyecto para ahorrar tiempo cuando deba crear un nuevo proyecto. </p> <p>Puede adjuntar plantillas a proyectos existentes o puede utilizarlas para crear nuevos proyectos. Toda la información especificada en la plantilla se transfiere a los proyectos creados con ella. </p> <p>Para obtener más información sobre las plantillas, consulte <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Descripción general de la plantilla del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Una tarea que forma parte de una plantilla. Las tareas de la plantilla se convierten en Tareas en el proyecto que se crea mediante la plantilla.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Una [!UICONTROL Note] y su colección de respuestas relacionadas con un tema en particular.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> En una lista o informe de [!UICONTROL Document], muestra una vista previa del documento en una miniatura. </p> <p> Seleccione <strong>[!UICONTROL Thumbnail]</strong> para ver una miniatura de entre 33 y 66 píxeles de ancho en el informe. </p> <p>El tamaño de la miniatura se ajusta al modificar el ancho de la columna en una lista o informe.</p> <p>Consulte también “[!UICONTROL Large Thumbnail]” en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Puede generar un informe de [!UICONTROL Time Off] para ver cuándo los usuarios han indicado días libres en su perfil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Informe de tiempo que permite a los usuarios especificar las horas reales que han dedicado a trabajar en proyectos, tareas o problemas, o las horas que han dedicado a otras actividades no relacionadas con el trabajo, como reuniones o formación. Además de especificar la cantidad de tiempo que ha dedicado a trabajar, también puede indicar si el tiempo está relacionado con el trabajo o si equivale a tiempo general utilizando Tipos de horas para definir los registros de tiempo. Para obtener información sobre las hojas de horas, consulte <a href="../../../timesheets/timesheets/timesheets-overview.md">Información general de hojas de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>Un [!UICONTROL Timesheet Profile] es una plantilla que [!DNL Workfront] utiliza para crear automáticamente plantillas de horas para los usuarios asociados con ellos. </p> <p>Puede configurar una serie de opciones que se aplicarán a cada plantilla de horas a medida que se cree. Algunas de estas configuraciones son: la frecuencia con la que se debe crear la plantilla de horas (semanal, cada dos semanas, dos veces al mes o mensualmente), el día de inicio de la plantilla de horas, los aprobadores de la plantilla de horas, los [!UICONTROL Hour Types] disponibles que los usuarios pueden asociar con las horas registradas.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>Este campo permite identificar y filtrar datos sobre un grupo de nivel superior y sus subgrupos en una lista o informe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>Este campo permite identificar datos sobre un grupo de nivel superior y sus subgrupos en una [!UICONTROL View] para una lista o informe.</p> <p>También puede hacerlo utilizando el campo [!UICONTROL Top Parent ID].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>En un informe de proyecto de [!UICONTROL project report], este campo muestra la suma redondeada de todas las horas del proyecto la última vez que se calcularon las finanzas del proyecto. [!UICONTROL Actual Hours] reflejan las horas exactas registradas en el proyecto. Normalmente, [!UICONTROL Actual Hours] debe coincidir con [!UICONTROL Total Hours].  Si [!UICONTROL Total Hours] aparece de forma significativamente diferente al campo [!UICONTROL Actual Hours], debe recalcular las finanzas en el proyecto.</p> <p>Para obtener más información acerca de cómo recalcular las finanzas del proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalcular las finanzas del proyecto</a>.</p> <p>En una vista de plantilla de horas [!UICONTROL Standard], este campo hace referencia a las horas totales registradas para los elementos de las fechas mostradas en una plantilla de horas. El campo [!UICONTROL Total Hours] para las plantillas de horas en esta vista integrada hace referencia al campo “[!UICONTROL hoursDuration]” que calcula dinámicamente la diferencia en horas entre las fechas de inicio y finalización de la plantilla de horas. Se utiliza para mostrar en rojo la columna [!UICONTROL Total Hours] si el usuario registra más tiempo que las horas disponibles en el lapso de tiempo de la plantilla de horas. Para obtener más información, consulte <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Ver total de horas en la plantilla de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>Atributo de una tarea. Determina cómo y cuándo se actualizarán los plazos proyectados para una tarea. Por ejemplo:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] requiere que una tarea se actualice manualmente. De lo contrario, pasará a ser [!UICONTROL Behind Schedule] y, a continuación, [!UICONTROL Late].</li> 
     <li>[!UICONTROL Auto Complete] completará automáticamente una tarea cuando haya pasado la fecha de vencimiento o [!UICONTROL Planned Completion Date].</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Información general sobre el modo de seguimiento de tareas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Un evento que inicia un escenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Tarea incompleta con una condición de [!UICONTROL Late], [!UICONTROL Behind Schedule] o [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>Una tarea que no está asignada a ningún usuario, rol o equipo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>Un ajuste en un proyecto que determina cuándo se recalculará el plazo proyectado del proyecto. El [!UICONTROL Update Type] puede tener los valores siguientes:</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccionar el tipo de actualización del proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Cuenta creada en [!DNL Workfront] para permitir que una persona inicie sesión e interactúe con el sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Objeto de informe que le indica:</p> 
    <ul> 
     <li>Usuarios que han delegado aprobaciones de tareas, problemas y proyectos</li> 
     <li>Usuarios que han tenido delegadas aprobaciones de tareas, problemas y proyectos</li> 
     <li>Cuando estas delegaciones comienzan y finalizan</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Crear un informe de delegación de usuario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>Todos los aspectos visuales e interactivos de la aplicación [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. [!DNL Workfront] administradores pueden cambiar esta configuración para personalizar aspectos de la interfaz de usuario.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>La disponibilidad de un usuario o rol en función de la programación asignada, el tiempo de espera y la carga de trabajo actual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>Una búsqueda combinada con un informe que muestra cómo los usuarios (recursos) están asignados o sobreasignados. Consulte “[!UICONTROL Resource Utilization]” en este artículo.</p> </td> 
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
   <td>Una medida del tiempo total del ciclo de trabajo (cuánto tiempo se tarda en completar un trabajo) y con qué frecuencia se realiza el trabajo en el tiempo comprometido originalmente (ratio trabajo-comprometido).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Las vistas hacen referencia a un elemento de informes que le permite modificar las columnas de un informe o de una lista de objetos.</p> 
   <p> Ver también se refiere al derecho de un usuario a ver únicamente información sobre un objeto, según su nivel de acceso o a un nivel de compartición de permisos sobre ese objeto.</p> 
   <p>En Workfront Planning, los registros se muestran en la página de tipo de registro en uno de los siguientes tipos de vista:</p>
   <ul><li>Tabla</li>
   <li>Cronología</li>
   <li>Calendario</li></ul>
   <p>En Workfront Planning, las vistas incluyen los filtros, agrupaciones, ordenación y otras opciones de configuración aplicadas a los registros de la pantalla.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/views/manage-record-views.md">Administrar vistas de registros</a>.</p>   
   <p>Workfront Planning requiere una licencia adicional.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> Es el mismo campo que iconos de estado, pero solamente está disponible para las siguientes vistas: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Para obtener más información, consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en las vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>En una lista de informes, muestra el número de veces que se ha visto el informe durante el último mes.<br>Para obtener más información acerca de la información de uso en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>En una lista de informes, muestra el número de veces que el informe se ha visto durante el último trimestre.<br>Para obtener más información acerca de la información de uso en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante el último año.<br>Para obtener más información acerca de la información de uso en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>En una lista de informes, muestra el número de veces que se ha visto el informe durante este mes.<br>Para obtener más información acerca de la información de uso en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>En una lista de informes, muestra el número de veces que el informe se ha visto durante este trimestre.<br>Para obtener más información acerca de la información de uso en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante este año.<br>Para obtener más información acerca de la información de uso en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Ver uso del informe</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> En un informe, cuando se utiliza la interfaz [!UICONTROL Text Mode], la línea de código en la que se puede especificar el ancho de cada columna en píxeles. Workfront proporciona una anchura sugerida para cada campo,
aunque, según el tipo de campo y el formato, es posible que desee realizar ajustes.
Debe utilizar la línea de código <code>[!UICONTROL usewidths=true]</code> adicional para aplicar el ancho especificado para la columna. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>En un informe de proyecto, tarea o problema, el uso de la siguiente instrucción en modo de texto muestra las horas planificadas del proyecto, tarea o problema:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Para obtener información acerca del uso del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Información general sobre sintaxis del modo de texto</a>. </p> 
   <p><b>SUGERENCIA</b> 
   <p>En un informe de problemas, al añadir uno de los campos [!UICONTROL Planned Hours], se añade el campo <code>work </code>al informe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>Uno de los dos tipos de licencia principales. Tiene menos acceso que [!UICONTROL Plan], pero puede crear y realizar actualizaciones en el sistema. Un usuario con una licencia de Trabajo tiene más habilidades que un titular de una licencia [!UICONTROL External], [!UICONTROL Reviewer] o [!UICONTROL Requester].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] glosario de licencias</a>.</p> <p>Trabajo puede hacer referencia al número de [!UICONTROL Planned Hours] de un proyecto, tarea o problema. Para obtener más información, consulte el campo “[!UICONTROL work]” en esta tabla. </p> <p><b>Sugerencia</b></p> <p> En un informe de problemas, al añadir uno de los campos [!UICONTROL Planned Hours], se añade el campo <code>work </code> al informe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>Estructura jerárquica de las tareas que va a ejecutar el equipo del proyecto en función de la relación principal/secundario.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>Un jefe de proyecto puede decidir utilizar este campo en lugar de [!UICONTROL Planned Hours] para estimar el esfuerzo necesario para completar una tarea. Este campo solo está visible cuando se cumplen las siguientes condiciones:</p> 
     <ul> 
      <li> <p>La tarea tiene un [!UICONTROL Simple Duration Type]. </p> <p><b>Sugerencia</b></p> <p> Si actualiza la tarea [!UICONTROL Duration Type] a cualquier otro tipo, este campo se oculta. </p> </li> 
      <li>El jefe de proyecto ha activado el campo [!UICONTROL Use Work Effort] para calcular automáticamente la tarea [!UICONTROL Planned Hours] en el proyecto. </li> 
     </ul> 
     <p>Para obtener información sobre el uso de [!UICONTROL Work Effort] en lugar de [!UICONTROL Planned Hours] para estimar el esfuerzo de la tarea, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Información general del esfuerzo de trabajo</a>. </p> 
     <p>Puede mostrar este campo en informes de tareas y listas.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>Este campo hace referencia a tareas o problemas de [!DNL Workfront]. </p> <p>El informe [!UICONTROL Work Item] muestra información sobre tareas y problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>Un [!UICONTROL Work Performance Indicator] (WPI) de la proporción de trabajo asignado para ejecutar su negocio frente a cambiar su negocio. El Mix WPI le ayuda a comprender, a nivel organizativo, si su estrategia tiene alguna asignación de trabajo real aplicada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Una designación de un personaje en el sistema que es elegible para recibir trabajo o rastrear tiempo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Role and Responsibilities]</td> 
   <td>Definir los propietarios y las partes interesadas para gestionar el alcance, la ejecución y las aprobaciones del asunto, la tarea, el proyecto, el programa o la cartera designados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>Una métrica cuantificable acordada por todas las partes interesadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>Colección de usuarios con un interés creado en los resultados de una solicitud de trabajo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management touchpoints]</td> 
   <td>Registros digitalizados de la comunicación entre las partes interesadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>Relación de mezcla, capacidad, velocidad, calidad y participación.</p> <p>WPI es un acrónimo común de [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>Método en el que se recibe, se prioriza y se ejecuta el trabajo. La forma de ejecutar el trabajo suele denominarse “flujo de trabajo” o “plan de proyecto” (una lista de tareas con fechas, relaciones de predecesoras, etc.). </p> <p>Un proceso de trabajo puede ser, por ejemplo, la producción de un único activo o la entrega de una campaña de varios activos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>En el informe [!UICONTROL Proof Approval], este campo muestra todas las plantillas de flujo de trabajo adjuntas a una prueba. Si no hay plantillas adjuntas, la columna está en blanco.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>Representa el porcentaje del tiempo equivalente a tiempo completo ([!UICONTROL FTE]) que el usuario está disponible para el trabajo real, sin incluir los gastos generales. [!UICONTROL Work Time] debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.</p>
   </p>El valor predeterminado del campo es 1, lo que indica que un usuario gasta todo su [!UICONTROL FTE] en trabajo real relacionado con el proyecto.  </p>
   <p>El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto. </p>
   <p> Las excepciones de horario y los días libres también pueden afectar a la capacidad del usuario. </p>
   <p>Para obtener más información acerca de cómo crear programaciones en Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear programación</a>. </p>
    <p>Workfront calcula la disponibilidad de un usuario en función de las preferencias de administración de recursos del área [!UICONTROL Setup]. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurar preferencias de administración de recursos</a>. </p> 
   <p>Puede actualizar el [!UICONTROL Work Time] de un usuario cuando edite o cree el usuario. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Editar el perfil de un usuario</a></p> 
   <b>SUGERENCIA</b> 
   <p>Establezca el valor de [!UICONTROL Work Time] en 1 para indicar que el usuario está disponible para el trabajo relacionado con el proyecto en su equivalente a tiempo completo.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>En la documentación de Workfront, este término se utiliza para describir el tiempo asignado al trabajo, de acuerdo con una programación.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>En un informe de proyecto, tarea o problema, el uso de la siguiente instrucción en modo de texto muestra el número de horas planificadas del proyecto, tarea o problema seguido de la palabra “Horas”:</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Para obtener información acerca del uso del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Información general sobre la sintaxis del modo de texto</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Workspace] </td> 
   <td> <p>En Workfront Planning, un espacio de trabajo es una colección de tipos de registros que definen el ciclo de vida operativo de una determinada organización. Un espacio de trabajo es el marco de trabajo de una unidad organizativa.</p>
   <p>Workfront Planning requiere una licencia adicional. </p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Crear espacios de trabajo</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


