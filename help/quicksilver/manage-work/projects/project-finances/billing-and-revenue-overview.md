---
content-type: overview
product-area: projects
navigation-topic: financials
title: Información general sobre facturación e ingresos
description: Como administrador del proyecto, puede utilizar las tarifas de facturación para capturar los ingresos de sus proyectos.
author: Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '3691'
ht-degree: 99%

---

# Información general sobre facturación e ingresos

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

Como administrador del proyecto, puede utilizar las tarifas de facturación para capturar los ingresos de sus proyectos.

En este artículo se describe el seguimiento de los ingresos de los proyectos. Los ingresos se calculan de forma diferente en el Informe de utilización. Para obtener información sobre los cálculos de ingresos en el informe de utilización, consulte [Ver información sobre la utilización de los recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Información general de las tarifas de facturación

Tenga en cuenta lo siguiente al trabajar con tarifas de facturación:

* Necesita una licencia estándar o de planificación con acceso de edición de datos financieros para gestionar las tarifas de facturación.\
  Para obtener más información sobre la concesión de acceso a datos financieros, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Las tarifas de facturación son cantidades de ingresos por unidad de trabajo asociada con funciones o usuarios.

  Multiplicar las tasas por las horas invertidas en el trabajo genera ingresos para sus proyectos.

* Una vez establecidas las tarifas de facturación, puede realizar un seguimiento de los ingresos creando registros de facturación para anotar lo que se ha facturado y lo que no.

  >[!TIP]
  >
  >Cuando marca un registro de facturación como Facturado, nunca se puede editar. Esto es importante cuando las tarifas varían y desea bloquear la información de ingresos y gastos en el proyecto. Añadir esta información a un registro de facturación y marcar ese registro como Facturado impide que se actualice cuando se actualizan las tarifas en el sistema.

  Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

* Puede crear tarifas de facturación para usuarios, funciones o puede tener una tarifa de facturación única para un proyecto o tarea.

>[!IMPORTANT]
>
>Las tarifas que calculan los ingresos pertenecen al usuario que registra la hora o a sus funciones.

* [Tarifas de facturación del usuario](#user-billing-rates)
* [Tarifas de facturación de la función](#job-role-billing-rates)
* [Tarifas de facturación fijas para proyectos o tareas](#fixed-billing-rates-for-projects-or-tasks)
* [Anular las tarifas de facturación](#override-billing-rates)

### Tarifas de facturación del usuario {#user-billing-rates}

Como administrador de usuarios, al crear un usuario, puede asociarlo a tarifas de facturación con fecha en vigor, especificando valores para los campos Facturación por hora y las fechas de las tarifas.

Para obtener más información sobre cómo crear usuarios, consulte el artículo [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

![Editar costes de usuario y tarifas de facturación](assets/edit-user-cost-billing-rate-1.png)

### Tarifas de facturación de funciones {#job-role-billing-rates}

Como administrador de Adobe Workfront, al crear una función, puede asociarla a tarifas de facturación con fecha en vigor especificando valores para los campos Facturación por hora y las fechas de las tarifas.

Puede definir el valor de la tarifa de facturación de una función mediante la Divisa base del sistema de Workfront o utilizando otra divisa personalizada.

Para obtener más información sobre cómo crear funciones y anular su divisa, consulte el artículo [Crear y administrar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

![Editar costes de función y tarifas de facturación](assets/edit-job-role-multiple-billing-rates-new.png)

### Tarifas de facturación fijas para proyectos o tareas {#fixed-billing-rates-for-projects-or-tasks}

Además de las tarifas por hora de usuario y función, también puede tener las siguientes tarifas de facturación fijas:

* Importe fijo para tipo de ingresos fijos por hora
* Importe fijo para tipo de ingresos fijos

Para obtener más información sobre cómo se usan las tarifas de facturación fijas para calcular los ingresos, consulte [Información general sobre los tipos de ingresos de tareas](#overview-of-task-revenue-types).

### Anular las tarifas de facturación {#override-billing-rates}

>[!IMPORTANT]
>
>Puede anular las tarifas de facturación asociadas con funciones. No puede anular las tarifas de facturación del usuario ni las tarifas fijas.

Puede anular las tarifas de facturación de funciones para lo siguiente:

* Una compañía específica

  Para obtener más información sobre cómo crear tarifas de facturación de funciones específicas para una compañía, consulte [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Un proyecto específico

  Para obtener más información sobre la creación de tarifas de facturación de función específicas de un proyecto, consulte el artículo [Información general sobre cómo anular las tarifas de facturación de funciones y calcular los ingresos de un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Realizar un seguimiento del importe de los ingresos

Workfront puede rastrear automáticamente los ingresos planificados cuando se crean tareas en función de las horas planificadas de las tareas.

También puede rastrear automáticamente los ingresos reales cuando se registran horas reales en las tareas, problemas y en el proyecto.

En la tabla siguiente se muestran los tipos de ingresos asociados a las tareas, problemas y proyectos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ingresos planificados</td> 
   <td> <p>Para las tareas, estos son los ingresos asociados con las horas planificadas de las tareas. Las horas planificadas de todas las tareas se acumulan en las horas planificadas del proyecto para contribuir al cálculo de las horas planificadas para el proyecto. </p> <p>Para obtener más información sobre las horas planificadas en Workfront, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Información general de horas planificadas</a>. </p> <ul><li><p>Workfront calcula los ingresos planificados para las tareas mediante esta fórmula:</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>NOTA</strong></br> La tarifa por hora de facturación de la fórmula tiene en cuenta cualquier cambio de tarifa que sea efectivo para la fecha.</p> </li><li><p>Workfront calcula los ingresos planificados para los proyectos mediante la siguiente fórmula:</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>NOTA</b>

<p>Los ingresos planificados del proyecto que se muestran en el área de Detalles del proyecto y en los informes del proyecto difieren de los ingresos planificados que se muestran en el informe Utilización. </p></li></ul> <p>Los ingresos planificados en el área de Detalles del proyecto reflejan los ingresos de la tarea asociados con las horas planificadas de la tarea, así como los ingresos fijos del proyecto. Los ingresos planificados en el informe Utilización muestran los ingresos planificados asociados únicamente a las horas planificadas de las asignaciones de tareas del proyecto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Si el proyecto tiene 1 tarea con 10 horas asignada a un consultor con una tasa horaria de 20 dólares y el proyecto tiene 100 dólares de ingresos fijos, el informe Utilización muestra 200 dólares para los ingresos planificados (los ingresos planificados asociados con las horas de la tarea). La sección Detalles del proyecto muestra 300 dólares (los ingresos planificados de la tarea y los ingresos fijos del proyecto). </p> 
     </div> </p> <p>Los ingresos planificados para la tarea se calculan usando las tarifas por hora de facturación de los usuarios o las funciones asignadas a las tareas. El tipo de ingresos de las tareas influye en la tasa (usuario o función) que se utiliza para calcular los ingresos planificados. Para obtener más información, consulte las secciones siguientes de este artículo:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Información general sobre tipos de ingresos de tareas</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Cálculos de ingresos para tareas basados en asignaciones de usuarios y funciones</a> </p> </li> 
    </ul> <p>Para obtener información acerca de los cálculos de ingresos planificados en el informe Utilización, vea <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información de utilización de recursos</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ingresos reales*</td> 
   <td> <p>Ingresos asociados con las horas reales de las tareas, los problemas y los proyectos. </p> <p>Por lo general, Workfront calcula los ingresos reales mediante esta fórmula:</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>NOTA</strong></br> La tarifa por hora de facturación de la fórmula tiene en cuenta cualquier cambio de tarifa que sea efectivo para la fecha.</p> <p>Para obtener información sobre los cálculos de ingresos reales en el informe Utilización, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Ver información sobre la utilización de los recursos</a>. </p> <p><b>Sugerencia</b>

No puede ver los ingresos reales en el nivel de problema, pero los ingresos asociados con las horas reales en los problemas contribuyen a los ingresos reales del proyecto. </p> </td>
</tr> 
 </tbody> 
</table>

*Para las horas reales, las tarifas del usuario siempre hacen referencia al usuario que registra las horas o a las tarifas de sus funciones. Para obtener información sobre cuándo usa Workfront las tasas del usuario y cuándo usa las tasas de sus funciones, consulte la sección [Cálculos de ingresos](#revenue-calculations) en este artículo.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Por ejemplo, si una tarea con tipo de ingresos por hora de usuario está planificada para tardar dos horas y el usuario asignado tiene una tasa de 30 $ por hora, los ingresos planificados de la tarea son 60 $. Cuando finaliza la tarea, si el usuario registra solo 1,5 horas como el tiempo real empleado para finalizar la tarea, la cantidad de ingresos reales es de 45 $. Si otro usuario que no está asignado a la tarea registra el tiempo, los ingresos reales se calculan en función de las tarifas de facturación de ese usuario.

Puede registrar ingresos de las siguientes maneras:

* Definiendo el Tipo de ingresos de sus tareas y asociando los usuarios o funciones asignados a los elementos de trabajo con las tarifas de facturación. Esto calcula los ingresos según la cantidad de horas planificadas o reales de los elementos de trabajo. Puede establecer un límite para la cantidad máxima que se cobra por hora, o no.\
  Para obtener más información acerca de cómo especificar el tipo de ingresos de una tarea, vea el artículo [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Facturando una tarifa de ingresos fijos para tareas o proyectos.\
  Si tiene tareas con ingresos fijos, la cantidad de ingresos fijos se añadirá como los ingresos planificados de una tarea o un proyecto, y los ingresos planificados de una tarea estarán disponibles para añadirse a un registro de facturación como ingresos fijos.
* Estableciendo una tarifa de ingresos fijos plana de facturación para un proyecto y, a continuación, estableciendo tarifas por hora para las tareas dentro del proyecto. Workfront añade las tarifas por hora para las tareas a la tarifa plana del proyecto.\
  Por ejemplo, un mecánico que utilice Workfront podría introducir un coste de piezas como ingresos fijos para el proyecto y, a continuación, facturar por horas el tiempo empleado en reparar un coche. Los ingresos fijos de proyectos o tareas se obtienen al finalizar.

También puede marcar sus tareas como &quot;No facturables&quot;, en cuyo caso no hay ingresos planificados o reales asociados a ellas.

## Información general de tipos de ingresos de tareas {#overview-of-task-revenue-types}

De forma predeterminada, el tipo de ingresos de todas las tareas nuevas se establece de acuerdo con las preferencias de tareas y problemas especificadas por el administrador de Workfront o del grupo.\
Para obtener más información sobre cómo definir las preferencias de tareas y problemas para la instancia de Workfront, consulte el artículo [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

El propietario del proyecto puede modificar el tipo de ingresos de las tareas y los ingresos fijos de los proyectos.\
Para obtener más información acerca de cómo especificar los ingresos fijos de un proyecto, vea el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).\
Para obtener más información acerca de cómo especificar el tipo de ingresos de una tarea, vea el artículo [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Puede aplicar los siguientes tipos de ingresos a sus tareas o proyectos:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de ingresos</strong> </p> </th> 
   <th> <p><strong>Descripción</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ingresos fijos</p> </td> 
   <td> <p>Este tipo se puede utilizar con proyectos y tareas. </p> <p>Al adjuntar una plantilla a un proyecto, los ingresos fijos de la plantilla se añaden a los ingresos fijos del proyecto. Para obtener más información, vea <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Información general sobre cómo adjuntar una plantilla a un proyecto</a>. </p> <p>Para las tareas, independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea. </p> <p>Los ingresos fijos de las tareas secundarias se suman a los ingresos de la tarea principal y, a continuación, a los ingresos del proyecto. Si se define un importe fijo en la tarea principal y/o en el proyecto, el importe se añade a los ingresos planificados acumulados de cualquier tarea secundaria.</p> <p>La cantidad de ingresos fijos en las tareas se puede incluir en un Registro de facturación del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario por hora</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas. </p> <p>La tarifa de facturación que establezca para un usuario específico multiplicada por el número de horas planificadas para esa tarea se convierte en la cantidad de ingresos planificados de la tarea. La tarifa de facturación que establezca para un usuario específico multiplicada por el número de horas que el usuario registra en la tarea es la cantidad de ingresos reales de la tarea. <br>Por ejemplo, cuando crea un usuario y establece 20 USD para su campo Facturación por hora, si el usuario envía 5 horas para una tarea en la hoja de horas, la cantidad de Facturación real de la tarea es de 100 USD.</p>
   <p>Un perfil de usuario puede contener múltiples tarifas de facturación con fechas en vigor. Por ejemplo, la primera tarifa de facturación de usuario de 20 dólares finaliza el 30 de abril de 2023 y la segunda tarifa de facturación de usuario de 25 dólares empieza el 1 de mayo de 2023. Si el usuario envía 2 horas el 28 de abril y 3 horas el 2 de mayo para una tarea, el importe de facturación real de la tarea es de 40 USD + 75 USD = 115 USD.</p>
   <p><b>Sugerencia</b>

Este es el tipo de ingresos predeterminado cuando crea una tarea.</p> </td>
</tr> 
  <tr> 
   <td> <p>Rol por hora</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas.</p> <p>Este tipo es similar a Usuario por hora, pero utiliza tarifas de funciones en lugar de tarifas de usuario.</p> <p><strong>NOTA</strong><br> Una función también puede tener múltiples tarifas de facturación con fechas en vigor.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Usuario por hora con límite</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas.</p> <p>Las tareas se facturan por hora como en Usuario por hora, pero tienen un importe límite que puede especificar. <br>Por ejemplo, si la tarifa de facturación de un usuario es de 25 USD, pero el importe límite de la tarea es de 20 USD y el usuario registra una hora, los ingresos reales de la tarea serán de 20 USD. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Función por hora con límite</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas.</p> <p>Este tipo es similar a Usuario por hora con límite, pero utiliza tarifas de funciones en lugar de tarifas de usuario. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuario por hora más fijos</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas. </p> <p>Las tareas se facturan por hora como en Usuario por hora, pero tienen una cantidad fija que puede añadir a la tarifa de usuario. El importe fijo especificado en la tarea se puede incluir en los registros de facturación del proyecto. El importe fijo no se multiplica por las horas de la tarea. Solo lo hace la tarifa de facturación del usuario. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rol por hora más fijos</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas. </p> <p>Las tareas se facturan por hora como en Rol por hora, pero tienen una cantidad fija adicional que puede añadir a la tarifa de función. El importe fijo especificado en la tarea se puede incluir en los registros de facturación del proyecto. El importe fijo no se multiplica por las horas de la tarea. Solo la tarifa de facturación de la función lo hace. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fijo por hora</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas.</p> <p>El límite o importe fijo que se establece para la tarea multiplicado por el número de horas introducidas en la tarea (independientemente del usuario o de sus funciones) es el importe de facturación.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>No facturable</p> </td> 
   <td> <p>Este tipo solo se puede utilizar para tareas.</p> <p>Este tipo de ingresos no afecta a los ingresos. </p> <p>Si un objeto principal tiene esta configuración, las tareas secundarias con un tipo de facturación seguirán aplicándose normalmente.</p> <p>Cuando un usuario sin acceso a datos financieros o un usuario sin permisos financieros en una plantilla crea un proyecto a partir de esa plantilla, éste es el tipo de ingresos predeterminado de las tareas del proyecto.</p> <p>Para obtener información sobre el acceso a los datos financieros, consulte el artículo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acceso a los datos financieros</a>.<br>Para obtener información sobre los permisos financieros de los objetos, consulte el artículo <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido de objetos</a>.<br>Para obtener información sobre la creación de proyectos a partir de plantillas, consulte el artículo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Crear un proyecto a partir de una plantilla</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Información general sobre los ingresos de las tareas principales

Si cambia una tarea independiente con información de facturación en ella a una tarea principal, la nueva tarea principal sigue conservando toda la información de facturación que se le haya aplicado previamente, junto con las horas aplicadas previamente. Cualquier información de facturación proveniente de las horas registradas en las tareas secundarias se resumirá como Ingresos reales en la nueva tarea principal.

Los ingresos planificados de las tareas secundarias también se resumen en la tarea principal.

## Información general sobre los ingresos de problemas 

Los problemas no tienen importes de ingresos planificados o reales, pero pueden tener un coste real.

Si registra horas para un problema y utiliza un tipo de hora que se marca como &quot;Contar como ingresos&quot;, Workfront calcula un importe del coste real según la tarifa del usuario que inicia sesión en ese momento. Este número se añade al coste real del proyecto. Las horas también se pueden incluir en un registro de facturación.

Para obtener más información sobre el seguimiento de los costes, consulte el artículo [Seguimiento de los costes](../../../manage-work/projects/project-finances/track-costs.md).

Para obtener más información sobre los tipos de horas, consulte el artículo [Administrar tipos de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Cálculos de ingresos

* [Cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Al calcular los ingresos de una tarea, tenga en cuenta lo siguiente:

* Si un usuario o una función muestra una tarifa de 0,00 $, Workfront la lee como una cantidad válida y multiplicará esta cantidad por el número de horas de la tarea para calcular los ingresos. Si no desea mostrar ingresos para sus tareas, asegúrese de que el campo de la tarifa de facturación de su usuario o función esté vacío.
* Cuando se aplican tarifas de facturación de función, Workfront utiliza la tarifa de anulación a nivel de proyecto, en lugar de la tarifa de facturación para esa función definida a nivel de sistema cada vez que hay una tarifa de anulación en el proyecto.
* En el caso de los ingresos reales, si el usuario o la función tienen varias tarifas de facturación con fechas en vigor, los ingresos de la tarea son la suma de los ingresos de cada período de tiempo en el que el usuario ha registrado el tiempo. Los ingresos planificados se basan en las horas planificadas para los períodos de tiempo.
* En el caso de varias personas asignadas en las tareas, se aplicarán los escenarios que se describen a continuación para cada persona asignada.

Existe una jerarquía cuya tarifa se utiliza en los cálculos de ingresos según las asignaciones de tareas.

Si el administrador de Workfront habilitó la opción **Asignar roles a entradas de horas manualmente** en el área Preferencias de plantillas de horas y horas, y el usuario que registra el tiempo en el proyecto selecciona un rol diferente para asociarlo a esta hora, los ingresos reales de la tarea o proyecto siempre se calculan en función del rol asociado a la entrada de horas. Para obtener información sobre la habilitación del tiempo de registro para una función específica, consulte el artículo [Configurar preferencias de plantillas de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Se dan los siguientes escenarios al calcular los ingresos de la tarea según el tipo de ingresos y la naturaleza de la asignación de la tarea:

* **El tipo de ingresos de la tarea es Usuario por hora**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Tarifa de facturación por hora</td> 
     <td>Sin asignación</td> 
     <td>Asignación de usuarios</td> 
     <td>Asignación de función</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tarifa de facturación por hora para ingresos planificados</td> 
     <td>0,00 $</td> 
     <td> Si un usuario tiene una tarifa de facturación en su perfil, esa tarifa se utiliza para calcular los ingresos planificados. De lo contrario, se utiliza la tarifa de facturación del sistema de su función principal. <br><p><b>NOTA</b>: El usuario puede asignarse a la tarea con una de sus funciones secundarias, pero la tarifa de la función principal se usa aquí en su lugar.</p><p>Si la función del usuario ha cambiado durante la asignación, se aplican las tarifa correctas cuando se vuelven a calcular las finanzas del proyecto.</p></td> 
     <td><p><span class="preview">Si se adjunta una tarjeta de tarifas al proyecto, los ingresos planificados se calculan en función de la función de la tarjeta de tarifas.</span></p> <p><span class="preview">Las tarifas de facturación se pueden anular en el nivel de proyecto.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tarifa de facturación por hora para ingresos reales</td> 
     <td>Si el usuario que registra las horas tiene una tarifa de facturación en su perfil, se utiliza esa tarifa. 
     <br><span class="preview">Cuando se registra tiempo para un usuario o función que tiene una asignación específica de la ubicación en las asignaciones avanzadas, se utiliza la tarifa de la ubicación.</span>
     <br>De lo contrario, se usa la tarifa de facturación de su función principal. Si no hay ninguna tarifa de facturación asociada con el usuario o su función principal, los ingresos reales son de 0,00 USD. <br><p><b>NOTA</b>

  Solo se tienen en cuenta para el cálculo las tarifas asociadas con el registro de tiempo del usuario, incluso cuando se asigna otro usuario a la tarea.</p></td>
  <td>Si el usuario que registra las horas tiene una tarifa de facturación en su perfil, se utiliza esa tarifa. <br><span class="preview">Cuando se registra tiempo para un usuario o función que tiene una asignación específica de ubicación en las asignaciones avanzadas, se utiliza la tarifa de la ubicación.</span><br>De lo contrario, se utiliza la tarifa de facturación de su función principal. Si no hay ninguna tarifa de facturación asociada con el usuario o su función principal, los ingresos reales son de 0,00 USD. <br><p><b>NOTA</b>

  Solo se tienen en cuenta para el cálculo las tarifas asociadas con el registro de tiempo del usuario, incluso cuando se asigna otro usuario a la tarea.</p></td>
  <td>Si el usuario que registra las horas tiene una tarifa de facturación en su perfil, se utiliza esa tarifa. De lo contrario, se utiliza la tarifa de facturación de su función principal.<br><p><b>NOTA</b>

  Si el usuario que registra el tiempo no tiene asociada una tarifa de facturación y no tiene una función o una tarifa de facturación para su función, se utiliza la tarifa de la función asociada con la tarea. Si no hay ninguna tarifa de facturación para esta función, los ingresos son de 0,00 USD.</p></td>
  </tr> 
   </tbody> 
  </table>

* **El tipo de ingresos de la tarea es de función por hora**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Tarifa de facturación por hora</td> 
     <td>Sin asignación</td> 
     <td>Asignación de usuarios</td> 
     <td>Asignación de función</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tarifa de facturación por hora para ingresos planificados</td> 
     <td>0,00 $</td> 
     <td><p>Workfront se fija en la función que desempeña el usuario en la tarea para calcular los ingresos planificados. <br>Si el usuario no está asociado con ninguna función en la tarea, el valor de los ingresos es de 0,00 USD.</p> <p><strong>NOTA</strong><br> Si la función del usuario ha cambiado durante la asignación, se aplican las tarifas correctas cuando se recalculan las finanzas del proyecto.</p> </td> 
     <td><p><span class="preview">Si se adjunta una tarjeta de tarifas al proyecto, los ingresos planificados se calculan en función de la función de la tarjeta de tarifas.</span></p> <p><span class="preview">Las tarifas de facturación se pueden anular en el nivel de proyecto.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tarifa de facturación por hora para ingresos reales</td> 
     <td>Workfront utiliza la tarifa de facturación de la función de trabajo principal del usuario que registra el tiempo. <br><span class="preview">Cuando se registra tiempo para un usuario o función que tiene una asignación específica de ubicación en las asignaciones avanzadas, se utiliza la tarifa de la ubicación.</span> <br>Si el usuario que registra el tiempo no tiene ninguna función asociada, o si la función principal no tiene tarifa de facturación, los ingresos reales son de 0,00 USD. </td> 
     <td> Si el usuario que registra el tiempo está asignado a la tarea, la tarifa de facturación de la función asociada con el usuario en la tarea se utiliza para calcular los ingresos reales. <br><span class="preview">Cuando se registra tiempo para un usuario o función que tiene una asignación específica de ubicación en las asignaciones avanzadas, se utiliza la tarifa de la ubicación.</span> <br>De lo contrario, se usa la tarifa de facturación de su función principal. Si el usuario no tiene ninguna función principal o si su función principal no tiene tarifa de facturación, los ingresos reales son de 0,00 USD. </td> 
     <td>Si una de las funciones del usuario que registra el tiempo se asigna a la tarea, se utiliza esa tarifa de función. Si la función de trabajo asignada a la tarea no está asociada con el usuario que registra el tiempo, se utiliza la tarifa de facturación de la función principal del usuario para calcular los ingresos reales. Si el usuario no tiene una función de trabajo o no hay ninguna tarifa asociada con su función principal, se utiliza la tarifa de la función asignada a la tarea. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### Cálculos de ingresos para proyectos

Puede realizar un seguimiento de los siguientes tipos de ingresos para proyectos:

* Los ingresos planificados para un proyecto se calculan mediante la siguiente fórmula:

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  Para obtener información sobre cómo se calculan los ingresos planificados para la tarea, consulte la sección [Cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) en este artículo.

* Los ingresos reales de un proyecto se calculan mediante la fórmula siguiente:

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

Para obtener información sobre cómo se calculan los ingresos reales de la tarea, consulte la sección [Cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) en este artículo.

Para los ingresos reales asociados con las horas registradas directamente en el proyecto o los problemas, Workfront utiliza la tarifa de facturación del usuario que registra el tiempo en el proyecto. Si el usuario no tiene ninguna tarifa de facturación asociada con su perfil, Workfront utiliza la tarifa de facturación de su función principal. Si ambas tarifas son cero, los ingresos reales asociados con las horas registradas en el proyecto o los problemas son cero.
