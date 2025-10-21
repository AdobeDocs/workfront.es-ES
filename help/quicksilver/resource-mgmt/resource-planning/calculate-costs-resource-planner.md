---
product-area: resource-management
navigation-topic: resource-planning
title: Calcular costes en el Planificador de recursos
description: Puede presupuestar sus recursos en el Planificador de recursos de Adobe Workfront utilizando valores de Coste, en lugar de valores de Horas o FTE. Los valores de coste no están disponibles para la vista **Ver por usuario** en el Planificador de recursos.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 98%

---

# Calcular costes en el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Puede presupuestar sus recursos en el Planificador de recursos de Adobe Workfront utilizando valores de Coste, en lugar de valores de Horas o FTE. Los valores de coste no están disponibles para la vista **Ver por usuario** en el Planificador de recursos.

>[!IMPORTANT]
>
>Debe asociar usuarios y funciones con las tarifas de Coste por hora para mostrar la información de coste en el Planificador de recursos.\
>Para obtener más información sobre cómo asociar las tarifas de Coste por hora con las funciones de trabajo, consulte [Crear y administrar funciones de trabajo](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Para obtener más información sobre cómo asociar las tarifas de Coste por hora con los usuarios, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Antes de presupuestar los recursos, asegúrese de que comprende bien qué trabajo se debe realizar (Horas planificadas, FTE o Coste) y qué disponibilidad de tiempo de trabajo tienen los usuarios (Horas disponibles, FTE o Coste).\
Para obtener más información sobre el funcionamiento del Planificador de recursos al presupuestar por horas o FTE, consulte [Información general sobre horas, FTE y costes en las vistas de proyecto y función del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td>
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a la administración de recursos que incluye acceso a Editar prioridades y horas presupuestadas en el Planificador de recursos</p> <p>Acceso de edición a datos financieros, proyectos y usuarios</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Permisos de administración a los proyectos para los que desea presupuestar información con capacidad de Administrar finanzas</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar información en el Planificador de recursos por Coste

De forma predeterminada, la información de disponibilidad y asignación se muestra en Horas en el Planificador de recursos.

Para mostrar la información sobre horas disponibles, planificadas y presupuestadas por Coste en el Planificador de recursos:

{{step1-to-resourcing}}

1. Vaya al Planificador de recursos.
1. (Condicional) Seleccione **Ver por proyecto** o **Ver por función**.\
   De manera predeterminada, la opción seleccionada es **Ver por proyecto**.\
   La información de asignación y disponibilidad se muestra en horas.

1. En el menú desplegable **Horas**, seleccione **Coste**.

   Si no tiene acceso a los datos financieros con su nivel de acceso, esta opción no está disponible.\
   Si los proyectos tienen una moneda diferente a la del sistema, el coste de estos proyectos se muestra en el Planificador de recursos convertido a la moneda del sistema. El administrador del sistema define la moneda del sistema.\
   Para obtener más información sobre cómo configurar la moneda del sistema en Workfront y las tasas de conversión, consulte [Configurar las tasas de cambio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcular coste disponible en el Planificador de recursos

Para mostrar los valores de Coste disponible en el Planificador de recursos, debe tener lo siguiente:

* Tarifas de coste por hora para los usuarios y los roles
* Información sobre la disponibilidad del usuario.

  La obtención de información sobre la disponibilidad del usuario depende de cómo configure el administrador de Workfront las preferencias de administración de recursos.\
  Para obtener más información sobre cómo calcular la disponibilidad del usuario y establecer las preferencias de administración de recursos, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

En la tabla siguiente se muestra cómo se calcula el coste disponible en el Planificador de recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Coste disponible</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Coste disponible por usuario</td> 
   <td> <p>El coste disponible por usuario se calcula con la fórmula siguiente:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Si el usuario no tuviera una tasa de coste por hora en su perfil, se utilizará en el cálculo la tasa de coste por hora de la función en la que aparezca. Si el usuario no tuviera ninguna función asociada a el, el coste por usuario disponible será de 0 $. </p> </td>
</tr> 
  <tr> 
   <td>Coste disponible por función</td> 
   <td> <p>El coste disponible por función se calcula con la fórmula siguiente:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Si la función no tuviera una tarifa de coste por hora, el coste por función disponible será de 0 $.</p> </td>
</tr> 
  <tr> 
   <td>Coste disponible por proyecto</td> 
   <td> <p>El coste disponible por proyecto se calcula con la fórmula siguiente:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcular el coste planificado en el planificador de recursos

Aunque no es posible ver información sobre tareas en el Planificador de recursos, los costes planificados de los usuarios, funciones y proyectos se calculan teniendo en cuenta la siguiente información sobre tareas:

* Tipo de asignación de la tarea.\
  Es posible dejar tareas sin asignar o asignarles las siguientes entidades:

   * Un usuario (con o sin función)
   * Una función
   * Un equipo\
     Una tarea asignada a un equipo se considera no asignada desde la perspectiva del Planificador de recursos.

* **Tipo de coste** de las tareas del proyecto.\
  Para obtener más información sobre el tipo de coste de una tarea, consulte [Rastreo de costes](../../manage-work/projects/project-finances/track-costs.md).

* Fechas en vigor de las tasas de coste de funciones y usuarios.

  Por ejemplo, si la función o usuario tuviera 10 horas planificadas en febrero y 10 horas planificadas en marzo, pero la tasa de coste cambió de 12 a 20 $ en marzo, el valor del coste planificado de febrero será de 120 $ y en marzo de 200 $.

>[!NOTE]
>
>Los costes planificados por usuario no influirán en el coste planificado del proyecto. En el Planificador de recursos, solo los costes planificados por funciones afectarán a los costes planificados del proyecto.

Existen los siguientes escenarios al calcular el coste planificado de usuarios, funciones y proyectos:

* Cuando **Tipo de costo** es **Usuario por hora** y no hay **ninguna asignación** en la tarea:

   * **Coste planificado por función y usuario**:

     Los costes planificados por función y usuario serán de 0,00 $.

   * **Coste planificado del proyecto**:

     El coste planificado del proyecto será de 0,00 $.

* Cuando **Tipo de coste** sea **Usuario por hora** y haya una **asignación de usuario** en la tarea:

   * **Coste planificado por función y usuario**:

     El coste planificado por usuario se calcula con la siguiente fórmula:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Si un usuario tuviera una tasa de coste en su perfil, esa tasa se utilizará para calcular el coste planificado. De lo contrario, se utilizará la tasa de coste por hora a nivel de sistema de su función principal.

     >[!NOTE]
     >
     >El usuario puede asignarse a la tarea con una de sus funciones secundarias, pero la tasa de la función principal se utilizará aquí en su lugar.

     El coste planificado por función se calcula con la fórmula siguiente:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Coste planificado del proyecto**:

     El coste planificado del proyecto será de 0,00 $.

* Cuando el **tipo de coste** sea **usuario por hora** y haya una **asignación de función** en la tarea:

   * **Coste planificado por función y usuario**:

     El coste planificado por usuario será de 0,00 $.

     El coste planificado por función se calcula con la fórmula siguiente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     La tasa de coste por hora a nivel de sistema de la función asignada a la tarea se utiliza para calcular el coste planificado.

   * **Coste planificado del proyecto**:

     El coste planificado del proyecto será de 0,00 $.

* Cuando el **Tipo de coste** sea **Función por hora** y no haya **ninguna asignación** en la tarea:

   * **Costo planificado por función y usuario**:

     Los costes planificados por función y usuario serán de 0,00 $.

   * **Coste planificado del proyecto**:

     El coste planificado del proyecto será de 0,00 $.

* Cuando el **Tipo de coste** sea **Función por hora** y haya una **asignación de usuario** en la tarea:

   * **Coste planificado por función y usuario**:

     El coste planificado por usuario será de 0,00 $.

     El coste planificado por función se calcula con la fórmula siguiente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront busca la función que cumple el usuario en la tarea para calcular el coste planificado para la función.

     Si el usuario no está asociado a ninguna función en la tarea, el coste planificado es de 0 USD.

   * **Coste planificado del proyecto**:

     El coste planificado del proyecto se calcula mediante la siguiente fórmula:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Cuando el **Tipo de coste** sea **Función por hora** y haya una **asignación de función** en la tarea:

   * **Coste planificado por función y usuario**:

     El coste planificado por usuario será de 0,00 $.

     El coste planificado por función se calcula con la fórmula siguiente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront busca la función que cumple el usuario en la tarea para calcular el coste planificado para la función.

   * **Coste planificado del proyecto**:

     El coste planificado del proyecto se calcula mediante la siguiente fórmula:

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

## Calcular el coste presupuestado en el planificador de recursos

Para mostrar los valores del coste presupuestado en el planificador de recursos, debe tener lo siguiente:

* Horas presupuestadas para funciones, usuarios y proyectos.
* Tarifas de coste por hora para usuarios y funciones.

>[!NOTE]
>
>Las horas presupuestadas para los proyectos se calculan en función de las horas presupuestadas para las funciones, no de los usuarios.

La siguiente tabla ilustra cómo se calcula el coste presupuestado en el Planificador de recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Coste presupuestado</strong> </th> 
   <th><strong>Cálculo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Coste presupuestado del usuario</td> 
   <td> <p>El coste presupuestado por usuario se calcula con la siguiente fórmula:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Si el usuario no tiene una tarifa de coste por hora en su perfil, el coste de usuario presupuestado es de 0 USD.</p> </p> </td>
</tr> 
  <tr> 
   <td>Coste presupuestado de función</td> 
   <td> <p>El coste presupuestado de la función se calcula con la siguiente fórmula:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Si la función no tiene una tasa de coste por hora, el coste de la función presupuestada es de 0 USD.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo presupuestado de proyecto</td> 
   <td> <p>El coste presupuestado por proyecto se calcula con la siguiente fórmula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
