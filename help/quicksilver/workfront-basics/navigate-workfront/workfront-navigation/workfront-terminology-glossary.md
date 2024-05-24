---
content-type: reference
navigation-topic: workfront-navigation
title: Glosario de [!DNL Adobe Workfront] terminología
description: El [!DNL Adobe Workfront] El glosario enumera los términos más utilizados en [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] interfaz, informes o intenta comprender el significado de [!DNL Workfront] conceptos definidos en la [!DNL Workfront] documentación.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 6371f6d19bfbad31c4564f9726f52e3ce394e516
workflow-type: tm+mt
source-wordcount: '20060'
ht-degree: 0%

---


# Glosario de [!DNL Adobe Workfront] terminología

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Este artículo debe utilizarse como referencia para comprender los términos que puede encontrar en la [!DNL Adobe Workfront] aplicación, en el [!DNL Workfront] o, en general, sobre la planificación y la gestión del trabajo. Actualmente estamos actualizando esta información y, como resultado, es posible que esta tabla no esté completa. Eliminaremos esta exención de responsabilidad cuando consideremos que esta información es exhaustiva.

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
   <td>Tarea incompleta en un proyecto actual en el que una tarea predecesora no impide trabajar y que no tiene una delimitación de tarea con una fecha planificada de inicio futura. En otras palabras, se puede trabajar en la actualidad.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Actividad]</td> 
   <td>Entrada [!DNL Workfront Goals], una actividad es un indicador de progreso para una meta. Puede ser una barra de progreso que actualice manualmente o un proyecto asociado con el objetivo. No puede mostrar las actividades en un informe y no puede acceder a ellas a través del [!DNL Workfront] API. Para obtener información sobre las actividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introducción a resultados y actividades en Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo real]</td> 
   <td> <p>En el caso de las tareas y los problemas, es el costo asociado con las horas reales registradas en relación con la tasa de costo por hora del recurso asignado a la tarea o el problema. Para los proyectos, este es un total de todos los [!UICONTROL Costos reales] de las tareas y problemas del proyecto. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de gasto real]</td> 
   <td> <p>Suma de [!UICONTROL Cantidades reales] para todos los gastos registrados de un proyecto o tarea.</p> <b>EJEMPLO </b>
   <p>Si crea un gasto para la Tarea 1 y especifica 600,00 $ en el campo [!UICONTROL Importe real], el [!UICONTROL Costo real de gasto] de esta tarea es 600,00 $. </p> 
   <p>Para un proyecto, [!DNL Workfront] utiliza la fórmula siguiente para calcular [!UICONTROL Costo de gasto real]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas reales]</td> 
   <td> <p>En un informe de proyecto, tarea o problema, [!UICONTROL Horas reales] es la suma de todas las horas registradas en el proyecto, tarea o problema.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span> Si en la ficha [!UICONTROL Actualizaciones] de la Tarea 1 hace clic en 'Registrar tiempo' y especifica 25 horas, las horas reales de la Tarea 1 = 25 horas. </p> <p>[!DNL Workfront] calcula [!UICONTROL Horas reales] para tareas o proyectos principales mediante las fórmulas siguientes:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de mano de obra real]</td> 
   <td> <p>El [!UICONTROL Costo real] asociado a la mano de obra invertida en una tarea o proyecto. </p> <p>Para una tarea, [!DNL Workfront] calcula el [!UICONTROL Costo real de mano de obra] mediante la fórmula siguiente:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Si la tarea tiene un [!UICONTROL Tipo de costo] de [!UICONTROL Usuario por hora], [!DNL Workfront] utiliza la tasa de usuario. Si la tarea tiene un [!UICONTROL Tipo de costo] de [!UICONTROL Rol por hora], [!DNL Workfront] utiliza la tasa de rol para calcular [!UICONTROL Coste laboral real]. </p> <p>Para un proyecto, [!DNL Workfront] utiliza la fórmula siguiente para calcular el [!UICONTROL Costo de mano de obra real]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Por ejemplo, si un usuario registra 5 horas para una tarea con un [!UICONTROL Usuario por hora] [!UICONTROL Tipo de costo] y su tarifa por hora es de 100 $, el [!UICONTROL Costo de mano de obra real] es de 500 $.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ingresos reales] </td> 
   <td> <p>Los [!UICONTROL Ingresos reales] de un proyecto o una tarea son la cantidad de dinero asociada con las [!UICONTROL Horas reales] del proyecto o la tarea. </p> <p>Para obtener información sobre el seguimiento de ingresos en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Resumen de facturación e ingresos</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Inicio real]</td> 
   <td>La marca de tiempo cuando un usuario cambia un objeto en curso en el trabajo asignado a él.</td> 
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
   <td>Un tipo de metodología basada en la evolución colaborativa de las necesidades y soluciones con equipos interfuncionales. Fomenta la flexibilidad y el cambio en función de un calendario fijo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Equipo Agile]</td> 
   <td>Se diferencia de un equipo tradicional porque toma su trabajo potencial de un registro de pendientes y trabaja en él en un período de tiempo establecido que se denomina iteración [!UICONTROL].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Todos mis equipos]</td> 
   <td> <p>Cuando se hace referencia a esto en [!UICONTROL filters], este campo muestra los usuarios que pertenecen a cualquiera de los equipos a los que pertenece el usuario que ha iniciado sesión o los elementos de trabajo asignados a cualquiera de los equipos a los que pertenece el usuario que ha iniciado sesión. </p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, solo puede generar un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de asignación]</td> 
   <td> <p>Puede encontrar este campo en los siguientes tipos de informes:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Proyecto] (Datos financieros)</li> 
     <li>[!UICONTROL Hora presupuestada]</li> 
    </ul> <p>Para un<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->Informe de [!UICONTROL Project (Financial Data)]: </p> 
    <ul> 
     <li>Genere este informe cuando trate de comprender <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> Cantidad de [!UICONTROL Horas planificadas] asignadas a los recursos.</li> 
     <li> <p>La [!UICONTROL Fecha de asignación] es el primer día (domingo) de una semana en que se inicia la asignación de una [!UICONTROL Función del trabajo] a una tarea. Un recurso ([!UICONTROL Función del trabajo]) puede tener tantas [!UICONTROL Fechas de asignación] como semanas durante la [!UICONTROL Duración] de las tareas a las que está asignado. Si las tareas se extienden durante varios meses, el primer día de un mes también puede convertirse en una [!UICONTROL Fecha de asignación] si se encuentra dentro de la [!UICONTROL Duración] de la tarea.</p> <p>Por ejemplo, puede tener un [!UICONTROL Rol] asignado a una tarea que dure más de 3 semanas y tenga 90 [!UICONTROL Horas planificadas]. Estas horas se distribuyen uniformemente durante la duración de la tarea, lo que hace que cada día asigne 6 [!UICONTROL Horas planificadas] a su rol:</p> <p><em> [!UICONTROL Horas planificadas diariamente] = [!UICONTROL Total de horas planificadas]/ Número de [!UICONTROL Días laborables] durante la [!UICONTROL Duración] de la tarea </em> </p> <p>Como resultado, hay tres [!UICONTROL Fechas de asignación], una para cada domingo de cada semana durante la [!UICONTROL Duración] de la tarea, cada una con un determinado número de [!UICONTROL Horas planificadas] asociadas a ellas.<br>Si la tarea comienza a mitad de la última semana de un mes y finaliza dos semanas después del comienzo de un nuevo mes, la tarea tendrá cuatro [!UICONTROL Fechas de asignación]: una por cada domingo de cada semana durante la [!UICONTROL Duración] de la tarea y otra por el primer día del nuevo mes.</p> <p>Para aprovechar al máximo esta información, le recomendamos que cree un <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Informe de proyecto (datos financieros) y agregue una agrupación de matriz para [!UICONTROL Fecha de asignación]. A continuación, agrupe los resultados semanalmente, mensualmente, trimestralmente o anualmente para obtener los datos más precisos.<br>Para obtener información sobre cómo crear una agrupación de matriz, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Creación de un informe de matriz</a>.</p> </li> 
    </ul> <p>La información financiera se rellena en los informes de [!UICONTROL Project (Financial Data)] sólo cuando los datos asociados a ella tienen menos de 5 años. Por ejemplo, si un rol se asignó a una tarea en enero de 2015 y hoy es septiembre de 2021, un campo financiero como la [!UICONTROL Fecha de asignación] para el rol no se rellena en el informe [!UICONTROL Proyecto (datos financieros)]. </p> 
    <div> 
     <p>Para un informe de [!UICONTROL Hora presupuestada]:</p> 
     <ul> 
      <li>Genere este informe cuando trate de comprender la cantidad de [!UICONTROL Horas presupuestadas] que se asigna a sus recursos o a sus proyectos en el Planificador de recursos.</li> 
      <li> <p>La [!UICONTROL Fecha de asignación] es el primer día (un domingo) de la semana para el que se presupuestaron las horas en el [!UICONTROL Planificador de recursos]. </p> <p><b>SUGERENCIA</b></p> <p>Si una semana abarca dos meses, se generan dos filas en el informe: una correspondiente al primer día de la semana (domingo de la primera semana, que es durante el primer mes) y la segunda fila muestra el primer día del segundo mes. </p> <p>Por ejemplo, si asigna un presupuesto de 8 horas a un usuario para la semana del 30 de junio (domingo) al 6 de julio (sábado), las dos filas mostrarán una [!UICONTROL Fecha de asignación] del 30 de junio y del 1 de julio. </p> </p> <p>Para obtener información sobre cómo presupuestar recursos en la [!DNL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de presupuesto en [!DNL Resource Planner] uso de las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>.</p> <p>Para obtener información acerca de cómo generar un informe de [!UICONTROL Hora presupuestada], consulte <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Informe: Horas presupuestadas</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anuncios]</td> 
   <td> <p>Una forma de comunicar a los usuarios información dentro del sistema. Esta información procede a menudo de [!DNL Workfront] al administrador o del administrador al usuario. </p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Envío de anuncios</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Integración de aplicaciones]</td> 
   <td>Normalmente, una aplicación representa un conector para una aplicación de software, pero también puede representar funciones especiales que manipulan datos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisión de aprobador]</td> 
   <td> <p>En el informe [!UICONTROL Proof Approval], este campo muestra las decisiones de aprobación de pruebas para pruebas que ya no están activas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fase del aprobador]</td> 
   <td>En el informe [!UICONTROL Proof Approval report], este campo muestra información sobre una fase actual de pruebas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprobación]</td> 
   <td> <p>Un elemento de trabajo determinado, como una tarea, un documento o una plantilla de horas, puede requerir que un supervisor u otro usuario firme el elemento de trabajo. Este proceso de desactivación se denomina aprobación. </p> <p>Para obtener más información, consulte <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Resumen del proceso de aprobación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de aprobación]</td> 
   <td>En el informe [!UICONTROL Proof Approval], este campo muestra la fecha de aprobación de una prueba.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aprobador]</td> 
   <td>Un usuario o rol que debe cerrar la sesión de un elemento de trabajo determinado o el usuario que aprueba las entradas de horas en las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignado a]</td> 
   <td> <p>En un informe de [!UICONTROL Tarea o Problema], este campo muestra el Propietario de la tarea o del problema o el [!UICONTROL Usuario principal asignado]. También puede filtrar o agrupar por este campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignación]</td> 
   <td>Usuario, rol o equipo asignado a un problema o tarea. Los proyectos, portafolios o programas no pueden tener asignaciones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignaciones]</td> 
   <td> <p>En un informe de [!UICONTROL Tarea] o [!UICONTROL Problema], este campo muestra una lista de todas las entidades (usuarios, roles, equipos) asignadas a la tarea o al problema. Puede filtrar por este campo utilizando los campos [!UICONTROL Asignación usuarios] y [!UICONTROL Asignación funciones]. Puede filtrar por el equipo asignado a la tarea o al problema mediante el campo Equipo. No se puede agrupar un informe por este campo.</p> <p>Los elementos de trabajo que se hayan colocado en la [!UICONTROL Papelera de reciclaje] seguirán mostrándose en algunos informes que hacen referencia al objeto [!UICONTROL Asignación] donde un [!DNL OR] se utiliza el modificador de filtro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Funciones de asignación]</td> 
   <td>
   <p>En un informe de [!UICONTROL Tarea] o [!UICONTROL Problema], este campo muestra información sobre las funciones del puesto asignadas a las tareas o problemas. Este campo muestra [!UICONTROL Primary Owners], así como otras funciones asignadas a tareas o problemas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado de asignación]</td> 
   <td> <p>En un informe de asignación, tarea o problema, [!UICONTROL Estado de asignación] muestra si los usuarios asignados a un elemento de trabajo han hecho clic en el botón [!UICONTROL Trabajar en ello] o en el botón [!UICONTROL Listo] para aceptar o completar el trabajo. Existen los siguientes [!UICONTROL Estados de asignación]:</p> 
    <ul> 
     <li><b>[!UICONTROL Solicitado]</b>: se ha asignado al usuario a la tarea o al problema, pero aún no ha hecho clic en el botón [!UICONTROL Trabajar en ello] para comenzar a trabajar en él.</li> 
     <li><b>[!UICONTROL Trabajando]</b>: el usuario ha hecho clic en el botón [!UICONTROL Trabajar en ello] y está trabajando en el elemento. </li> 
     <li><b>[!UICONTROL Listo]</b>: el usuario ha hecho clic en el botón [!UICONTROL Listo] y ha completado su trabajo en el elemento. </li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Información general sobre el botón [!UICONTROL Trabajar en ello] y [!UICONTROL Listo]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipos de asignación]</td> 
   <td>
   <p>En un informe de [!UICONTROL task] o [!UICONTROL issue], este campo muestra información sobre los equipos asignados a las tareas o problemas. El campo muestra [!UICONTROL Primary Owners], así como otros equipos asignados a tareas o problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuarios de asignación]</td> 
   <td>
   <p>En un informe de [!UICONTROL Tarea] o [!UICONTROL Problema], este campo muestra información sobre los usuarios asignados a las tareas o problemas. Este campo muestra [!UICONTROL Primary Owners], así como otros usuarios asignados a tareas o problemas. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo]</td> 
   <td>Un atributo es un rasgo de [!DNL Workfront] objeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Área de auditoría]</td> 
   <td> <p>Las auditorías son mensajes del sistema que registran una acción que se produjo en Workfront. Se registran los siguientes tipos de auditoría:</p> 
    <ul> 
     <li>[!UICONTROL Cambio de ámbito]</li> 
     <li>[!UICONTROL Acción de datos adjuntos]</li> 
     <li>[!UICONTROL Edición general]</li> 
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
   <td>Colección de notas generadas automáticamente por eventos que se supervisan a través de los cambios registrados ([!UICONTROL Audit Areas]). Cada nota registra quién realizó la acción, qué hizo y cuándo lo hizo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automático Y Al Cambiar]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Project Update]. Esto recalculará las escalas de tiempo Proyectado y Planificado del proyecto cuando se ejecute el proceso de recálculo nocturno y cuando se realice cualquier actualización del proyecto o de las tareas dentro del proyecto. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilidad</p></td> 
   <td> <p>Este término se utiliza en relación con la "disponibilidad de usuarios" o la "disponibilidad de recursos" y muestra la cantidad de tiempo que el recurso (usuario o función del puesto) está disponible para trabajar. </p> 
   <p>Workfront calcula la disponibilidad del usuario utilizando varios campos y en función de la configuración de las preferencias de Administración de recursos del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferencias de administración de recursos</a>. </p>
   <p>Para obtener más información sobre la disponibilidad de los recursos, consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introducción a la administración de recursos</a></p>
   Alternativamente, "capacidad" también se utiliza para hacer referencia a la disponibilidad de recursos. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Sólo automático]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Project Update]. Esto recalculará las escalas de tiempo Proyectadas y Planificadas cuando se ejecute el proceso de recálculo nocturno.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Trabajos "como de costumbre" que contribuyen a la consecución de los objetivos empresariales primarios diarios.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Registro de pendientes]</td> 
   <td>El área en un entorno ágil en el que se guardan nuevos problemas hasta que estén listos para trabajar.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Línea base]</td> 
   <td>Una fuente de datos para medir iteraciones en un entorno Agile.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Gasto facturable]</td> 
   <td> <p>Un gasto marcado como facturable al cliente. Puede ser un gasto planificado o un gasto real.</p> <p>Los campos Costo de gasto facturable planificado y Costo de gasto facturable real están disponibles para que los agregue a las vistas e informes. No aparecen en las páginas de detalles del proyecto o la tarea.</p>
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
   <td>[!UICONTROL Registro de facturación]</td> 
   <td> <p>Registra los ingresos, horas o gastos que se pueden facturar. Esta información se puede utilizar para crear facturas en un sistema de contabilidad externo.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Crear registros de facturación</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Estado del registro de facturación</td> 
   <td> <p>En un informe Registro de facturación u Hora, el estado de un registro de facturación indica si el registro de facturación se ha facturado o no. No puede eliminar un proyecto o editar el tiempo asociado con un registro de facturación Facturado. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crear registros de facturación</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Marca]</td> 
   <td><p>Proceso de personalización [!DNL Workfront] para dar a la interfaz una apariencia que refleje su empresa mediante el uso de sus colores y logotipos.</p><p><strong>NOTA</strong><br>Si su organización se ha incorporado a [!DNL Adobe Experience Cloud], la marca no está disponible.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rutas de exploración]</td> 
   <td> <p>El área en la parte superior de la página que muestra la ubicación jerárquica de la ubicación del usuario en la aplicación.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obtener más información, consulte <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Resumen de rutas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado del presupuesto]</td> 
   <td> <p>Este es un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado y el campo no se puede actualizar. </p> <p>Este campo muestra si el proyecto se ha agregado al [!UICONTROL Programador de capacidades] y si se ha completado el cálculo de presupuesto para él. El [!UICONTROL Programador de capacidades] se ha eliminado de [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL Fecha presupuestada de finalización]</td> 
   <td> <p>Este es un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado. Este campo no se puede actualizar. </p>
   <p> Este campo sigue visible en los informes y listas de [!UICONTROL proyecto] y [!UICONTROL tareas].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo presupuestado]</td>

