---
content-type: reference
product-area: projects
navigation-topic: financials
title: Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos
description: Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Puede presupuestar los recursos para el trabajo mediante el planificador de recursos de Adobe Workfront.

A medida que se presupuestan los recursos para el trabajo en proyectos, Workfront calcula el costo de trabajo presupuestado para las funciones, los proyectos y los usuarios en función de los valores de coste por hora.

El costo de trabajo presupuestado del planificador de recursos de un proyecto es un cálculo entre el costo asociado con las funciones de trabajo asignadas para completar el trabajo en el proyecto y la cantidad de horas estimadas (horas presupuestadas del planificador de recursos) que pueden tomar cada función para completar el trabajo.

>[!IMPORTANT]
>
>El costo de trabajo presupuestado del planificador de recursos para los usuarios no afecta al del proyecto. Solo el coste laboral de las funciones laborales afecta al coste del proyecto.

## Visión General del Coste Laboral Presupuestado para Funciones Laborales y el Proyecto

Workfront utiliza el Coste de trabajo presupuestado de las funciones de trabajo del proyecto para calcular el Coste de trabajo presupuestado del proyecto.

>[!TIP]
>
>El Coste Laboral Presupuestado de un proyecto en el Caso Empresarial aparece como Coste Laboral Presupuestado del Planificador de Recursos en los informes y listas.

La variable **Coste de trabajo presupuestado** (o Coste de trabajo presupuestado del planificador de recursos) de un proyecto se calcula mediante la siguiente fórmula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Los campos utilizados en el cálculo anterior se refieren a lo siguiente:

