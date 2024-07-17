---
content-type: reference
product-area: projects
navigation-topic: financials
title: Comprender el costo laboral presupuestado y las horas presupuestadas de los proyectos
description: Comprender el costo laboral presupuestado y las horas presupuestadas de los proyectos
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Comprender el costo laboral presupuestado y las horas presupuestadas de los proyectos

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Puede presupuestar los recursos para el trabajo mediante el Planificador de recursos de Adobe Workfront.

A medida que presupueste los recursos para el trabajo en proyectos, Workfront calculará el costo de mano de obra presupuestado para los roles, proyectos y usuarios en función de los valores de costo por hora.

El costo de mano de obra presupuestado del planificador de recursos de un proyecto es un cálculo entre el costo asociado con los roles asignados para completar el trabajo del proyecto y la cantidad de horas estimadas (horas presupuestadas del planificador de recursos) que puede tomar cada rol para completar el trabajo.

>[!IMPORTANT]
>
>El Costo de mano de obra presupuestado del Planificador de recursos para los usuarios no afecta al del proyecto. Solo el coste laboral de los roles afecta al coste del proyecto.

## Visión General del Coste Laboral Presupuestado para Roles y el Proyecto

Workfront utiliza el coste de mano de obra presupuestado de los roles del proyecto para calcular el coste de mano de obra presupuestado del proyecto.

>[!TIP]
>
>El costo de mano de obra presupuestado de un proyecto en el caso empresarial se muestra como Costo de mano de obra presupuestado del Planificador de recursos en informes y listas.

El **Costo de mano de obra presupuestado** (o Costo de mano de obra presupuestado del planificador de recursos) de un proyecto se calcula mediante la siguiente fórmula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Los campos utilizados en el cálculo anterior hacen referencia a lo siguiente:

