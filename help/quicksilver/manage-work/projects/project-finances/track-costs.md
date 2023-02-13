---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Seguimiento de costes
description: Puede realizar un seguimiento de los costes de los proyectos, las tareas y los problemas en Adobe Workfront.
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2364'
ht-degree: 1%

---

# Seguimiento de costes

Puede realizar un seguimiento de los costes de los proyectos, las tareas y los problemas en Adobe Workfront.

## Cómo calcula Workfront los costes

Para realizar un seguimiento de los costes, debe asociar usuarios y funciones de trabajo con tasas de coste por hora.

Las tasas de coste por hora son cantidades de costes por unidad de trabajo asociadas con funciones de trabajo o usuarios. Al multiplicar las tasas por las horas dedicadas al trabajo, se generan costes para sus proyectos, tareas o problemas.

Existen los siguientes escenarios:

* Si el tipo de coste de las tareas es Usuario por hora, la tasa por hora del usuario calcula los costes de la tarea y del proyecto.

   Para obtener información sobre cómo asociar usuarios con tasas de coste, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si el tipo de coste de las tareas es Función por hora, la tasa horaria de la función de trabajo calcula los costes de la tarea y del proyecto.

   Para obtener información sobre cómo asociar funciones de trabajo con tasas de coste, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront calcula solamente el costo real para problemas y problemas que no tienen un tipo de costo. Para obtener más información, consulte la sección [Cómo realiza Workfront el seguimiento de los costes de los problemas](#how-workfront-tracks-costs-for-issues) en este artículo.

>[!TIP]
>
>No puede anular las tasas de coste de los proyectos. Una vez establecida la tasa de costo por hora en una función de usuario o de trabajo, esa tasa calcula todos los costos del sistema.

## Índices de rendimiento de costes de Workfront

Workfront calcula una serie de índices de rendimiento de costes para los proyectos, de modo que se pueda realizar un seguimiento de los proyectos para lograr una mayor rentabilidad.\
Para obtener más información sobre el cálculo de índices de rendimiento de costes, consulte:

* [Calcular el índice de rendimiento de costes (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcular el Índice de Rendimiento del Programa de Costes (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcular el índice de rendimiento de la programación (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Cómo realiza Workfront el seguimiento de los costes de las tareas y los proyectos

* [Cómo realiza Workfront el seguimiento de los costes](#how-workfront-tracks-costs)
* [Cómo calcula Workfront los costes previstos, presupuestados y reales](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Cómo calcula Workfront los tipos de coste para las tareas](#how-workfront-calculates-cost-types-for-tasks)

### Cómo realiza Workfront el seguimiento de los costes  {#how-workfront-tracks-costs}

Puede rastrear varios tipos de Costes para tareas y proyectos en Workfront. Los costes generales se calculan mediante la fórmula siguiente:

```
Costs = Labor Costs + Expense Costs
```

* **Costes laborales** están asociados a las horas en tareas y proyectos y a las tasas de Costo por hora de los recursos asociados con tareas. En general, Workfront calcula los siguientes costes laborales:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Costes laborales planificados</td> 
     <td> <p>Se calculan mediante la fórmula siguiente:</p><pre>Costes Laborales Planificados = Horario Planificado * Tasa de Coste por Hora</pre> </td> 
    </tr> 
    <tr> 
     <td>Costes laborales presupuestados</td> 
     <td> <p>Se calculan mediante la fórmula siguiente:</p><pre>Costes laborales presupuestados = Horas presupuestadas * Tasa de costo por hora</pre> </td> 
    </tr> 
    <tr> 
     <td>Costes laborales reales</td> 
     <td> <p>Se calculan mediante la fórmula siguiente:</p><pre>Costes laborales reales = Horas reales * Tasa de costo por hora</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   Para obtener más información, consulte la [Cómo calcula Workfront los costes previstos, presupuestados y reales](#how-workfront-calculates-planned-budgeted-and-actual-costs) en este artículo.

* **Gastos** están asociados con Gastos en proyectos y tareas.\
   Al crear un proyecto, puede definir los gastos planificados para todo el proyecto. Además, puede asociar gastos con tareas nuevas o existentes. Para obtener más información, consulte [Administrar los gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Costes fijos** se definen como una cantidad fija de coste para un proyecto. Esto forma parte del Costo planeado del proyecto que representa la cantidad de dinero que necesita para completar el proyecto.

   >[!TIP]
   >
   >Al adjuntar una plantilla a un proyecto, el coste fijo de una plantilla se agrega al coste fijo del proyecto. Para obtener más información, consulte [Descripción general de cómo adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Cómo calcula Workfront los costes previstos, presupuestados y reales {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calcula el coste planeado y el coste real de cada tarea individual de un proyecto. Workfront utiliza estos cálculos para tareas individuales a fin de calcular el coste planeado y el coste real del proyecto.

* [Costo planificado](#planned-cost)
* [Costo presupuestado](#budgeted-cost)
* [Costo real](#actual-cost)

#### Costo planificado {#planned-cost}

El costo planeado de un proyecto es el costo asociado con el trabajo planificado (horas planificadas) en el proyecto.

El coste planificado de un proyecto se calcula mediante la fórmula siguiente:

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

* 
   * 

Por ejemplo, tiene los siguientes gastos en la pestaña Expenses de una tarea: un gasto de marketing de 100 $ y un gasto administrativo de 50 $. En la pestaña Finanzas, seleccione el tipo de coste Usuario por hora . Un usuario se asigna a la tarea y la tasa por hora del usuario es de 15 $. El usuario tiene asignado trabajar 5 horas en esta tarea. En la pestaña Gastos del proyecto, tiene un costo planificado de 100 $ para un gasto denominado Consultoría. También tiene un costo fijo de 200 $ para el proyecto.

El costo planeado del proyecto se calcula de la siguiente manera:

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense)+$15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost)= $525
```

#### Costo presupuestado {#budgeted-cost}

El costo presupuestado de un proyecto es el costo asociado con el trabajo presupuestado (horas presupuestadas) en el proyecto.

El coste presupuestado del proyecto es el mismo que el coste previsto del proyecto si se cumplen las dos condiciones siguientes:

* Las horas planificadas de las tareas del proyecto coinciden con las horas presupuestadas (en el planificador de recursos)
* La tarea Tipo de facturación es Función por hora.

El coste presupuestado del proyecto se calcula mediante la fórmula siguiente si se cumplen las siguientes condiciones:

* Las horas previstas de las tareas del proyecto no coinciden con las horas presupuestadas (en el planificador de recursos)
* El tipo de facturación de las tareas es Función por hora.

Cuando se cumplen las condiciones anteriores, Workfront calcula el coste presupuestado del proyecto mediante la fórmula siguiente:
<pre>Coste de proyecto presupuestado = Coste de trabajo presupuestado + Coste de gastos presupuestado de todas las tareas + Coste de gastos presupuestado del proyecto</pre>

#### Costo real {#actual-cost}

El costo real de un proyecto es el costo asociado con el trabajo real (horas registradas) del proyecto.

El costo real se calcula mediante la fórmula siguiente:

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project
```

.

Por ejemplo, tiene los siguientes gastos en la pestaña Expenses de una tarea: un gasto de marketing con un costo real de 110 dólares y un gasto administrativo con un costo real de 40 dólares. Seleccione el tipo de coste Función por hora y asigne la función de trabajo Consultor a la tarea. La tasa de la función de trabajo del consultor es de 15 $ por hora y hay 6 horas registradas en la tarea para la función de trabajo del consultor. También hay un gasto de consultoría asociado al proyecto (en la pestaña Gastos ), con un costo real de 100 $ y un usuario con una tasa de costo por hora de 20 $ en sus registros de perfil de usuario de 10 horas en el proyecto.

El costo real del proyecto se calcula de la siguiente manera:

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project)= $540
```

>[!NOTE]
>
>Al iniciar sesión en un proyecto, existen los siguientes escenarios al calcular el costo laboral real del proyecto:
>
>* De forma predeterminada, Workfront utiliza la tasa Costo por hora del usuario para calcular Coste laboral real.
>* Si el usuario que registra la hora no está asociado con ningún coste, Workfront utiliza la tasa Costo por hora de la función principal del usuario.
>* Si el administrador de Workfront ha habilitado la variable **Asignar roles de trabajo a las entradas de hora manualmente** en el área Preferencias de hojas de horas y horas , y el usuario que inicia sesión en el proyecto selecciona una función diferente para asociarla a esta hora, el costo real del proyecto se calcula en función de la función especificada cuando se registraron las horas. Para obtener información sobre cómo habilitar el tiempo de registro para una función de trabajo específica, consulte el artículo [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
>


### Cómo calcula Workfront los tipos de coste para las tareas {#how-workfront-calculates-cost-types-for-tasks}

El coste previsto y real de las tareas y sus costes laborales están determinados por el tipo de coste de cada tarea.

Puede configurar el tipo de coste para tareas individuales dentro del proyecto. Cada tipo de coste afecta a los valores Costo planeado y Costo real .

Para obtener información sobre cómo modificar el tipo de coste de una tarea, consulte [Actualizar tipo de costo de tarea](../../../manage-work/tasks/task-information/update-task-cost-type.md).

La siguiente tabla describe la tarea disponible Tipos de costo en Workfront:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de costo de tarea</strong> </p> </th> 
   <th> <p><strong>Descripción</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Usuario por hora</p> </td> 
   <td> <p>Este es el tipo de coste predeterminado al crear una tarea.</p> <p><strong>Coste planificado</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Cuando el Coste Laboral Planificado se calcule por:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Nota:   <p>Considere los siguientes impactos: usar el tipo de coste por hora de usuario y calcular el coste planeado:</p> 
     <ul> 
      <li>Si asigna varios recursos a una tarea, Workfront ajusta los cálculos de Coste planificado en función del porcentaje de la tarea asignada a cada recurso.</li> 
      <li>El valor del campo Costo planeado puede variar según se vea el Costo planeado desde la propia tarea o desde el informe de uso.<br><strong>Al ver el coste planeado desde la propia tarea:</strong> El campo Costo planeado tiene en cuenta el campo Costo/Hr establecido en el nivel Función de trabajo (cuando el campo Costo/Hr no se ha configurado en el nivel de usuario).<br><strong>Al consultar Costo planeado desde el informe de uso del proyecto:</strong> El campo Costo planeado no tiene en cuenta el campo Costo/Hr establecido en el nivel Función de trabajo. En su lugar, si desea que el informe de utilización tenga en cuenta el campo Costo/Hora establecido en el nivel Función de Trabajo, debe establecer el Tipo de Coste en la tarea en Función por hora. </li> 
     </ul> </p> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Donde el Coste de Trabajo Real se calcula mediante:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Por ejemplo, un usuario tiene una tasa de costo por hora de 20 dólares en su perfil. Cuando se registran 5 horas para una tarea, el Coste de trabajo real es de 100 dólares para esa tarea. Si el usuario no tiene asociada una tasa de costo por hora, el costo real calcula en función de la tasa de costo por hora de su función de trabajo principal. Si no tienen una función de trabajo o la tasa de costo por hora de su función de trabajo no está definida, entonces el costo real de la tarea es cero. </p> <p>Nota: Los costes reales se calculan en función de la tasa Costo por hora para el usuario que está registrando la hora, independientemente de quién esté asignado a la tarea. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rol por hora</p> </td> 
   <td> <p><strong>Coste planificado</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Donde el Coste Laboral Planificado de la Tarea se calcula mediante:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Nota: Si asigna varios recursos a una tarea, Workfront ajusta los cálculos de horas planificadas en función del porcentaje de la tarea asignada a cada recurso.</p> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Donde el Coste de Trabajo Real de la Tarea se calcula mediante:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Por ejemplo, una tarea se asigna a una función de trabajo o a un usuario con una función de trabajo cuya tasa de costo por hora es de 20 dólares. Cuando un usuario registra 5 horas para una tarea, el Coste de trabajo real es de 100 dólares para esa tarea. Si el usuario asignado a la tarea no tiene una función de trabajo asociada a él en la tarea, el coste real calcula en función de la tasa de coste por hora de su función de trabajo principal. Si no tienen una función de trabajo o la tasa de costo por hora de su función de trabajo no está definida, entonces el costo real de la tarea es cero. </p> <p>Nota:   <p> La tarea Hora real de una función por hora calcula en función de las funciones de trabajo de los usuarios asociados con la tarea, no de las funciones asociadas con el usuario que está registrando la hora.</p> <p>Si el administrador de Workfront ha habilitado la variable <strong>Asignar roles de trabajo a las entradas de hora manualmente</strong> en el área Preferencias de hojas de horas y horas , y el usuario que inicia sesión en la tarea selecciona una función diferente para asociarla a esta hora, la tarea Costo real de una función por hora calcula en función de la función especificada cuando se registraron las horas. Para obtener información sobre cómo habilitar el tiempo de registro para una función de trabajo específica, consulte el artículo <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configuración de las preferencias de horas y horas</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fijo por hora</p> </td> 
   <td> <p><strong>Coste planificado</strong> se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Donde el Coste de Trabajo de Tareas se calcula mediante:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Donde el Coste de Trabajo de Tarea Real se calcula mediante:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Este tipo de coste no tiene en cuenta usuarios individuales ni funciones de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sin costo</p> </td> 
   <td> <p>Este tipo de coste no afecta a los costes. Si una tarea principal tiene este Tipo de Coste, las subtareas con otro Tipo de Coste calculan según sus Tipos de Coste individuales y el Coste de la tarea principal se ve afectado en consecuencia. </p> <p>Cuando un usuario sin acceso a datos financieros o un usuario sin permisos financieros en una plantilla crea un proyecto a partir de esa plantilla, este es el tipo de coste predeterminado para las tareas del proyecto.</p> <p>Para obtener información sobre el acceso a los datos financieros, consulte el artículo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concesión de acceso a datos financieros</a>.</p> <p>Para obtener información sobre los permisos financieros en objetos, consulte el artículo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartir permisos financieros en un objeto</a>.</p> <p>Para obtener información sobre la creación de proyectos a partir de plantillas, consulte el artículo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Creación de un proyecto mediante una plantilla</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Cómo realiza Workfront el seguimiento de los costes de los problemas {#how-workfront-tracks-costs-for-issues}

Los problemas no tienen ni afectan a los siguientes tipos de costes en un proyecto:

* Costo planificado
* Costo presupuestado

Sin embargo, los problemas pueden tener un **Costo real** que también afecta al coste real del proyecto.

La siguiente tabla explica cómo se calcula el costo real para los problemas, según el tipo de asignación en el problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Costo real del problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Asignación de usuarios</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>La tasa de coste por hora del usuario que está registrando la hora se tiene en cuenta aquí, independientemente de quién esté asignado al problema. </p> <p>Si el usuario que registra la hora no tiene una tasa de costo por hora en su perfil, la tasa Costo por hora de su rol de trabajo principal calcula el costo real del problema. Si el usuario que está registrando la hora no tiene ninguna función en su perfil o ninguna tasa asociada a él, las horas reales se calculan utilizando la tasa Costo por hora de la función de trabajo principal del usuario asignado principal en el problema. Si esa función no tiene ninguna tasa definida, el costo real del problema es cero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Asignación de funciones</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>La tasa de coste por hora del usuario que registra el tiempo del problema se tiene en cuenta aquí, independientemente de la función que se asigne al problema. </p> <p>Si el usuario que registra la hora no tiene asociada una tasa de costo por hora, la tasa de costo por hora de su función principal calcula el costo real del problema.<br>Si el usuario que está registrando la hora no tiene ninguna función en su perfil o ninguna tasa asociada a él, el coste real del problema es cero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sin asignación</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Si el usuario que registra la hora no tiene una tasa de costo por hora asociada con su perfil, la tasa Costo por hora de su rol de trabajo principal calcula el costo real del problema. </p> <p>Si el usuario que está registrando la hora no tiene ninguna función de trabajo asociada con su perfil o su función de trabajo principal no tiene definida una tasa de coste por hora, el coste real del problema es cero. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