<td> <p>Es el costo asociado con los recursos de presupuesto de un proyecto. </p>
   <p>El campo se muestra en las siguientes áreas de [!DNL Workfront] con los siguientes nombres:</p>
   <ul>
   <li><strong>[!UICONTROL Costo presupuestado]</strong>: en el panel [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Costo]</strong>: en las áreas de [!UICONTROL Utilización] al ver información por [!UICONTROL Coste]</li>
   <li><strong>[!UICONTROL Costo presupuestado de proyecto]</strong>: en listas e informes</li>
   </ul>   
    <p>El [!UICONTROL Costo presupuestado] del proyecto se calcula mediante la fórmula siguiente:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Para obtener más información acerca del cálculo de [!UICONTROL Costo presupuestado] y comprender los distintos nombres de este concepto en [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular costo presupuestado de proyecto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Horas presupuestadas]</td> 
   <td> <p>Horas presupuestadas para recursos del trabajo que deben completar en los proyectos. Este campo hace referencia a las horas presupuestadas en el área de [!UICONTROL Presupuestación de recursos] del [!UICONTROL Caso comercial] (o en el [!UICONTROL Planificador de recursos]) para el proyecto o para los recursos del proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender [!UICONTROL Costo de mano de obra presupuestado] y [!UICONTROL Horas presupuestadas] para proyectos</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Para obtener información sobre cómo presupuestar usuarios en la [!DNL Resource Planner], consulte el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Recursos de presupuesto en [!DNL Resource Planner] uso de las vistas [!UICONTROL Project] y [!UICONTROL Role]</a>. </p> 
    <p>Las horas presupuestadas en el área de [!UICONTROL Presupuestación de recursos] del [!UICONTROL Caso comercial] o el [!UICONTROL Planificador de recursos] se muestran en las siguientes áreas de [!DNL Workfront] y bajo los siguientes nombres:</p> 
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
        <td>Área de [!UICONTROL Presupuestación de recursos] del caso comercial de [!UICONTROL]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Planificador de recursos] visto por [!UICONTROL Horas]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas presupuestadas]</td> 
        <td> <p>Vista del informe de utilización [!UICONTROL Hours]</p> <p>Para obtener más información acerca del informe [!UICONTROL Utilización], vea el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Descripción general del informe [!UICONTROL Resource Utilization]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Horas]</td> 
        <td> <p>Informe de [!UICONTROL Hora presupuestada]</p><p>El objeto [!UICONTROL Hora presupuestada] del informe Hora presupuestada hace referencia a información relacionada con una herramienta de administración de recursos obsoleta. Sólo el botón "[!UICONTROL. Horas]" en este informe hace referencia a las horas presupuestadas en el área de [!UICONTROL Resource Planner] o [!UICONTROL Resource Budgeting] del caso comercial de [!UICONTROL] del proyecto. </p> <p>Para obtener más información sobre cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creación de un informe personalizado</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Horas presupuestadas del planificador de recursos] </td> 
        <td> <p>Encontrado en los siguientes informes:</p>
        <ul>
        <li>Informe de [!UICONTROL Project]
        <li>Informe de [!UICONTROL Project (Financial Data)]
        <li>Informe de [!UICONTROL Tarea]
        <li>Informe de [!UICONTROL Issue]
        <li>Informe de [!UICONTROL Hora presupuestada]</li>
        </ul>
         <p>Para obtener más información sobre cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creación de un informe personalizado</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Cualquier otra mención de [!UICONTROL Horas presupuestadas] en [!DNL Adobe Workfront] hace referencia a horas presupuestadas utilizando funciones obsoletas que se han eliminado de Workfront Son campos de sólo consulta y no se actualizan con la información actual cuando se utilizan las herramientas de presupuesto de recursos actuales. </p>
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
   <td>[!UICONTROL Costo de mano de obra presupuestado]</td> 
   <td> <p>Es el costo asociado con las horas que usted, como gerente de recursos, presupueste para sus roles de trabajo para el trabajo que necesitan completar en los proyectos. </p> <p>El [!UICONTROL Costo de mano de obra presupuestado] de un informe de proyecto se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Este campo puede hacer referencia a lo siguiente:</p> 
    <ul> 
     <li> <p>Costes laborales mostrados en el área de [!UICONTROL Presupuestación de recursos] del [!UICONTROL Caso comercial] o en el [!UICONTROL Planificador de recursos] asociados al coste de los roles de un proyecto. Para obtener información acerca del cálculo del [!UICONTROL Costo de mano de obra presupuestado], vea el artículo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Comprender el costo laboral presupuestado] y [!UICONTROL Horas presupuestadas] para proyectos</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Costes laborales mostrados en el área de [!UICONTROL Presupuestación de recursos] del [!UICONTROL Caso comercial] que reflejan los [!UICONTROL Costes de personas] estimados en una iniciativa vinculada al proyecto desde el [!DNL Scenario Planner] cuando utiliza el Scenario Planner para presupuestar los recursos del proyecto. Para obtener información sobre las iniciativas, consulte <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Información general sobre iniciativas en el Scenario Planner</a>. </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">El [!DNL Scenario Planner] descripción general</a>. </p> </li> 
     <p>Se muestra en las siguientes áreas de bajo los siguientes nombres:</p>
   <ul>
   <li><strong>[!UICONTROL Costo de mano de obra presupuestado]</strong>: en el área de [!UICONTROL Presupuestación de recursos] del caso comercial de [!UICONTROL].
   <li><strong>[!UICONTROL Costo presupuestado]</strong>: en la vista del informe de [!UICONTROL Utilización] [!UICONTROL Coste]
   <p>Para obtener más información, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información de utilización de recursos </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: en el [!DNL Resource Planner] Proyecto o [!DNL Role] vistas, al ver por coste
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: en los siguientes informes: 
   <ul>
    <li>Informe de [!UICONTROL Project]</li>
    <li>Informe de [!UICONTROL Project (Financial Data)]</li>
    <li>Informe de [!UICONTROL Tarea]</li>
    <li>Informe de [!UICONTROL Issue]</li>
    <li>Informe de [!UICONTROL Hora presupuestada]</li> 
    </ul>
    <p>Para obtener más información sobre cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creación de un informe personalizado</a>.</p>
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
  <td> <p>Este es un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado. Este campo no se puede actualizar.</p>
  <p>Estas áreas se han eliminado de [!DNL Workfront]. </p> 
  <p>El campo sigue visible en los informes y listas de [!UICONTROL proyecto] y [!UICONTROL tarea].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Gráfico de evolución de [!UICONTROL]</td> 
   <td>Gráfico de líneas que proporciona una representación visual del trabajo completado y restante.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Caso comercial]</td> 
   <td> <p>Herramienta utilizada para evaluar si un proyecto debe pasar del estado [!UICONTROL Idea] al estado [!UICONTROL Planificación]. En otras palabras, un [!UICONTROL business case] ayuda a la organización a decidir si merece la pena iniciar y completar el proyecto o no, especialmente cuando se comparan proyectos con otros en un portafolio.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Crear un [!UICONTROL Business Case] para un proyecto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Caso comercial Horas presupuestadas]</td> 
   <td> <p>Este es un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado. Este campo no se puede actualizar.</p> <p>Este campo sigue visible en el proyecto y en las listas e informes de [!UICONTROL task]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignación calculada]</td> 
   <td> <p>Uno de los tipos de duración de la tarea [!UICONTROL] . Se calculará el porcentaje de un día laborable de 8 horas que el usuario asignado a la tarea se asignará a la tarea, según la [!UICONTROL Duración] de la tarea y el [!UICONTROL Trabajo requerido].</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la tarea [!UICONTROL Duración] y [!UICONTROL Tipo de duración]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabajo calculado]</td> 
   <td> <p>Uno de los tipos de duración de la tarea [!UICONTROL]. Esto calculará el [!UICONTROL Trabajo requerido] de una tarea, dados los porcentajes de [!UICONTROL Duración] y [!UICONTROL Asignación] del usuario (que se basan en un día laborable de 8 horas).</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la tarea [!UICONTROL Duración] y [!UICONTROL Tipo de duración]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendario]</td> 
   <td> <p>Hay dos tipos de calendarios en [!DNL Workfront]: los informes de calendario y [!UICONTROL Home Calendar].</p> <p>[!UICONTROL Home Calendar] es un calendario personal que permite a un usuario gestionar su carga de trabajo con respecto a las horas disponibles en [!DNL Workfront]. Los usuarios también pueden integrar su [!UICONTROL Calendario principal] con [!DNL Outlook] ([!DNL Google] y [!DNL Microsoft] integración futura). </p> <p>Para obtener más información acerca de [!UICONTROL Calendario principal], vea <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">Vista de [!UICONTROL Calendario principal]</a>.</p> <p>Un informe de calendario es un informe dinámico en el que los usuarios pueden ver la fecha y otros detalles importantes de un evento, como la fecha de vencimiento, el estado del trabajo y el usuario al que se ha asignado el evento.</p> <p> Para obtener más información sobre los informes de calendario, consulte <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Resumen de informes de calendario</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Puede Iniciar]</td> 
   <td> <p>Este campo indica si una tarea está lista para comenzar a trabajar. Si el inicio está listo para trabajar en el campo [!UICONTROL Puede comenzar] de la tarea se establece en [!UICONTROL True]. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Información general de "[!UICONTROL Puede comenzar]" para tareas</a>.</p> 
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
   <td> <p>Tiempo disponible de un recurso en el que se les puede asignar un trabajo. Consulte Disponibilidad. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Categoría]</p> </td> 
   <td> <p>Una categoría es un formulario personalizado. Se pueden generar informes para este objeto y mostrarlos en otros informes de objetos. No todos los objetos pueden tener un formulario o una categoría personalizados. Los siguientes objetos pueden tener un formulario personalizado: <br></p> 
    <ul> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Tarea]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Documento]</li> 
     <li>[!UICONTROL Gasto]</li> 
     <li>[!UICONTROL Programa]</li> 
     <li>[!UICONTROL Usuario]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de categoría]</td> 
   <td> <p>Cuando se agrega como una columna a la vista de cualquiera de los siguientes objetos, se muestra una lista de todos los formularios personalizados asociados a estos objetos:</p> 
    <ul> 
     <li>[!UICONTROL Proyecto]</li> 
     <li>[!UICONTROL Tarea]<br></li> 
     <li>[!UICONTROL Problema]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Documento]<br></li> 
     <li>[!UICONTROL Gasto]<br></li> 
     <li>[!UICONTROL Programa]<br></li> 
     <li>[!UICONTROL Usuario]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Administración de cambios]</td> 
   <td>Área de práctica centrada en definir, comprender y adaptar el trabajo planificado a los cambios en los factores de ámbito, horario, costo y recursos.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Pedido de cambio]</td> 
   <td>Tipo de problema planteado en un proyecto que describe un cambio solicitado en el ámbito acordado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambiar sólo]</td> 
   <td>Uno de los [!UICONTROL Update Types] del proyecto. Solo actualiza las escalas de tiempo de [!UICONTROL Proyecto proyectado] y [!UICONTROL Planificado] cuando se realizan actualizaciones en las tareas o ediciones en el proyecto o tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pedido de cambio]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Issue], que normalmente indica que se debe realizar una cantidad de trabajo no planeada antes de completar el proyecto.</p> <p>Para obtener más información acerca de los tipos de problemas de [!UICONTROL], vea la sección Tipos de problemas predeterminados en el artículo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizar tipos de problemas predeterminados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea secundaria]</td> 
   <td>Una tarea que es una [!UICONTROL Subtarea] de una [!UICONTROL Tarea principal] ([!UICONTROL Tarea de resumen]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Secundarios]</td> 
   <td>Colección de [!UICONTROL Subtasks] a una [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] y [!UICONTROL Training]</td> 
   <td>Módulos de aprendizaje, certificaciones, estándares o una comunidad de prácticas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compromiso]</td> 
   <td>Una herramienta de comunicación para que los usuarios establezcan expectativas sobre los resultados de las tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de confirmación]</td> 
   <td>Una herramienta de comunicación para que el usuario establezca expectativas en torno a los resultados de las tareas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comunicación] y [!UICONTROL Informes]</td> 
   <td>Estándares para revisar las excepciones y el estado de un proyecto, programa o portafolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Una [!UICONTROL Company] es una unidad organizativa de [!DNL Workfront]. </p> 
   <p> Puede asociar un usuario o un proyecto a una compañía. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Crear y editar compañías</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización]</td> 
   <td> <p>La fecha en la que se establece que se completará un proyecto, tarea o problema. Existen varios tipos de [!UICONTROL Fechas de finalización] en [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Fecha real de finalización]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Descripción general del proyecto [!UICONTROL Fecha real de finalización] </a>.</li> 
     <li>[!UICONTROL Fecha planificada de finalización]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establecer la fecha planificada de finalización del proyecto [!UICONTROL]</a> y <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Fecha planificada de finalización]</a>.</li> 
     <li>[!UICONTROL Fecha proyectada de finalización]. Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre [!UICONTROL Fecha proyectada de finalización] para proyectos, tareas y problemas</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Día de finalización]</td> 
   <td>El día, relativo al inicio de la [!UICONTROL Template], en el que se supone que debe completarse una [!UICONTROL Template Task] o una [!UICONTROL Template].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo de finalización]</td> 
   <td> <p>Esto indica cómo se marcará un proyecto como [!UICONTROL Complete]. Puede tener dos valores:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: un usuario debe cambiar el estado del proyecto a [!UICONTROL Completado].</li> 
     <li>[!UICONTROL Automatic]: el estado del proyecto cambiará automáticamente a [!UICONTROL Complete] cuando todas las tareas del proyecto estén 100% completadas y todos los problemas estén cerrados.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condición]</td> 
   <td> <p>Es una representación visual del progreso de una tarea, problema o proyecto.</p> <p>En los proyectos, el propietario del proyecto puede establecer manualmente la condición o puede establecerla automáticamente [!DNL Workfront], en función del estado de progreso del proyecto. </p> <p>Los valores posibles para la condición del proyecto son:</p> 
    <ul> 
     <li>[!UICONTROL En Destino]</li> 
     <li>[!UICONTROL En Riesgo]</li> 
     <li>[!UICONTROL Tiene Problemas]</li> 
    </ul> <p>Para obtener más información sobre las condiciones del proyecto, consulte el artículo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Información general sobre [!UICONTROL Condición del proyecto] y [!UICONTROL Tipo de condición]</a>.</p>
     <p>Puede asociar condiciones de tarea y problema con un número que se puede mostrar en los informes. Las siguientes listas muestran los nombres y números predeterminados para las condiciones de tarea y problema. El administrador del sistema puede actualizar los nombres de las condiciones y puede agregar nuevas condiciones con números diferentes. Una vez que un número está asociado a una condición, no se puede editar.  </p> 
     <p>En el caso de las tareas, el propietario de la tarea establece manualmente la condición. Los valores posibles para la condición de tarea son:</p> 
    <ul> 
     <li>[!UICONTROL va sin problemas] (0)<br></li> 
     <li> [!UICONTROL Algunas preocupaciones] (1)<br></li> 
     <li>[!UICONTROL Impedimentos mayores] (2)</li> 
    </ul> <p>Para obtener más información sobre las condiciones de las tareas, consulte el artículo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Actualizar [!UICONTROL Condición] para tareas y problemas</a>.</p> <p>En el caso de los problemas, el propietario del problema establece la condición manualmente. Los valores posibles para la condición de problema son:<br></p> 
    <ul> 
     <li>[!UICONTROL va sin problemas] (0)<br></li> 
     <li>[!UICONTROL Algunas preocupaciones] (1)<br></li> 
     <li>[!UICONTROL Impedimentos mayores] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Cuando se realiza el seguimiento del campo [!UICONTROL Condición] en los informes de [!UICONTROL Entrada de cuaderno], los valores [!UICONTROL Nuevo] y [!UICONTROL Antiguo número] muestran el número asociado a la condición en lugar de su nombre. Si una condición no está definida originalmente para una tarea o un problema y posteriormente la actualiza, la entrada de cuaderno que captura la actualización mostrará el [!UICONTROL Valor de número anterior] del campo [!UICONTROL Condición] como -2.147.483.648. Consulte también "[!UICONTROL Nuevo valor de número]", "[!UICONTROL Valor de número anterior]" y "[!UICONTROL Entrada de cuaderno]" en este artículo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actualización de condición]</td> 
   <td> <p>Este campo muestra la condición actual de tareas, proyectos o problemas. Esta opción muestra las actualizaciones más recientes que los propietarios de tareas, proyectos o problemas han proporcionado en el campo [!UICONTROL Estado de la actualización], junto con la nueva condición.</p> <p>Los comentarios realizados en las actualizaciones de condición no se muestran en la columna [!UICONTROL Condition Update]; solo se muestra la actualización principal.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de restricción]</td> 
   <td> <p>Si utiliza una [!UICONTROL Task Constraint] vinculada a una fecha específica, como [!UICONTROL Must Start On], esa fecha específica se convierte en la [!UICONTROL Constraint Date] de la tarea.</p> <p>Las siguientes delimitaciones de tareas actualizan el campo [!UICONTROL Fecha de delimitación]:</p> 
    <ul> 
     <li>[!UICONTROL Debe Comenzar El]</li> 
     <li>[!UICONTROL Debe Finalizar El]</li> 
     <li>[!UICONTROL No iniciar después de]</li> 
     <li>[!UICONTROL No iniciar antes de]</li> 
    </ul> <p><b>SUGERENCIA</b></p>   
     <ul> 
      <li> <p>Una tarea con una [!UICONTROL Restricción] de [!UICONTROL Fechas fijas] no tiene [!UICONTROL Fecha de restricción]. </p> </li> 
      <li> <p> [!UICONTROL Fecha de restricción] solo se puede ver en un informe o vista personalizada.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Día de restricción]</td> 
   <td> <p>Si utiliza una restricción de tarea en una tarea de plantilla vinculada a un día específico, como Debe comenzar el, ese día específico se convierte en el día de restricción de la tarea de plantilla.</p> <p>Las siguientes restricciones de tarea actualizan el campo [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Debe Comenzar El]</li> 
     <li>[!UICONTROL Debe Finalizar El]</li> 
     <li>[!UICONTROL No iniciar después de]</li> 
     <li>[!UICONTROL No iniciar antes de]</li> 
    </ul> <p><b>SUGERENCIA</b></p> <p>  [!UICONTROL Día de restricción] solo se puede ver en un informe o vista personalizada. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de restricción]</td> 
   <td> <p>Tendencia de programación de una tarea. Por ejemplo, [!UICONTROL Lo antes posible] programará una tarea para que comience lo antes posible y [!UICONTROL No finalizar después de] programará una tarea para que finalice en la fecha de restricción [!UICONTROL] y no más tarde.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tarea de [!UICONTROL]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menú contextual]</td> 
   <td>Menú, situado en la parte izquierda de la pantalla, en el que los elementos cambian para correlacionarse con el contenido activo. Por ejemplo, cuando un usuario está viendo un proyecto, el [!UICONTROL Menú contextual] mostrará vínculos a información y herramientas relacionadas con el proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Creador de problema convertido]</td> 
   <td>Campo de un informe de proyecto o tarea que muestra información sobre el usuario que es el [!UICONTROL Contacto principal] de un problema cuando el problema se convierte en un proyecto o tarea. El campo también aparece en la sección [!UICONTROL Detalles del proyecto], donde muestra el nombre del [!UICONTROL Contacto principal] del problema convertido. Consulte también "[!UICONTROL Contacto principal]" en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo]</td> 
   <td> <p>La cantidad monetaria que debe gastar al completar un proyecto, tarea o problema. </p> <p>Puede realizar un seguimiento de varios tipos de costes laborales, gastos y riesgos relacionados con el proyecto.Para obtener información sobre el seguimiento de costes en [!DNL Workfront] consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Seguimiento de costes</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de costo]</td> 
   <td>Para una tarea, el [!UICONTROL Tipo de costo] determina cómo acumulará costos la tarea. Algunos ejemplos son [!UICONTROL Fijo por hora], [!UICONTROL Usuario por hora] y [!UICONTROL Usuario por hora más fijo]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependencias entre proyectos]</td> 
   <td> <p>Una tarea de un proyecto depende de una tarea de un proyecto diferente.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Crear predecesoras entre proyectos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Datos personalizados]</td> 
   <td> <p>Datos que son únicos para una organización. Las organizaciones pueden personalizar [!DNL Workfront] mediante la creación de formularios y campos personalizados. Esta información personalizada puede impulsar la creación de informes para KPI, auditoría y combinación de demanda. </p> <p>[!UICONTROL Custom Data] se puede vincular a:</p> 
    <ul> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tareas]</li> 
     <li>[!UICONTROL Usuarios]</li> 
     <li>[!UICONTROL Compañías]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Gastos]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de datos personalizados]</td> 
   <td>Opción para especificar si un campo de [!UICONTROL Datos personalizados] está almacenado en la base de datos como texto, fecha, número o moneda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de presentación personalizada]</td> 
   <td>El tipo de visualización de campo de un campo personalizado. Algunos ejemplos son [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo personalizado]</td> 
   <td>Para los datos personalizados que permiten al usuario seleccionar entre varias opciones, estos son los valores entre los que puede seleccionar un usuario. Las opciones personalizadas solo son válidas en [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons] y [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Etiqueta de formulario personalizado]</td> 
   <td>Al utilizar un tipo de presentación personalizado con opciones personalizadas, este es el texto de la interfaz de usuario que se mostrará en el menú desplegable, en las casillas de verificación o en los botones de opción de esa opción personalizada.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor personalizado]</td> 
   <td>Al utilizar un campo personalizado con opciones personalizadas, este es el valor que se almacenará en la base de datos para una opción en particular.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vista personalizada]</td> 
   <td>Definición de los campos de datos o columnas que se muestran para cada objeto de una lista.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cliente]</td> 
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
   <td> <p> Puede agregar este campo en un informe o en una vista del objeto Informe para mostrar los tableros en los que el informe aparece en una lista. </p> <p> Puede utilizar este campo para filtrar por informes que también se enumeran en un tablero específico. </p> <p> Para obtener más información sobre la inclusión de información de tableros en los informes de objetos de informe, consulte la sección "Explicación de los informes que aparecen en los tableros" en el artículo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Acceso y organización de informes</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de datos]</td> 
   <td>Consulte "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Días de retraso]</td> 
   <td> <p>Este campo muestra una diferencia de fecha entre [!UICONTROL Inicio planificado] y [!UICONTROL Hoy] si falta la [!UICONTROL Fecha real de finalización].</p> <p>También muestra una diferencia de fecha entre [!UICONTROL Finalización real] y [!UICONTROL Finalización planificada], cuando hay una [!UICONTROL Fecha real de finalización].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Programación predeterminada]</td> 
   <td> <p>Horas laborables predeterminadas personalizables que se asignarán a usuarios y proyectos de una organización. </p> <p>Los programas se utilizan para calcular las fechas planificadas, de inicio y de finalización de las tareas asignadas a los usuarios.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Entregable]</td> 
   <td>Bienes o servicios cuantificables que deben suministrarse al finalizar un proyecto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Administración de demanda]</td> 
   <td>Puntuación y priorización de los procesos de admisión.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Objetivos de departamento]</td> 
   <td>Objetivos exclusivos de un departamento específico que se centran en mejorar las métricas operativas dentro del departamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>El vínculo entre dos tareas que requieren que una tarea cambie de estado antes de que la otra tarea también pueda cambiar de estado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de dependencia]</td> 
   <td> <p>Tipo de relación de programación entre una tarea y sus predecesoras. Un ejemplo es [!UICONTROL Finalizar-Iniciar], que requiere que la primera tarea deba Finalizar antes de que la segunda tarea pueda Iniciar.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Información general sobre los tipos de dependencia entre tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Documento]</td> 
   <td>Cualquier archivo adjunto a un objeto en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Cada vez que se carga el mismo documento en el mismo objeto, se le asigna un número de versión. Los usuarios pueden ver y cambiar varias opciones de una versión anterior de un documento.</p> <p>Para obtener más información, consulte <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Administrar versiones de documentos</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duración]</td> 
   <td> <p>Ventana de tiempo asignado para la finalización de un problema o proyecto de tarea (determinado por el número de días entre el [!UICONTROL Inicio planificado] y la finalización planificada).</p> 
    <ul> 
     <li>Para las tareas, Duración es un campo editable si el Tipo de duración de la tarea no es Simple. Si el tipo de duración de la tarea es Simple o si la restricción de tarea es Fechas fijas, Duración es un cálculo realizado por Workfront.</li> 
     <li>En el caso de los problemas, Duración siempre es un campo editable y debe representar una estimación de un número de días que requerirían que se resolviera el problema.</li> 
     <li>Para los proyectos, Duración es un cálculo realizado por [!DNL Workfront] y representa la diferencia en días entre el Inicio planificado de la tarea más temprana y la [!UICONTROL Finalización planificada] de la última tarea del proyecto.</li> 
    </ul> <p>Para obtener más información acerca de la diferencia entre [!UICONTROL Duración] y [!UICONTROL Duración planificada] para las tareas, vea el artículo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Diferencia entre [!UICONTROL Duración planificada] y [!UICONTROL Duración] para tareas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duración en minutos]</td> 
   <td>Este campo muestra la misma información que el campo [!UICONTROL Duration] en minutos en lugar de días. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duración por resolicitud]</td> 
   <td> <p>Esto aparece en los cuadros [!UICONTROL Detalles de la tarea] y [!UICONTROL Editar tarea] de un elemento principal de tareas recurrentes. Muestra la duración de cada tarea recurrente. Para obtener información sobre la creación de tareas recurrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creación de tareas recurrentes</a>. </p> <p> <span>Las duraciones modificadas en tareas recurrentes individuales no muestran el valor indicado en este campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo de duración]</td> 
   <td> <p>Campo de tarea que indica cómo se asigna el trabajo necesario para completar la tarea a los usuarios asignados a lo largo de la duración de la tarea. Representa la relación entre la [!UICONTROL Duración] de la tarea, el [!UICONTROL Trabajo requerido] y la cantidad de tiempo, o [!UICONTROL Asignación], que los recursos asignados deben dedicar a la tarea para completarla. </p> <p>Este campo aparece en la ficha [!UICONTROL Detalles] de una tarea. </p> <p>Las opciones para el tipo de duración de una tarea son:</p> 
    <ul> 
     <li>[!UICONTROL Asignación calculada]</li> 
     <li>[!UICONTROL Trabajo calculado]</li> 
     <li>[!UICONTROL Condicionada por el esfuerzo]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la tarea [!UICONTROL Duración] y [!UICONTROL Tipo de duración]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unidad de duración]</td> 
   <td>La unidad que se utiliza para medir el tiempo en una búsqueda de energía.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condicionada por el esfuerzo]</td> 
   <td>Relación entre la cantidad de usuarios y el tiempo que tardará la tarea en completarse. A medida que agrega más usuarios, el tiempo total programado para que se complete la tarea disminuye, pero la duración de la tarea permanece igual. Por ejemplo, si una tarea está bombardeando un barril de cacahuetes, agregar más personas reducirá el tiempo programado, pero la duración en días-persona seguirá siendo la misma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo transcurrido]</td> 
   <td> <p>[!UICONTROL Tiempo transcurrido] es una unidad de tiempo para la [!UICONTROL Duración] de una tarea. Es el tiempo entre la [!UICONTROL Fecha planificada de inicio] y la [!UICONTROL Fecha planificada de finalización] de una tarea que incluye días festivos, fines de semana y días libres. En otras palabras, el tiempo transcurrido es el paso de los días del calendario. </p> <p>[!DNL Workfront] admite las siguientes unidades de tiempo transcurrido para la duración de la tarea:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minutos transcurridos]</p> </li> 
     <li> <p>[!UICONTROL Horas transcurridas]</p> </li> 
     <li> <p>[!UICONTROL Días transcurridos]</p> </li> 
     <li> <p>[!UICONTROL Semanas]</p> </li> 
     <li> <p>[!UICONTROL Meses transcurridos]</p> </li> 
    </ul> <p>Para obtener más información sobre la duración de las tareas, incluido el tiempo transcurrido, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la tarea [!UICONTROL Duración] y [!UICONTROL Tipo de duración]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización]</td> 
   <td> <p> En un informe de [!UICONTROL Rate], es la fecha en la que finaliza una nueva tarifa de facturación para un rol a nivel de proyecto. Las horas asociadas con el proyecto que son anteriores a esta fecha se multiplican por esta tarifa de facturación para calcular los ingresos del proyecto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Participación]</td> 
   <td>El [!UICONTROL Indicador de rendimiento del trabajo] (WPI) que indica cuándo disminuye el compromiso y la confianza en la tarea, proyecto, equipo u organización. Esto indica que es necesario actuar para revivir esa creencia y ese compromiso. WPI se mediría haciendo preguntas simples, "¿Entendió lo que se esperaba de usted? ¿El trabajo que se le ha asignado ha marcado una diferencia en la organización? ¿Hiciste un gran trabajo?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Metas interfuncionales que contribuyen a las métricas de los objetivos de la empresa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Evento]</td> 
   <td>Cualquier cambio en un proyecto o tarea.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Controlador de eventos]</td> 
   <td>Tareas automatizadas que se producen cuando se producen eventos. Un ejemplo común es una notificación automática por correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificación de eventos]</td> 
   <td>Correo electrónico que se genera desde un controlador de eventos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gastos]</td> 
   <td>Un costo no laboral en tareas o proyectos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externo]</td> 
   <td> <p>Normalmente, es un tipo de licencia, o un usuario con dicha licencia. Un usuario con un tipo de licencia de este tipo solo tiene la capacidad de revisar la información en el sistema. No pueden participar activamente en el trabajo.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] información general sobre licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sistema externo]</td> 
   <td>Cualquier servicio o software que esté almacenado y regido fuera del sistema de registro designado.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Campo]</td> 
   <td><p>Cualquier objeto Workfront o la información asociada a él, tal como aparece en la base de datos. </p>
   <p>Por ejemplo, "proyecto", "usuario", "hora" son tanto objetos de Workfront como campos. "Nombre", "estado", "propietario", "fecha de inicio" son campos de Workfront asociados a los objetos anteriores. </p>

