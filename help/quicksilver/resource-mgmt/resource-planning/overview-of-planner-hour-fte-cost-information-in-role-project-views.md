---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos
description: Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2973'
ht-degree: 0%

---

# Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

La principal función del planificador de recursos es presupuestar los recursos para el trabajo que deben realizar en un proyecto. Puede ver el tiempo disponible de sus recursos, así como asignar su tiempo a los proyectos a los que están asignados.

Para obtener información sobre la presupuestación de recursos en el planificador de recursos, consulte [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

En este artículo se describen algunos de los conceptos clave que debe conocer antes de comenzar a presupuestar los recursos en el planificador de recursos.

## Información general sobre los recursos de presupuesto

Tenga en cuenta lo siguiente al presupuestar recursos mediante el planificador de recursos:

* Puede presupuestar la asignación de los recursos especificando una cantidad de horas, FTE o Coste que los recursos pueden utilizar para completar el trabajo en los proyectos. Cuando se presupuestan el tiempo o el costo de un recurso, las horas disponibles, el tiempo disponible, el tiempo disponible o el costo del recurso disminuyen en la cantidad presupuestada. Como resultado, los importes de horas disponibles, horas a plazo, o costes para los proyectos que siguen al proyecto para el que está presupuestando disminuyen para esos usuarios y funciones en esos proyectos.

   >[!IMPORTANT]
   >
   >Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información del presupuesto no sea precisa.

* Puede presupuestar horas, FTE o costo de los recursos para cualquier lapso de tiempo mostrado en el Planificador de recursos, independientemente de la cronología del proyecto. Por ejemplo, si desea indicar que los recursos podrían no estar disponibles durante la cronología del proyecto (donde están asociados con Horario planificado), pero que podrían estar disponibles durante otro tiempo, puede hacerlo presupuestándolos para lapsos de tiempo en los que las horas planificadas sean cero, si es que están disponibles para funcionar. Después de hacerlo, puede cambiar manualmente la cronología del proyecto para que coincida con la disponibilidad de los recursos.

   >[!NOTE]
   >
   >Le recomendamos que presupueste manualmente sus horas, FTE o Coste para las funciones de trabajo o para los usuarios primero. Puede utilizar las opciones automáticas para presupuestar el tiempo de sus proyectos y recursos solo cuando esté seguro de que la cantidad de horas planificadas, horas de espera o costes siempre debe coincidir con las horas, horas de espera o costes presupuestados.\
   >Para obtener información sobre el uso de las opciones automáticas para la presupuestación en el planificador de recursos, consulte la sección &quot;Proyecto presupuestario y funciones automáticamente&quot; en el artículo [Revisar la disponibilidad y asignación de recursos con el planificador de recursos de Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* El cálculo de FTE o costes es idéntico al de las horas de presupuestación, en las que Adobe Workfront utiliza los valores FTE y de coste en lugar de horas para los recursos que se presupuestan.

   Para obtener más información sobre cómo se calculan los costes en el planificador de recursos, consulte [Calcular los costes en el planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* La asignación de presupuestos para sus recursos en el Planificador de recursos se realiza de las siguientes maneras:

   * Manualmente

      O

   * Automáticamente, utilizando las opciones de proyecto y función en la variable **Ver por proyecto** y **Ver por función** vistas.
   Para obtener más información, consulte [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Cuando un usuario cambia de funciones de trabajo, se elimina, desactiva o elimina de un grupo de recursos, las horas presupuestadas para la función no cambian y se redistribuyen a los usuarios restantes de la función. Si ya no hay ningún usuario asociado con la función de trabajo, las horas presupuestadas para la función se convierten en cero.

Para obtener más información sobre las opciones de proyecto y función, consulte la sección [Comprender los valores de Horas, FTE y Coste en Resource Planner](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) en este artículo.

## Comprender los valores de Horas, FTE y Coste en Resource Planner {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Antes de presupuestar los recursos y actualizar la información de horas presupuestadas en el planificador de recursos, debe estar familiarizado con los siguientes conceptos

* **Horas, FTE o costo planeados**: El trabajo que debe realizarse tal como se define en las tareas y los problemas.
* **Horas, FTE o costo disponibles**: Cantidad de tiempo que los usuarios o las funciones de trabajo están disponibles para trabajar, según las programaciones asociadas con los usuarios.

Esta información se muestra en el Planificador de recursos para cada recurso (usuario o función) y para cada proyecto.

Para obtener información sobre la visualización en las vistas Proyecto y Función del proyecto, consulte el artículo [Información general sobre navegación del planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Para obtener información sobre cómo se calculan los costes en el planificador de recursos, consulte el artículo [Calcular los costes en el planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>Presupuestar por costo es idéntico al presupuestado por horas o por tiempo invertido, pero debe comprender cómo calcula Workfront el coste para el planificador de recursos.
>
>Para obtener información sobre cómo se calculan los costes en el planificador de recursos, consulte el artículo [Calcular los costes en el planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

En las tablas siguientes se muestra la información de asignación y disponibilidad que aparece en el Planificador de recursos al aplicar la vista Proyecto o Función. Puede ver esta información por horas, a tiempo completo o por costo:

* [La columna AVL (disponible)](#the-avl-available-column)
* [La columna PLN (Planificado)](#the-pln-planned-column)
* [La columna BDG (Presupuestado)](#the-bdg-budgeted-column)
* [La columna VAR (Varianza)](#the-var-variance-column)
* [La columna NET](#the-net-column)

### La columna AVL (disponible) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td><strong>Descripción</strong> </td> 
  </tr> 
  <tr> 
   <td>Proyecto </td> 
   <td> <p>Total de horas, FTE o costes para los que todos los usuarios del proyecto están disponibles para trabajar según su programación, durante el lapso de tiempo seleccionado. </p> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>El total de horas, FTE o costes para los que todos los usuarios asociados a esta función están disponibles para trabajar según su programación y sus <strong>Porcentaje de disponibilidad de FTE</strong> para esa función específica, para el lapso de tiempo seleccionado. </p> <p>Tenga en cuenta lo siguiente: </p> 
    <ul> 
     <li>Si ningún usuario está asociado con una función de trabajo, el valor de Horario disponible para la función de trabajo es cero. </li> 
     <li>Si un usuario está asociado con una función de trabajo principal, pero la variable <strong>Porcentaje de disponibilidad de FTE</strong> para el rol es 0%, el valor del rol de trabajo Horario disponible es cero.</li> 
     <li>Si el usuario está asociado con Otras funciones y la variable <strong>Porcentaje de disponibilidad de FTE</strong> para las funciones es 0%, las otras funciones no se enumeran en el planificador de recursos y el usuario solo se muestra debajo de su función principal.</li> 
    </ul> <p>Para obtener más información sobre la variable <strong>Porcentaje de disponibilidad de FTE</strong> para una función de trabajo, consulte el artículo <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</p> <p>Para obtener más información acerca de cómo se calcula la disponibilidad de la función de trabajo en el Planificador de recursos, consulte la sección "Calcular las horas disponibles y FTE para una función de trabajo en el Planificador de recursos" en el artículo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Horas, FTE o Coste que el usuario está disponible para trabajar, según su programación, en el lapso de tiempo seleccionado. Este número resta las horas asociadas con lo siguiente:</p> 
    <ul> 
     <li>excepciones de programación</li> 
     <li>tiempo de espera del usuario</li> 
     <li>horas presupuestadas para otros proyectos. </li> 
    </ul> <p>Las horas, los FTE o el coste disponibles para un usuario cambian según lo siguiente: </p> 
    <ul> 
     <li>cómo se calculan su programación y el FTE en función de las preferencias de gestión de recursos a nivel de sistema.<br><p>Para obtener más información sobre el cálculo de la disponibilidad de funciones de usuario y de trabajo, consulte el artículo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos</a>.</p>
     Para obtener más información sobre la configuración de las preferencias de Gestión de recursos en Workfront, consulte <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a></li> 
    </ul> 
    <ul> 
     <li>el <strong>Prioridad de Planificación de Proyectos</strong>, si el usuario está presupuestado para trabajar.<br>Para obtener más información sobre cómo afecta la prioridad de planificación de proyectos a las horas disponibles de un usuario, consulte <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Información general sobre navegación del planificador de recursos </a>. </li> 
    </ul> <p>Si el usuario está programado para su desactivación, las horas disponibles, los FTE o el coste de los días posteriores a la fecha de desactivación son cero. <br>Para obtener más información sobre la desactivación de usuarios, consulte el artículo <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### La columna PLN (Planificado) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td><strong>Descripción</strong> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td> <p>El total de horas planificadas, FTE o costes de todas las funciones de trabajo o usuarios enumerados en el proyecto, incluido el <strong>Sin función</strong> o <strong>Sin usuario</strong> , para el lapso de tiempo seleccionado y tal y como se muestra en la pestaña Detalles del proyecto del proyecto . </p> <p><b>NOTA</b>

Los ajustes manuales de las asignaciones diarias de usuarios podrían cambiar el valor de las horas planificadas semanales, mensuales o trimestrales en el Planificador de Recursos. Puede ajustar manualmente las asignaciones de usuario diarias para tareas y problemas mediante el equilibrador de carga de trabajo. Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.</p> </td>
</tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Total de horas planificadas de todas las tareas asignadas a la función, durante el lapso de tiempo seleccionado. </p> <p>La variable <strong>Sin función</strong> mostrará las horas planificadas asociadas con tareas que no están asignadas y asignadas a equipos (cuyas horas aparecen en la lista del <strong>Sin usuario</strong> ), o se asigna a usuarios que no están asociados a una función de trabajo. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Horario planificado de todas las tareas asignadas al usuario en una función específica, durante el lapso de tiempo seleccionado. </p> <p>La variable <strong>Sin usuario</strong> mostrará las horas planificadas asociadas con tareas que no están asignadas o asignadas a equipos. </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente al ver las horas planificadas:

* Aunque no puede ver información sobre las asignaciones de tareas en el Planificador de recursos en las vistas Proyecto y Función, la cantidad de horas planificadas proviene de las horas planificadas sobre las tareas de los proyectos.
* Las horas planificadas se distribuyen por igual a cada día dentro de la Duración de las tareas, para cada recurso que se les asigne. La duración de la tarea se basa en la tarea Fechas de inicio y finalización planificadas e incluye todos los días del calendario dentro de ese periodo de tiempo.\
   Workfront tiene en cuenta la programación del usuario o del proyecto al distribuir Horario planificado a usuarios o proyectos. En este caso, las horas planificadas se distribuyen por igual a cada día dentro de la Duración de las tareas, excluyendo los fines de semana, los días de descanso y las excepciones de programación.\
   Si, por ejemplo, muestra el Planificador de recursos por semana y tiene tareas que abarcan varias semanas en los proyectos, el número de horas planificadas por semana depende de cuántos días dentro de esa semana formen parte de la duración de la tarea. Esto funciona de manera similar cuando se muestra el Planificador de recursos por mes o trimestre y cuando las tareas abarcan varios meses o trimestres.\
   Los días de fin de semana, las excepciones de programación y los días de tiempo libre se excluyen de esta distribución.
* Las siguientes categorías de tareas se incluyen en el cálculo de las horas planificadas para cada recurso:

   * tareas asignadas a usuarios en grupos de recursos, funciones de trabajo o equipos del proyecto\
      Si las tareas están asignadas a equipos, su asignación aparecerá en **Sin función** y **Sin usuario** secciones. Puede ver las horas planificadas asociadas con los equipos, pero no puede presupuestarlas, ya que no hay funciones ni usuarios asociados a las tareas.

   * tareas no asignadas

* Las horas planificadas en el planificador de recursos no incluyen las horas planificadas asociadas con lo siguiente:

   * tareas principales
   * tareas asignadas a usuarios sin grupos de recursos
   * problemas, cuando la variable **Incluir horas de problemas** está desactivado.

* Las horas planificadas no se muestran en el planificador de recursos si la duración de la tarea es cero.
* Las horas planificadas asociadas con usuarios desactivados no se muestran.

### La columna BDG (Presupuestado) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td><strong>Descripción</strong> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td> <p>Una entrada manual para estimar cuántas horas, FTE o Coste se presupuestan para un proyecto durante un lapso de tiempo seleccionado. </p> <p>En la vista Proyecto, las horas presupuestadas para el proyecto se distribuyen a las funciones de trabajo enumeradas en el proyecto. La cantidad de horas planificadas para cada función determina cómo se distribuyen las horas presupuestadas a las funciones. Las horas presupuestadas se distribuyen a las funciones con valores de horas planificadas más altos. </p> <p>En la vista Rol, las horas presupuestadas para el proyecto no se distribuyen a las funciones ni a los usuarios del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Una entrada manual para estimar cuántas horas presupuestará para una función, para un lapso de tiempo seleccionado. </p> <p>Si ningún usuario está asociado con la función de trabajo, no puede estimar las horas presupuestadas para la función de trabajo. </p> <p>En la vista Rol, las horas presupuestadas para la función se distribuyen a los proyectos enumerados en la función. La cantidad de horas planificadas para cada proyecto determina cómo se distribuyen las horas presupuestadas a los proyectos. Las horas presupuestadas se distribuyen a los proyectos con valores de horas planificadas más altos.</p> <p>En la vista Proyecto, las horas presupuestadas para la función no se distribuyen a los proyectos ni a los usuarios asociados con la función. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Entrada manual para estimar cuántas horas presupuesta un usuario durante un lapso de tiempo seleccionado. </p> <p> <p><b>NOTA</b>   Puede calcular las horas presupuestadas para los usuarios que no están asignados a tareas pero que están asociados a un grupo de recursos en un proyecto porque estos usuarios también aparecen en el planificador de recursos. Sin embargo, las horas previstas deben ser cero si no se les asignan tareas. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente al trabajar con horas presupuestadas:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Los recursos solo se pueden presupuestar si se dispone de permisos de edición en Gestión de recursos y Datos financieros y Administrar finanzas en los proyectos.

   Para obtener información sobre el acceso necesario para presupuestar recursos, consulte el artículo [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* De forma predeterminada, las horas presupuestadas en el planificador de recursos son cero para todos los recursos y para todos los proyectos.
* Puede calcular manualmente las horas presupuestadas para los usuarios y las funciones, o puede utilizar uno de los vínculos de la función de proyecto o de trabajo **Más** para actualizarlos según el número de horas planificadas.\
   Para obtener más información sobre las opciones de proyecto y función, consulte la sección [Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos](#Budget) en este artículo.

* El período de tiempo más pequeño para el que puede presupuestar horas, FTE o Coste es de una semana. No puede presupuestar horas, FTE ni Coste para un día.
* Las horas presupuestadas se distribuyen de forma equitativa a cada día dentro de la duración de las tareas, para cada recurso asignado a ellas. La duración de la tarea se basa en la tarea Fechas de inicio y finalización planificadas e incluye todos los días del calendario dentro de ese periodo de tiempo.\
   Workfront tiene en cuenta la programación del usuario o del proyecto al distribuir las horas presupuestadas a usuarios o proyectos. En este caso, las horas presupuestadas se distribuyen por igual a cada día dentro de la duración de las tareas, excluyendo los fines de semana, pero incluyendo las excepciones de tiempo libre y de programación.\
   Si, por ejemplo, muestra el Planificador de recursos por semana y tiene tareas que abarcan varias semanas, el número de horas presupuestadas por semana depende de cuántos días dentro de esa semana formen parte de la duración de la tarea. Los días de fin de semana se excluyen de esta distribución. Esto funciona de manera similar cuando se muestra el Planificador de recursos por mes o trimestre y cuando las tareas abarcan varios meses o trimestres.

* Puede informar sobre las horas presupuestadas seleccionando Hora presupuestada como objeto de informe para un nuevo informe.\
   Para obtener información sobre los objetos sobre los que puede informar en Workfront, consulte la sección &quot;Informar sobre objetos&quot; en el artículo [Explicación de los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   Para obtener información sobre la creación de un informe de horas de presupuesto, consulte el artículo [Informe: Hora presupuestada](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Las horas presupuestadas anteriormente para los usuarios que se desactivaron posteriormente no se muestran.

### La columna VAR (Varianza) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td><strong>Descripción</strong> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td> <p>La variable Hora, FTE o Variación de costo muestra si tiene suficientes horas presupuestadas para que el proyecto realice todas las horas planificadas para el proyecto. </p> <p>La hora del proyecto, FTE o la variación de coste se calcula mediante la fórmula siguiente:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>La variable Hora, FTE o Variación de Coste muestra si tiene suficientes horas presupuestadas, FTE o Coste para que la función cumpla las horas planificadas asignadas. </p> <p>La hora de rol, FTE o la variación de coste se calcula mediante la fórmula siguiente:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Las variaciones de horas, de tiempo libre o de costes muestran si tiene suficientes horas presupuestadas para que el usuario cumpla las horas planeadas asignadas a ellas. </p> <p>Las horas del usuario, FTE o Varianza de coste se calculan mediante la fórmula siguiente:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Cuando las horas, los datos a tiempo completo o la variación de coste aparecen en rojo, se ha calculado que hay menos horas presupuestadas que las horas planificadas del trabajo real que debe completarse. En este caso, es posible que las horas presupuestadas no sean suficientes para completar el trabajo.

### La columna NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td><strong>Descripción</strong> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td> 
    <div> 
     <p>Las horas netas, el tiempo de espera o el coste del proyecto pueden mostrar una de las siguientes características: </p> 
     <ul> 
      <li> <p>La diferencia entre el tiempo o coste disponible y el tiempo o coste presupuestado del proyecto:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>La diferencia entre el tiempo o coste disponible y el tiempo o coste planeado del proyecto, cuando los valores Usar planeado (PLN) en los cálculos NETOS están habilitados: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>SUGERENCIA</b></p>        
  <p>Esta opción solo se aplica cuando se personaliza la vista en la sección Mostrar elementos seleccionados .</p>
  <p>Para obtener más información, consulte <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Revisar la disponibilidad y asignación de recursos con el planificador de recursos de Adobe Workfront</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> 
    <div> 
     <p>La función Horas Netas, FTE o Coste puede mostrar una de las siguientes características: </p> 
     <ul> 
      <li> <p>La diferencia entre el tiempo o coste disponible y el tiempo o coste presupuestado de la función:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La diferencia entre el tiempo o coste disponible y el tiempo o coste planeado de la función, cuando los valores Usar planeado (PLN) en los cálculos de NET están habilitados:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>SUGERENCIA</b> <span>

Esta opción solo se aplica cuando se personaliza la vista en la sección Mostrar elementos seleccionados .</span> </p> <p><span>Para obtener más información, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revisar la disponibilidad y asignación de recursos con el planificador de recursos de Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Usuario</td> 
   <td> 
    <div> 
     <p>El usuario Hora Neta, FTE o Costo puede mostrar una de las siguientes opciones: </p> 
     <ul> 
      <li> <p>La diferencia entre el tiempo o coste disponible y el tiempo o coste presupuestado para el usuario:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La diferencia entre el tiempo o coste disponible y el tiempo o coste planeado para el usuario, cuando los valores Usar planeado (PLN) en los cálculos NETOS están habilitados:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>SUGERENCIA</b> <span>

Esta opción solo se aplica cuando se personaliza la vista en la sección Mostrar elementos seleccionados .</span> </p> <p><span>Para obtener más información, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revisar la disponibilidad y asignación de recursos con el planificador de recursos de Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Cuando las horas netas, los FTE o los costes se muestran en rojo, no hay suficiente tiempo o presupuesto disponible para cubrir ninguno de los dos** o el tiempo o coste planeado asociado al trabajo. En este caso, los recursos están sobreasignados.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
