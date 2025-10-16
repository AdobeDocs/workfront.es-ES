---
product-area: resource-management
navigation-topic: resource-planning
title: Presupuestar recursos en el Planificador de recursos mediante las vistas de proyecto y función
description: Puede presupuestar recursos en el Planificador de recursos de Adobe Workfront mediante las vistas Proyecto y Rol. No puede presupuestar recursos mediante la vista Usuario en el Planificador de recursos.
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 5%

---

# Presupuestar recursos en el Planificador de recursos utilizando las vistas Proyecto y Rol

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

La función principal del Planificador de recursos es presupuestar los recursos para el trabajo que se debe completar en los proyectos.

>[!IMPORTANT]
>
>Puede presupuestar sus recursos solamente si aplica las vistas **Ver por proyecto** o **Ver por rol** al Planificador de recursos.

Antes de comenzar a presupuestar información en el Planificador de recursos, consulte los siguientes artículos:

* [Información general del planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Información general sobre horas, EJC y costes en las vistas Proyecto y Función del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

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
   <td> <p>Acceso de edición a la administración de recursos que incluye acceso a Editar prioridades y horas presupuestadas en el Planificador de recursos</p> <p>Editar acceso a datos financieros para presupuestar recursos por costo</p> <p>Editar el acceso a Proyectos y Usuarios</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Administrar permisos a los proyectos para los que desea presupuestar información</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Presupuestar recursos en el Planificador de recursos

* [Recursos de presupuesto en la vista de proyecto](#budget-resources-in-the-project-view)
* [Recursos de presupuesto en la vista de rol](#budget-resources-in-the-role-view)
* [Presupuestar recursos de forma masiva](#budget-resources-in-bulk)

### Recursos de presupuesto en la vista de proyecto {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. Se muestra el **Planificador** de forma predeterminada.
1. (Condicional) Seleccione la vista **Vista por proyecto**.
1. Expanda los proyectos y las funciones del puesto para administrar la asignación del proyecto, las funciones del puesto o los usuarios.
1. Para presupuestar la asignación para los usuarios, realice una de las siguientes acciones:

   * En la columna **BDG**, especifique manualmente un número de horas presupuestadas, ETC o costo para los usuarios.

   * Haga clic en el menú **Más** para el rol de usuario y luego haga clic en **Establecer horas planificadas de usuarios según lo presupuestado**.\
     Las horas presupuestadas de cada usuario se calculan mediante la siguiente fórmula:

     `User Budgeted Hours = User Planned Hours`

1. Para presupuestar la asignación para los roles, realice una de las siguientes acciones:

   * En la columna **BDG**, especifique manualmente un número de horas presupuestadas, ETC o costo para el rol.

     >[!NOTE]
     >
     >Las horas presupuestadas de rol se agregan a las horas presupuestadas de proyecto.

   * (Condicional) Si ha presupuestado horas para usuarios, haga clic en el menú **Más** para el rol y, a continuación, haga clic en **Total de horas presupuestadas de usuario para el rol**.\
     Las horas presupuestadas de cada rol se calculan con la siguiente fórmula:

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * Haga clic en el menú **Más** del proyecto y, a continuación, haga clic en **Establecer horas planificadas de roles según lo presupuestado**.\
     Las horas presupuestadas de cada rol se calculan con la siguiente fórmula:\
     *

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* Las horas presupuestadas de rol se agregan a las horas presupuestadas de proyecto.
     >* Los usuarios pueden presupuestarse para los roles primario y otro (o secundario).
     >* El **porcentaje de disponibilidad de ETC** para los roles del usuario debe ser un número diferente al 0% para las horas disponibles para mostrar un valor en el Planificador de recursos para un rol. Si un usuario está asociado con un rol con un 0% **Porcentaje de disponibilidad de FTE**, el valor de Horas disponibles es cero para ese rol. En este caso, la función podría mostrar un **valor neto** negativo.\
     >Para obtener más información sobre el **porcentaje de disponibilidad de FTE** para los roles, consulte el artículo [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   * En la columna **BDG**, especifique manualmente una cantidad de horas presupuestadas, ETC o costo para el proyecto. Esto distribuye el número de horas presupuestadas del proyecto a cada rol dentro del proyecto. Se dan los siguientes escenarios:

      * Si el número de horas presupuestadas del proyecto que especifica es igual a las horas planificadas del proyecto, las horas presupuestadas del rol coinciden con las horas planificadas del rol.
      * Si el número de horas presupuestadas del proyecto que especifica no coincide con las horas planificadas del proyecto, las horas presupuestadas del rol se distribuyen según el porcentaje de horas planificadas que se necesite para cada rol.\
        Por ejemplo, si un proyecto tiene 20 horas planificadas y se distribuyen entre dos funciones de puesto (el consultor requiere 12 horas planificadas y el ingeniero requiere 8 horas planificadas), y se presupuestan 30 horas para el proyecto, las horas se distribuyen de la siguiente manera: la función Consultor recibe 18 horas presupuestadas y la función Ingeniero recibe 12 horas presupuestadas.

1. Para presupuestar la asignación para el proyecto, realice una de las siguientes acciones:

   * Presupuestar las funciones en el proyecto, tal como se describe en el paso 7.\
     Las horas presupuestadas del proyecto se calculan mediante la siguiente fórmula:

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * En la columna **BDG**, especifique manualmente una cantidad de horas presupuestadas, ETC o costo para el proyecto.\
     Esto actualiza las horas presupuestadas de la función, como se describe en el paso 7.\
     ![presupuesto_para_proyecto.png](assets/budget-for-project-350x182.png)

1. Haga clic en **Guardar**.\
   Después de presupuestar los recursos en el Planificador de recursos, las horas presupuestadas de los recursos y cualquier costo asociado con ellos se enumeran en el caso comercial de cada proyecto.\
   Para obtener más información acerca del área de presupuesto de recursos del caso empresarial, vea la sección &quot;Presupuestación de recursos&quot; en el artículo [Información general sobre las áreas del caso empresarial](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Seleccione la vista de usuario para ver si hay sobreasignaciones de usuarios o infrautilización entre las horas disponibles y las planificadas para cada usuario. Las horas presupuestadas no son visibles en la vista de usuario.

   Para obtener información sobre cómo Workfront calcula la disponibilidad de un usuario, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Recursos de presupuesto en la vista de rol {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

Debe tener acceso de edición a los permisos de administración de recursos y datos financieros y administración de finanzas en los proyectos para presupuestar recursos en el Planificador de recursos. Si solo tiene acceso de visualización a al menos un proyecto enumerado en un rol, no puede presupuestar las asignaciones para el rol en la vista de rol. Puede seguir asignando presupuestos para los proyectos en los que tenga permisos de administración.

Para obtener información sobre el acceso necesario para los recursos de presupuesto, consulte el artículo [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Para presupuestar asignaciones en el Planificador de recursos en la vista **** roles:

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recursos**.
1. Se muestra el **Planificador** de forma predeterminada.
1. (Condicional) Seleccione la vista **Vista por rol**.
1. Expanda los roles y los proyectos para administrar la asignación del proyecto, los roles o los usuarios.
1. Para presupuestar la asignación para los usuarios, realice una de las siguientes acciones:

   * En la columna **BDG**, especifique manualmente un número de horas presupuestadas, ETC o costo para los usuarios.
   * Haga clic en el menú **Más** del proyecto y luego haga clic en **Establecer horas planificadas de usuarios según lo presupuestado**.\
     Las horas presupuestadas de cada usuario se calculan mediante la siguiente fórmula:

     `User Budgeted Hours = User Planned Hours`

1. Para presupuestar la asignación para los roles, realice una de las siguientes acciones:

   * En la columna **BDG**, especifique manualmente un número de horas presupuestadas, ETC o costo para los roles.\
     Esto distribuye las horas presupuestadas de función a las horas presupuestadas de proyecto de los proyectos a los que tiene acceso para administrar.

   * Haga clic en el menú **Más** para el rol y luego haga clic en **Establecer horas planificadas de proyectos según lo presupuestado&quot;.**Las horas presupuestadas de la función se calculan con la siguiente fórmula:\
     *

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *Las horas presupuestadas del proyecto se calculan mediante la siguiente fórmula:

     `Project Budgeted Hours = Project Planned Hours`

   * En la columna **BDG**, especifique manualmente un número de horas presupuestadas, ETC o costo para los proyectos enumerados en el rol.\
     Esto agrega el número de horas presupuestadas del proyecto al rol.

   >[!NOTE]
   >
   >Los usuarios pueden presupuestarse para los roles primario y otro (o secundario). El **porcentaje de disponibilidad de ETC** para los roles del usuario debe ser un número diferente al 0% para las horas disponibles para mostrar un valor en el Planificador de recursos para un rol. Si un usuario está asociado con un rol con un 0% **Porcentaje de disponibilidad de FTE**, el valor de Horas disponibles es cero para ese rol. En este caso, la función podría mostrar un **valor neto** negativo.\
   >Para obtener más información sobre el **porcentaje de disponibilidad de FTE** para los roles, consulte el artículo [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Para presupuestar la asignación para el proyecto, realice una de las siguientes acciones:

   * En la columna **BDG**, especifique manualmente un número de horas presupuestadas, ETC o costo para los proyectos.\
     Esto también actualiza las horas presupuestadas de las funciones en las que aparece el proyecto.

   * Haga clic en el menú **Más** para el rol y luego haga clic en **Establecer horas planificadas de proyectos como presupuestadas**.\
     Las horas presupuestadas del proyecto se calculan mediante la siguiente fórmula:

     `Project Budgeted Hours = Project Planned Hours`

     Las horas presupuestadas del proyecto se agregan a las horas presupuestadas del rol.

   * (Condicional) Si ha presupuestado las horas de los usuarios, haga clic en el menú **Más** del proyecto y, a continuación, haga clic en **Total de horas presupuestadas de usuario para el proyecto**.\
     Las horas presupuestadas del proyecto se calculan mediante la siguiente fórmula:

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![presupuesto_por_rol.png](assets/budget-by-role-350x181.png)

1. Haga clic en **Guardar**.\
   Después de presupuestar los recursos en el Planificador de recursos, las horas presupuestadas de los recursos y cualquier costo asociado con ellos se enumeran en el caso comercial de cada proyecto.
Para obtener más información acerca de cómo comprender el área de presupuesto de recursos del caso empresarial, vea el artículo [Presupuesto de recursos en el caso empresarial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Opcional) Seleccione la vista **Ver por usuario** para ver si hay sobreasignaciones de usuarios o infrautilización entre las horas disponibles y las planificadas para cada usuario. Las horas presupuestadas no son visibles en la vista Ver por usuario.

### Presupuestar recursos de forma masiva {#budget-resources-in-bulk}

Puede presupuestar las asignaciones de sus recursos de forma masiva mediante vínculos rápidos. Los vínculos rápidos sólo están disponibles para las vistas de proyecto y de rol.

![Opciones de presupuesto automáticas](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Al utilizar los enlaces rápidos para asignar presupuestos a recursos, la presupuestación se aplica automáticamente solo a los períodos de tiempo mostrados en la pantalla. Si la cronología de un proyecto abarca un período de tiempo más largo que el que se muestra en la pantalla, debe desplazarse de izquierda a derecha y, a continuación, utilizar los vínculos rápidos para presupuestar automáticamente los recursos.

Para presupuestar los recursos de forma masiva:

1. Vaya a.\
   Para obtener más información sobre el acceso al Planificador de recursos, consulte la sección Acceso al Planificador de recursos en el artículo [Información general del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   En la lista se muestra una lista de los proyectos que puede administrar.

1. (Opcional) Expanda cada proyecto para ver una lista de funciones del puesto asociadas a él.\
   O
1. (Opcional) Seleccione **Ver por rol** y expanda cada rol para ver una lista de los proyectos asociados con él.
1. Pase el ratón sobre el nombre de un proyecto o de una función de trabajo.
1. Haga clic en el icono **Más** ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)que se muestra en el extremo derecho del nombre del proyecto o rol.

1. Haga clic en una de las opciones disponibles para especificar automáticamente la cantidad de horas presupuestadas (BDG) para otros objetos.

   En función de si ha hecho clic en el icono Más de un proyecto o de un rol, las opciones de presupuestación por lotes difieren. La tabla siguiente ilustra las opciones disponibles para proyectos y funciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Vista de proyecto</strong> </td> 
      <td><strong>Vista de rol</strong> </td> 
     </tr> 
     <tr> 
      <td>Opciones de proyecto</td> 
      <td> 
       <ul> 
        <li><strong>Establecer horas planificadas de roles según lo presupuestado</strong>: seleccione esta opción para que las horas presupuestadas del rol sean idénticas a las horas planificadas. El total de horas presupuestadas de los roles se mostrará para las horas presupuestadas del proyecto. </li> 
        <li><strong>Ajustar fechas de presupuesto</strong> : Seleccione esta opción para mover las horas presupuestadas a un intervalo de tiempo diferente.<br>Para obtener más información acerca del ajuste de fechas de presupuesto, vea <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Ajustar fechas de presupuesto en el Planificador de recursos</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Establecer horas planificadas de usuarios según lo presupuestado</strong>: seleccione esta opción para que las horas presupuestadas del usuario sean idénticas a las horas planificadas. </li> 
        <li><strong>Total de horas presupuestadas de usuario para el proyecto</strong>: seleccione esta opción para sumar todas las horas presupuestadas de usuario y mostrar el total como horas presupuestadas del proyecto y del rol. Le recomendamos que utilice esta opción después de haber presupuestado manualmente a los usuarios o de haber utilizado primero la opción anterior. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Opciones de rol</td> 
      <td> 
       <ul> 
        <li><strong>Establecer horas planificadas de usuarios según lo presupuestado</strong>: seleccione esta opción para que las horas presupuestadas del usuario sean idénticas a sus horas planificadas. </li> 
        <li><strong>Total de horas presupuestadas de usuario para el rol</strong>: seleccione esta opción para sumar todas las horas presupuestadas del usuario y mostrar el total como horas presupuestadas para el rol y el proyecto. Le recomendamos que utilice esta opción después de haber presupuestado manualmente a los usuarios o de haber utilizado primero la opción anterior. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Establecer horas planificadas de proyectos según lo presupuestado</strong>: seleccione esta opción para que las horas presupuestadas de proyecto sean idénticas a las horas planificadas de proyecto. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Es posible que algunas de las opciones no se muestren si faltan algunos de los requisitos previos para trabajar en el Planificador de recursos.
   >
   >
   >Para obtener más información sobre los requisitos previos que se deben cumplir para obtener presupuestos precisos en el Planificador de recursos, consulte la sección &quot;Requisitos previos para trabajar en el Planificador de recursos&quot; en el artículo [Resumen del planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   >Por ejemplo, es posible que algunas de las opciones no se muestren en los siguientes casos:
   >
   >   
   >   
   >   * Cuando los proyectos no están asociados al conjunto de recursos
   >   * Cuando los conjuntos de recursos asociados a proyectos no contienen usuarios
   >   * Cuando los conjuntos de recursos asociados a proyectos contienen usuarios sin ninguna función de trabajo asociada a ellos.
   >   
   >
