---
content-type: reference
product-area: projects
navigation-topic: financials
title: Comprender el coste presupuestado de la mano de obra y las horas presupuestadas para proyectos
description: Comprender el coste presupuestado de la mano de obra y las horas presupuestadas para proyectos
author: Lisa
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 100%

---

# Comprender el coste presupuestado de la mano de obra y las horas presupuestadas para proyectos

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Puede presupuestar los recursos para el trabajo mediante el Planificador de recursos de Adobe Workfront.

A medida que presupueste los recursos para el trabajo en proyectos, Workfront calculará el coste de mano de obra presupuestado de las funciones, proyectos y usuarios en función de los valores de coste por hora.

El coste de mano de obra presupuestado del planificador de recursos de un proyecto es un cálculo entre el coste asociado a las funciones del puesto asignadas para completar el trabajo del proyecto y la cantidad de horas estimadas (horas presupuestadas del planificador de recursos) que puede tardar cada función en completar el trabajo.

>[!IMPORTANT]
>
>El coste de mano de obra presupuestado del Planificador de recursos para los usuarios no afecta al del proyecto. Solo el coste de mano de obra de las funciones del puesto afecta al coste del proyecto.

## Información general sobre el coste de mano de obra presupuestado para las funciones del puesto y el proyecto

Workfront utiliza el coste de mano de obra presupuestado de las funciones del puesto del proyecto para calcular el coste de mano de obra presupuestado del proyecto.

>[!TIP]
>
>El coste de mano de obra presupuestado de un proyecto en el caso empresarial se muestra como coste de mano de obra presupuestado del Planificador de recursos en informes y listas.

El **costo de mano de obra presupuestado** (o costo de mano de obra presupuestado del planificador de recursos) de un proyecto se calcula mediante la siguiente fórmula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Los campos utilizados en el cálculo anterior hacen referencia a lo siguiente:

