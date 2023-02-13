---
navigation-topic: business-case-and-scorecards
title: Recursos presupuestarios en el caso empresarial utilizando el planificador de recursos
description: Como parte de la planificación de recursos, puede utilizar el Planificador de recursos a nivel de proyecto para presupuestar las funciones de trabajo necesarias para completar el trabajo en un proyecto cuando cree el caso empresarial.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# Recursos presupuestarios en el caso empresarial utilizando el planificador de recursos

Como parte de la planificación de recursos, puede utilizar el Planificador de recursos a nivel de proyecto para presupuestar las funciones de trabajo necesarias para completar el trabajo en un proyecto cuando cree el caso empresarial.

Para obtener más información sobre cómo crear un caso empresarial, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>La información introducida en el Planificador de recursos a nivel de proyecto también es visible en el Planificador de recursos a nivel de sistema. Lo contrario también es cierto. Para obtener información acerca del planificador de recursos, consulte [Información general del planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

También puede presupuestar recursos en el caso empresarial mediante el planificador de escenarios de Adobe Workfront. Para obtener más información, consulte [Recursos de presupuesto en el caso empresarial con el planificador de escenarios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Adobe Workfront</a>*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>*</td> 
   <td> <p>Revisar o superior</p> <p>Importante: Debe tener una licencia de Plan para modificar la información de presupuesto de recursos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente: </p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Datos financieros</p> </li> 
    </ul> <p>Para obtener información sobre el acceso necesario a los recursos presupuestarios, consulte también <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Acceso necesario para presupuestar recursos en Adobe Workfront</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Adobe Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de comenzar, debe hacer lo siguiente:

* Cumplir todos los requisitos previos para la planificación de recursos en Adobe Workfront. Para obtener más información, consulte [Información general del planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Asocie grupos de recursos al proyecto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   No se pueden presupuestar recursos asignados a problemas en el caso empresarial. Puede presupuestarlos en el Planificador de recursos a nivel de sistema. Para obtener más información acerca del planificador de recursos, consulte [Información general del planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Aunque no se trata de un requisito previo, también se recomienda indicar las horas programadas para las tareas del proyecto. Esto le ayuda a comprender la cantidad de trabajo que una tarea puede necesitar completar, lo que le ayuda a decidir cuánto tiempo se deben presupuestar los recursos para completar la tarea. Para obtener información sobre cómo asociar tareas con horas planificadas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Aplicar grupos de recursos a un proyecto y recursos presupuestarios en el caso empresarial

>[!IMPORTANT]
Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información del presupuesto no sea precisa.

Para aplicar grupos de recursos y recursos del proyecto presupuestario en el caso práctico de un proyecto sin grupo de recursos:

1. Vaya al proyecto cuyos recursos desea presupuestar.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. (Condicional) Si su empresa no tiene una licencia para el planificador de escenario de Workfront, haga clic en **Editar presupuesto de recursos** en el **Presupuestación de recursos** y, a continuación, continúe con el paso 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Opcional y condicional) Si la información del proyecto se ha publicado desde una iniciativa del planificador de escenarios, realice una de las siguientes acciones:

   * Seleccione Planificador de recursos en la **Elija qué horas utilizar para calcular el costo laboral presupuestado del proyecto** y, a continuación, haga clic en **Elija > Editar presupuesto de recursos**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Si se seleccionó el Planificador de escenario para presupuestar recursos para el proyecto, haga clic en **Cambiar** > **Editar presupuesto de recursos**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Esta opción utiliza las horas presupuestadas del proyecto para calcular el coste laboral presupuestado del proyecto.

   El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Le recomendamos que tome la decisión de usar el Planificador de recursos o el Planificador de escenario cuando empiece a trabajar en un proyecto. A menudo, el cambio entre los dos durante la vida del proyecto puede crear incoherencias en la forma en que se presupuestan los recursos para el proyecto.

1. En el **Seleccionar grupo de recursos** , especifique una o varias **Grupos de recursos**.

   Debe especificar solo Grupos de recursos que se rellenen con usuarios activos.

   >[!TIP]
   Si el proyecto ya está asociado con grupos de recursos, el Planificador de recursos se muestra de forma predeterminada. Para agregar más grupos de recursos al proyecto, edite el proyecto. Para obtener información sobre cómo editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Haga clic en **Aplicar**.

   Se muestra el Planificador de recursos para el proyecto seleccionado.

   De forma predeterminada, las 20 primeras funciones de trabajo asociadas con este proyecto se enumeran en la sección Presupuestación de recursos en orden alfabético. 

   Para obtener más información acerca del planificador de recursos, consulte [Información general del planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budget_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Opcional y condicional) Expanda las funciones de trabajo para ver los usuarios asociados a ellas.

   >[!NOTE]
   Los usuarios activos se muestran bajo las funciones de trabajo asociadas a ellos solo si cumplen los siguientes criterios:
   * Pertenecen a uno de los Grupos de Recursos del proyecto.
   * Tienen asignadas horas presupuestadas.
   * Están asociados a una de las funciones de trabajo del proyecto.


    

1. Haga clic en **Hoy** para volver al lapso de tiempo de hoy.
1. (Opcional) Haga clic en **Semana**, **Mes** o **Trimestre** para mostrar información del proyecto en distintos intervalos de tiempo.
1. (Opcional) Haga clic en el **Horas** menú desplegable y seleccione **Horas**,**FTE** o **Costo** para cambiar la forma en que se muestra la información en el planificador de recursos. De forma predeterminada, se muestran las horas.

1. (Opcional) Haga clic en **Exportar** para exportar el planificador de recursos a un archivo de Excel.

   >[!NOTE]
   Puede exportar datos de hasta 12 períodos de tiempo a la vez.

1. (Opcional) Haga clic en el **Pantalla completa** icono ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) para mostrar el Planificador de recursos en modo de pantalla completa.

1. Actualice el **BDG** Campo (Horas presupuestadas) con valores de hora, tiempo de espera o costo para los usuarios, las funciones o el proyecto mediante una de las siguientes acciones:

   * Calcule manualmente la cantidad de valores de horas, horas y horas o costes para roles, usuarios o el proyecto.

      O

   * Haga clic en el **Opciones** para el proyecto o las funciones de trabajo y seleccione una opción para presupuestar automáticamente las horas para las funciones, los usuarios o el proyecto.
   Para obtener más información sobre la presupuestación en la vista de proyecto del planificador de recursos, consulte [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Puede presupuestar horas, FTE o costes de los recursos para cualquier lapso de tiempo mostrado en el área de Presupuestación de recursos, independientemente de la cronología del proyecto. Por ejemplo, si desea indicar que los recursos podrían no estar disponibles durante la cronología del proyecto (donde están asociados con Horario planificado), pero que podrían estar disponibles durante otro tiempo, puede hacerlo presupuestándolos para lapsos de tiempo en los que las horas planificadas sean cero, si es que están disponibles para funcionar.

1. (Opcional) Para comprender si puede mover las horas, los FTE o los costes presupuestados a otro intervalo de tiempo, haga clic en el botón **Opciones** icono, luego **Ajustar fechas de presupuesto**.

   Para obtener más información sobre el ajuste de fechas presupuestadas, consulte [Ajustar fechas de presupuesto en el planificador de recursos](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Haga clic en **Guardar**.

   Si tiene tasas de costo por hora asociadas con las funciones de su trabajo, al presupuestar los recursos en el área de Presupuestación de Recursos se calcula la variable **Coste de trabajo presupuestado** del proyecto. El Coste Laboral Presupuestado se muestra en el área Presupuestación de Recursos del Caso Empresarial y en el Resumen de Casos Empresariales.

   >[!TIP]
   El coste se muestra en el caso empresarial en la moneda del proyecto.

   La información de presupuesto especificada en el caso empresarial también se muestra en el planificador de recursos.
