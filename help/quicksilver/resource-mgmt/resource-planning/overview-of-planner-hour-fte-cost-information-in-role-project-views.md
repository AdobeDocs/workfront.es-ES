---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Visión General de Horas, ETC e Información de Costos en las Vistas de Proyectos y Rol del Planificador de Recursos
description: Información general sobre horas, EJC y costes en las vistas Proyecto y Función del Planificador de recursos
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: c9e77e11fafbf224639289977783e95ccb45a9e2
workflow-type: tm+mt
source-wordcount: '3086'
ht-degree: 94%

---

# Información general sobre horas, EJC y costes en las vistas Proyecto y Función del Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

La principal función del Planificador de recursos es presupuestar los recursos para el trabajo que se debe llevar a cabo en un proyecto. Puede ver el tiempo disponible de los recursos, así como asignar su tiempo a los proyectos en los que están asignados.

Para obtener información sobre cómo presupuestar recursos en el Planificador de recursos, consulte [Presupuestar recursos en el Planificador de recursos mediante las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

En este artículo se describen algunos de los conceptos clave que debe conocer antes de comenzar a presupuestar los recursos en el Planificador de recursos.

## Información general sobre presupuestar recursos

Tenga en cuenta lo siguiente al presupuestar recursos mediante el Planificador de recursos:

* Puede presupuestar la asignación de los recursos especificando la cantidad de horas, EJC o coste que los recursos pueden utilizar para completar el trabajo de los proyectos. Al presupuestar el tiempo o el coste para un recurso, las horas disponibles, el EJC o el coste del recurso disminuyen en la cantidad presupuestada. Como resultado, los importes de horas disponibles, EJC o costes para los proyectos que siguen al proyecto para el que está presupuestando disminuyen para esos usuarios y funciones en esos proyectos.

  >[!IMPORTANT]
  >
  >Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información de presupuestación no sea precisa.

* Puede presupuestar las horas, los jornadas completas o el coste de los recursos para cualquier lapso de tiempo mostrado en el Planificador de recursos, independientemente de la duración del proyecto. Por ejemplo, si desea indicar que los recursos podrían no estar disponibles durante la duración del proyecto (cuando estén asociados con Horas planificadas), pero podrían estar disponibles durante otro período, puede presupuestarlos para períodos de tiempo en los que las horas planificadas sean cero, si es entonces cuando estarán disponibles para trabajar. Después de hacer esto, puede cambiar manualmente la línea de tiempo del proyecto para que coincida con la disponibilidad de los recursos.

  >[!NOTE]
  >
  >Le recomendamos que presupueste manualmente sus horas, EJC o coste para funciones de trabajo o para usuarios primero. Puede utilizar las opciones automáticas para presupuestar el tiempo de sus proyectos y recursos si tiene claro que la cantidad de Horas planificadas, EJC o Coste debería coincidir siempre con las Horas, EJC o Coste presupuestados.\
  >Para obtener información acerca del uso de las opciones automáticas para la presupuestación en el Planificador de recursos, consulte la sección &quot;Presupuestar el proyecto y las funciones automáticamente&quot; en el artículo [Revisar la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* Presupuestar el valor de EJC o los costes es idéntico a presupuestar horas; Adobe Workfront utiliza los valores de EJC y de coste en lugar de horas para los recursos presupuestados.

  Para obtener más información sobre cómo se calculan los costes en el Planificador de recursos, consulte [Calcular costes en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* La presupuestación de asignaciones para los recursos en el Planificador de recursos se realiza de las siguientes maneras:

   * Manualmente

     O

   * Automáticamente, mediante las opciones de proyecto y función en las vistas **Ver por proyecto** y **Ver por función**.

  Para obtener más información, consulte [Recursos de presupuesto en el Planificador de recursos mediante las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Cuando un usuario cambia de función, se elimina, se desactiva o se quite de un conjunto de recursos, las horas presupuestadas para la función no cambian y se redistribuyen a los demás usuarios de la función. Si ya no hay ningún usuario asociado con la función, las horas presupuestadas de la función pasarán a ser cero.

Para obtener más información acerca de las opciones de proyecto y función, consulte la sección [Comprender los valores de horas, EJC y coste en el Planificador de recursos](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) en este artículo.

## Comprender los valores de horas, EJC y coste en el Planificador de recursos {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Antes de presupuestar los recursos y actualizar la información de Horas presupuestadas en el Planificador de recursos, debe conocer los siguientes conceptos

* **Horas planificadas, EJC o coste**: el trabajo que debe realizarse según se ha definido en las tareas y los problemas.
* **Horas disponibles, EJC o costes**: la cantidad de tiempo que los usuarios o funciones de trabajo están disponibles para trabajar, según los horarios asociados con los usuarios.

Esta información se muestra en el Planificador de recursos para cada recurso (usuario o función) y para cada proyecto.

Para obtener información acerca de lo que se muestra en las vistas de proyecto y vista de funciones del proyecto, vea el artículo [Información general sobre la navegación del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Para obtener información acerca de cómo se calculan los costes en el Planificador de recursos, vea el artículo [Calcular costes en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>La presupuestación por coste es idéntica a la presupuestación por horas o por tiempo completo, pero debe comprender cómo calcula Workfront el coste para el planificador de recursos.
>
>Para obtener información acerca de cómo se calculan los costes en el Planificador de recursos, vea el artículo [Calcular costes en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

En las tablas siguientes se muestra la información de asignación y disponibilidad que aparece en el Planificador de recursos al aplicar la vista Proyecto o Función. Puede ver esta información por horas, EJC o costes:

* [La columna AVL (disponible)](#the-avl-available-column)
* [La columna PLN (planificado)](#the-pln-planned-column)
* [La columna BDG (presupuestado)](#the-bdg-budgeted-column)
* [La columna VAR (varianza)](#the-var-variance-column)
* [La columna NET](#the-net-column)

### AVL La columna (Disponible {#the-avl-available-column}

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
   <td> <p>El total de horas, equivalente a jornadas completas o coste para el que todos los usuarios del proyecto están disponibles para trabajar según su programación, durante el lapso de tiempo seleccionado. </p> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td> <p>El total de horas, equivalente a jornadas completas o coste para el que todos los usuarios asociados con esta función están disponibles para trabajar según su programación y su <strong>Porcentaje de disponibilidad de EJC</strong> para esa función específica, durante el lapso de tiempo seleccionado. </p> <p>Tenga en cuenta lo siguiente: </p> 
    <ul> 
     <li>Si no hay ningún usuario asociado a una función, el valor de Horas disponibles para esa función es cero. </li> 
     <li>Si un usuario está asociado con una función principal, pero el <strong>Porcentaje de disponibilidad de EJC</strong> para la función es del 0 %, el valor de Horas disponibles para esa función es cero.</li> 
     <li>Si el usuario está asociado con otras funciones y el <strong>Porcentaje de disponibilidad de EJC</strong> para las funciones es del 0 %, las otras funciones no aparecen en el Planificador de recursos y el usuario solo aparece bajo su Función principal.</li> 
    </ul> <p>Para obtener más información sobre el <strong>Porcentaje de disponibilidad de EJC</strong> para una función, consulte el artículo <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> <p>Para obtener más información acerca de cómo se calcula la disponibilidad de las funciones en el Planificador de recursos, consulte la sección “Calcular las Horas disponibles y el EJC para una función en el Planificador de recursos” en el artículo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Información general sobre el cálculo de horas y el EJC para usuarios y funciones en el Planificador de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Horas, EJC o Coste para los que el usuario está disponible para trabajar, según su programación, durante el lapso de tiempo seleccionado. Este número resta las horas asociadas con lo siguiente:</p> 
    <ul> 
     <li>excepciones de programación</li> 
     <li>días libres del usuario</li> 
     <li>horas presupuestadas para otros proyectos. </li> 
    </ul> <p>Las horas disponibles, el equivalente a jornadas completas o el coste de un usuario cambian de acuerdo con lo siguiente: </p> 
    <ul> 
     <li>cómo se calculan su programación y su EJC en función de las preferencias de administración de recursos a nivel del sistema.<br><p>Para obtener más información sobre cómo calcular la disponibilidad de usuarios y funciones, consulte el artículo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Información general sobre el cálculo de horas y EJC para usuarios y funciones en el Planificador de recursos</a>.</p>
     Para obtener más información sobre cómo configurar las preferencias de Administración de recursos en Workfront, consulte <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a></li> 
    </ul> 
    <ul> 
     <li>la <strong>Prioridad de planificación del proyecto</strong>, si se ha presupuestado el trabajo para el usuario.<br>Para obtener más información sobre cómo afecta la prioridad de la planificación del proyecto a las horas disponibles de un usuario, consulte <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Información general de navegación del Planificador de recursos</a>. </li> 
    </ul> <p>Si ya se ha programado la desactivación del usuario, las horas disponibles, el equivalente a jornadas completas o el coste de los días posteriores a la fecha de desactivación serán cero. <br>Para obtener más información sobre cómo desactivar usuarios, consulte el artículo <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### La columna PLN (planificado) {#the-pln-planned-column}

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
   <td> <p>El total de horas planificadas, EJC o coste de todas las funciones o usuarios enumerados en el proyecto, también en las secciones <strong>Sin función</strong> o <strong>Sin usuario</strong>, durante el lapso de tiempo seleccionado y tal como se muestra en la pestaña Detalles del proyecto en cuestión. </p> <p><b>NOTA</b>

Los ajustes manuales de las asignaciones diarias de usuarios podrían cambiar el valor de las horas planificadas semanales, mensuales o trimestrales en el Planificador de recursos. Puede ajustar manualmente las asignaciones diarias de usuarios para tareas y problemas mediante el Distribuidor de cargas de trabajo. Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.</p> </td>
</tr> 
  <tr> 
   <td>Función</td> 
   <td> <p>El total de horas planificadas de todas las tareas asignadas a la función durante el lapso de tiempo seleccionado. </p> <p>La sección <strong>Sin función</strong> mostrará las horas planificadas asociadas con tareas que están sin asignar, asignadas a equipos (cuyas horas se enumeran en la sección <strong>Sin usuario</strong>) o asignadas a usuarios que no están asociados con una función. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Las horas planificadas de todas las tareas asignadas al usuario en una función específica durante el lapso de tiempo seleccionado. </p> <p>La sección <strong>Sin usuario</strong> mostrará las horas planificadas asociadas con tareas que estén sin asignar o asignadas a equipos. </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente al consultar las horas planificadas:

* Aunque no puede ver información sobre las asignaciones de tareas en el Planificador de recursos en las vistas Proyecto y Función, la cantidad de horas planificadas procede de las horas planificadas en las tareas de los proyectos.
* Las horas planificadas se distribuyen equitativamente a cada día dentro de la Duración de las tareas, para cada recurso asignado a ellas. La duración de la tarea se basa en las fechas de inicio y de finalización planificadas para la tarea e incluye todos los días del calendario dentro de ese período de tiempo.\
  Workfront tiene en cuenta la programación del usuario o del proyecto al distribuir las horas planificadas a usuarios o proyectos. En este caso, las horas planificadas se distribuyen equitativamente a cada día dentro de la Duración de las tareas, excluyendo los fines de semana, los días libres y las excepciones de programación.\
  Si ve el Planificador de recursos por semana, por ejemplo, y tiene tareas que abarcan varias semanas en proyectos, el número de horas planificadas por semana dependerá de cuántos días de esa semana formen parte de la duración de la tarea. Esto funciona de manera similar cuando se ve el Planificador de recursos por mes o trimestre y cuando las tareas abarcan varios meses o trimestres.\
  De esta distribución se excluyen los días de fin de semana, las excepciones de programación y los días libres.
* Las siguientes categorías de tareas se incluyen en el cálculo de las horas planificadas para cada recurso:

   * tareas asignadas a usuarios en conjuntos de recursos, funciones o equipos en el proyecto\
     Si las tareas se asignan a equipos, su asignación aparecerá en las secciones **Sin función** y **Sin usuario**. Puede ver las horas planificadas asociadas con los equipos, pero no puede presupuestarlas, ya que no hay funciones ni usuarios asociados a las tareas.

   * tareas sin asignar

* Las horas planificadas en el Planificador de recursos no incluyen las horas planificadas asociadas con lo siguiente:

   * tareas principales
   * tareas asignadas a usuarios sin conjuntos de recursos
   * problemas, cuando la configuración **Incluir horas de problemas** está deshabilitada.

* Las horas planificadas no se muestran en el Planificador de recursos si la duración de la tarea es cero.
* Las horas planificadas asociadas con los usuarios desactivados no se muestran.

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
   <td> <p>Una entrada manual para estimar cuántas horas, FTE o Coste ha presupuestado para un proyecto, para un lapso de tiempo seleccionado. </p> <p>En la vista Proyecto, las horas presupuestadas para el proyecto se distribuyen entre las funciones enumeradas en el proyecto. La cantidad de horas planificadas para cada función determina cómo se distribuyen las horas presupuestadas a las funciones. Las horas presupuestadas se distribuyen a las funciones con valores de horas planificadas más altos. </p> <p>En la vista Función, las horas presupuestadas para el proyecto no se distribuyen entre las funciones ni entre los usuarios del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td> <p>Una entrada manual para estimar cuántas horas ha presupuestado para una función, para un lapso de tiempo seleccionado. </p> <p>Si no hay ningún usuario asociado a la función, no puede calcular las horas presupuestadas para la función de trabajo. </p> <p>En la vista Función, las horas presupuestadas para la función se distribuyen a los proyectos enumerados en la función. La cantidad de horas planificadas para cada proyecto determina cómo se distribuyen las horas presupuestadas a los proyectos. Las horas presupuestadas se distribuyen a los proyectos con valores de horas planificadas más altos.</p> <p>En la vista Proyecto, las horas presupuestadas para la función no se distribuyen entre los proyectos ni entre los usuarios asociados a la función. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>Una entrada manual para estimar cuántas horas ha presupuestado para un usuario durante un lapso de tiempo seleccionado. </p> <p> <p><b>NOTA</b>   Puede calcular las horas presupuestadas de los usuarios que no están asignados a tareas, pero que están asociadas a un conjunto de recursos en un proyecto, porque estos usuarios también aparecen en el Planificador de recursos. Sin embargo, las Horas planificadas deben ser cero si no están asignadas a ninguna tarea. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente al trabajar con Horas presupuestadas:

* Solo puede presupuestar recursos cuando tiene acceso de edición a los permisos de administración de recursos y datos financieros y administración de finanzas en los proyectos.

  Para obtener información sobre el acceso necesario para los recursos de presupuesto, consulte el artículo [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* De manera predeterminada, las horas presupuestadas en el Planificador de recursos son cero para todos los recursos y para todos los proyectos.
* Puede calcular manualmente las horas presupuestadas de los usuarios y las funciones, o puede usar uno de los vínculos en los menús **Más** de Proyecto o Función para actualizarlos de acuerdo con el número de Horas planificadas.\
  Para obtener más información acerca de las opciones de proyecto y función, consulte la sección [Información general sobre horas, FTE e información de coste en las vistas Proyecto y Función del Planificador de recursos](#Budget) en este artículo.

* El período de tiempo más pequeño para el que puede presupuestar horas, FTE o Coste es una semana. No puede presupuestar horas, FTE ni coste para un día.
* Las horas presupuestadas se distribuyen equitativamente a cada día dentro de la Duración de las tareas, para cada recurso asignado a ellas. La duración de la tarea se basa en las fechas de inicio y de finalización planificadas para la tarea e incluye todos los días del calendario dentro de ese período de tiempo.

  Workfront tiene en cuenta la programación del usuario o del proyecto al distribuir las horas presupuestadas a usuarios o proyectos. En este caso, las horas presupuestadas se distribuyen equitativamente a cada día dentro de la Duración de las tareas, excluyendo los fines de semana, pero incluyendo las excepciones de tiempo libre y de programación.

  Si muestra el Planificador de recursos por semana, por ejemplo, y tiene tareas que abarcan varias semanas, el número de horas presupuestadas por semana depende de cuántos días dentro de esa semana formen parte de la Duración de la tarea. Los días de fin de semana se excluyen de esta distribución. Esto funciona de manera similar cuando se ve el Planificador de recursos por mes o trimestre y cuando las tareas abarcan varios meses o trimestres.

* Puede crear informes sobre las horas presupuestadas seleccionando Hora presupuestada como objeto de informe para un nuevo informe.

  Para obtener información sobre los objetos de los que puede informar en Workfront, consulte la sección &quot;Informar sobre objetos&quot; en el artículo [Comprender los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Para obtener información sobre cómo generar un informe de Horas presupuestadas, consulte el artículo [Informe: Horas presupuestadas](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* No se muestran las horas presupuestadas anteriormente para usuarios que fueron desactivados posteriormente.

  Tenga en cuenta que el costo de mano de obra presupuestado de un proyecto aún incluye las horas presupuestadas de los usuarios que se desactivaron en el Planificador de recursos.

  Por ejemplo: si se asigna una función a dos usuarios y se agregan horas presupuestadas (20 horas por usuario, que totalizan 40 horas), y luego el total se establece manualmente para la función, la desactivación de uno de los usuarios en el Planificador de recursos hace que sus horas ya no se consideren en el cálculo (con lo que el total se reduce a 20 horas). Sin embargo, la presupuestación del proyecto conserva correctamente el total establecido manualmente para el rol, por lo que las horas del usuario desactivado se siguen incluyendo en el cálculo (quedan 40 horas).

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
   <td> <p>La variación de hora, ETC o coste muestra si se tienen suficientes horas presupuestadas para que el proyecto cumpla con todas las horas planificadas. </p> <p>La variación de hora, ETC o coste del proyecto se calcula mediante la fórmula siguiente:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td> <p>La variación de hora, ETC o coste muestra si se tienen suficientes horas, ETC o coste presupuestados para que la función lleve a cabo las horas planificadas asignadas. </p> <p>La variación de hora, ETC o coste de la función se calcula con la fórmula siguiente:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>La variación de hora, ETC o coste muestra si se tienen suficientes horas presupuestadas para que el usuario cumpla con las horas planificadas asignadas. </p> <p>La variación de hora, ETC o coste del usuario se calcula con la fórmula siguiente:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Cuando se muestre en rojo el valor de la variación de hora, ETC o coste, se habrán estimado menos horas presupuestadas que las horas planificadas del trabajo real que se debe completar. En este caso, las horas presupuestadas podrían no ser suficientes para completar el trabajo.

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
     <p>Las horas, ETC o coste neto del proyecto mostrarán una de las siguientes opciones: </p> 
     <ul> 
      <li> <p>Diferencia entre el coste o tiempo disponible y el coste o tiempo presupuestado del proyecto:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>Diferencia entre el coste o tiempo disponible y el coste o tiempo planificado del proyecto, cuando la opción Usar valores planificados (PLN) de la configuración Cálculos netos esté habilitada: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>Sugerencia</b></p>        
  <p>Esta opción solo se aplicará cuando se personalice la vista de la sección Mostrar los elementos seleccionados.</p>
  <p>Para obtener más información, consulte <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Revisar la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td> 
    <div> 
     <p>Las horas netas, ETC o coste de la función pueden mostrarse como una de las siguientes opciones: </p> 
     <ul> 
      <li> <p>Diferencia entre el coste o tiempo disponible y el coste o tiempo presupuestado de la función:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Diferencia entre el coste o tiempo disponible y el coste o tiempo planificado de la función, cuando se habilite la configuración Usar valores planificados (PLN) en los cálculos de red:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>Sugerencia</b> <span>

Esta opción solo se aplicará cuando se personalice la vista de la sección Mostrar los elementos seleccionados.</span> </p> <p><span>Para obtener más información, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revisión de la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Usuario</td> 
   <td> 
    <div> 
     <p>Las horas netas, ETC o coste del usuario pueden mostrarse como una de las siguientes opciones: </p> 
     <ul> 
      <li> <p>Diferencia entre el coste o tiempo disponible y el coste o tiempo presupuestado del usuario:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Diferencia entre el coste o tiempo disponible y el coste o tiempo planificado del usuario, cuando se habilite Usar valores planificados (PLN) en la configuración Cálculos de red:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>Sugerencia</b> <span>

Esta opción solo se aplicará cuando se personalice la vista de la sección Mostrar los elementos seleccionados.</span> </p> <p><span>Para obtener más información, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revisión de la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Cuando el valor de Horas netas, ETC o Coste aparece en rojo, no hay suficiente tiempo disponible o presupuesto para cubrir el tiempo presupuestado o planificado o el costo asociado con el trabajo. En este caso, habrá una asignación excesiva de recursos.

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