<p>Cuando se hace referencia a objetos, los términos "objetos" y "campos" se pueden utilizar indistintamente.</p>
   <p>En el ámbito de los informes, los "campos" hacen referencia a los objetos o a la información sobre el objeto que desea capturar en el informe.</p>

<p><b>NOTA</b></p>

<p>En los informes de texto, los campos hacen referencia a los objetos o a su información tal como aparece en la base de datos.</p>
   <p>A veces, el nombre que se ve en la interfaz de usuario es diferente del nombre del campo en la base de datos. Por ejemplo, "issue" es el nombre del objeto en la interfaz de Workfront, pero "opTask" es el nombre del objeto (o el campo) en la base de datos de Workfront. </p> 
   <p> Es importante utilizar el campo tal como aparece en la base de datos al escribir un informe, una vista, un filtro o una agrupación en modo texto, o al crear un campo calculado.</p>

<p>Para obtener más información, consulte <a href="../../../wf-api/general/api-explorer.md">Explorador de API</a> y <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Introducción al modo de texto</a>.</p>

<p>De forma predeterminada, Workfront incluye un conjunto de campos que definen ambos objetos y su información. También puede crear campos personalizados para definir objetos, pero no puede crear objetos personalizados.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Uno de los principales componentes básicos de un informe o un elemento de lista que define la información que se muestra en la pantalla. Para obtener más información sobre los elementos de informes, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de informes: filtros, vistas y agrupaciones</a>.</p> <p>El filtro determina los resultados que se muestran en un informe o en un [!DNL Workfront] lista de paneles, como proyectos, tareas o problemas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Proceso para administrar los datos de costes laborales, gastos e ingresos en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo fijo]</td> 
   <td>Puede definir una cantidad fija de costos para un proyecto. Esto es parte del [!UICONTROL Costo planificado] del proyecto que representa la cantidad de dinero que usted necesita para completar el proyecto. Para obtener información sobre los costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ingresos fijos]</td> 
   <td>Puede definir una cantidad fija de ingresos para un proyecto. Esto es parte de los [!UICONTROL Ingresos planificados] del proyecto que representa la cantidad de dinero que usted podría obtener si completa el proyecto. Para obtener información sobre los ingresos, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Resumen de facturación e ingresos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicadores]</td> 
   <td> <p> Es el mismo campo que [!UICONTROL Status Icons], pero sólo está disponible para las vistas siguientes: </p> 
    <ul> 
     <li> [!UICONTROL Plantillas] </li> 
     <li> [!UICONTROL Gastos] </li> 
    </ul> <p> Para obtener más información, consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta]</td> 
   <td>Las carpetas se utilizan para organizar documentos o informes asociados a un objeto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (equivalente a tiempo completo)</td> 
   <td>Equivalente a tiempo completo que indica la cantidad de tiempo que un recurso está disponible para trabajar. 
   El campo [!UICONTROL FTE] se muestra en las áreas siguientes: 
  <ul>
   <li> Perfil del usuario, al editar o crear el usuario </li>
   <li> [!UICONTROL Planificador de recursos] </li>
   <li> [!UICONTROL Scenario Planner] (se requiere una licencia adicional para Workfront Scenario Planner) </li>
   <li> Listas de usuarios e informes </li> </ul>

<p>[!UICONTROL FTE] debe ser un número decimal de hasta 1 y no puede ser 0. </p>
   <p> Un [!UICONTROL FTE] de 1 (que es el valor predeterminado para el campo [!UICONTROL FTE] de un usuario, tal como se define en su perfil) significa que un recurso (usuario o función) funciona todo el número de horas, según la programación que calcula su disponibilidad. </p>
   <p>El administrador de Workfront decide qué horario utilizar para determinar la disponibilidad del usuario.  </p>
   <ul>
   <li> Cuando se utiliza el horario predeterminado de [!UICONTROL], Workfront utiliza el [!UICONTROL FTE] del usuario que se encuentra en su perfil para calcular la disponibilidad. </li>
   <li> Cuando se usa el Horario del usuario, Workfront usa el tiempo libre del usuario, el valor de [!UICONTROL Tiempo de trabajo] y las horas de [!UICONTROL Horario predeterminado] para calcular el [!UICONTROL FTE] del usuario. </li> </ul>

<p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferencias de administración de recursos</a>.  </p>
   <p>Para obtener más información sobre la creación de programaciones en [!DNL Workfront], consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creación de una programación</a>. </p>

