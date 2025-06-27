---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Seguimiento de costes
description: Puede realizar un seguimiento de los costos de los proyectos, las tareas y los problemas en Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 23a5c90b9321b72a20f21752f957b3be0a9f3a02
workflow-type: tm+mt
source-wordcount: '2499'
ht-degree: 5%

---

# Realizar un seguimiento de los costes

<!-- Audited: 02/2024 -->

Puede realizar un seguimiento de los costos de los proyectos, las tareas y los problemas en Adobe Workfront.

## Cálculo de costes de Workfront

Para realizar un seguimiento de los costes, debe asociar los usuarios y las funciones del puesto con las tasas de coste por hora.

Las tasas de coste por hora son cantidades de costes por unidad de trabajo asociados con roles o usuarios. Multiplicar las tasas por las horas invertidas en el trabajo genera costos para sus proyectos, tareas o problemas.

Se dan los siguientes escenarios:

* Si el Tipo de costo de las tareas es Usuario por hora, la tarifa por hora del usuario calcula los costos de la tarea y del proyecto.

  Para obtener información acerca de cómo asociar usuarios con tasas de costo, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si el tipo de coste de las tareas es Rol por hora, la tasa por hora de la función de trabajo calcula los costes de la tarea y del proyecto.

  Para obtener información sobre cómo asociar roles con tasas de costo, consulte [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront calcula solamente el coste real de los problemas y los problemas no tienen un tipo de coste. Para obtener más información, consulte la sección [Cómo Workfront realiza un seguimiento de los costos de los problemas](#how-workfront-tracks-costs-for-issues) en este artículo.

>[!TIP]
>
>No se pueden anular las tasas de costo de los proyectos. Una vez establecida la tarifa de coste por hora de un usuario o rol, esa tarifa calcula todos los costes del sistema.

## Índices de rendimiento de costes de Workfront

Workfront calcula una serie de índices de rendimiento de costes para los proyectos, de modo que se pueda realizar un seguimiento de los proyectos para comprobar su rentabilidad.\
Para obtener más información sobre el cálculo de índices de rendimiento de costes, consulte:

* [Calcular el índice de rendimiento de costes (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcular índice de rendimiento de programación de costes (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcular el índice de rendimiento de programación (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Cómo Workfront realiza un seguimiento de los costos de tareas y proyectos

Los tipos de costos se calculan de manera diferente para las tareas y para los proyectos.

### Cómo Workfront rastrea los costes {#how-workfront-tracks-costs}

Puede realizar un seguimiento de varios tipos de costos para tareas y proyectos en Workfront. Los costes totales se calculan mediante la fórmula siguiente:

`Costs = Labor Costs + Expense Costs`

* **Los costos de mano de obra** están asociados con las horas de las tareas y proyectos y con las tasas de costo por hora de los recursos asociados con las tareas. Por lo general, Workfront calcula los siguientes costes laborales:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Costos laborales planificados</td> 
     <td> <p>Se calculan mediante la fórmula siguiente:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Costos laborales presupuestados</td> 
     <td> <p>Se calculan mediante la fórmula siguiente:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Costos laborales reales</td> 
     <td> <p>Se calculan mediante la fórmula siguiente:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> 
     <p><strong>NOTA</strong>
     <p>Workfront calcula el coste laboral real utilizando las horas reales heredadas. Para obtener más información, vea <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Ver horas reales</a>. </p>

  </td> 
    </tr> 
   </tbody> 
  </table>

  Para obtener más información, consulte la sección [Cómo calcula Workfront los costos planificados, presupuestados y reales](#how-workfront-calculates-planned-budgeted-and-actual-costs) en este artículo.

* **Los costos de gastos** están asociados con gastos en proyectos y tareas.\
  Al crear un proyecto, puede establecer los gastos planeados para todo el proyecto. Además, puede asociar gastos con tareas nuevas o existentes. Para obtener más información, consulte [Administrar gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Los costos fijos** se definen como una cantidad fija de costos para un proyecto. Esto es parte del costo planificado del proyecto, que representa la cantidad de dinero que usted necesita para completar el proyecto.

  >[!TIP]
  >
  >Al adjuntar una plantilla a un proyecto, el costo fijo de una plantilla se agrega al costo fijo del proyecto. Para obtener más información, vea [Información general sobre cómo adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Cómo calcula Workfront los costes planificados, presupuestados y reales {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calcula el costo planificado y el costo real de cada tarea individual de un proyecto. Workfront utiliza estos cálculos para tareas individuales a fin de calcular el costo planificado y el costo real del proyecto.

#### Costo planificado {#planned-cost}

El costo planificado de un proyecto es el costo asociado con el trabajo planificado (horas planificadas) en el proyecto.

El costo planificado de un proyecto se calcula mediante la siguiente fórmula:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Por ejemplo, tiene los siguientes gastos en la pestaña Gastos de una tarea: un gasto de marketing de 100 $ y un gasto administrativo de 50 $. En la pestaña Finanzas, seleccione el tipo de coste por hora Usuario. Se asigna un usuario a la tarea y la tarifa por hora del usuario es de 15 $. Se asigna al usuario 5 horas de trabajo en esta tarea. En la pestaña Gastos del proyecto, tiene un costo planificado de 100 $ para un gasto llamado Consultoría. También tiene un Costo fijo de $200 para el proyecto.

El costo planificado del proyecto se calcula de la siguiente manera:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

La tasa por hora de la fórmula tiene en cuenta cualquier cambio efectivo de fecha de la tasa.

#### Costo presupuestado {#budgeted-cost}

El costo presupuestado de un proyecto es el costo asociado con el trabajo presupuestado (horas presupuestadas) en el proyecto.

El costo presupuestado del proyecto es el mismo que el costo planificado del proyecto si se cumplen las dos condiciones siguientes:

* Las horas planificadas de las tareas del proyecto coinciden con las horas presupuestadas (en el Planificador de recursos).
* El tipo de facturación de las tareas es Rol por hora.

El coste presupuestado del proyecto se calcula mediante la fórmula siguiente si se cumplen las siguientes condiciones:

* Las horas planificadas de las tareas del proyecto no coinciden con las horas presupuestadas (en el Planificador de recursos).
* El tipo de facturación de las tareas es Rol por hora.

Cuando se cumplen las condiciones anteriores, Workfront calcula el coste presupuestado del proyecto mediante la fórmula siguiente:

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Costo real {#actual-cost}

El costo real de un proyecto es el costo asociado con el trabajo real (horas registradas) del proyecto.

El coste real se calcula mediante la fórmula siguiente:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Por ejemplo, tiene los siguientes gastos en la ficha Gastos de una tarea: un gasto de marketing con un costo real de 110 $ y un gasto administrativo con un costo real de 40 $. Seleccione el tipo de coste Rol por hora y asigne el rol Consultor a la tarea. La tarifa de la función de consultor es de 15 $ por hora y hay 6 horas registradas en la tarea para la función de consultor. Hay un gasto de consultoría asociado al proyecto (en la pestaña Gastos), con un costo real de 100 dólares y un usuario con una tasa de costo por hora de 20 dólares en sus registros de perfil de usuario 10 horas en el proyecto. También tiene un Costo fijo de $200 para el proyecto.

El costo real del proyecto se calcula de la siguiente manera:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

La tasa por hora de la fórmula tiene en cuenta cualquier cambio efectivo de fecha de la tasa.

>[!NOTE]
>
>El costo de gasto real del proyecto se calcula de la siguiente manera:
>>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Estos costes no se duplican en el cálculo de costes reales. Por ejemplo, si un costo fijo es parte del costo de gasto real del proyecto, no se agrega por separado al costo real.

>[!NOTE]
>
>Al registrar el tiempo en un proyecto, existen los siguientes escenarios al calcular el costo de mano de obra real del proyecto:
>
>* De forma predeterminada, Workfront utiliza la tarifa Costo por hora del usuario para calcular el Costo de mano de obra real.
>* Si el usuario que registra la hora no está asociado a ningún coste, Workfront utiliza la tasa de coste por hora de la función principal del usuario.
>* Si el administrador de Workfront habilitó la opción **Asignar roles a las entradas de horas manualmente** en el área de Preferencias de horas y hojas de horas de Configuración y el usuario que inicia sesión en el proyecto selecciona una función diferente para asociarla a esta hora, el costo real del proyecto se calcula en función de la función especificada cuando se registraron las horas. Para obtener información sobre la habilitación del tiempo de registro para una función específica, consulte el artículo [Configurar preferencias de plantillas de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Cómo calcula Workfront los tipos de coste de las tareas {#how-workfront-calculates-cost-types-for-tasks}

El coste planificado y real de las tareas y sus costes de mano de obra vienen determinados por el tipo de coste de cada tarea.

Puede configurar el Tipo de coste para tareas individuales dentro del proyecto. Cada tipo de coste afecta a los valores de Coste planificado y Coste real.

Para obtener información acerca de cómo modificar el tipo de costo de una tarea, vea [Actualizar tipo de costo de tarea](../../../manage-work/tasks/task-information/update-task-cost-type.md).

En la tabla siguiente se describen los tipos de coste de tarea disponibles en Workfront:

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>Tipo de costo de tarea</strong> </p> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>Usuario por hora</p> </td> 
   <td> <p>Éste es el tipo de costo predeterminado al crear una tarea.</p> <p><strong>Costo planificado</strong> se calcula mediante la siguiente fórmula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Donde el costo laboral planificado se calcula por:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Nota: <p>Tenga en cuenta los siguientes impactos de utilizar el tipo de coste por hora de usuario y calcular el coste planificado:</p> 
     <ul> 
      <li>Si asigna varios recursos a una tarea, Workfront ajusta los cálculos del costo planificado en función del porcentaje de la tarea asignada a cada recurso.</li>
      <li>Para tasas de costo efectivas por fecha, el costo de mano de obra planificada es la suma de los costos planificados de cada período de tiempo cubierto en la tarea.</li>
      <li>El valor del campo Costo planificado puede variar dependiendo de si ve el costo planificado desde la propia tarea o desde el informe de utilización.<br><strong>Al ver el costo planificado desde la propia tarea:</strong> El campo Costo planificado tiene en cuenta el campo Costo/hora establecido en el nivel de rol (cuando el campo Costo/hora no se ha establecido en el nivel de usuario).<br><strong>Al ver el costo planificado desde el informe de utilización del proyecto:</strong> El campo Costo planificado no tiene en cuenta el campo Costo/hora establecido en el nivel de rol. En su lugar, si desea que el informe Utilización tenga en cuenta el campo Coste/Hora establecido en el nivel de Rol, debe establecer el Tipo de coste de la tarea en Rol por hora. </li> 
     </ul> </p> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>donde el coste laboral real se calcula por:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Por ejemplo, un usuario tiene una tasa de coste por hora de 20 $ en su perfil. Cuando registran 5 horas para una tarea, el costo de mano de obra real es de 100 $ para esa tarea. Si el usuario no tiene asociada una tarifa de coste por hora, el coste real se calcula según la tarifa de coste por hora de su rol principal. Si no tienen un rol o la tasa de costo por hora de su rol no está definida, el costo real de la tarea es cero. </p> <p>Nota: Los costes reales se calculan según la tasa de coste por hora del usuario que registra el tiempo, independientemente de quién esté asignado a la tarea. Además, la tarifa por hora de facturación en la fórmula tiene en cuenta cualquier cambio de fecha en vigor de la tarifa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rol por hora</p> </td>
   <td> <p><strong>Costo planificado</strong> se calcula mediante la siguiente fórmula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>donde el costo de mano de obra planificado para la tarea se calcula mediante:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Nota: Si asigna varios recursos a una tarea, Workfront ajusta los cálculos de las horas planificadas en función del porcentaje de la tarea asignada a cada recurso. Además, la tasa por hora de la fórmula tiene en cuenta cualquier cambio efectivo de fecha de la tasa.</p> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>donde el costo de mano de obra real de la tarea se calcula mediante:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Por ejemplo, una tarea se asigna a un rol o a un usuario con un rol para el cual la tasa de costo por hora es de $20. Cuando un usuario registra 5 horas para una tarea, el costo de mano de obra real es de 100 $ para esa tarea. Si el usuario asignado a la tarea no tiene una función de trabajo asociada a él en la tarea, el coste real se calcula según la tasa de coste por hora de su rol principal. Si no tienen un rol o la tasa de costo por hora de su rol no está definida, el costo real de la tarea es cero. </p> <p>Nota: Las horas reales de una tarea de rol por hora se calculan según los roles de trabajo de los usuarios asociados a la tarea, no según los roles asociados al usuario que está registrando la hora. Además, la tarifa por hora de facturación en la fórmula tiene en cuenta cualquier cambio de fecha en vigor de la tarifa.</p> <p>Si el administrador de Workfront habilitó la opción <strong>Asignar roles a las entradas de hora manualmente</strong> en el área Preferencias de horas y hojas de horas en Configuración y el usuario que registra el tiempo en la tarea selecciona una función diferente para asociarla con este tiempo, el costo real de una tarea por hora de función calcula según la función especificada cuando se registraron las horas. Para obtener información sobre la habilitación del tiempo de registro para una función específica, consulte el artículo <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar preferencias de plantillas de horas y de horas</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fijo por hora</p> </td> 
   <td> <p><strong>Costo planificado</strong> se calcula mediante la siguiente fórmula:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>donde el costo de mano de obra de la tarea se calcula por:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Donde el costo de mano de obra de la tarea real se calcula mediante:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Este tipo de coste no tiene en cuenta los usuarios individuales ni las funciones del puesto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sin coste</p> </td> 
   <td> <p>Este tipo de coste no afecta a los costes. Si una tarea principal tiene este tipo de costo, las subtareas con otro tipo de costo calculan según sus tipos de costo individuales y el costo de la tarea principal se ve afectado en consecuencia. </p> <p>Cuando un usuario sin acceso a datos financieros o un usuario sin permisos financieros en una plantilla crea un proyecto a partir de esa plantilla, este es el tipo de coste predeterminado para las tareas del proyecto.</p> <p>Para obtener información sobre el acceso a los datos financieros, consulte el artículo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acceso a los datos financieros</a>.</p> <p>Para obtener información acerca de los permisos financieros de los objetos, vea el artículo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartir permisos financieros de un objeto</a>.</p> <p>Para obtener información acerca de cómo crear proyectos a partir de plantillas, vea el artículo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Crear un proyecto mediante una plantilla</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo Workfront rastrea los costes de los problemas {#how-workfront-tracks-costs-for-issues}

Los problemas no tienen los siguientes tipos de costos en un proyecto y no los afectan:

* Costo planificado
* Costo presupuestado

Los problemas, sin embargo, pueden tener un **Costo real**, que también afecta al Costo real del proyecto.

En la tabla siguiente se explica cómo se calcula el costo real de los problemas, según el tipo de asignación del problema:

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>Asignación de usuarios</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>La tasa de costo por hora del usuario que registra la hora se tiene en cuenta aquí, independientemente de quién esté asignado al problema. </p> <p>Si el usuario que registra el tiempo no tiene una tasa de costo por hora en su perfil, la tasa de costo por hora de su rol principal calcula el costo real del problema.</p> <p>Si el usuario que registra la hora no tiene ninguna función en su perfil o no tiene ninguna tasa asociada a él, las horas reales se calculan utilizando la tasa de coste por hora de la función de trabajo principal de la persona asignada principal en el problema. Si esa función no tiene definida ninguna tasa, el costo real del problema es cero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Asignación de funciones</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>La tasa de costo por hora del usuario que registra el tiempo en el problema se tiene en cuenta aquí, independientemente de la función que se asigne al problema. </p> <p>Si el usuario que registra el tiempo no tiene asociada una tasa de costo por hora, la tasa de costo por hora de su rol principal calcula el costo real del problema.</p><p>Si el usuario que registra la hora no tiene ninguna función en su perfil o no tiene ninguna tasa asociada, el coste real del problema es cero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sin asignación</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo real</strong> se calcula mediante la fórmula siguiente:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Si el usuario que registra el tiempo no tiene una tasa de costo por hora asociada a su perfil, la tasa de costo por hora de su rol principal calcula el costo real del problema. </p> <p>Si el usuario que registra el tiempo no tiene ninguna función de trabajo asociada a su perfil o la función de trabajo principal no tiene definida una tasa de coste por hora, el coste real del problema es cero. </p> </td> 
  </tr> 
 </tbody> 
</table>