* Horas presupuestadas para las funciones del puesto en el área de Presupuesto de recursos del proyecto o del Planificador de recursos.

  Para obtener más información sobre el presupuesto de recursos en el Planificador de recursos, consulte la sección &quot;Presupuesto de recursos en el Planificador de recursos&quot; en el artículo [Información general sobre el Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Para obtener más información sobre el presupuesto de recursos en el área de Presupuestación de recursos del caso empresarial, consulte [Presupuesto de recursos en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* La **tarifa de coste por hora de una función de trabajo** en el cálculo anterior se refiere al coste asociado a cada función de trabajo en el proyecto.\
  Para obtener más información sobre la creación y administración de funciones del puesto y asociarlos a tarifas de coste, consulte el artículo [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront calcula toda la información sobre los costes utilizando la divisa del proyecto. Si especifica Horas presupuestadas para los recursos en el Planificador de recursos, se deshabilita la opción para cambiar la divisa del proyecto.\
>Para obtener más información sobre cómo cambiar la moneda de un proyecto, consulte el artículo [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Información general sobre el costo de mano de obra presupuestado para usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>El costo de mano de obra presupuestado del usuario no afecta al costo de mano de obra presupuestado del proyecto. Solo el coste de mano de obra de las funciones del puesto de un proyecto afecta al costo de mano de obra presupuestado del planificador de recursos del proyecto.
> 
>El total de todos los costes de mano de obra de todos los usuarios puede ser igual o no al coste de mano de obra presupuestado del planificador de recursos de las funciones del puesto asociadas a los usuarios.
>
>Si estima las horas presupuestadas de los usuarios en el Planificador de recursos, los costes asociados a ellas son los de las funciones del puesto asociadas a los usuarios.No son costes asociados a los usuarios ni a sus tarifas.

Si los usuarios están asociados a las funciones del puesto del proyecto y sus horas están presupuestadas en el Planificador de recursos, el costo de mano de obra presupuestado se muestra con los siguientes nombres, según el lugar donde los vea en Workfront:

* [!UICONTROL **Costo de mano de obra presupuestado**]: el área de Presupuestación de recursos del caso empresarial bajo sus respectivas funciones.

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: el Planificador de recursos al ver información en la vista de proyecto y función por coste.

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Los usuarios se muestran en el área de Presupuestación de recursos del caso empresarial bajo sus respectivas funciones o en el Planificador de recursos si cumplen los siguientes requisitos:

* Están asociados a una de las funciones del puesto del proyecto.
* Tienen horas presupuestadas especificadas en el Planificador de recursos.
* Tienen una tarifa de coste por hora asociada a su perfil.

  Para obtener más información sobre cómo añadir tarifas de coste por hora a los usuarios, consulte el artículo [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* El usuario forma parte de uno de los conjuntos de recursos asociados al proyecto.

El costo de mano de obra presupuestado de un usuario se calcula mediante la siguiente fórmula:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Localización del costo de mano de obra presupuestado de un proyecto

El costo de mano de obra presupuestado, tal como se refleja en el área de presupuesto de recursos del caso empresarial o del planificador de recursos, se muestra en las siguientes áreas de Workfront con los siguientes nombres:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nombre para mostrar el costo de mano de obra presupuestado</strong></td> 
     <td><strong>Área de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Costo de mano de obra presupuestado</td> 
     <td>Área de presupuestación de recursos del caso empresarial</td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado</td> 
     <td><p>Vista de coste del informe de utilización</p><p>Para obtener más información, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ver información de utilización</a>.</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Vistas de proyecto o rol del Planificador de recursos, por coste</td> 
    </tr> 
    <tr> 
     <td>Costo de mano de obra presupuestado del proyecto del Planificador de recursos</td> 
     <td> <p>Informe de proyecto</p> <p>Informe de proyecto (datos financieros)</p> <p>Informe de tarea</p> <p>Informe de problema</p> <p>Informe de horas presupuestadas</p> <p>Para obtener información sobre la creación de un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Si utiliza el planificador de escenarios de Adobe Workfront para presupuestar recursos del proyecto, el costo de mano de obra presupuestado en el área de Presupuestación de recursos del caso empresarial es el mismo que los Costes de personas de la iniciativa vinculada al proyecto. El Planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de recursos de Workfront, consulte [Información general sobre el planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md). Para obtener información sobre el presupuesto de recursos mediante el planificador de escenarios, consulte [Presupuesto de recursos en el caso empresarial con el planificador de recursos](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Localizar las horas presupuestadas de un proyecto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Las horas presupuestadas afectan al valor del costo de mano de obra presupuestado (o el costo presupuestado del planificador de recursos) del proyecto.

El costo de mano de obra presupuestado de un proyecto es el costo asociado a las funciones del puesto asignadas para completar el trabajo del proyecto y la cantidad de horas estimadas (horas presupuestadas) que puede requerir cada función para completar el trabajo.

Puede ver las horas presupuestadas en Workfront en los campos enumerados en la tabla siguiente.

>[!NOTE]
>
>Cualquier otra mención de &quot;Horas presupuestadas&quot; en Workfront hace referencia a horas presupuestadas mediante funciones obsoletas que se han eliminado de Workfront. Son campos de solo consulta y no se actualizan con la información actual cuando se utilizan las herramientas de presupuestación de recursos actuales.

Las horas presupuestadas en el área de Presupuestación de recursos del caso comercial o del planificador de recursos se muestran en las siguientes áreas de Workfront y con los siguientes nombres:

* **Horas**: área de Presupuestación de recursos del caso empresarial
* **BDG**: planificador de recursos visualizado por horas
* **Horas presupuestadas**: vista de horas del informe de utilización
Para obtener más información, consulte [Ver información sobre la utilización de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Horas  presup.**: informe de las horas presupuestadas

  El objeto Hora presupuestada del informe Hora presupuestada hace referencia a información relacionada con una herramienta de administración de recursos obsoleta. Solo el campo &quot;Horas  presup.&quot; en este informe hace referencia a las horas presupuestadas en el Planificador de recursos o en el área de Presupuestación de recursos del caso comercial del proyecto.

  Para obtener más información sobre la creación de un informe, consulte el artículo **Crear un informe personalizado**.
* **Horas presupuestadas del planificador de recursos**: en los siguientes informes:

   * Informe de proyecto
   * Informe de proyecto (datos financieros)
   * Informe de tarea
   * Informe de problema
   * Informe de horas presupuestadas