<p><b>NOTA</b></p>
   <p>Para todos los cálculos del [!UICONTROL Scenario Planner], Workfront utiliza el siguiente valor: 1 [!UICONTROL FTE] = 8 Horas.</p>
   <p>Para obtener más información, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introducción al Planificador de escenarios [!UICONTROL]</a>. </p>
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
   <td>Diagrama de Gantt de [!UICONTROL]</td> 
   <td> <p>Una escala de tiempo visual de las fechas del proyecto en una vista de calendario basada en las fechas planificadas o proyectadas a medida que las tareas del proyecto están programadas actualmente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Meta]</td> 
   <td><p>Hay dos conceptos de objetivos en [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Metas del proyecto</b>: Un conjunto de objetivos empresariales acordados por las partes interesadas relevantes de un proyecto. Los objetivos del proyecto forman parte del caso empresarial de un proyecto. </p> <p>No puede mostrar los objetivos del proyecto en listas o informes, pero puede acceder a ellos a través de la API. </p> <p>Para obtener información sobre los objetivos del proyecto de caso empresarial, consulte <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Crear metas de caso comercial </a>. </p> </li> 
     <li> <p><b>Objetivos estratégicos</b>: una meta estratégica es un objetivo que se crea para planificar la estrategia de trabajo para un período de tiempo específico. Puede crear estos tipos de objetivos utilizando [!DNL Workfront Goals]. Su organización debe adquirir una licencia adicional y debe tener acceso a esta función para poder crear objetivos estratégicos. [!DNL Workfront Goals] solo están disponibles con una licencia adicional.</p> 
     <p>Para obtener más información, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] descripción general </a>. </p> 
     <p>Puede mostrar objetivos estratégicos en un objetivo o en un informe de proyecto y acceder a ellos a través de la API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Jerarquía de metas]</td> 
   <td> <p>En los informes de [!UICONTROL Goal] y [!UICONTROL Project], se trata de un campo de recopilación que muestra las metas de la jerarquía a la que pertenece una meta estratégica cuando se alinea con otras metas. Los objetivos se separan con un delimitador ▸. </p> <p>En este campo solo se muestran los padres de la meta y la meta. Las metas secundarias no se muestran. </p> <p>Para obtener información sobre cómo alinear objetivos en [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Información general sobre la alineación de objetivos en [!DNL Workfront Goals]</a>. </p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] descripción general </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Puntuación de éxito de [!UICONTROL Goal]</td> 
   <td> En un informe de [!UICONTROL Project], este campo se usa para hacer referencia a los objetivos de nivel de proyecto asociados con el caso de [!UICONTROL Business]. Actualmente, este es un campo obsoleto y no está asociado con ninguna funcionalidad.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objetivos] </td> 
   <td> <p>En un informe de [!UICONTROL Project], se trata de un campo de recopilación que muestra todos los objetivos estratégicos asociados a un proyecto. Los objetivos se separan con comas.</p> <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] descripción general</a>. Para obtener más información sobre las metas estratégicas y los objetivos de proyecto en [!DNL Workfront], consulte "[!UICONTROL Goal]" en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Preferencias de la interfaz global de [!UICONTROL]</td> 
   <td>Configuración de la interfaz que afecta a todos los usuarios. [!UICONTROL Preferencias de interfaz global] se puede sobrescribir con las Preferencias de interfaz de usuario de [!UICONTROL].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Grupo]</td> 
   <td> <p>Colección de usuarios (posiblemente del mismo departamento o unidad de negocio) que tienen acceso a los mismos objetos. Además de los usuarios, los grupos pueden asociarse con portafolios, programas y proyectos,<span> plantillas de proyecto,</span> compañías, equipos, programaciones, plantillas de diseño y perfiles de hojas de horas.</p> <p>También puede conceder permisos a objetos por grupo. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general de grupos</a>.</p> <p>En una lista o informe de objetos de uno de los tipos siguientes, puede utilizar el campo [!UICONTROL Group] para enumerar qué objetos de ese tipo están asociados a un grupo determinado: usuario, portafolio, programa, proyecto, etc. <span>plantilla de proyecto</span>, empresa, equipo, programación, plantilla de diseño o perfil de hoja de horas.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Administrador de grupo]</td> 
   <td> <p>Usuarios que administran los objetos, accesos y usuarios de grupos de usuarios designados.</p> <p> En un informe de [!UICONTROL Group], este campo muestra los nombres de los usuarios designados como [!UICONTROL Group Administrators] en el grupo. Para obtener más información sobre los administradores de grupo, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Grupo con acceso de administración]</td> 
   <td> <p> En una plantilla de diseño [!UICONTROL], un perfil de hoja de horas [!UICONTROL] o un informe de programación [!UICONTROL], este campo muestra los grupos a los que tienen acceso los administradores del grupo para modificar la plantilla. También puede filtrar este informe por este campo. </p> <p> Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Agrupación]</td> 
   <td> <p>Elemento de informe que se utiliza para categorizar la información de una lista según un criterio común.</p> <p>Para obtener más información, consulte la sección "[!UICONTROL Groupings]" en el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de informes: filtros, vistas y agrupaciones</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de transferencia]</td> 
   <td> <p>La fecha en la que una tarea está disponible para trabajar. La [!UICONTROL Fecha de transferencia] es un cálculo y no se puede establecer manualmente. <br>Para obtener más información acerca de [!UICONTROL Fecha de entrega], vea el artículo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Información general de [!UICONTROL Fecha de transferencia de tareas]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Un nombre alternativo para describir el área de [!UICONTROL Requests] de [!DNL Workfront]. Puede usar el área de [!UICONTROL Requests] para procesar tickets de asistencia al cliente, solicitudes de proyectos, tickets de servicio de asistencia, etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propietario]</td> 
   <td>En un informe de [!UICONTROL Hour], el [!UICONTROL Owner] es el usuario al que se atribuyen las horas. Esto es diferente al usuario que realmente registra la hora. Estas dos entidades pueden ser a veces dos usuarios diferentes. <br>Para obtener más información sobre cómo registrar la hora de otro usuario, consulte el artículo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrar tiempo</a>.</td> 
  </tr>

<tr> 
   <td>Estado de hora</td> 
   <td> <p>Atributo establecido por Workfront para las horas reales que los usuarios registran para tareas, problemas o proyectos. </p>

Las entradas de hora pueden tener uno de los siguientes estados en Workfront:
<ul>
   <li><b>Enviado</b>: las horas se han registrado en un proyecto, tarea o problema. Forman parte de un registro de facturación o aún no se han agregado a un registro de facturación.</li>
   <li><b>Aprobado</b>: se han registrado las horas y el propietario del proyecto las ha aprobado. Forman parte de un registro de facturación o aún no se han agregado a un registro de facturación.</li> 
   <li><b>No aprobado</b>: el propietario del proyecto ha registrado las horas y las ha rechazado. Forman parte de un registro de facturación o aún no se han agregado a un registro de facturación.</li>
   <li><b>Facturado</b>: se han registrado las horas, se han agregado a un registro de facturación y el estado del registro de facturación se ha marcado como Facturado. No es necesario que el propietario del proyecto los apruebe.</li>
   <li><b>Facturado y aprobado</b>: se han registrado las horas, aprobadas por el propietario del proyecto y el estado del registro de facturación se ha marcado como Facturado.</li>
   </ul>


<p>Cuando las horas son parte de un registro de facturación, el Estado de hora indica si las horas se han aprobado o si se ha facturado el Registro de facturación al que pertenecen. El estado de hora de una entrada de hora solo es visible en una lista de horas o un informe. </p>

<p>Para obtener más información sobre cómo agregar horas a los registros de facturación, consulte la sección "Agregar horas a registros de facturación" en el artículo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crear registros de facturación</a>.</p>

<p>Para obtener más información sobre la aprobación de las horas en los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Requerir tiempo de aprobación de un proyecto</a>.</p>

<p><b>SUGERENCIA</b></p>

<p>Las horas generales que no se registran directamente en los elementos de trabajo no muestran un estado de hora. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Tipo de hora]</td> 
   <td> <p>Atributo que puede establecerse para Horas reales que los usuarios registran para tareas, problemas o proyectos. También es un atributo para las horas registradas que no están directamente vinculadas al trabajo, como [!UICONTROL Vacation] y [!UICONTROL Time Off].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Administrar tipos de horas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>El ID es un indicador alfanumérico asociado a cada objeto de [!DNL Workfront]. Identifica de forma exclusiva cada objeto del [!DNL Workfront] base de datos. Puede ver el ID de cualquier objeto en un informe o una lista para cada objeto. </p> <p><b>SUGERENCIA</b></p>   <p>También puede ver el ID en la dirección URL de la página del objeto. Por ejemplo, el identificador de un proyecto puede parecerse al número indicado en la siguiente dirección URL al acceder a la página Detalles del proyecto de [!UICONTROL]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Metas individuales]</td> 
   <td>Metas individuales que contribuyen a las métricas de las metas del equipo, pero no relacionadas con el desarrollo personal o profesional.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Acceso heredado]</td> 
   <td>Función de uso compartido que permite el acceso para propagarse de un objeto a otro. Por ejemplo, el acceso heredado del usuario del proyecto definido en los registros del programa y del portafolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Iniciativa]</td> 
   <td> <p>En el [!DNL Workfront Scenario Planner], puede dividir un plan en varias iniciativas para que sea más fácil administrarlo. <span>Puede generar un informe de [!UICONTROL Iniciativa] y tener acceso a la información de [!UICONTROL Iniciativa] en un informe de [!UICONTROL Proyecto].</span></p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">El [!DNL Scenario Planner] descripción general</a>. </p> <p>El [!DNL Initiative] el informe no es visible en su [!DNL Workfront] a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia. No puede tener acceso a [!UICONTROL Initiatives] a través de la API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Función del puesto de la iniciativa]</span> </td> 
   <td> <p><span>El tipo de informe Función de [!UICONTROL Initiative Job Role] muestra información sobre las funciones de trabajo asociadas a una iniciativa de plan en [!DNL Workfront Scenario Planner].</span> </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">El [!DNL Scenario Planner] descripción general</a>. </p> <p><span>Este tipo de informe no es visible en su [!DNL Workfront] a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Iniciativa Trabajo Horas]</span> </td> 
   <td> <p><span> En un informe de función de [!UICONTROL Initiative Job Role], se muestra el número de horas asociadas a una función de trabajo en una iniciativa.</span> </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">El [!DNL Scenario Planner] descripción general</a>. </p> <p>Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no son visibles en su [!DNL Workfront] a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Iniciativa Recuento de funciones]</td> 
   <td> <p>En un informe de función de [!UICONTROL Initiative Job Role], se muestra el número de funciones de puesto específicas asociadas a una iniciativa.</p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">El [!DNL Scenario Planner] descripción general</a>. </p> <p>Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no son visibles en su [!DNL Workfront] a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de última publicación de la iniciativa]</td> 
   <td> <p>Campo de un informe de [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] y [!UICONTROL Project] que muestra la última fecha de publicación de una iniciativa de plan en un proyecto. Puede publicar iniciativas para crear proyectos o actualizar proyectos vinculados a las iniciativas.</p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">El [!DNL Scenario Planner] descripción general</a>. </p> <p><span>Para obtener información sobre la publicación de iniciativas, consulte</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publicar escenarios para crear y actualizar proyectos en [!DNL Workfront Scenario Planner]</a>. Este campo no es visible en su [!DNL Workfront] a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Búsqueda en línea]</td> 
   <td>Búsqueda realizada, durante el proceso de cumplimentación de un formulario, para buscar posibles entradas para un campo específico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuración de interfaz]</td> 
   <td>El área de la aplicación que permite definir vistas personalizadas, filtros, agrupaciones, controles de lista, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Es El Objetivo De La Empresa]</p></td> 
   <td> <p>Entrada [!DNL goal reports], muestra un valor "[!UICONTROL True]/ [!UICONTROL False]" para cada objetivo estratégico para indicar si su organización está asignada al objetivo como propietario. </p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] descripción general </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema]</td> 
   <td> <p>Elemento de trabajo no planeado que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Se clasifica y evalúa para un examen posterior del esfuerzo de trabajo</p> <p>Un problema de [!UICONTROL] también puede ser una solicitud del servicio de asistencia de [!UICONTROL]. [!UICONTROL Solicitudes de cambio], [!UICONTROL Solicitudes] y [!UICONTROL Errores] también son [!UICONTROL Problemas].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Administración de problemas]</td> 
   <td> <p>Proceso y reglas que rigen la definición de tipos de problemas y el proceso de enrutamiento, clasificación o tráfico asociado a cada tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Propietario de problema]</td> 
   <td>El equipo o usuarios responsables de probar y completar un problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
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
   <td>[!UICONTROL Rol]</td> 
   <td> <p>Se utiliza para identificar las funciones y responsabilidades laborales diarias de un usuario. Los roles se pueden asignar a elementos de trabajo para identificar la aptitud necesaria para completar un proceso de trabajo sin asignarla a un usuario específico. </p> <p>Un usuario puede tener más de una función. Algunos ejemplos son Diseñador gráfico o Consultor.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Entrada de cuaderno]</p> </td> 
   <td> <p>Objeto de informe que proporciona información acerca de las actualizaciones del sistema para los campos controlados que aparecen en el área de [!UICONTROL Actualizaciones] de proyectos, tareas, problemas y otros objetos.</p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Informe sobre el área de [!UICONTROL Updates]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicador Kanban]</td> 
   <td> <p>En un informe de [!UICONTROL Tarea] o de [!UICONTROL Problema], el campo [!UICONTROL Indicador Kanban] muestra el estado del indicador que se ha establecido en el artículo del panel Kanban de [!UICONTROL]. Los valores posibles son [!UICONTROL On Track], [!UICONTROL Ready to Pull] y [!UICONTROL Is Blocked].</p> <p>Para obtener más información acerca de cómo establecer el estado del indicador en las historias del panel de historias de [!UICONTROL Kanban], consulte el artículo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Usar marcas en las historias del panel Kanban de [!UICONTROL]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Un valor que se puede medir y que demuestra la eficacia con la que una empresa logra los objetivos clave de su negocio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retardo]</td> 
   <td>Cantidad de tiempo que debe transcurrir después de que [!UICONTROL Fecha planificada de finalización] de la tarea predecesora haya transcurrido hasta que pueda comenzar la tarea dependiente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de retardo]</td> 
   <td> <p>Método de cálculo del retardo de [!UICONTROL]. Puede ser:</p> 
    <ul> 
     <li>[!UICONTROL Días] (días laborables)</li> 
     <li>[!UICONTROL Días del calendario] (omitir festivos)</li> 
     <li>[!UICONTROL Porcentaje]</li> 
     <li>[!UICONTROL Día de la semana]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Resumen de tipos de retardo</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura grande]</td> 
   <td> <p> En una lista o informe de [!UICONTROL Document], muestra una vista previa del documento en una miniatura. </p> <p>Seleccionar <strong>[!UICONTROL Miniatura grande]</strong> para ver una miniatura de 400 píxeles de ancho en el informe.</p> <p>El tamaño de la miniatura se ajusta al modificar el ancho de la columna en una lista o informe.</p> <p>Consulte también "[!UICONTROL Miniatura]" en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Últimos 10 visores]</td> 
   <td> <p>En una lista de informes, este campo muestra los nombres de hasta 10 usuarios que han visto el informe más recientemente.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última nota de condición]</td> 
   <td> <p>Este campo muestra la última actualización introducida en un objeto por el propietario del objeto. Es la actividad o interacción más reciente del propietario sobre un objeto.</p> <p>El [!DNL Last Condition Note] está vacía si se ha eliminado el texto de la última nota de un objeto. Cuando se introduce una nota nueva en el objeto, esta se convierte en la última nota y se vuelve a mostrar en la columna. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de última actualización de finanzas]</td> 
   <td>En un informe de [!UICONTROL project], este campo registra la fecha y la hora en que se calcularon y actualizaron por última vez las finanzas del proyecto. Para obtener información sobre las finanzas del proyecto, consulte <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Resumen de finanzas del proyecto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última nota]</td> 
   <td> <p>Este campo muestra la última actualización introducida en un objeto por cualquier usuario. Esta es la actividad o interacción más reciente de un objeto.</p> <p>La columna [!UICONTROL Última nota] está vacía si se ha eliminado el texto de la última nota de un objeto. Cuando se introduce una nota nueva en el objeto, esta se convierte en la última nota y se vuelve a mostrar en la columna.</p>
   <p>Cuando este campo se agrega a un informe de [!UICONTROL Tarea], las actualizaciones que queden en los objetos secundarios, como problemas, subtareas, documentos, etc. — de la tarea no se muestran en esta columna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última visualización por]</td> 
   <td> <p>En una lista de informes, este campo muestra información sobre el usuario que vio el informe por última vez.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Última fecha de visualización]</td> 
   <td> <p>En una lista de informes, este campo muestra la fecha en la que se mostró el informe por última vez.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Plantilla de diseño]</td> 
   <td>Definido por el administrador del sistema o del grupo para identificar las fichas e informes que se muestran en el espacio de trabajo de un usuario determinado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de diseño]</td> 
   <td>Junto con [!UICONTROL Vistas personalizadas], el [!UICONTROL Tipo de diseño] especifica el tipo de [!UICONTROL Vista personalizada]. Actualmente, solo está disponible List. En el futuro, [!UICONTROL Detail] (la vista [!UICONTROL Detail] de un objeto) puede estar disponible.</td> 
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
   <td>Plantilla para una única tarea que se utiliza para proporcionar un nombre coherente de las [!UICONTROL Tareas] y las [!UICONTROL Tareas de plantilla] en toda la aplicación.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de licencia]</td> 
   <td>Tipo de licencia asignada a un [!UICONTROL nivel de acceso]. Es [!UICONTROL Full User], [!UICONTROL Limited User] o [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan de límite de licencia]</td> 
   <td> <p>En una vista o informe de [!UICONTROL Group], este campo muestra el número máximo de licencias de [!UICONTROL Plan] que se pueden asignar a usuarios que tienen el grupo respectivo designado como su [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabajo de límite de licencia]</td> 
   <td> <p>En una vista o informe de [!UICONTROL Group], este campo muestra el número máximo de licencias de [!UICONTROL Work] que se pueden asignar a usuarios que tienen el grupo respectivo designado como su [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuario limitado]</td> 
   <td>Tipo de licencia que permite crear un [!DNL Access Level] que contiene privilegios de solo vista, con la capacidad de enviar problemas, introducir notas y cargar documentos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Controles de lista]</td> 
   <td> <p>Parte de [!UICONTROL Interface Setup] que permite vincular filtros, vistas y agrupaciones personalizados a usuarios individuales o globalmente a todos los usuarios.</p> </td> 
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
   <td>[!UICONTROL Solo manual]</td> 
   <td> <p>Uno de los [!UICONTROL Tipos de actualización] de un proyecto [!UICONTROL]. Esta configuración permite actualizar las escalas de tiempo de [!UICONTROL Proyecto proyectado] y [!UICONTROL Planificado] solo cuando se hace clic en "[!UICONTROL Escalas de tiempo recalculadas]". Los proyectos configurados de esta manera se omitirán durante el proceso de cálculo nocturno y cuando se actualicen el proyecto o las tareas del proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el proyecto [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Hace referencia al usuario que ha iniciado sesión actualmente. </p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, solo puede generar un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo de usuarios]</td> 
   <td> <p>Este es un campo obsoleto. Cualquier información que este campo pueda mostrar está relacionada con una función que [!DNL Workfront] se ha eliminado y el campo no se puede actualizar. </p> <p>En versiones anteriores de [!DNL Workfront], puede actualizar este campo al crear o editar un rol. Muestra el número total de usuarios que se pueden asociar a un rol en cada proyecto. Un valor de cero permitido para un número ilimitado de usuarios que se pueden asignar en un proyecto. </p>El campo sigue visible en algunos informes y listas, pero la información mostrada no se puede actualizar. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Hito]</td> 
   <td> <p>Un marcador que puede asociar a una tarea para indicar que se ha alcanzado un punto clave en el proyecto cuando se completa la tarea. Por lo general, puede utilizar hitos para mostrar un evento significativo, como la finalización de una fase del proyecto o un conjunto de actividades críticas. [!UICONTROL Milestones] suelen estar asociados a tareas principales. Debe crear los hitos para poder adjuntarlos a las tareas. Para obtener información sobre los hitos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Creación de una trayectoria del hito</a> y <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Asociar hitos a tareas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruta de hitos]</td> 
   <td>Colección de [!UICONTROL milestones]. [!UICONTROL Rutas de hitos] se utiliza en proyectos para distinguir proyectos con ciertos tipos de [!UICONTROL Hitos] de proyectos con un conjunto diferente de [!UICONTROL Hitos].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarea de hito]</td> 
   <td>Una tarea marcada para indicar un evento del que se puede realizar una medición.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Módulo]</td> 
   <td>Un solo paso dentro de un escenario en [!DNL Workfront Fusion] que realiza alguna función basada en la aplicación asociada.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mi función principal]</td> 
   <td> <p>Cuando se hace referencia a esto en los filtros, se muestran los usuarios que tienen la misma función principal [!UICONTROL] que el usuario que ha iniciado sesión, o los elementos de trabajo asignados a la función principal [!UICONTROL] del usuario que ha iniciado sesión.</p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, solo puede generar un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mi equipo de inicio]</td> 
   <td> <p>Cuando se hace referencia a esto en los filtros, este campo muestra los usuarios que pertenecen al [!UICONTROL Equipo de inicio] del usuario que ha iniciado sesión o los elementos de trabajo asignados al [!UICONTROL Equipo de inicio] del usuario que ha iniciado sesión. </p> <p>Se recomienda utilizar este campo en un filtro para que los informes sean más genéricos al compartirlos con otros usuarios. De este modo, solo puede generar un informe que muestre información diferente en función de quién inicia sesión para verlo, ya que la información siempre se personaliza para el usuario que ha iniciado sesión. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convención de nomenclatura]</td> 
   <td>Conjunto de reglas de toda la organización que utilizan datos para crear nombres de proyectos, tareas y entregables.</td> 
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
   <td>En un informe de [!UICONTROL Entrada de cuaderno], se muestra el valor actualizado de un campo que reemplaza al valor de [!UICONTROL Número anterior].
   Para obtener más información, consulte "[!UICONTROL Valor de número anterior]" en este artículo.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Gasto no facturable]</td> 
   <td> <p>Un gasto que no está marcado como facturable al cliente. Puede ser un gasto planificado o un gasto real.</p> <p>Los campos Costo de gasto no facturable planificado y Costo de gasto real no facturable están disponibles para que los agregue a las vistas e informes. No aparecen en las páginas de detalles del proyecto o la tarea.</p>
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
   <td>[!UICONTROL Día no laborable]</td> 
   <td>Un día que no está asignado a la finalización de ninguna asignación. Generalmente es un día de vacaciones, un día festivo o un fin de semana. El término se muestra en el explorador de API. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nota]</td> 
   <td>Un comentario o una actualización realizados en un [!DNL Workfront] objeto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto de nota]</td> 
   <td> <p>Muestra el texto de una actualización introducida por un usuario en cualquier objeto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Número de metas vinculadas]</td> 
   <td> <p>En un informe de [!UICONTROL Project], es el número de objetivos estratégicos asociados al proyecto. Para obtener información sobre cómo asociar proyectos con objetivos estratégicos, consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Agregar proyectos a metas en  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Para obtener información acerca de los objetivos estratégicos, consulte "[!UICONTROL Goal]" en este artículo.</p> 
   <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Agregar proyectos a metas en [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objeto]</td> 
   <td> <p>La información que se muestra en [!DNL Adobe Workfront] se representa mediante objetos que se almacenan en [!DNL Workfront] base de datos. Los objetos son lo que impulsa la información en Workfront. Algunos ejemplos de objetos son los siguientes:</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tareas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Tableros]</li> 
     <li>[!UICONTROL Informes]</li> 
     <li>[!UICONTROL Grupos]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Usuarios]</li> 
     <li>[!UICONTROL Compañías]</li> 
     <li>[!UICONTROL Formularios personalizados]</li>
     <li>[!UICONTROL Campos personalizados]</li>  
     <li>[!UICONTROL Horas]</li> 
     <li>[!UICONTROL Tarifas de facturación]</li> 
     <li>[!UICONTROL Plantillas]</li> 
     <li>[!UICONTROL Tareas de plantilla]</li>