* Horas presupuestadas para los roles en el área de Presupuesto de recursos del proyecto o del Planificador de recursos.

  Para obtener más información acerca de cómo presupuestar recursos en el Planificador de recursos, vea la sección &quot;Presupuestando recursos en el Planificador de recursos&quot; en el artículo [Información general del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Para obtener más información acerca de cómo presupuestar recursos en el área de Presupuestación de recursos del caso empresarial, vea [Presupuesto de recursos en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* La **tasa de costo por hora de un rol** en el cálculo anterior se refiere al costo asociado con cada rol en el proyecto.\
  Para obtener más información sobre cómo crear y administrar roles de trabajo y asociarlos con las tasas de costo, consulte el artículo [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront calcula toda la información de costes utilizando la divisa del proyecto. Si especifica Horas presupuestadas para los recursos en el Planificador de recursos, se deshabilita la opción para cambiar la divisa del proyecto.\
>Para obtener más información acerca de cómo cambiar la moneda de un proyecto, vea el artículo [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Visión General del Coste Laboral Presupuestado para Usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>El costo de mano de obra presupuestado del usuario no afecta el costo de mano de obra presupuestado del proyecto. Sólo el costo laboral de los roles de trabajo de un proyecto afecta al costo de mano de obra presupuestado del planificador de recursos del proyecto.
> 
>El total de todos los costos laborales de todos los usuarios puede ser igual o no al costo laboral presupuestado del planificador de recursos de los roles asociados con los usuarios.
>
>Si estima las horas presupuestadas de los usuarios en el Planificador de recursos, los costos asociados con ellas son los de los roles asociados con los usuarios. No son costes asociados a los usuarios ni a sus tarifas.

Si los usuarios están asociados con los roles del proyecto y sus horas están presupuestadas en el Planificador de recursos, el Coste de mano de obra presupuestado se muestra con los siguientes nombres, según el lugar donde los vea en Workfront:

* [!UICONTROL **Costo de mano de obra presupuestado**]: El área de Presupuestación de recursos del caso empresarial bajo sus respectivos roles.

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: Planificador de recursos al ver información en la vista de proyecto y rol por costo.

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Los usuarios se muestran en el área de Presupuestación de recursos del caso empresarial bajo sus respectivos roles o en el Planificador de recursos si cumplen los siguientes requisitos:

* Están asociados a uno de los roles del proyecto.
* Tienen horas presupuestadas especificadas en el Planificador de recursos.
* Tienen una tarifa de costo por hora asociada a su perfil.

  Para obtener más información acerca de cómo agregar tarifas de costo por hora a los usuarios, vea el artículo [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* El usuario forma parte de uno de los conjuntos de recursos asociados al proyecto.

El costo de mano de obra presupuestado de un usuario se calcula mediante la siguiente fórmula:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Localizar el costo de mano de obra presupuestado de un proyecto

El costo de mano de obra presupuestado, tal como se refleja en el área de presupuesto de recursos del caso comercial o del planificador de recursos, se muestra en las siguientes áreas de Workfront con los siguientes nombres:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nombre para mostrar Coste laboral presupuestado</strong></td> 
     <td><strong>Área de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Costo de mano de obra presupuestado</td> 
     <td>Área de presupuesto de recursos del caso empresarial</td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado</td> 
     <td><p>Vista de coste del informe de utilización</p><p>Para obtener más información, vea <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ver información de utilización</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Vistas de proyecto o rol del Planificador de recursos, por costo</td> 
    </tr> 
    <tr> 
     <td>Costo de mano de obra presupuestado del proyecto del planificador de recursos</td> 
     <td> <p>Informe de proyecto</p> <p>Informe de proyecto (datos financieros)</p> <p>Informe de tareas</p> <p>Informe de problema</p> <p>Informe de horas presupuestadas</p> <p>Para obtener información acerca de cómo crear un informe, vea el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Si utiliza el planificador de escenarios de Adobe Workfront para presupuestar recursos del proyecto, el costo de mano de obra presupuestado en el área de presupuesto de recursos del caso empresarial es el mismo que el costo de personas de la iniciativa vinculada al proyecto. El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general sobre el Scenario Planner](../../../scenario-planner/scenario-planner-overview.md). Para obtener información acerca de cómo presupuestar recursos mediante el Scenario Planner, vea [Presupuesto de recursos en el caso comercial con el Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Localizar las horas presupuestadas de un proyecto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Las horas presupuestadas afectan al valor del costo de mano de obra presupuestado (o el costo presupuestado del planificador de recursos) del proyecto.

El costo de mano de obra presupuestado de un proyecto es el costo asociado con los roles asignados para completar el trabajo del proyecto y la cantidad de horas estimadas (horas presupuestadas) que puede requerir cada rol para completar el trabajo.

Puede ver las horas presupuestadas en Workfront en los campos enumerados en la tabla siguiente.

>[!NOTE]
>
>Cualquier otra mención de &quot;Horas presupuestadas&quot; en Workfront hace referencia a horas presupuestadas mediante funciones obsoletas que se han eliminado de Workfront. Son campos de sólo consulta y no se actualizan con la información actual cuando se utilizan las herramientas de presupuesto de recursos actuales.

Las horas presupuestadas en el área de Presupuestación de recursos del Caso comercial o del Planificador de recursos se muestran en las siguientes áreas de Workfront y con los siguientes nombres:

* **Horas**: área de presupuesto de recursos del caso comercial
* **BDG**:Planificador de recursos visto por horas
* **Horas presupuestadas**: vista de horas del informe de utilización
Para obtener más información, consulte [Ver información de utilización de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Horas**: informe de horas presupuestadas

  El objeto Hora presupuestada del informe Hora presupuestada hace referencia a información relacionada con una herramienta de administración de recursos obsoleta. Sólo el &quot;Bud&quot;. El campo &quot;Horas&quot; de este informe hace referencia a las horas presupuestadas en el Planificador de recursos o en el área de Presupuestación de recursos del caso comercial del proyecto.

  Para obtener más información acerca de cómo crear un informe, vea el artículo **Crear un informe personalizado**.
* **Horas presupuestadas del planificador de recursos**: en los siguientes informes:

   * Informe de proyecto
   * Informe de proyecto (datos financieros)
   * Informe de tareas
   * Informe de problema
   * Informe de horas presupuestadas
