---
product-area: resource-management
navigation-topic: resource-planning
title: Calcular costos en el Planificador de recursos
description: Puede presupuestar sus recursos en el Planificador de recursos de Adobe Workfront utilizando valores de Costo, en lugar de valores de Horas o FTE. Los valores de costo no están disponibles para la vista **Ver por usuario** en el Planificador de recursos.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Calcular costos en el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Puede presupuestar sus recursos en el Planificador de recursos de Adobe Workfront utilizando valores de Costo, en lugar de valores de Horas o FTE. Los valores de coste no están disponibles para **Ver por usuario** vista en el Planificador de recursos.

>[!IMPORTANT]
>
>Debe asociar usuarios y roles con tasas de costo por hora para mostrar la información de costo en el Planificador de recursos.\
>Para obtener más información sobre la asociación de tasas de coste por hora con roles de trabajo, consulte [Crear y administrar roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Para obtener más información sobre cómo asociar las tarifas de costo por hora con los usuarios, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Antes de presupuestar los recursos, asegúrese de que comprende bien qué trabajo se debe realizar (Horas planificadas, ETC o Costo) y qué tiempo están abiertos a trabajar los usuarios (Horas disponibles, ETC o Costo).\
Para obtener más información acerca de cómo comprender la información del Planificador de recursos al realizar presupuestos por horas o ETC, consulte [Información general sobre horas, ETC y costos en las vistas Proyecto y Rol del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Editar prioridades y horas presupuestadas en el Planificador de recursos</p> <p>Editar acceso a datos financieros, proyectos y usuarios</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos a los proyectos para los que desea presupuestar información con capacidad de Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Mostrar información en el Planificador de recursos por costo

De forma predeterminada, la información de disponibilidad y asignación se muestra en Horas en el Planificador de recursos.

Para mostrar la información disponible, planificada y presupuestada por costo en el Planificador de recursos:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Clic **Recursos**.
1. Vaya al Planificador de recursos.
1. (Condicional) Seleccione **Ver por proyecto** o **Ver por rol**.\
   De forma predeterminada **Ver por proyecto** está seleccionado.\
   La información de asignación y disponibilidad se muestra en horas.

1. Desde el **Horas** menú desplegable, seleccione **Coste**.

   Si no tiene acceso a los datos financieros en su nivel de acceso, esta opción no está disponible.\
   Si los proyectos tienen una moneda diferente a la del sistema, el costo de estos proyectos se muestra en el Planificador de recursos convertido a la moneda del sistema. El administrador del sistema define la moneda del sistema.\
   Para obtener más información sobre la configuración de la divisa del sistema en Workfront y las tasas de conversión, consulte [Configurar tasas de cambio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budget.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcular el costo disponible en el planificador de recursos

Para mostrar los valores de Costo disponible en el Planificador de recursos, debe tener lo siguiente:

* Tarifas de costo por hora para los usuarios y los roles
* Información sobre la disponibilidad del usuario.

  La obtención de información sobre la disponibilidad del usuario depende de cómo configure el administrador de Workfront las Preferencias de administración de recursos.\
  Para obtener más información sobre cómo calcular la disponibilidad de los usuarios y establecer las Preferencias de administración de recursos, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

En la tabla siguiente se muestra cómo se calcula el costo disponible en el Planificador de recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Costo disponible</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Coste disponible de usuario</td> 
   <td> <p>El coste disponible por usuario se calcula mediante la fórmula siguiente:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Si el usuario no tiene una tasa de coste por hora en su perfil, se utiliza en el cálculo la tasa de coste por hora de la función en la que aparece. Si el usuario no tiene ninguna función asociada a él, el coste de usuario disponible es de 0 $. </p> </td>
</tr> 
  <tr> 
   <td>Costo disponible de rol</td> 
   <td> <p>El coste disponible por rol se calcula mediante la fórmula siguiente:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Si la función no tiene una tarifa de coste por hora, el coste de la función disponible es de 0 $.</p> </td>
</tr> 
  <tr> 
   <td>Costo disponible de proyecto</td> 
   <td> <p>El coste disponible por proyecto se calcula mediante la fórmula siguiente:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcular el costo planificado en el planificador de recursos

Aunque no puede ver información de tareas en el Planificador de recursos, los costos planificados para los usuarios, roles y proyectos se calculan teniendo en cuenta la siguiente información de tareas:

* Tipo de asignación de la tarea.\
  Puede dejar una tarea sin asignar o asignar las siguientes entidades a una tarea:

   * Un usuario (con o sin rol)
   * Un rol
   * Un equipo\
     Una tarea asignada a un equipo se considera no asignada, desde la perspectiva del Planificador de recursos.

* El **Tipo de coste** de las tareas del proyecto.\
  Para obtener más información sobre el tipo de coste de una tarea, consulte [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md).

* Las fechas en vigor de las tasas de coste para los roles de trabajo y los usuarios.

  Por ejemplo, si el rol o usuario tiene 10 horas planificadas en febrero y 10 horas planificadas en marzo, pero la tasa de coste ha cambiado de 12 a 20 dólares en marzo, el valor del coste planificado en febrero es de 120 dólares y en marzo el coste planificado es de 200 dólares.

>[!NOTE]
>
>Los costos planificados por el usuario no influyen en el costo planificado del proyecto. En el Planificador de recursos, sólo los costos planificados para roles afectan a los costos planificados para el proyecto.

Existen los siguientes escenarios al calcular el costo planificado para usuarios, roles y el proyecto:

* Si la variable **Tipo de coste** es **Usuario por hora **y hay **sin asignación** en la tarea:

   * **Costo planificado por rol y usuario**:

     Los costos planificados por el rol y el usuario son de $0,00.

   * **Costo planificado del proyecto**:

     El costo planificado del proyecto es de $0,00.

* Si la variable **Tipo de coste** es **Usuario por hora** y hay un **asignación de usuario** en la tarea:

   * **Costo planificado por rol y usuario**:

     El coste planificado por el usuario se calcula mediante la siguiente fórmula:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Si un usuario tiene una tasa de coste en su perfil, esa tasa se utiliza para calcular el coste planificado. De lo contrario, se utiliza la tasa de coste por hora a nivel de sistema de su rol principal.

     >[!NOTE]
     >
     >El usuario puede asignarse a la tarea con uno de sus roles de trabajo secundarios, pero la tasa del rol principal se utiliza aquí en su lugar.

     El coste planificado de rol se calcula mediante la fórmula siguiente:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Costo planificado del proyecto**:

     El costo planificado del proyecto es de $0,00.

* Si la variable **Tipo de coste** es **Usuario por hora** y hay un **asignación de rol** en la tarea:

   * **Costo planificado por rol y usuario**:

     El costo planificado por el usuario es de 0,00 $.

     El coste planificado de rol se calcula mediante la fórmula siguiente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     La tasa de costo por hora a nivel de sistema de la función de trabajo asignada a la tarea se utiliza para calcular el costo planificado.

   * **Costo planificado del proyecto**:

     El costo planificado del proyecto es de $0,00.

* Si la variable **Tipo de coste** es **Rol por hora** y hay **sin asignación** en la tarea:

   * **Costo planificado por rol y usuario**:

     Los costos planificados por el rol y el usuario son de $0,00.

   * **Costo planificado del proyecto**:

     El costo planificado del proyecto es de $0,00.

* Si la variable **Tipo de coste** es **Rol por hora** y hay un **asignación de usuario** en la tarea:

   * **Costo planificado por rol y usuario**:

     El costo planificado por el usuario es de 0,00 $.

     El coste planificado de rol se calcula mediante la siguiente fórmula:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront busca la función que cumple el usuario en la tarea para calcular el coste planificado de la función.

     Si el usuario no está asociado con ningún rol en la tarea, el costo planificado es de 0,00 $.

   * **Costo planificado del proyecto**:

     El costo planificado del proyecto se calcula mediante la siguiente fórmula:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Si la variable **Tipo de coste** es **Rol por hora** y hay un **asignación de rol** en la tarea:

   * **Costo planificado por rol y usuario**:

     El costo planificado por el usuario es de 0,00 $.

     El coste planificado de rol se calcula mediante la siguiente fórmula:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront busca la función que cumple el usuario en la tarea para calcular el coste planificado de la función.

   * **Costo planificado del proyecto**:

     El costo planificado del proyecto se calcula mediante la siguiente fórmula:

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
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
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Calcular costo presupuestado en el planificador de recursos

Para mostrar los valores de costo presupuestado en el Planificador de recursos, debe tener lo siguiente:

* Horas presupuestadas para roles, usuarios y proyectos.
* Tarifas de costo por hora para usuarios y roles.

>[!NOTE]
>
>Las horas presupuestadas de los proyectos se calculan en función de las horas presupuestadas de los roles, no de las de los usuarios.

La siguiente tabla ilustra cómo se calcula el costo presupuestado en el Planificador de recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Costo presupuestado</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo presupuestado de usuario</td> 
   <td> <p>El coste presupuestado por usuario se calcula mediante la siguiente fórmula:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Si el usuario no tiene una tarifa de coste por hora en su perfil, el coste de usuario presupuestado es de 0,00 $.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo presupuestado de rol</td> 
   <td> <p>El coste presupuestado de la función se calcula mediante la siguiente fórmula:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Si la función no tiene una tasa de coste por hora, el coste de la función presupuestado es de 0,00 $.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo presupuestado de proyecto</td> 
   <td> <p>El costo presupuestado por proyecto se calcula mediante la siguiente fórmula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