<p><b>NOTA</b></p>
  <p>Esta no es una lista extensa. </p>

</ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipos de objeto]</td> 
   <td>Si crea un informe o una lista que contiene todos los formularios personalizados, puede utilizar este campo como vista o filtro para ver qué tipos de objetos están asociados a cada formulario. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Valor de número anterior]</td> 
   <td>En un informe de [!UICONTROL Journal Entry], se muestra el valor original de un campo antes de que se actualizara. Una vez actualizado el valor de un campo, se mostrará como [!UICONTROL Nuevo valor numérico] en un informe de [!UICONTROL Entrada de cuaderno]. Para obtener más información, consulte "[!UICONTROL Nuevo valor numérico]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Solo al cambiar]</td> 
   <td> <p>Uno de los tipos de [!UICONTROL Project Update]. Si se selecciona esta opción, las escalas de tiempo de [!UICONTROL Proyecto proyectado] y [!UICONTROL Planificado] solo se actualizan cuando se realiza una actualización o cambio en el proyecto o en una tarea del proyecto. No actualiza el proyecto todas las noches.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Tarea de operación de [!UICONTROL]</td> 
   <td> <p>El nombre de [!UICONTROL Issue] en el [!DNL Workfront] base de datos, utilizada en informes de modo de texto o datos personalizados calculados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abrir]</td> 
   <td>Problema o tarea que no se ha completado pero en el que se está trabajando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organigrama]</td> 
   <td>Abreviatura de Organigrama. Es un gráfico que muestra la jerarquía de una organización. También aparece en la ficha de la pantalla de detalles de [!UICONTROL Usuario] que muestra y permite establecer las relaciones de [!UICONTROL Compañía] y [!UICONTROL Informes] del usuario [!UICONTROL].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuración organizativa]</td> 
   <td>Esto define [!UICONTROL Compañías], [!UICONTROL Grupos] y [!UICONTROL Perfiles de seguridad] para su organización.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Otros grupos]</td> 
   <td> <p>En un informe o vista que enumera usuarios, este campo muestra todos los grupos de los que es miembro cada usuario. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Anular moneda]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Rol], esta es la moneda asociada a un rol. Es una anulación de la [!UICONTROL Base Currency] tal como se establece en el área [!UICONTROL Setup] por el método [!DNL Workfront] administrador. </p> 
     <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Anular facturación/hora de moneda]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Rol], es la tarifa por hora de facturación del rol utilizando la [!UICONTROL Moneda de anulación] seleccionada del rol.</p> 
     <p> Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Anular coste/ hora de la moneda]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Rol], es la tarifa de coste por hora del rol utilizando la [!UICONTROL Moneda de anulación] seleccionada del rol. </p> 
     <p>Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Propietario]</td> 
   <td>El usuario responsable de la finalización del objeto designado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Tipo de propietario]</span> </td> 
   <td> 
    <div> 
     <p>En un informe de [!UICONTROL Goal], se muestra el tipo de propietario asignado a un objetivo estratégico. Los siguientes son los tipos de propietario de objetivos:</p> 
     <ul> 
      <li> <p>[!UICONTROL Usuario]</p> </li> 
      <li> <p>[!UICONTROL Equipo] </p> </li> 
      <li> <p>[!UICONTROL Grupo]</p> </li> 
     </ul> 
     <p>No se muestra ningún valor en este campo cuando el propietario de la meta es su organización. </p> 
     <p>Esto requiere una licencia adicional. Para obtener información acerca de [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] descripción general</a>. </p> 
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
   <td>En un informe, este campo muestra información sobre el objeto principal del objeto. Por ejemplo, en un informe de [!UICONTROL issue], puede mostrar información sobre la tarea o el proyecto en el que se ha registrado el problema; en un informe de tareas, puede mostrar información sobre la tarea principal directa o sobre el proyecto. Para obtener más información sobre los objetos que pueden tener elementos primarios en [!DNL Workfront], consulte la sección "Interdependencia y jerarquía de objetos" en el artículo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retardo principal]</td> 
   <td>Cantidad de tiempo que debe transcurrir entre el inicio de la [!UICONTROL Tarea principal] y el inicio de la [!UICONTROL Subtarea].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea principal]</td> 
   <td>También se conoce como [!UICONTROL Summary Task]. Ésta es una tarea que tiene Subtareas (también denominadas [!UICONTROL Tareas secundarias]). La [!UICONTROL Duración], [!UICONTROL Trabajo requerido] y [!UICONTROL Porcentaje completado] de la tarea principal se calcula a partir de las subtareas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Recursos a tiempo parcial]</td> 
   <td>Usuario con licencia que tiene menos capacidad que la programación predeterminada definida en el sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Porcentaje completado]</td> 
   <td> <p>Campo de proyecto, tarea o problema que muestra qué porcentaje del trabajo asociado con la tarea, el proyecto o el problema se ha completado.</p> <p>Puede actualizar este campo manualmente para problemas y tareas de trabajo. </p> <p>Para los proyectos y las tareas principales, este campo es un resumen de todas las tareas de trabajo y no se puede actualizar de forma manual. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Información general sobre el proyecto [!UICONTROL Porcentaje completado]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permiso]</td> 
   <td> <p>Derechos que se conceden a un usuario sobre un objeto, normalmente otorgados para que pueda completar el trabajo en el elemento o verlo. Puede conceder permisos a:</p> 
    <ul> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tareas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programas]</li> 
     <li>[!UICONTROL Informes]</li> 
     <li>[!UICONTROL Tableros]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Vistas]</li> 
     <li>[!UICONTROL Filtros]</li> 
     <li>[!UICONTROL Agrupaciones]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido en objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Es un tipo de licencia completa en la [!DNL Workfront] sistema. Los usuarios deben tener esto para acceder a todas las funciones de [!DNL Workfront].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] información general sobre licencias</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL plan] (en el [!DNL Scenario Planner])</td> 
   <td> <p>Un plan es el objeto principal al trabajar con [!DNL Workfront] Planificador de escenarios. Puede esbozar la estrategia para el futuro a corto y largo plazo de su empresa, identificar cada resultado de alto nivel y añadirlo como plan a la [!DNL Workfront] Planificador de escenarios. </p> <p>No puede mostrar [!DNL Scenario Planner] planes en un informe y no puede acceder a ellos a través del [!DNL Workfront] API. </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">El [!DNL Scenario Planner] descripción general</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planificado]</td> 
   <td> <p>El lapso de tiempo en el que está programado que ocurra algo. Cuando crea proyectos, tareas o problemas en [!DNL Workfront], se establecen las fechas de inicio y finalización planificadas, así como el periodo de tiempo planificado durante el cual se producen. Estos valores representan su intención original o estiman el tiempo que un elemento debería tardar en completarse. </p></td> 
  </tr> 
  <tr> 
   <td>Beneficio planificado de [!UICONTROL]</td> 
   <td>Se trata de una entrada manual para que el administrador del proyecto calcule si la finalización de un proyecto reportaría algún beneficio monetario a la organización. Especificar este valor puede formar parte de la creación de un [!UICONTROL Business Case] para el proyecto. Debe tener permisos de [!UICONTROL Manage] en el proyecto para actualizar este valor.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Horas presupuestadas planificadas]</td> 
   <td> <p>En un informe de [!UICONTROL Hora presupuestada], se muestra el número de horas presupuestadas para proyectos o [!UICONTROL Funciones del trabajo] en el [!UICONTROL Planificador de recursos]. </p> <p>Para obtener información acerca de cómo presupuestar proyectos o roles en [!UICONTROL Resource Planner], vea el artículo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Presupuestar recursos en el [!UICONTROL Planificador de recursos] utilizando las vistas [!UICONTROL Proyecto] y [!UICONTROL Función]</a>. Para obtener información acerca del informe [!UICONTROL Horas presupuestadas], vea el artículo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Informe: Horas presupuestadas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha planificada de finalización]</td> 
   <td> <p>Puede establecer manualmente la [!UICONTROL Fecha planificada de finalización] en una fecha de su elección. Si no establece la [!UICONTROL Fecha planificada de finalización], [!DNL Workfront] lo establece automáticamente. Cuando se establece automáticamente, la fecha planificada de finalización de [!UICONTROL] es: [!UICONTROL Fecha planificada de inicio] + [!UICONTROL Duración]</p> <p>Para obtener más información, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Descripción general de la tarea [!UICONTROL Fecha planificada de finalización]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establecer la fecha planificada de finalización del proyecto [!UICONTROL]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo planificado]</td> 
   <td> <p>Un total del [!UICONTROL Costo de mano de obra planificado] y el [!UICONTROL Costo de gasto planificado] del proyecto. Esto no incluye el [!UICONTROL Costo de riesgo planificado] en el proyecto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duración planificada]</td> 
   <td> <p>La [!UICONTROL Duración planificada] de una tarea suele ser la misma que la [!UICONTROL Duración] de la tarea. Representa la diferencia en días entre el [!UICONTROL Inicio planificado] y las [!UICONTROL Fechas planificadas de finalización] de la tarea. </p> <p>Cuando la tarea tiene un tipo de [!UICONTROL Duración] de [!UICONTROL Condicionada por el esfuerzo], la [!UICONTROL Duración planificada] puede diferir de la [!UICONTROL Duración] de la tarea, en función de cuántos recursos asigne a la tarea. </p> <p>Por ejemplo, si una tarea con un tipo de [!UICONTROL Duración] de [!UICONTROL Condicionada por el esfuerzo] tiene una [!UICONTROL Duración] de 3 días y asigna un recurso con una programación a tiempo completo a la tarea, la [!UICONTROL Duración planificada] también tendrá 3 días. Si asigna tres recursos con una programación a tiempo completo a la misma tarea, la [!UICONTROL Duración] permanece 3 días, pero la [!UICONTROL Duración planificada] pasa a ser 1 día. La Duración planificada de [!UICONTROL] también cambia las fechas de inicio planificado de [!UICONTROL] y de finalización planificada de [!UICONTROL] de la tarea para reflejar la nueva Duración planificada de [!UICONTROL]. Como resultado, la cronología del proyecto también se ve afectada. </p> <p>Para obtener más información acerca de la diferencia entre [!UICONTROL Duración] y [!UICONTROL Duración planificada] para las tareas, vea el artículo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Diferencia entre [!UICONTROL Duración planificada] y [!UICONTROL Duración] para tareas</a>.</p> <p>Los proyectos y problemas no tienen una duración planificada de [!UICONTROL]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duración planificada en minutos]</td> 
   <td> <p>La [!UICONTROL Duración planificada en minutos] de un proyecto o un problema es la [!UICONTROL Duración] del proyecto o problema en minutos. </p> <p>Las tareas no tienen un campo de [!UICONTROL Duración planificada en minutos]. </p> <p>Las [!UICONTROL Tareas de plantilla] tienen un campo de [!UICONTROL Duración planificada en minutos] que muestra la [!UICONTROL Duración planificada] de la tarea en minutos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de gasto planificado]</td> 
   <td> <p>Suma de [!UICONTROL Cantidades planificadas] para todos los gastos registrados de un proyecto o tarea.</p> <p><b>EJEMPLO</b></p>
   <p>Si crea un gasto para la Tarea 1 y escribe 600,00 $ en el campo [!UICONTROL Importe planificado], el costo de gasto planificado de [!UICONTROL] para esta tarea es 600,00 $. </p> 
   <p>Para un proyecto, [!DNL Workfront] utiliza la fórmula siguiente para calcular [!UICONTROL Costo de gasto planificado]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horas planificadas]</td> 
   <td> <p>Este campo aparece en las áreas de [!UICONTROL proyectos], [!UICONTROL tareas] y problemas, informes de proyectos, tareas o problemas y herramientas de administración de recursos como [!UICONTROL Planificador de recursos], [!UICONTROL Distribuidor de cargas de trabajo] y el informe [!UICONTROL Utilización]. </p> <p>Muestra el número de horas que el propietario del proyecto estima que cada tarea o problema debería tardar en completarse. En los proyectos, suele ser un resumen de las [!UICONTROL Horas planificadas] de las tareas del proyecto. </p> <p>El campo [!UICONTROL Horas planificadas] puede mostrar información diferente según el lugar desde el que se vea. Para obtener información sobre las horas planificadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Resumen de horas planificadas</a>.</p> <p>Las horas planificadas se almacenan en minutos en el [!DNL Workfront] base de datos. Al escribir cálculos utilizando este campo, asegúrese de que tiene en cuenta el hecho de que las horas se muestran como minutos.<br></p> <p>De forma predeterminada, las horas planificadas se distribuyen de forma equitativa a todos los días dentro de la duración de un elemento de trabajo y también de forma equitativa para todos los recursos asignados a la tarea. Los usuarios pueden actualizar el número diario de horas planificadas para un elemento de trabajo o las horas planificadas individuales para cada usuario asignado.</p> <p>La actualización de este campo difiere para los proyectos, las tareas y los problemas: </p> 
    <ul> 
     <li> <p>Para los problemas, puede actualizar manualmente este campo. Las horas planificadas de problema no se agregan a las horas planificadas del proyecto. </p> <p><b>SUGERENCIA</b></p> <p>En un informe de problemas, uno de los campos [!UICONTROL Horas planificadas] se reemplaza por el campo [!UICONTROL Trabajo]. El campo muestra la cantidad de horas planificadas sobre el problema. Para obtener más información, consulte los campos "trabajo" o "[!UICONTROL Trabajo]" en esta tabla. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para las tareas, puede actualizar manualmente este campo cuando el [!UICONTROL Duration Type] de la tarea sea [!UICONTROL Calculated Assignment] o [!UICONTROL Simple]. Este campo se calcula por [!DNL Workfront] cuando el [!UICONTROL Tipo de duración] de la tarea es [!UICONTROL Trabajo calculado] o [!UICONTROL Condicionado por el esfuerzo].<br>Para obtener información acerca de [!UICONTROL Duración de la tarea], vea el artículo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la tarea [!UICONTROL Duración] y [!UICONTROL Tipo de duración]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Para proyectos, [!DNL Workfront] calcula las horas planificadas agregando todas las horas planificadas de todas las tareas del proyecto. </p> </li> 
    </ul> <p><b>SUGERENCIA</b></p> <p>También puede mostrar las [!UICONTROL Horas planificadas] en los informes de [!UICONTROL proyecto], [!UICONTROL tarea] o [!UICONTROL problemas] utilizando el modo de texto y haciendo referencia a campos adicionales. Para obtener más información, consulte el "<code>work</code>", "[!UICONTROL Work]" y "<code>workRequiredExpression</code>" en esta tabla. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de mano de obra planificado]</td> 
   <td> 
    <p>Para una tarea, la tasa por hora del usuario o rol multiplicada por el número de horas asignadas al usuario o rol.</p> <p>Para un proyecto, es un total de todos los [!UICONTROL Costos de mano de obra planificados] de todas las tareas.</p> <p>El uso de la tasa del usuario o rol depende del tipo de costo seleccionado para la tarea dada. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de [!UICONTROL]</td> 
   <td> <p>Las tareas y los proyectos pueden mostrar un valor para [!UICONTROL Ingresos planificados] en [!DNL Workfront]. [!UICONTROL Ingresos planificados] representa la cantidad de dinero asociada con las [!UICONTROL Horas planificadas] de las tareas del proyecto. Para los proyectos, también puede incluir los [!UICONTROL Fixed Revenue] del proyecto. </p> <p>En el caso de las tareas, estos son los ingresos asociados con las [!UICONTROL Horas planificadas] de tareas. Las horas planificadas de todas las tareas se acumulan en las horas planificadas del proyecto para contribuir al cálculo de las [!UICONTROL Horas planificadas] del proyecto. </p> 
   <p>[!DNL Workfront] calcula [!UICONTROL Ingresos planificados] para tareas y proyectos mediante las fórmulas siguientes:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Los [!UICONTROL Ingresos planificados] del proyecto que se muestran en el área [!UICONTROL Detalles del proyecto] y en los informes de proyecto difieren de los ingresos planificados que se muestran en el informe [!UICONTROL Utilización]. </p> <p>Los [!UICONTROL Ingresos planificados] del área [!UICONTROL Detalles del proyecto] reflejan los ingresos de la tarea así como los ingresos fijos del proyecto. Los [!UICONTROL Ingresos planificados] del [!UICONTROL Informe de utilización] muestran los [!UICONTROL Ingresos planificados] asociados únicamente a las tareas del proyecto. </p> 
     <p><b>EJEMPLO</b></p>  
      <p>Si el proyecto tiene 1 tarea con 10 horas, asignada a un consultor con una tarifa por hora de 20 $ y el proyecto tiene 100 $ de [!UICONTROL Ingresos fijos], el informe de [!UICONTROL Utilización] muestra 200 $ para los [!UICONTROL Ingresos planificados] (los [!UICONTROL Ingresos planificados] asociados con las horas de la tarea). La sección [!UICONTROL Detalles del proyecto] muestra 300 $ (los [!UICONTROL Ingresos planificados] de la tarea y los ingresos fijos del proyecto). </p> 
    <p>Para obtener información sobre el seguimiento de ingresos en [!DNL Workfront] consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Resumen de facturación e ingresos</a>. </p> 
    <p>Para obtener información acerca de los cálculos de [!UICONTROL Ingresos planificados] en el informe Utilización de [!UICONTROL], consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ver información de utilización de recursos </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de riesgo planificado]</td> 
   <td> <p>El total del [!UICONTROL Costo potencial] de todos los riesgos en el proyecto teniendo en cuenta su probabilidad de que ocurran. Esta cantidad no se incluye en el [!UICONTROL Costo planificado] del proyecto.</p> <p>El [!UICONTROL Costo de riesgo planificado] de un proyecto se calcula mediante la siguiente fórmula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil de portal]</td> 
   <td>Colección definida por el administrador de fichas y secciones de portal que aparece en la [!DNL Workfront] Aplicación [!UICONTROL Home] y otros paneles.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sección de portal]</td> 
   <td>Un componente de una ficha en un panel o página de portal. Generalmente, un solo informe, gráfico, calendario o lista de información clave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Ficha de un portal o panel que contiene hasta tres secciones de portal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Colección de proyectos que tienen características unificadoras. Estos proyectos suelen competir por los mismos recursos, presupuesto o franja horaria. Puede dividir Portfolio en Programas y asociar los proyectos con los Programas antes de agregarlos a un Portfolio.</p> <p>Para obtener más información sobre los portafolios, consulte <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Información general del Portfolio en [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Administración de Portfolio]</td> 
   <td>Área de práctica centrada en administrar una colección o programas relacionados y esfuerzos de proyecto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>A [!DNL Workfront] herramienta para ayudar a evaluar y priorizar proyectos dentro de un portafolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Propietario del Portfolio]</td> 
   <td>La parte interesada responsable de la priorización y el presupuesto de una cartera.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo de riesgo potencial]</td> 
   <td>Este es un campo de proyecto que se puede localizar en listas e informes. Muestra el coste potencial de los riesgos asociados con el proyecto, en caso de que se produzcan. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular costo de riesgo potencial </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecesora]</td> 
   <td> <p>Tarea que debe completarse antes de finalizar una tarea dependiente. También es una tarea que está marcada como [!UICONTROL Dependencia] para otra tarea. Las tareas predecesoras permiten al planificador establecer una lógica de dependencia de secuencias, como iniciar una tarea una vez finalizada otra.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Información general sobre predecesoras de tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compañía principal]</td> 
   <td>Compañía a la que pertenece el usuario según lo designado en su configuración de usuario. Las empresas también pueden asociarse a proyectos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contacto principal]</td> 
   <td><p>El [!UICONTROL Primary Contact] es el creador de un problema y lo designa automáticamente [!DNL Workfront] cuando alguien crea el problema. Puede actualizar manualmente este campo si tiene [!DNL Manage] permisos para el problema. Un problema solo puede tener un contacto principal.</p> 
   <p>Si cambia el Contacto principal, el usuario designado originalmente como contacto principal seguirá teniendo acceso al problema con [!UICONTROL Manage].</p>
   <p>Al convertir un problema en una tarea o un proyecto, el usuario designado como [!UICONTROL Contacto principal] del problema se convierte en el [!UICONTROL Creador de problema convertido] del proyecto o tarea. Si el [!UICONTROL Contacto principal] del problema se actualiza después de convertirlo, el [!UICONTROL Creador de problema convertido] se conservará como el [!UICONTROL Contacto principal] del problema en el momento en que se produjo la conversión. Consulte también "[!UICONTROL Creador de problema convertido]" en este artículo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Prioridad]</td> 
   <td>Un valor que se puede asignar a una tarea, problema o proyecto para designar la importancia que tiene. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privado]</td> 
   <td>En un [!UICONTROL Note] o [!UICONTROL Document], esta opción oculta ese objeto a la mayoría de los visualizadores. Para una cola de solicitudes de ayuda privada, sólo los usuarios del equipo del proyecto pueden enviar problemas a esa cola (o proyecto) a través del área de [!UICONTROL Solicitudes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil]</td> 
   <td>Toda la información sobre una cuenta de usuario.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Programa]</td> 
   <td> <p>Un subconjunto dentro de un portafolio, donde proyectos similares pueden agruparse para lograr un beneficio bien definido.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Administración de programas]</td> 
   <td>Gestión de dependencias, riesgos, problemas, requisitos y soluciones entre proyectos para mantener el programa en buen estado y lograr el beneficio definido del programa.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Propietario del programa]</td> 
   <td>La parte interesada responsable de supervisar y organizar las actividades para garantizar que los objetivos del proyecto se ajusten a los objetivos de la empresa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progreso]</span> </td> 
   <td> <p>En un informe de [!UICONTROL Goal], muestra el porcentaje de lo cerca que está un objetivo estratégico de completarse. El porcentaje de progreso se muestra como un número. Para obtener información acerca de los objetivos estratégicos, consulte "[!UICONTROL Goal]" en esta tabla.</p> <p>Este campo solo está visible si su organización ha adquirido [!DNL Workfront] Metas. Para obtener información sobre la administración de objetivos estratégicos con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Agregar proyectos a metas en [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado de progreso]</td> 
   <td> <p>En los informes Proyecto, Tarea y Objetivo, este campo muestra el estado de progreso de los proyectos, tareas u objetivos estratégicos. Para obtener más información, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Resumen del estado del progreso del proyecto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Resumen del estado de progreso de tareas</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Información general sobre el progreso y la condición de la meta en [!DNL Adobe Workfront Goals]</a> </p>
     <p>El informe [!UICONTROL Goal] y el estado de progreso de [!UICONTROL] para [!DNL goals] Los campos de solo son visibles si su organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre los objetivos estratégicos en [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] descripción general</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Proyecto]</td> 
   <td> <p>Una gran cantidad de trabajo que debe completarse dentro de un marco de tiempo específico y debe utilizar un presupuesto y un número de recursos específicos. Para hacerlo manejable, se divide el proyecto en una serie de tareas. Completar todas las tareas significa la finalización del proyecto. Para obtener información sobre la planificación de un proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Información general sobre la planificación de un proyecto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horas planificadas de asignación del proyecto]</td> 
   <td> <p>En un informe de [!UICONTROL Rol de la iniciativa], se muestra el número de [!UICONTROL Horas planificadas] asociadas a un rol asignado a tareas o problemas del proyecto. Este campo y el tipo de informe [!UICONTROL Initiative Job Role] no se muestran en su [!DNL Workfront] a menos que su empresa haya adquirido un [!DNL Workfront Scenario Planner] licencia. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md">El [!DNL Workfront Scenario Planner] descripción general</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detalles del proyecto]</td> 
   <td>Los detalles del estado actual de un proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo presupuestado de proyecto]</td> 
   <td> <p> Es el [!UICONTROL Costo presupuestado] de un proyecto tal como se muestra en listas e informes.</p><p>Consulte también "[!UICONTROL Costo presupuestado]" en este artículo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Administración de proyectos]</td> 
   <td>Conjunto de directivas que rige los umbrales para la creación, categorización y denominación de proyectos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Costes generales del proyecto]</td> 
   <td>En un informe de [!UICONTROL Hour], este campo se reserva para la información financiera vinculada a las horas registradas con el tipo de hora de [!UICONTROL Project Time]. Los proyectos pueden tener sus propias Tarifas de facturación y si se registra una hora directamente en un proyecto, esas tarifas se utilizarán en los cálculos. En función de la configuración del proyecto, los proyectos también pueden tener distintas monedas y puede haber una conversión de moneda para esas horas. El objeto [!UICONTROL Project Overhead] permite [!DNL Workfront] para obtener esa información.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propietario del proyecto]</td> 
   <td>Usuario responsable de administrar el ámbito, la cronología y las asignaciones de un proyecto. Aprobador predeterminado para pedidos de cambio, cambios financieros y entregables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planificación de proyectos]</td> 
   <td>Procesos para desarrollar y mantener la programación del proyecto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Patrocinador de proyecto]</td> 
   <td>Un perfil de partes interesadas designado al que debe estar relacionado cada uno de los usuarios. Entrada [!DNL Workfront], estos se designan como [!UICONTROL Niveles de acceso]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Equipos del proyecto]</td> 
   <td> <p>Colección de usuarios o funciones asignadas a un proyecto</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Información general del equipo del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seguimiento de proyectos]</td> 
   <td>Los datos utilizados para medir el estado y el alcance de un proyecto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proyectado]</td> 
   <td> <p>Una estimación de la marca de tiempo del momento en que se completará el trabajo en función de las horas planificadas y el porcentaje completado de una tarea, problema o proyecto.</p> <p>Hace referencia a fechas o a la [!UICONTROL Duración] de tareas, problemas o proyectos. Normalmente, designa fechas y duraciones más fieles a la vida útil de los elementos de trabajo, después de que ya se haya completado algún trabajo o haya transcurrido algún tiempo. </p> <p>Por ejemplo, la [!UICONTROL Fecha proyectada de finalización] de una tarea es la fecha en la que [!DNL Workfront] estima que la tarea se completará, en función del trabajo realizado en ella hasta el momento, la cantidad de personas asignadas y el tiempo transcurrido desde la fecha de inicio.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plazo de revisión]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el día de la semana, la fecha, la hora del día y el año de la fecha límite de la prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisión de revisión]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el estado de decisión de la prueba (pendiente, cambios necesarios o aprobados)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de revisión]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el nombre de la prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Páginas de revisión]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), este campo muestra el número de páginas incluidas en la prueba.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progreso de revisión]</td> 
   <td> <p>En los informes que contienen el objeto [!UICONTROL Document Version] (como un informe [!UICONTROL Document Version] y un informe [!UICONTROL Proof Approval]), muestra el estado de progreso de la prueba ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Resumen del progreso de prueba</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Progreso de prueba e información general de estado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revisión]</td> 
   <td>Proceso de revisión en el que uno o varios usuarios marcan y comentan contenido que debe cambiarse en una imagen, un documento de texto, un vídeo o contenido web interactivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>En un [!UICONTROL Note] o [!UICONTROL Document], esta opción hace que el objeto sea accesible para otros usuarios o incluso para personas externas [!DNL Workfront]. Para una cola de solicitudes de ayuda de [!UICONTROL], [!UICONTROL Public] significa que todos los usuarios que pueden enviar problemas a un proyecto pueden enviarlos a través del área de solicitudes de [!UICONTROL].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Calidad]</td> 
   <td>La percepción de la calidad del trabajo dentro de la organización.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cola]</td> 
   <td>También se denomina Cola del servicio de asistencia o Cola de solicitudes de ayuda de [!UICONTROL]. Este es un proyecto que se ha publicado en el área de [!UICONTROL Solicitudes] para permitir que los usuarios envíen problemas. Normalmente, las colas se crean para temas concretos, como [!UICONTROL Bugs], [!UICONTROL Solicitudes de proyectos], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propiedades de cola]</td> 
   <td>Esta configuración define las reglas de envío de problemas para un proyecto que se publica en el área de [!UICONTROL Solicitudes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tema de cola]</td> 
   <td> <p>Propiedad de una cola de solicitudes de ayuda de [!UICONTROL] que permite a los usuarios que envían un problema seleccionar un tema. Los temas pueden:</p> 
    <ul> 
     <li>Debe asociarse con un formulario de datos personalizado.</li> 
     <li>Asigne el problema automáticamente a un usuario, rol o equipo a través del conjunto de reglas de enrutamiento en el tema seleccionado.</li> 
     <li>Mover el problema a otro proyecto o cola a través del conjunto de reglas de enrutamiento del tema seleccionado.</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crear temas de cola</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rango]</td> 
   <td> <p>En un informe de [!UICONTROL Nivel de acceso], puede indicar manualmente un [!UICONTROL Rango] del [!UICONTROL Nivel de acceso]. Esto le ayuda, ya que [!DNL Workfront] para identificar visualmente el nivel de complejidad asociado con cada nivel de acceso. Por ejemplo, puede proporcionar números menores para niveles de acceso más complejos ([!UICONTROL Plan]-level) y números mayores para niveles de acceso menos complejos ([!UICONTROL Requester]-level). No puede clasificar los niveles de acceso estándar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Este campo de un informe de tareas indica si una tarea de [!UICONTROL Agile] se ha marcado como [!UICONTROL Ready] en el registro de pendientes. Este indicador solo se aplica a las tareas de [!UICONTROL Agile], que son tareas asignadas a un equipo de [!UICONTROL Agile]. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frecuencia de periodicidad]</td> 
   <td> <p>Campo que se muestra en el cuadro [!UICONTROL Detalles de tarea] o [!UICONTROL Editar tarea] de un elemento primario de tareas recurrentes. Es la frecuencia con la que ocurren las tareas en la periodicidad. Para obtener información sobre la creación de tareas recurrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creación de tareas recurrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de referencia]</td> 
   <td> <p>Los proyectos, las tareas y los problemas se asocian automáticamente con un número de referencia único a medida que se crean. Puede ver el [!UICONTROL Número de referencia] en la página de [!UICONTROL Detalles] de proyectos, tareas o problemas, o en una lista o informe. </p> <p><b>SUGERENCIA</b><p><br>Se puede diferir a los números de referencia cuando dos elementos tengan el mismo nombre, ya que los números de referencia son siempre únicos. </p> <p>[!DNL Workfront] genera automáticamente números de referencia secuenciales a nivel del sistema. Cada proyecto, tarea o problema obtiene el siguiente número disponible en la secuencia. <br></p> <p>Por ejemplo, si el usuario A crea una tarea, [!DNL Workfront] puede asignar automáticamente a la tarea el número de referencia 100. Si el usuario B crea un problema justo después de esto, [!DNL Workfront] asigna al problema el número de referencia 101. No se pueden editar manualmente los números de referencia. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema de rechazo]</td> 
   <td>En un proyecto o informe de tarea, este es el problema que se crea cuando se rechaza la aprobación del proyecto o la tarea. Para obtener información sobre los problemas de rechazo, consulte el artículo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Crear un proceso de aprobación para elementos de trabajo</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo de riesgo restante]</td> 
   <td> <p>Campo de proyecto que muestra la diferencia entre el [!UICONTROL Costo de riesgo planificado] de un proyecto y el total de todos los [!UICONTROL Costos reales] de todos los riesgos del proyecto. </p> <p>El [!UICONTROL Costo de riesgo restante] de un proyecto se calcula mediante la fórmula siguiente:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Replanificación]</td> 
   <td>Cambiar las fechas de un proyecto para reparar o superar problemas. Por ejemplo, un proyecto que ha estado en espera durante varios meses tendría que volver a planificarse para reflejar las fechas precisas. Es una operación manual de ajustar las fechas del proyecto o las de las tareas. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Informe]</td> 
   <td>Gráfico o tabla que contiene información sobre un determinado [!DNL Workfront] y sus atributos relacionados.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Solicitud]</td> 
   <td> <p>Tipo de problema que se clasifica en una sola cola centralizada y que no está relacionado con un esfuerzo de trabajo en curso.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Cola de solicitudes]</td> 
   <td>El registro de problemas pendientes que se administra mediante un proceso de tráfico y clasificación.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Velocidad de solicitud]</td> 
   <td>Tiempo total del ciclo de trabajo para ingerir y completar una solicitud.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Solicitante]</td> 
   <td>Normalmente es un tipo de licencia. Un usuario con una licencia de solicitante puede enviar solicitudes para que se produzcan nuevos trabajos en el sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo reservado]</td> 
   <td>Días especificados en el horario personal de un usuario, lo que indica que el usuario no estará disponible para trabajar. Consulte "[!UICONTROL Días no laborables]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver problema]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia al problema que resuelve el problema. </p> <p>Para obtener información sobre la visualización de objetos de resolución en los informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información de objetos solucionables y de resolución en un informe</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver proyecto]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia al proyecto que resuelve el problema. </p> <p>Para obtener información sobre la visualización de objetos de resolución en los informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información de objetos solucionables y de resolución en un informe</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolver tarea]</td> 
   <td> <p>En un informe de problemas, utilice este campo en vistas o filtros para hacer referencia a la tarea que resuelve el problema. </p> <p>Para obtener información sobre la visualización de objetos de resolución en los informes, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Ver información de objetos solucionables y de resolución en un informe</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso]</td> 
   <td>Usuarios o funciones que existen en [!DNL Workfront] y se asignan a equipos de proyecto, tareas y problemas. Son responsables de completar el trabajo asociado con proyectos, tareas o problemas. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Administración de recursos]</td> 
   <td> <p>[!UICONTROL Resource Management] es un conjunto de herramientas empresariales que le permite prever con precisión el uso de los recursos en función de su disponibilidad, de modo que el trabajo que debe realizarse se complete a tiempo y según el presupuesto. </p> <p>Con las herramientas de gestión de recursos, puede planificar las necesidades de capacidad a largo plazo y de programación a corto plazo de sus recursos. </p> <p>Para obtener información sobre la administración de recursos en [!DNL Workfront], consulte <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introducción a la administración de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de gerentes de recursos]</td> 
   <td><p>En un informe de proyecto, puede utilizar esta opción al crear un filtro para buscar un administrador de recursos específico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gerentes de recursos]</td> 
   <td> <p>En un informe de proyecto o vista de lista, se trata de un campo informativo que muestra los usuarios designados para realizar actividades de administración de recursos en el proyecto.  Cuando se usa "[!UICONTROL Resource Managers]" en un informe, se muestra una lista de administradores de recursos, separados con comas cada uno de los administradores de recursos del proyecto. Puede designar hasta 30 administradores de recursos en un proyecto determinado.</p> <p>Para obtener más información, consulte el artículo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designar gerentes de recursos para un proyecto o plantilla </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Horas presupuestadas del planificador de recursos] </td> 
   <td>Horas presupuestadas para el proyecto y recursos asociados con él en el [!UICONTROL Resource Planner]. Consulte también "[!UICONTROL Horas presupuestadas]" en este artículo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Planificador de recursos] </td> 
   <td>Un avanzado [!DNL Workfront] herramienta que le permite ver y administrar recursos entre proyectos, roles o usuarios. Para obtener más información, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resumen del Planificador de recursos</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planificador de recursos Costo de mano de obra presupuestado]</td> 
   <td> <p>Es el costo asociado con las horas presupuestadas para los roles del proyecto que se usan en el Planificador de recursos. </p> <p>Consulte también "Coste laboral presupuestado" en este artículo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Conjuntos de recursos]</td> 
   <td> <p>Los conjuntos de recursos son conjuntos de usuarios que se pueden asociar a un proyecto. Los usuarios del mismo conjunto de recursos suelen pertenecer al mismo departamento, tener aptitudes similares o complementarias o estar financiados con cargo al mismo presupuesto. Puede asociar varios conjuntos de recursos a un proyecto o a un usuario. Un conjunto de recursos se puede asignar exclusivamente a un proyecto o compartir en varios proyectos.</p> 
   <p>Para obtener más información sobre los conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resumen de conjuntos de recursos </a>.</p> 
   <p>En los informes de proyecto, los conjuntos de recursos muestran todos los conjuntos asociados a un proyecto. Este objeto no se puede utilizar en una agrupación.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilización de recursos]</td> 
   <td>Informe que muestra la cantidad de horas disponibles durante un período de tiempo determinado y la cantidad de horas programadas para cada usuario en el informe. Esto también se calcula en [!UICONTROL Horas promedio por día] y un porcentaje de asignación.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Resultado]</td> 
   <td>Entrada [!DNL Workfront Goals], un resultado es un indicador de progreso para una meta. Puede ser un número, un valor porcentual o una cantidad de moneda que actualice manualmente. No puede mostrar los resultados en un informe y no puede acceder a ellos a través del [!DNL Workfront] API. Para obtener información sobre las actividades, consulte <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introducción a resultados y actividades en Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ingresos]</td> 
   <td>Un importe facturable por la tarea o el proyecto. La cantidad puede ser por hora, fija o una combinación de ambas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de ingresos]</td> 
   <td>El tipo de ingresos determina cómo devengará ingresos la tarea. Algunos ejemplos son [!UICONTROL Fijo por hora], [!UICONTROL Rol por hora] y [!UICONTROL Rol por hora sin tope]. Para obtener información sobre el seguimiento de ingresos en [!DNL Workfront] consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Resumen de facturación e ingresos</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revisor]</td> 
   <td>Normalmente es un tipo de licencia. Un usuario con una licencia de [!UICONTROL Reviewer] tiene la capacidad de revisar y aprobar elementos de trabajo en el sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Riesgo]</td> 
   <td> <p>Puede referirse a los siguientes conceptos en [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Campo de un proyecto que indica lo riesgoso que puede ser un proyecto. Puede priorizar la ejecución de sus proyectos en función del nivel de riesgo. Los proyectos pueden tener los siguientes niveles de riesgo:</p> <p>- [!UICONTROL Muy bajo]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medio]</p> <p>- [!UICONTROL Alta]</p> <p>- [!UICONTROL Muy alto]</p> <p>Los niveles de riesgos que indique para un proyecto no se pueden personalizar. </p> <p> Para obtener información sobre cómo actualizar el riesgo de un proyecto, consulte la sección "Configuración del proyecto" del artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>. Puede mostrar el campo de riesgo de un proyecto en los informes. </p> </li> 
     <li> <p>Evento que puede producirse durante la duración de un proyecto y que identifica un impacto potencial en el costo, el ámbito o la programación del proyecto. Defina los riesgos potenciales para un proyecto y asocie una probabilidad de que se produzcan o un coste a medida que crea el caso comercial del proyecto. Para obtener información sobre cómo agregar riesgos al caso empresarial del proyecto, consulte "Crear y editar riesgos en proyectos". </p> <p>No se pueden mostrar los riesgos definidos en [!UICONTROL Business Case] en los informes. Sólo se pueden mostrar varios tipos de costos de riesgo en informes y listas. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo de riesgo]</td> 
   <td> <p>Coste asociado con los riesgos de un proyecto. A continuación se indican los costos de riesgo asociados con los proyectos que se pueden mostrar en los informes:</p> 
    <ul> 
     <li> <p>[!UICONTROL Costo real]: campo de un riesgo que muestra el costo real del riesgo que se ha producido. Además de los informes y las listas, puede localizarlos en el cuadro [!UICONTROL Editar riesgo] al editar o crear un riesgo. </p> <p>Para costos de proyecto, tarea o problema, vea "[!UICONTROL Costo real]" en este artículo. </p> </li> 
     <li> <p>[!UICONTROL Costo de riesgo planificado]: campo del proyecto que muestra un total de todos los [!UICONTROL Costo de riesgo potencial] del proyecto. Consulte también "[!UICONTROL Costo de riesgo planificado]" en este artículo. </p> <p>Para obtener información sobre el costo de riesgo potencial, consulte <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular costo de riesgo potencial </a>. </p> </li> 
     <li> <p>[!UICONTROL Costo de riesgo restante]: campo del proyecto que muestra la diferencia entre el total de [!UICONTROL Costo real] de todos los riesgos y el [!UICONTROL Costo de riesgo planificado]. Consulte también "Costo de riesgo restante" en este artículo. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Administración de riesgos]</td> 
   <td>Procesos para identificar, mitigar y supervisar el riesgo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Función]</td> 
   <td>Consulte "[!UICONTROL Rol]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enrutamiento]</td> 
   <td>Asignar o mover automáticamente un problema, normalmente debido a un tema de la cola o como ruta predeterminada (regla de enrutamiento) para la cola.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Regla de enrutamiento]</td> 
   <td>Configuración de proyectos y temas de colas que asigna automáticamente un problema a un usuario, rol o equipo, o mueve el problema a otro proyecto o tema de la cola. Las reglas de enrutamiento se utilizan generalmente con colas de solicitudes de ayuda para asignar automáticamente problemas entrantes.</td> 
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
   <td>Una búsqueda cuyos criterios de búsqueda se hayan guardado. Las búsquedas guardadas facilitan la ejecución del mismo cada vez sin tener que volver a introducir los criterios de búsqueda.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Escenario] (en [!DNL Workfront Fusion]) </td> 
   <td> <p>Un escenario se compone de una serie de pasos (módulos) que indican cómo se deben transferir y transformar los datos entre aplicaciones o servicios.</p> <p>Para obtener información sobre escenarios en [!DNL Workfront Fusion], consulte <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] descripción general del escenario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Escenario] (en el [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>En el [!DNL Scenario Planner], un escenario es una copia de un plan. </p> <p>El [!DNL Scenario Planner] requiere una licencia adicional. Para obtener más información sobre [!DNL Workfront Scenario Planner], consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">El [!DNL Scenario Planner] descripción general</a>. </p> <p>Para obtener información sobre la creación de escenarios, consulte <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Cree y compare escenarios de plan en la [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Programación]</td> 
   <td>El horario de trabajo semanal, incluyendo los tiempos de trabajo, combinado con los días libres (tales como días festivos) y los días de excepción (tales como un día laborable sábado). Puede asociar programaciones con proyectos y usuarios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exención de horario]</td> 
   <td>También se conoce como [!UICONTROL Modified Shift]. Días programados, a diferencia de los tiempos de trabajo semanales normales definidos por el horario. Por ejemplo, un sábado programado para trabajar, cuando el horario está configurado para trabajar únicamente de lunes a viernes, sería una [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Informe programado]</td> 
   <td> <p>Cuando se genera un informe de informes, se puede mostrar información sobre las programaciones del informe, si está programado para su envío, utilizando el campo [!UICONTROL Informe programado]. Este campo muestra varios valores, uno para cada programación de cada informe, en una lista con viñetas. Para obtener más información sobre la programación de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Resumen de entrega de informes</a>.</p> <p>Dado que este campo muestra varios valores, no se puede utilizar en una agrupación. Solo puede acceder a él en un filtro o una vista. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambio de ámbito]</td> 
   <td>Una pista de auditoría de [!UICONTROL] que, si está activa, genera una nota cada vez que se realiza un cambio en el ámbito de un proyecto o tarea, como si se cambia una [!UICONTROL Duración de la tarea] o las [!UICONTROL Predecesoras].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sección]</td> 
   <td>Área de la pantalla, con su propio encabezado, creada para organizar los datos personalizados con fines de visualización.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salto de sección]</td> 
   <td>Un espacio o borde entre secciones.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>Configuración que permite al usuario interactuar con determinados objetos del sistema y no con otros. Consulte también "[!UICONTROL Niveles de acceso]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuración]</td> 
   <td>Área en la que los administradores pueden definir las configuraciones y preferencias del sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gravedad]</td> 
   <td> <p>[!UICONTROL Gravedad] es una indicación de la probabilidad de que un elemento afecte a la finalización del trabajo. Por ejemplo, un problema con una gravedad alta de [!UICONTROL] puede bloquear por completo la finalización de una tarea, pero un problema con una gravedad baja de [!UICONTROL] puede ser meramente estético.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Actualizar gravedad del problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gravedades]</td> 
   <td>Consulte "[!UICONTROL Gravedad]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>Uso compartido de [!UICONTROL]</td> 
   <td>Acción de permitir que otros usuarios vean o editen un elemento específico en [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de Slack]</td> 
   <td>En una vista de tareas o informe, [!UICONTROL Fecha de Slack] muestra la fecha exacta en la que una tarea podría afectar definitivamente a la [!UICONTROL Fecha de finalización] del proyecto. Para obtener información acerca de la [!UICONTROL Fecha de Slack] de una tarea, consulte <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Resumen de fecha de Slack de tarea</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asignaciones inteligentes]</td> 
   <td> <p>Al asignar tareas o problemas a los usuarios, [!DNL Workfront] hace recomendaciones ([!UICONTROL Smart Assignments]) sobre quiénes son los mejores usuarios para completar el trabajo, en función del tiempo que tengan disponible para completarlo y de su relación con el proyecto.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Información general sobre asignaciones inteligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Origen]</td> 
   <td> <p>Indica el objeto principal de otro objeto. Por ejemplo, un documento adjunto a una tarea tiene el nombre de la tarea en el campo [!UICONTROL Origen] de un informe o vista de [!UICONTROL Documento]; un problema registrado en un proyecto tiene el nombre del proyecto en el campo [!UICONTROL Origen] de un informe o vista de problema. </p> 
   <p>Los siguientes informes muestran una columna Origen en la que puede ver información sobre el objeto principal:</p>
  <ul><li>Informes de problemas</li>
    <li>Informes por hora</li>
    <li>Informes de documentos </li>
    </ul>
   <p>Si los usuarios no tienen permisos para el objeto principal de un problema, hora o documento, la columna Origen del informe se muestra vacía, incluso cuando el informe está configurado para mostrarse o para entregarse con los derechos de acceso de otro usuario. </p>
   <p> Para mostrar información sobre el objeto principal en el informe, se recomienda añadir una columna para el objeto principal en la que se pueda mostrar el nombre del objeto principal. </p>
    <p>Por ejemplo, puede agregar cualquiera de las siguientes opciones a un informe con una columna Origen: </p>
    <ul><li>Las columnas Nombre del proyecto, Nombre de tarea o Nombre del problema se transfieren a un documento o informe de horas.</li>
    <li>Las columnas Nombre del proyecto o Nombre de tarea se transfieren a un informe de problemas. </li> </ul>
    Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Ejecutar y entregar un informe con los derechos de acceso de otro usuario</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de inicio]</td> 
   <td> <p>La fecha en la que está establecido el inicio del trabajo en un elemento. Hay varias fechas de inicio en [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planificado]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Proyectado] </li> 
    </ul> <p>En un informe de tasas de [!UICONTROL], esta es la fecha en la que se inicia una nueva tasa de facturación para un rol en el nivel de proyecto. Las horas asociadas con el proyecto que son posteriores a esta fecha se multiplican por esta tarifa de facturación para calcular los ingresos del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estado]</td> 
   <td> <p>Indicador utilizado para indicar la posición del flujo de trabajo de un elemento de trabajo o de un objetivo estratégico.</p> <p>Para los proyectos, [!UICONTROL Estado] es una configuración del proyecto que indica si el proyecto es:</p> 
    <ul> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL En espera] </li> 
     <li>[!UICONTROL Completo] </li> 
     <li>[!UICONTROL Inactivo]</li> 
    </ul> <p>Para obtener más información sobre el estado de un proyecto, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Acceso a la lista de estados de proyectos del sistema</a>.</p>
    <p>Para las tareas, [!UICONTROL Estado] es una configuración de la tarea que indica si la tarea es:</p> 
    <ul> 
     <li>[!UICONTROL Nuevo]</li> 
     <li>[!UICONTROL En Curso]</li> 
     <li>[!UICONTROL Completo]</li> 
    </ul> <p>Para obtener más información sobre el estado de la tarea, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Acceso a la lista de estados de tareas del sistema</a></p> <p>En el caso de los problemas, [!UICONTROL Estado] es una configuración del problema que indica si este problema es:</p> 
    <ul> 
     <li>[!UICONTROL Nuevo]</li> 
     <li>[!UICONTROL En Curso]</li> 
     <li>[!UICONTROL Esperando comentarios]</li> 
     <li>[!UICONTROL En espera]</li> 
     <li>[!UICONTROL Resuelto]</li> 
     <li>[!UICONTROL no se puede resolver]</li> 
     <li>[!UICONTROL No Se Puede Duplicar]</li> 
     <li>[!UICONTROL Verificado completo]</li> 
     <li>[!UICONTROL Reabierto]</li> 
    </ul> <p>Para obtener más información sobre los estados de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceso a la lista de estados de problemas del sistema</a>.</p> 
    <p>Para los objetivos estratégicos, el [!UICONTROL Estado] es una configuración del objetivo que indica si el objetivo es:</p> 
     <ul> 
      <li>[!UICONTROL Activo]</li> 
      <li>[!UICONTROL Borrador]</li> 
      <li>[!UICONTROL Inactivo]</li> 
      <li>[!UICONTROL Cerrado]</li> 
     </ul> 
     <p>Para obtener más información acerca de los objetivos estratégicos, consulte "[!UICONTROL Goal]" o "[!UICONTROL Goals]" en este artículo. </p> 
     <p>Para los objetivos estratégicos, este campo solo es visible si la organización ha adquirido [!DNL Workfront Goals]. Para obtener información sobre la administración de objetivos estratégicos con [!DNL Workfront Goals], consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] descripción general</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambio de estado]</td> 
   <td>Una pista de auditoría de [!UICONTROL]. Se genera una nota cuando un usuario cambia el estado del proyecto, tarea o problema.</td> 
  </tr> 
  <tr> 
   <td>Iconos de estado</td> 
   <td> <p>Puede agregar el campo integrado [!UICONTROL Iconos de estado] como una columna en las vistas para mejorar la visibilidad de los puntos clave sobre los objetos, como:</p> 
    <ul> 
     <li>Un objeto tiene documentos adjuntos</li> 
     <li>Un objeto está asociado a un proceso de aprobación</li> 
     <li>Un objeto tiene notas adicionales asociadas</li> 
     <li>Un gasto es facturable o reembolsable </li> 
     <li>Una tarea se encuentra en una ruta crítica</li> 
     <li>Un usuario pertenece a una empresa, a un equipo o está ubicado en una zona horaria diferente </li> 
    </ul> <p>Puede agregar el campo [!UICONTROL Status Icons] en las vistas de los objetos siguientes: </p> 
    <ul> 
     <li>[!UICONTROL Tareas]</li> 
     <li>[!UICONTROL Problemas]</li> 
     <li>[!UICONTROL Proyectos]</li> 
     <li>[!UICONTROL Tareas de plantilla]</li> 
     <li>[!UICONTROL Plantillas]</li> 
     <li>[!UICONTROL Gastos]</li> 
     <li>[!UICONTROL Documentos]</li> 
     <li>[!UICONTROL Usuarios]</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actualización de estado]</td> 
   <td> <p>En un informe de proyecto, tarea o problema, este campo muestra la actualización de estado más reciente que los propietarios de objetos han proporcionado en el área "[!UICONTROL Updates]". En el caso de los proyectos, esto significa que los comentarios realizados por el Propietario del proyecto, así como las tareas y problemas, significan que los comentarios realizados por los usuarios asignados.</p> 
   <p> Los comentarios realizados al actualizar el estado de un objeto no se muestran en la columna [!UICONTROL Status Update].</p> <p>Para mostrar los estados '[!UICONTROL New],' '[!UICONTROL In Process],' y '[!UICONTROL Complete]', utilice la columna [!UICONTROL Status].</p> <p>Para obtener más información sobre los estados, consulte el artículo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Actualizar estado de la tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estados]</td> 
   <td>Consulte "[!UICONTROL Status]" en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Guión gráfico]</td> 
   <td>Gráfico que representa el estado de las historias (tareas de la metodología Agile) y cómo progresan hacia su finalización.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Horas de la historia]</td> 
   <td>Métrica utilizada para medir la dificultad o complejidad de una historia. Los equipos de Agile pueden elegir si desean utilizar horas o puntos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Métrica utilizada para medir la dificultad o complejidad de una historia. Los equipos de Agile pueden elegir si desean utilizar horas o puntos.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Estratégico]</td> 
   <td>Trabajo a largo plazo que cambia la organización o cómo funciona la organización.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Alineación estratégica]</td> 
   <td>Medir y alinear los objetivos de la compañía en portafolios y programas.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Se utiliza en las columnas del informe al utilizar la interfaz de modo de texto. </p>
   <p>El <code>[!UICONTROL stretch]</code> se utiliza para identificar qué columnas ocupan espacio adicional que la vista no necesita. La anchura de la interfaz de usuario del espacio de trabajo de un usuario típico es de unos 850 píxeles. Esto significa que si tiene una vista con cuatro columnas (150 píxeles cada una), esa vista ocupará 600 de 850 píxeles. Hay 250 píxeles adicionales en la interfaz de usuario que se añadirán a las columnas que tengan un porcentaje de ampliación proporcionado. </p>
   <p>La ampliación de una columna se impone cuando se utiliza la línea de código adicional: <code>[!UICONTROL usewidths=true]</code> para al menos una de las columnas de la vista. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Suscriptores]</td> 
   <td> <p>Usuarios que se suscriben a proyectos, tareas o problemas.</p> <p>Cuando se utiliza este campo en un informe, se muestra una lista de suscriptores, cada uno de los cuales está separado por una coma.</p> <p>Para obtener más información, consulte el artículo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Suscribirse a elementos en [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea de resumen]</td> 
   <td>Consulte "[!UICONTROL Tarea principal]" en este artículo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtarea]</td> 
   <td>Una tarea secundaria, que se encuentra debajo de una tarea principal.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Control de sistema]</td> 
   <td>Conjunto de directivas que rigen los cambios y el mantenimiento de un sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Integración de sistemas]</td> 
   <td>Proceso de vinculación física o funcional de diferentes sistemas informáticos y aplicaciones de software para actuar como un todo coordinado.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tarea]</td> 
   <td> <p>Una actividad que debe realizarse como paso hacia el logro de un objetivo final (completar el proyecto).</p> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Información general sobre tareas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Atributo de tarea]</td> 
   <td>Otros campos u objetos asociados a una tarea e indican determinados detalles sobre la tarea. Algunos ejemplos son [!UICONTROL Fecha planificada de finalización] y [!UICONTROL Estado].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restricción de tarea]</td> 
   <td>Consulte "[!UICONTROL Tipo de restricción]" y "[!UICONTROL Fecha de restricción]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Administración de tareas]</td> 
   <td>Conjunto de directivas que rigen los umbrales de creación, asignación, cierre y visibilidad de tareas.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Propietario de tarea]</td> 
   <td>El equipo o usuario responsable de la estimación del esfuerzo y la finalización de la tarea</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Equipo]</td> 
   <td> <p>Una colección de usuarios que trabajan para lograr objetivos comerciales o objetivos similares. Estos usuarios se pueden asignar colectivamente a un elemento de trabajo asignando el equipo al elemento de trabajo.</p> <p>Para obtener más información sobre los equipos, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Resumen de equipos</a>.</p> <p>Los proyectos pueden tener un [!UICONTROL Equipo del proyecto], que contiene todos los usuarios o roles asociados con el trabajo en el proyecto.</p> <p>Para obtener más información sobre los equipos del proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Las plantillas de proyecto son descripciones genéricas de los proyectos más repetibles. Puede definir tareas, temas de colas, formularios personalizados, adjuntar documentos o aprobaciones cuando cree una plantilla de proyecto para ahorrar tiempo cuando deba crear un nuevo proyecto. </p> <p>Puede adjuntar plantillas a proyectos existentes o puede utilizarlas para crear nuevos proyectos. Toda la información especificada en la plantilla se transfiere a los proyectos creados con ella. </p> <p>Para obtener más información sobre las plantillas, consulte <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Resumen de plantilla de proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Una tarea que forma parte de una plantilla. Las Tareas de plantilla se convierten en Tareas en el proyecto que se crea mediante la plantilla.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subproceso]</td> 
   <td>Una [!UICONTROL Note] y su colección de respuestas relacionadas con un tema en particular.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura]</td> 
   <td> <p> En una lista o informe de [!UICONTROL Document], muestra una vista previa del documento en una miniatura. </p> <p> Seleccionar <strong>[!UICONTROL Miniatura]</strong>  para ver una miniatura de entre 33 y 66 píxeles de ancho en el informe. </p> <p>El tamaño de la miniatura se ajusta al modificar el ancho de la columna en una lista o informe.</p> <p>Consulte también "[!UICONTROL Miniatura grande]" en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo libre]</td> 
   <td>Puede generar un informe de [!UICONTROL Tiempo libre] para ver cuándo los usuarios han indicado tiempo libre en su perfil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de horas]</td> 
   <td> <p>Informe de tiempo que permite a los usuarios especificar las horas reales que dedicaron a trabajar en proyectos, tareas o problemas, o las horas que dedicaron a otras actividades no relacionadas con el trabajo, como reuniones o formación. Además de especificar la cantidad de tiempo que ha dedicado a trabajar, también puede indicar si el tiempo está relacionado con el trabajo o si equivale a tiempo general utilizando Tipos de horas para definir los registros de tiempo. Para obtener información sobre las plantillas de horas, consulte <a href="../../../timesheets/timesheets/timesheets-overview.md">Resumen de hojas de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Perfil de hoja de horas]</td> 
   <td> <p>Un [!UICONTROL Perfil de hoja de horas] es una plantilla que [!DNL Workfront] utiliza para crear automáticamente hojas de horas para los usuarios asociados a ellas. </p> <p>Puede configurar una serie de opciones que se aplicarán a cada plantilla de horas a medida que se cree. Algunas de estas configuraciones son: la frecuencia con la que se debe crear la plantilla de horas (semanal, cada dos semanas, dos veces al mes o mensualmente), el día de inicio de la plantilla de horas, los aprobadores de la plantilla de horas, los [!UICONTROL Tipos de horas] disponibles que los usuarios pueden asociar con las horas registradas.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Id. principal superior] </td> 
   <td> <p>Este campo permite identificar y filtrar datos sobre un grupo de nivel superior y sus subgrupos en una lista o informe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre principal superior] </td> 
   <td> <p>Este campo permite identificar datos sobre un grupo de nivel superior y sus subgrupos en una [!UICONTROL View] para una lista o informe.</p> <p>También puede hacerlo utilizando el campo [!UICONTROL Top Parent ID].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total de horas]</td> 
   <td> <p>En un informe de proyecto de [!UICONTROL], este campo muestra la suma redondeada de todas las horas del proyecto la última vez que se calcularon las finanzas del proyecto. [!UICONTROL Horas reales] reflejan las horas exactas registradas en el proyecto. Normalmente, [!UICONTROL Horas reales] debe coincidir con [!UICONTROL Horas totales]. Si [!UICONTROL Horas totales] aparece de forma significativamente diferente al campo [!UICONTROL Horas reales], debe recalcular las finanzas en el proyecto.</p> <p>Para obtener más información sobre cómo recalcular las finanzas del proyecto, consulte el artículo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalcular finanzas del proyecto</a>.</p> <p>En una vista de plantilla de horas [!UICONTROL Standard], este campo hace referencia a las horas totales registradas para los elementos de las fechas mostradas en una plantilla de horas. El campo [!UICONTROL Total de horas] para las plantillas de horas en esta vista integrada hace referencia al campo "[!UICONTROL hoursDuration]" que calcula dinámicamente la diferencia en horas entre las fechas de inicio y finalización de la plantilla de horas. Se utiliza para mostrar en rojo la columna [!UICONTROL Total Hours] si el usuario registra más tiempo que las horas disponibles en el lapso de tiempo de la hoja de horas. Para obtener más información, consulte <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Ver las horas totales en la hoja de horas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>Atributo de una tarea. Determina cómo y cuándo se actualizarán las escalas de tiempo proyectadas para una tarea. Por ejemplo:</p> 
    <ul> 
     <li>[!UICONTROL El usuario debe actualizar] requiere que una tarea se actualice manualmente. De lo contrario, pasará a ser [!UICONTROL Retrasado del horario] y, a continuación, [!UICONTROL Retrasado].</li> 
     <li>[!UICONTROL Completar automáticamente] completará automáticamente una tarea cuando haya pasado la fecha de vencimiento o [!UICONTROL Fecha planificada de finalización].</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Información general del modo de seguimiento de tareas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Déclencheur]</td> 
   <td>Un evento que inicia un escenario.</td> 
  </tr> 
  <tr> 
   <td>Tarea con problemas de [!UICONTROL]</td> 
   <td>Tarea incompleta con una condición de [!UICONTROL Late], [!UICONTROL Behind Schedule] o [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tarea sin asignar]</td> 
   <td>Una tarea que no está asignada a ningún usuario, rol o equipo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de actualización]</td> 
   <td> <p>Configuración de un proyecto que determina cuándo se recalculará la escala de tiempo de Proyectado del proyecto. [!UICONTROL Update Type] puede tener los valores siguientes:</p> 
    <ul> 
     <li>[!UICONTROL Automático y al cambiar]</li> 
     <li>[!UICONTROL Sólo automático]</li> 
     <li>[!UICONTROL Solo manual] </li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleccione el tipo de actualización del proyecto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usuario]</td> 
   <td>Una cuenta creada en [!DNL Workfront] para permitir que una persona inicie sesión e interactúe con el sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Delegación de usuario]</p> </td> 
   <td> <p>Objeto de informe que le indica:</p> 
    <ul> 
     <li>Qué usuarios han delegado aprobaciones de tareas, problemas y proyectos</li> 
     <li>Qué usuarios han tenido delegadas aprobaciones de tareas, problemas y proyectos</li> 
     <li>Cuando estas delegaciones comienzan y finalizan</li> 
    </ul> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Creación de un informe de delegación de usuario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz de usuario de [!UICONTROL]</td> 
   <td>Todos los aspectos visuales e interactivos de la [!DNL Workfront] aplicación.</td> 
  </tr> 
  <tr> 
   <td>Preferencias de interfaz de usuario de [!UICONTROL]</td> 
   <td>[!UICONTROL Configuración de interfaz de usuario]. [!DNL Workfront] los administradores pueden cambiar esta configuración para personalizar aspectos de la interfaz de usuario de.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilización]</td> 
   <td>La disponibilidad de un usuario o rol en función de la programación asignada, el tiempo de espera y la carga de trabajo actual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilización de usuarios]</td> 
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
   <td>[!UICONTROL Velocidad]</td> 
   <td>Una medida del tiempo total del ciclo de trabajo (cuánto tiempo se tarda en completar una parte del trabajo) y la frecuencia con la que se realiza el trabajo en el tiempo asignado originalmente (relación trabajo a compromiso).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Ver]</td> 
   <td> <p>Las vistas hacen referencia a un elemento de informes que le permite modificar las columnas de un informe o de una lista de objetos.</p> 
   <p> Ver también hace referencia al derecho de un usuario a ver únicamente información sobre un objeto, según su nivel de acceso o en un nivel de uso compartido de permisos de ese objeto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ver iconos]</td> 
   <td> <p> Es el mismo campo que Status Icons, pero solo está disponible para las siguientes vistas: </p> 
    <ul> 
     <li> [!UICONTROL Documentos] </li> 
    </ul> <p> Para obtener más información, consulte el artículo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Iconos de estado integrados en vistas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas del mes pasado]</td> 
   <td> <p>En una lista de informes, muestra el número de veces que se ha visto el informe durante el último mes.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas del último trimestre]</td> 
   <td>En una lista de informes, muestra el número de veces que el informe se ha visto durante el último trimestre.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas del último año]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante el último año.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas de este mes]</td> 
   <td> <p>En una lista de informes, muestra el número de veces que se ha visto el informe durante este mes.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas de este trimestre]</td> 
   <td>En una lista de informes, muestra el número de veces que el informe se ha visto durante este trimestre.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Ver uso del informe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vistas de este año]</td> 
   <td>En una lista de informes, muestra el número de veces que se ha visto el informe durante este año.<br>Para obtener más información sobre el uso de la información en las listas de informes, consulte el artículo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Ver uso del informe</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> En un informe, cuando se utiliza la interfaz [!UICONTROL Text Mode], la línea de código en la que se puede especificar el ancho de cada columna en píxeles. Workfront proporciona una anchura sugerida para cada campo, aunque según el tipo de campo y el formato, puede que desee realizar ajustes.