* Horas presupuestadas para funciones de trabajo en el área de Presupuestación de Recursos del proyecto o el Planificador de Recursos.

   Para obtener más información sobre la presupuestación de recursos en el Planificador de recursos, consulte la sección &quot;Recursos de presupuestación en el Planificador de recursos&quot; en el artículo [Información general del planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   Para obtener más información sobre la presupuestación de recursos en el área Presupuestación de recursos del caso empresarial, consulte [Recursos presupuestarios en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* La variable **Tasa de costo por hora de una función de trabajo** en el cálculo anterior hace referencia al coste asociado a cada función de trabajo del proyecto.\
   Para obtener más información sobre la creación y administración de funciones de trabajo y su asociación con las tasas de coste, consulte el artículo [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront calcula toda la información de coste utilizando la moneda del proyecto. Si especifica Horario presupuestado para los recursos en el Planificador de recursos, la opción para cambiar la moneda del proyecto estará deshabilitada.\
>Para obtener más información sobre cómo cambiar la moneda de un proyecto, consulte el artículo [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Descripción general del coste laboral presupuestado para usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>El costo laboral presupuestado por el usuario no afecta al costo laboral presupuestado del proyecto. Sólo el costo laboral de las funciones laborales de un proyecto afecta al costo laboral presupuestado del planificador de recursos del proyecto.
> 
>El total de todos los costes laborales de todos los usuarios puede o no igualar el coste laboral presupuestado del planificador de recursos de las funciones laborales asociadas a los usuarios.
>
>Si calcula las horas presupuestadas para los usuarios del Planificador de recursos, los costes asociados a ellas son los de las funciones de trabajo asociadas a los usuarios. No son costes asociados a los usuarios ni a sus tarifas.

Si los usuarios están asociados a las funciones de trabajo del proyecto y sus horas están presupuestadas en el Planificador de recursos, su Costo de trabajo presupuestado se muestra con los nombres siguientes, según la ubicación en la que los vea en Workfront:

* [!UICONTROL **Coste de trabajo presupuestado**]: El área de Presupuestación de Recursos del Caso de Negocio bajo sus respectivas funciones.

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: Planificador de recursos cuando se ve información en la vista Proyecto y Función por Costo.

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Los usuarios se muestran en el área de Presupuestación de Recursos del Caso de Negocio bajo sus respectivas funciones o en el Planificador de Recursos si cumplen los siguientes requisitos:

* Están asociados a una de las funciones de trabajo del proyecto.
* Tienen las horas presupuestadas especificadas en el Planificador de recursos.
* Tienen una tasa de costo por hora asociada con su perfil.

   Para obtener más información sobre cómo agregar tasas de costo por hora a los usuarios, consulte el artículo [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* El usuario forma parte de uno de los grupos de recursos asociados al proyecto.

El coste laboral presupuestado de un usuario se calcula mediante la fórmula siguiente:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Localización del costo de trabajo presupuestado de un proyecto

El Coste Laboral Presupuestado tal como se refleja en el área de Presupuestación de Recursos del Caso Empresarial o el Planificador de Recursos se muestra en las siguientes áreas de Workfront con los nombres siguientes:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nombre para mostrar Costo de mano de obra presupuestado</strong></td> 
     <td><strong>Área de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Costo de mano de obra presupuestado</td> 
     <td>Área de presupuestación de recursos del caso empresarial</td> 
    </tr> 
    <tr> 
     <td>Costo presupuestado</td> 
     <td><p>Informe de utilización Vista Coste</p><p>Para obtener más información, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ver información de utilización</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Vistas Proyecto o Función del Planificador de Recursos, por Coste</td> 
    </tr> 
    <tr> 
     <td>Coste de trabajo presupuestado del proyecto del planificador de recursos</td> 
     <td> <p>Informe del proyecto</p> <p>Informe de proyecto (datos financieros)</p> <p>Informe de tareas</p> <p>Informe de problemas</p> <p>Informe de hora presupuestada</p> <p>Para obtener información sobre cómo crear un informe, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Si utiliza Adobe Workfront Scenario Planner para presupuestar los recursos del proyecto, el Coste de trabajo presupuestado en el área Presupuestación de recursos del caso empresarial es el mismo que el Coste de personas de la iniciativa vinculada al proyecto. El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md). Para obtener información sobre cómo presupuestar recursos mediante el planificador de escenarios, consulte [Recursos de presupuesto en el caso empresarial con el planificador de escenarios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Localizar las horas presupuestadas de un proyecto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Las horas presupuestadas afectan al valor del costo laboral presupuestado (o el costo presupuestado del planificador de recursos) del proyecto.

El costo de trabajo presupuestado de un proyecto es el costo asociado con las funciones de trabajo asignadas para completar el trabajo del proyecto y la cantidad de horas estimadas (horas presupuestadas) que pueden tomar cada rol para completar el trabajo.

Puede ver las horas presupuestadas en Workfront en los campos enumerados en la siguiente tabla.

>[!NOTE]
>
>Cualquier otra mención de &quot;Horario presupuestado&quot; en Workfront hace referencia a las horas presupuestadas utilizando funciones obsoletas que se han eliminado de Workfront. Son campos de solo vista y no se actualizan con la información actual cuando se utilizan herramientas de presupuestación de recursos actuales.

Las horas presupuestadas en el área de Presupuestación de Recursos del Caso de Negocio o el Planificador de Recursos se muestran en las siguientes áreas de Workfront y con los nombres siguientes:

* **Horas**: Área de presupuestación de recursos del caso empresarial
* **BDG**:Planificador de recursos visto por horas
* **Horas presupuestadas**: Vista Horas del informe de uso Para obtener más información, consulte [Ver información de utilización de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Horas**: Informe de hora presupuestada

   El objeto Hora presupuestada del informe Hora presupuestada hace referencia a información relacionada con una herramienta de administración de recursos obsoleta. Sólo el &quot;Bud&quot;. El campo &quot;Horas&quot; de este informe se refiere a las horas presupuestadas en el Planificador de Recursos o en el área de Presupuestación de Recursos del Caso de Negocio del proyecto.

   Para obtener más información sobre la creación de informes, consulte el artículo **Crear un informe personalizado**.
* **Horario presupuestado del planificador de recursos**: en los siguientes informes:

   * Informe del proyecto
   * Informe de proyecto (datos financieros)
   * Informe de tareas
   * Informe de problemas
   * Informe de hora presupuestada
