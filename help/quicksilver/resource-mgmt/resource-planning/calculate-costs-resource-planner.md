---
product-area: resource-management
navigation-topic: resource-planning
title: Calcular los costes en el planificador de recursos
description: '(Alina: ***Vinculado a la planificación en el artículo Planificador de recursos, Explicación de las áreas del Planificador de recursos. - no mueva/cambie/elimine)'
author: Alina
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 0%

---

# Calcular los costes en el planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

Puede presupuestar los recursos en el planificador de recursos de Adobe Workfront utilizando los valores de Coste, en lugar de los valores de Horas o FTE. Los valores de coste no están disponibles para la variable **Ver por usuario** en el Planificador de recursos.

>[!IMPORTANT]
>
>Debe asociar usuarios y funciones de trabajo con las tasas de Costo por hora para mostrar la información de Coste en el Planificador de Recursos.\
>Para obtener más información sobre cómo asociar tasas de costo por hora con funciones de trabajo, consulte [Crear y administrar funciones de trabajo](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Para obtener más información sobre cómo asociar las tasas de costo por hora con los usuarios, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Antes de presupuestar los recursos, asegúrese de comprender bien qué trabajo se debe realizar (horas planificadas, tiempo de espera medio o coste) y a qué hora los usuarios están abiertos al trabajo (horas disponibles, tiempo de espera medio o coste).\
Para obtener más información sobre cómo comprender la información del planificador de recursos al realizar presupuestos por horas o por horas, consulte [Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a la Administración de recursos que incluye acceso a Editar prioridades y horas de presupuesto en el Planificador de recursos</p> <p>Editar acceso a datos financieros, proyectos y usuarios</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre los permisos de los proyectos para los que desea presupuestar información con capacidad para Administrar finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar información en el Planificador de Recursos por Coste

De forma predeterminada, la información de disponibilidad y asignación se muestra en Horas en el Planificador de recursos.

Para mostrar la información Disponible, Planificado y Presupuestado por Coste en el Planificador de Recursos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recurso**.
1. Vaya a .
1. (Condicional) Seleccione **Ver por proyecto** o **Ver por función**.\
   De forma predeterminada **Ver por proyecto** está seleccionado.\
   La información de asignación y disponibilidad se muestra en Horas.

1. En el **Horas** menú desplegable, seleccione **Costo**.

   Si no tiene acceso a Datos financieros en el nivel de acceso, esta opción no está disponible.\
   Si los proyectos tienen una moneda diferente a la moneda del sistema, el Coste de estos proyectos se muestra en el Planificador de recursos convertido en la moneda del sistema. El administrador del sistema define la moneda del sistema.\
   Para obtener más información sobre la configuración de la moneda del sistema en Workfront y las tasas de conversión, consulte [Configurar tipos de cambio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budget.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcular Coste Disponible en el Planificador de Recursos

Para mostrar los valores de Coste disponible en el Planificador de recursos debe tener lo siguiente:

* Tarifas de coste por hora para usuarios y funciones
* Información sobre la disponibilidad del usuario.

   La obtención de información sobre la disponibilidad del usuario depende de cómo configure el administrador de Workfront las preferencias de administración de recursos.\
   Para obtener más información sobre cómo calcular la disponibilidad del usuario y establecer las preferencias de administración de recursos, consulte [Configurar las preferencias de Administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

La siguiente tabla ilustra cómo se calcula el costo disponible en el Planificador de recursos:

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
   <td>Coste disponible del usuario</td> 
   <td> <p>El coste disponible por usuario se calcula mediante la fórmula siguiente:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Si el usuario no tiene una tasa de coste por hora en su perfil, se utiliza en el cálculo la tasa de coste por hora de la función de trabajo en la que aparece. Si el usuario no tiene ninguna función asociada, el costo de usuario disponible es de 0 $. </p> </td>
</tr> 
  <tr> 
   <td>Costo disponible de rol</td> 
   <td> <p>El costo disponible por función se calcula mediante la fórmula siguiente:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Si la función no tiene una tasa de costo por hora, el costo de función disponible es de 0 $.</p> </td>
</tr> 
  <tr> 
   <td>Costo disponible del proyecto</td> 
   <td> <p>El costo disponible por proyecto se calcula mediante la fórmula siguiente:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcular Coste Planificado en el Planificador de Recursos

Aunque no puede ver la información de tareas en el planificador de recursos, los costes planificados para usuarios, funciones y proyectos se calculan teniendo en cuenta la siguiente información de tareas:

* Tipo de asignación en la tarea.\
   Puede dejar una tarea sin asignar o asignar las siguientes entidades a una tarea:

   * Un usuario (con o sin una función de trabajo)
   * Un papel
   * Un equipo\
      Una tarea asignada a un equipo se considera sin asignar, desde la perspectiva del Planificador de Recursos.

* La variable **Tipo de costo** de las tareas del proyecto.\
   Para obtener más información sobre el tipo de coste de una tarea, consulte [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md).

>[!NOTE]
>
>Los costes planificados por el usuario no influyen en el coste planificado del proyecto. En el Planificador de Recursos, sólo los costos planificados de función afectan a los costos planificados del proyecto.

Existen las siguientes situaciones al calcular el coste planeado para usuarios, funciones y el proyecto:

* Cuando la variable **Tipo de costo** es **Por hora de usuario **y hay **sin asignación** en la tarea:

   * **Función y costo planificado por el usuario**:

      Los costes planeados por el usuario y la función son de 0,00 $.

   * **Costo planeado del proyecto**:

      El costo planeado del proyecto es de 0,00 $.

* Cuando la variable **Tipo de costo** es **Usuario por hora** y hay un **asignación de usuarios** en la tarea:

   * **Función y costo planificado por el usuario**:

      El coste planificado por el usuario se calcula mediante la fórmula siguiente:



      ```
      User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
      ```

      Si un usuario tiene una tasa de coste en su perfil, esa tasa se utiliza para calcular el coste planeado. De lo contrario, se utiliza la tasa de costo por hora a nivel de sistema de su función principal.

      >[!NOTE]
      >
      >El usuario puede asignarse a la tarea con una de sus funciones de trabajo secundarias, pero la tasa de la función de trabajo principal se utiliza aquí en su lugar.

      El coste planificado de función se calcula mediante la fórmula siguiente:

      ```
      Role Planned Cost = SUM(User Planned Cost)
      ```

   * **Costo planeado del proyecto**:

      El costo planeado del proyecto es de 0,00 $.

* Cuando la variable **Tipo de costo** es **Usuario por hora** y hay un **asignación de funciones de trabajo** en la tarea:

   * **Función y costo planificado por el usuario**:

      El costo planeado por el usuario es de 0,00 $.

      El coste planificado de función se calcula mediante la fórmula siguiente:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      La tasa Costo por hora a nivel de sistema de la función de trabajo asignada a la tarea se utiliza para calcular Coste planificado.

   * **Costo planeado del proyecto**:

      El costo planeado del proyecto es de 0,00 $.

* Cuando la variable **Tipo de costo** es **Función por hora** y hay **sin asignación** en la tarea:

   * **Función y costo planificado por el usuario**:

      Los costes planeados por el usuario y la función son de 0,00 $.

   * **Costo planeado del proyecto**:

      El costo planeado del proyecto es de 0,00 $.

* Cuando la variable **Tipo de costo** es **Función por hora** y hay un **asignación de usuarios** en la tarea:

   * **Función y costo planificado por el usuario**:

      El costo planeado por el usuario es de 0,00 $.

      La función Costo planeado se calcula mediante la siguiente fórmula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront examina la función de trabajo que el usuario cumple en la tarea para calcular el coste planeado de la función.

      Si el usuario no está asociado a ninguna función de la tarea, el coste planeado es de 0,00 $.

   * **Costo planeado del proyecto**:

      El costo planificado del proyecto se calcula mediante la fórmula siguiente:

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

* Cuando la variable **Tipo de costo** es **Función por hora** y hay un **asignación de funciones de trabajo** en la tarea:

   * **Función y costo planificado por el usuario**:

      El costo planeado por el usuario es de 0,00 $.

      La función Costo planeado se calcula mediante la siguiente fórmula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront examina la función de trabajo que el usuario cumple en la tarea para calcular el coste planeado de la función.

   * **Costo planeado del proyecto**:

      El costo planificado del proyecto se calcula mediante la fórmula siguiente:

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

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

Para mostrar los valores de Coste presupuestado en el planificador de recursos, debe tener lo siguiente:

* Horas presupuestadas para funciones, usuarios y proyectos.
* Tarifas de coste por hora para usuarios y funciones.

>[!NOTE]
>
>Las horas presupuestadas para los proyectos se calculan en función de las horas presupuestadas para las funciones, no de las de los usuarios.

La siguiente tabla ilustra cómo se calcula el costo presupuestado en Resource Planner:

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
   <td>Coste presupuestado del usuario</td> 
   <td> <p>El coste presupuestado por usuario se calcula mediante la fórmula siguiente:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Si el usuario no tiene una tasa de costo por hora en su perfil, el costo de usuario presupuestado es de 0,00 $.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo presupuestado de función</td> 
   <td> <p>El coste presupuestado de funciones se calcula mediante la fórmula siguiente:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Si la función no tiene una tasa de costo por hora, el costo de función presupuestado es de 0,00 $.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo presupuestado de proyecto</td> 
   <td> <p>El costo presupuestado por proyecto se calcula mediante la fórmula siguiente:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