Debe utilizar el adicional <code>[!UICONTROL usewidths=true]</code> línea de código para exigir el ancho especificado para la columna. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>En un informe de proyecto, tarea o problema, el uso de la siguiente instrucción en modo de texto muestra las horas planificadas del proyecto, tarea o problema:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Para obtener información sobre el uso del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Resumen de sintaxis de modo de texto</a>. </p> 
   <p><b>SUGERENCIA</b> 
   <p>En un informe de problemas, al agregar uno de los campos [!UICONTROL Horas planificadas], se agrega el campo <code>work </code>al informe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trabajo]</td> 
   <td> <p>Uno de los dos tipos de licencia principales. Tiene menos acceso que el plan [!UICONTROL], pero puede crear y actualizar el sistema. Un usuario con una licencia de trabajo tiene más capacidades que un titular de licencia de [!UICONTROL Externo], [!UICONTROL Revisor] o [!UICONTROL Solicitante].</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] información general sobre licencias</a>.</p> <p>Trabajo puede hacer referencia al número de [!UICONTROL Horas planificadas] de un proyecto, tarea o problema. Para obtener más información, consulte el campo "[!UICONTROL work]" en esta tabla. </p> <p><b>SUGERENCIA</b></p> <p> En un informe de problemas, al agregar uno de los campos [!UICONTROL Horas planificadas], se agrega el campo <code>work </code>al informe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Estructura del desglose de trabajo]</td> 
   <td>Estructura jerárquica de las tareas que va a ejecutar el equipo del proyecto en función de la relación principal/secundario.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Esfuerzo de trabajo] </td> 
   <td> 
    <p>Un jefe de proyecto podría decidir utilizar este campo en lugar de [!UICONTROL Horas planificadas] para calcular el esfuerzo necesario para completar una tarea. Este campo solo está visible cuando se cumplen las siguientes condiciones:</p> 
     <ul> 
      <li> <p>La tarea tiene un [!UICONTROL Tipo de duración simple]. </p> <p><b>SUGERENCIA</b></p> <p> Si actualiza la tarea [!UICONTROL Duration Type] a cualquier otro tipo, este campo se oculta. </p> </li> 
      <li>El jefe de proyecto ha habilitado el campo [!UICONTROL Usar esfuerzo de trabajo] para calcular automáticamente las horas planificadas de la tarea en el proyecto. </li> 
     </ul> 
     <p>Para obtener información sobre el uso de [!UICONTROL Esfuerzo de trabajo] en lugar de [!UICONTROL Horas planificadas] para calcular el esfuerzo de la tarea, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen de esfuerzo de trabajo</a>. </p> 
     <p>Puede mostrar este campo en informes de tareas y listas.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Elemento de trabajo]</td> 
   <td> <p>Este campo hace referencia a tareas o problemas en [!DNL Workfront]. </p> <p>El informe [!UICONTROL Elemento de trabajo] muestra información sobre tareas y problemas. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Combinación de administración de trabajo]</td> 
   <td>Un [!UICONTROL Indicador de rendimiento del trabajo] (WPI) de la proporción de trabajo asignado para ejecutar su negocio frente a cambiar su negocio. El WPI de mezcla le ayuda a comprender, a nivel organizativo, si su estrategia tiene aplicada alguna asignación de trabajo real.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurso de administración de trabajo]</td> 
   <td>Una designación de un personaje en el sistema que es elegible para recibir trabajo o rastrear tiempo.</td> 
  </tr> 
  <tr> 
   <td>Función y responsabilidades de [!UICONTROL Work Management]</td> 
   <td>Definir los propietarios y las partes interesadas para administrar el ámbito, la ejecución y las aprobaciones de la cuestión, tarea, proyecto, programa o portafolio designados.</td> 
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
   <td>[!UICONTROL Puntos de contacto de administración de trabajo]</td> 
   <td>Registros digitalizados de la comunicación entre las partes interesadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicadores de rendimiento del trabajo] </td> 
   <td> <p>Relación de mezcla, capacidad, velocidad, calidad y participación.</p> <p>WPI es un acrónimo común de [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proceso de trabajo]</td> 
   <td> <p>Método en el que se recibe, se prioriza y se ejecuta el trabajo. La forma en que ejecuta el trabajo se denomina normalmente "flujo de trabajo" o "plan del proyecto" (una lista de tareas con fechas, relaciones de predecesoras, etc.). </p> <p>Algunos ejemplos de proceso de trabajo pueden ser la producción de un solo recurso o la entrega de una campaña de varios recursos. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plantilla de flujo de trabajo]</td> 
   <td>En el informe [!UICONTROL Proof Approval], este campo muestra todas las plantillas de flujo de trabajo adjuntas a una prueba. Si no hay plantillas adjuntas, la columna está en blanco.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tiempo de trabajo]</td> 
   <td>

