---
product-area: resource-management
navigation-topic: resource-planning
title: Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función
description: Puede presupuestar recursos en el planificador de recursos de Adobe Workfront mediante las vistas Proyecto y Función. No puede presupuestar recursos utilizando la vista Usuario en el Planificador de Recursos.
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '2160'
ht-degree: 0%

---

# Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

La función principal del planificador de recursos es presupuestar los recursos para el trabajo que debe completarse en los proyectos.

>[!IMPORTANT]
>
>Puede presupuestar los recursos solo si aplica la variable **Ver por proyecto** o **Ver por función** vistas al planificador de recursos.

Antes de empezar a presupuestar información en el planificador de recursos, consulte los siguientes artículos:

* [Información general del planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Edite el acceso a la Administración de recursos que incluye acceso a Editar prioridades y horas de presupuesto en el Planificador de recursos</p> <p>Editar el acceso a Datos Financieros para presupuestar recursos por Coste</p> <p>Editar acceso a Proyectos y usuarios</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre los permisos de los proyectos para los que desea presupuestar información</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Recursos presupuestarios en el planificador de recursos

* [Recursos de presupuesto en la vista de proyecto](#budget-resources-in-the-project-view)
* [Recursos presupuestarios en la vista de funciones](#budget-resources-in-the-role-view)
* [Recursos presupuestarios en masa](#budget-resources-in-bulk)

### Recursos de presupuesto en la vista de proyecto {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recurso**.
1. La variable **Planificador** se muestra de forma predeterminada.
1. (Condicional) Seleccione el **Ver por proyecto** vista.
1. Expanda los proyectos y las funciones de trabajo para administrar la asignación para el proyecto, las funciones de trabajo o los usuarios.
1. Para presupuestar la asignación para los usuarios, realice una de las siguientes acciones:

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para los usuarios.

   * Haga clic en el **Más** para la función de trabajo del usuario y, a continuación, haga clic en **Establecer las horas planificadas de los usuarios como presupuestadas**.\
      Las horas presupuestadas de cada usuario se calculan mediante la fórmula siguiente:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Para presupuestar la asignación para funciones de trabajo, realice una de las siguientes acciones:

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para la función de trabajo.

      >[!NOTE]
      >
      >La función Horario presupuestado se agrega a las horas presupuestadas del proyecto.

   * (Condicional) Si ha presupuestado horas para los usuarios, haga clic en el **Más** para la función de trabajo y, a continuación, haga clic en **Horario presupuestado total de los usuarios para la función**.\
      Las horas presupuestadas para cada función se calculan mediante la fórmula siguiente:

      ```
      Role Budgeted Hours = SUM(User Budgeted Hours)
      ```

   * Haga clic en el **Más** para el proyecto y, a continuación, haga clic en **Establecer las horas planificadas de los roles como presupuestadas**.\
      Las horas presupuestadas para cada función se calculan mediante la fórmula siguiente:\
      *

      ```
      Role Budgeted Hours = Role Planned Hours
      ```

      >[!NOTE]
      >   
      >* La función Horario presupuestado se agrega a las horas presupuestadas del proyecto.
      >* Los usuarios pueden presupuestarse tanto para las funciones primarias como para las demás (o secundarias).
      >* La variable **Porcentaje de disponibilidad de FTE** para las funciones del usuario debe ser un número diferente de 0% para que las horas disponibles muestren un valor en el Planificador de recursos para una función de trabajo. Si un usuario está asociado con una función con un 0% **Porcentaje de disponibilidad de FTE**, el valor Horario disponible es cero para esa función de trabajo. En este caso, la función puede mostrar un valor negativo **Valor neto**.\
         >Para obtener más información sobre la variable **Porcentaje de disponibilidad de FTE** para las funciones de trabajo, consulte el artículo [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).


   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para el proyecto. Esto distribuye el número de horas presupuestadas del proyecto a cada función del proyecto. Existen los siguientes escenarios:

      * Si el número de horas presupuestadas del proyecto es igual a las horas planificadas del proyecto, las horas presupuestadas del rol coinciden con las horas planificadas del rol.
      * Si el número de horas presupuestadas del proyecto que especifique no es igual al número de horas planificadas del proyecto, las horas presupuestadas de funciones se distribuyen según el porcentaje de horas planificadas necesarias para cada función.\
         Por ejemplo, si un proyecto tiene 20 horas planificadas y se distribuyen entre dos funciones (el consultor requiere 12 horas planificadas y el ingeniero requiere 8 horas planificadas) y se presupuestan 30 horas para el proyecto, las horas se distribuyen de la siguiente manera: la función de consultor recibe 18 horas presupuestadas y la de ingeniero recibe 12 horas presupuestadas.

1. Para presupuestar la asignación para el proyecto, realice una de las siguientes acciones:

   * Asigne un presupuesto a las funciones del proyecto, tal como se describe en el paso 7.\
      El horario presupuestado del proyecto se calcula mediante la fórmula siguiente:

      ```
      Project Budgeted Hours = SUM(Role Budgeted Hours)
      ```

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para el proyecto.\
      Esto actualiza la función Horario presupuestado, como se describe en el paso 7.\
      ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Haga clic en **Guardar**.\
   Una vez presupuestados los recursos en el planificador de recursos, las horas presupuestadas de los recursos y los costes asociados a ellos se enumeran en el caso empresarial de cada proyecto.\
   Para obtener más información sobre el área de Presupuestación de Recursos del caso empresarial, consulte la sección &quot;Presupuestación de Recursos&quot; en el artículo [Información general sobre las áreas del caso empresarial](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Seleccione la vista Usuario para ver si el usuario tiene sobreasignaciones o subutilización entre las horas Disponible y Planificado para cada usuario. Las horas presupuestadas no están visibles en la vista Usuario.

   Para obtener información sobre cómo calcula Workfront la disponibilidad de un usuario, consulte [Configurar las preferencias de Administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Recursos presupuestarios en la vista de funciones {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

Debe tener acceso de edición a Gestión de recursos y Datos financieros y administrar finanzas en los proyectos para poder presupuestar recursos en el Planificador de recursos. Si solo tiene acceso a Ver al menos un proyecto enumerado en una función de trabajo, no puede presupuestar asignaciones para la función en la vista Función. Puede seguir asignando presupuestos a los proyectos en los que tenga permisos de gestión.

Para obtener información sobre el acceso necesario para presupuestar recursos, consulte el artículo [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Para presupuestar asignaciones en el Planificador de recursos en la vista Función***:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recurso**.
1. La variable **Planificador** se muestra de forma predeterminada.
1. (Condicional) Seleccione el **Ver por función** vista.
1. Expanda las funciones de trabajo y los proyectos para administrar la asignación para el proyecto, las funciones de trabajo o los usuarios.
1. Para presupuestar la asignación para los usuarios, realice una de las siguientes acciones:

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para los usuarios.
   * Haga clic en el **Más** para el proyecto y, a continuación, haga clic en **Establecer las horas planificadas de los usuarios como presupuestadas**.\
      Las horas presupuestadas de cada usuario se calculan mediante la fórmula siguiente:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Para presupuestar la asignación para funciones de trabajo, realice una de las siguientes acciones:

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para las funciones de trabajo.\
      Esto distribuye la función Horario presupuestado al proyecto de horas presupuestadas para los proyectos que tiene acceso para administrar.

   * Haga clic en el **Más** para la función de trabajo, haga clic en **Establecer las horas programadas de los proyectos como presupuestadas.**Las horas de rol presupuestadas se calculan con la fórmula siguiente:\
      *

      ```
      Role Budgeted Hours = SUM(Project Budgeted Hours)
      ```

      *Las horas presupuestadas del proyecto se calculan con la fórmula siguiente:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para los proyectos enumerados en la función de trabajo.\
      Esto agrega el número de horas presupuestadas del proyecto a la función.
   >[!NOTE]
   >
   >Los usuarios pueden presupuestarse tanto para las funciones primarias como para las demás (o secundarias). La variable **Porcentaje de disponibilidad de FTE** para las funciones del usuario debe ser un número diferente de 0% para que las horas disponibles muestren un valor en el Planificador de recursos para una función de trabajo. Si un usuario está asociado con una función con un 0% **Porcentaje de disponibilidad de FTE**, el valor Horario disponible es cero para esa función de trabajo. En este caso, la función puede mostrar un valor negativo **Valor neto**.\
   >Para obtener más información sobre la variable **Porcentaje de disponibilidad de FTE** para las funciones de trabajo, consulte el artículo [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Para presupuestar la asignación para el proyecto, realice una de las siguientes acciones:

   * En el **BDG** , especifique manualmente un número de horas presupuestadas, FTE o coste para los proyectos.\
      Esto también actualiza las horas presupuestadas para las funciones en las que se enumera el proyecto.

   * Haga clic en el **Más** para la función de trabajo y, a continuación, haga clic en **Establecer las horas planificadas de los proyectos como presupuestadas**.\
      Las horas presupuestadas del proyecto se calculan mediante la fórmula siguiente:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

      Las horas presupuestadas del proyecto se añaden a la función Horario presupuestado.

   * (Condicional) Si ha presupuestado las horas para los usuarios, haga clic en el botón **Más** para el proyecto y, a continuación, haga clic en **Total de horas presupuestadas de los usuarios para el proyecto**.\
      Las horas presupuestadas del proyecto se calculan con la fórmula siguiente:

      ```
      Project Budgeted Hours = SUM(User Budgeted Hours)
      ```

      ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Haga clic en **Guardar**.\
   Una vez presupuestados los recursos en el planificador de recursos, las horas presupuestadas de los recursos y los costes asociados a ellos se enumeran en el caso empresarial de cada proyecto.\
   Para obtener más información sobre cómo comprender el área de Presupuestación de Recursos del caso empresarial, consulte el artículo [Recursos presupuestarios en el caso empresarial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Opcional) Seleccione el **Ver por usuario** vista para notar cualquier sobreasignación o infrautilización de usuario entre el horario disponible y el horario planificado para cada usuario. Las horas presupuestadas no están visibles en la vista Ver por usuario .

### Recursos presupuestarios en masa {#budget-resources-in-bulk}

Puede presupuestar asignaciones para sus recursos de forma masiva al utilizar vínculos rápidos. Los vínculos rápidos solo están disponibles para las vistas Proyecto y Función.

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Al utilizar los vínculos rápidos a las asignaciones presupuestarias para los recursos, el presupuesto se aplica automáticamente solo a los períodos de tiempo mostrados en la pantalla. Si la cronología de un proyecto abarca un período de tiempo superior al que se muestra en la pantalla, debe desplazarse de izquierda a derecha y, a continuación, utilizar los vínculos rápidos para presupuestar automáticamente los recursos.

Para presupuestar los recursos de forma masiva:

1. Vaya a .\
   Para obtener más información sobre el acceso al planificador de recursos, consulte la sección &quot;Acceso al planificador de recursos&quot; en el artículo [Información general del planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   En la lista se muestra una lista de los proyectos que puede administrar.

1. (Opcional) Expanda cada proyecto para ver una lista de las funciones de trabajo asociadas a él.\
   O
1. (Opcional) Seleccione **Ver por función**, expanda cada función para ver una lista de los proyectos asociados a ella.
1. Pase el ratón sobre el nombre de un proyecto o de una función de trabajo.
1. Haga clic en el **Más** icono ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)que se muestra a la derecha del nombre del proyecto o del rol.

1. Haga clic en una de las opciones disponibles para especificar automáticamente la cantidad de horas presupuestadas (BDG) para otros objetos.

   Dependiendo de si ha hecho clic en el icono Más de un proyecto o una función, las opciones para la presupuestación en bloque difieren. La tabla siguiente ilustra las opciones disponibles para proyectos y funciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Vista de proyectos</strong> </td> 
      <td><strong>Vista de rol</strong> </td> 
     </tr> 
     <tr> 
      <td>Opciones del proyecto</td> 
      <td> 
       <ul> 
        <li><strong>Establecer las horas planificadas de los roles como presupuestadas</strong>: Seleccione esta opción para que las horas presupuestadas de la función sean idénticas a las horas planificadas. El total de horas presupuestadas para las funciones se mostrará para las horas presupuestadas del proyecto. </li> 
        <li><strong>Ajustar fechas de presupuesto</strong> : Seleccione esta opción para mover las horas presupuestadas a otro intervalo de tiempo.<br>Para obtener más información sobre el ajuste de fechas de presupuesto, consulte <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Ajustar fechas de presupuesto en el planificador de recursos</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Establecer las horas planificadas de los usuarios como presupuestadas</strong>: Seleccione esta opción para que las horas presupuestadas del usuario sean idénticas a las horas planificadas del usuario. </li> 
        <li><strong>Total de horas presupuestadas de los usuarios para el proyecto</strong>: Seleccione esta opción para agregar todas las horas presupuestadas del usuario y mostrar el total como horas presupuestadas para el proyecto y para la función. Le recomendamos que utilice esta opción después de haber presupuestado manualmente a sus usuarios o de haber utilizado primero la opción anterior. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Opciones de rol</td> 
      <td> 
       <ul> 
        <li><strong>Establecer las horas planificadas de los usuarios como presupuestadas</strong>: Seleccione esta opción para que las horas presupuestadas del usuario sean idénticas a las horas planificadas. </li> 
        <li><strong>Horario presupuestado total de los usuarios para la función</strong>: Seleccione esta opción para agregar todas las horas presupuestadas del usuario y mostrar el total como horas presupuestadas para la función y el proyecto. Le recomendamos que utilice esta opción después de haber presupuestado manualmente a sus usuarios o de haber utilizado primero la opción anterior. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Establecer las horas planificadas de los proyectos como presupuestadas</strong>: Seleccione esta opción para que el proyecto Horario presupuestado sea idéntico al del proyecto Horario planificado. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Es posible que algunas de las opciones no se muestren si faltan algunos de los requisitos previos para trabajar en el Planificador de recursos.
   >
   >
   >Para obtener más información sobre los requisitos previos que deben cumplirse para una presupuestación precisa en el Planificador de recursos, consulte la sección &quot;Requisitos previos para trabajar en el Planificador de recursos&quot; en la sección [Información general del planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artículo.\
   >Por ejemplo, es posible que algunas de las opciones no se muestren en los siguientes escenarios:
   >
   >   
   >   
   >   * Cuando los proyectos no están asociados con el grupo de recursos
   >   * Cuando los grupos de recursos asociados a proyectos no contienen usuarios
   >   * Cuando los grupos de recursos asociados a proyectos contienen usuarios sin funciones de trabajo asociadas a ellos.