<p>Representa el porcentaje de tiempo equivalente a tiempo completo ([!UICONTROL FTE]) que el usuario está disponible para el trabajo real, sin incluir la sobrecarga. [!UICONTROL Work Time] debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.</p>
   </p>El valor predeterminado del campo es 1, lo que indica que un usuario gasta todo su [!UICONTROL FTE] en trabajo real relacionado con el proyecto.  </p>
   <p>El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto. </p>
   <p> Las excepciones de horario y los días libres también pueden afectar a la capacidad del usuario. </p>
   <p>Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creación de una programación</a>. </p>
    <p>Workfront calcula la disponibilidad de un usuario en función de las preferencias de Administración de recursos del área [!UICONTROL Setup]. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurar preferencias de administración de recursos</a>. </p> 
   <p>Puede actualizar el [!UICONTROL Tiempo de trabajo] de un usuario cuando edite o cree el usuario. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Edición del perfil de un usuario</a></p> 
   <b>SUGERENCIA</b> 
   <p>Establezca el valor de [!UICONTROL Tiempo de trabajo] en 1 para indicar que el usuario está disponible para el trabajo relacionado con el proyecto en su equivalente a tiempo completo.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo de trabajo]</td> 
   <td>En la documentación de Workfront, este término se utiliza para describir el tiempo asignado al trabajo, de acuerdo con un horario.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>En un informe de proyecto, tarea o problema, el uso de la siguiente instrucción en modo de texto muestra el número de horas planificadas del proyecto, tarea o problema seguido de la palabra "Horas":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Para obtener información sobre el uso del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Resumen de sintaxis de modo de texto</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
