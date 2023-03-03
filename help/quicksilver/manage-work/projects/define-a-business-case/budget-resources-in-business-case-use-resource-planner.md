---
navigation-topic: business-case-and-scorecards
title: Presupuestar recursos en el caso comercial utilizando el Planificador de recursos
description: Como parte de la planificación de recursos, puede utilizar el Planificador de recursos en el nivel de proyecto para presupuestar los roles de trabajo necesarios para completar el trabajo en un proyecto al crear el caso empresarial.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# Presupuestar recursos en el caso comercial utilizando el Planificador de recursos

Como parte de la planificación de recursos, puede utilizar el Planificador de recursos en el nivel de proyecto para presupuestar los roles de trabajo necesarios para completar el trabajo en un proyecto al crear el caso empresarial.

Para obtener más información sobre la creación de un caso empresarial, consulte [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>La información introducida en el Planificador de recursos de nivel de proyecto también se puede ver en el Planificador de recursos de nivel de sistema. Lo contrario también es cierto. Para obtener información sobre el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

También puede presupuestar recursos en el caso empresarial mediante Adobe Workfront Scenario Planner. Para obtener más información, consulte [Presupuestar recursos en el caso empresarial con el Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

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
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a>*</td> 
   <td> <p>Revisar o superior</p> <p>Importante: Debe tener una licencia de planificación para modificar la información de presupuesto de recursos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente: </p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Datos financieros</p> </li> 
    </ul> <p>Para obtener información sobre el acceso necesario para presupuestar los recursos, consulte también <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Acceso necesario a los recursos del presupuesto en Adobe Workfront</a>.</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Adobe Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Antes de empezar, debe hacer lo siguiente:

* Cumpla todos los requisitos previos para la planificación de recursos en Adobe Workfront. Para obtener más información, consulte [Resumen del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Asocie conjuntos de recursos al proyecto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   No puede presupuestar recursos asignados a problemas en el caso comercial. Puede presupuestarlos en el Planificador de recursos del sistema. Para obtener más información sobre el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Aunque no se trata de un requisito previo, también le recomendamos que indique las horas planificadas para las tareas del proyecto. Esto le ayuda a comprender la cantidad de trabajo que una tarea puede necesitar para completarse, lo que le ayuda a tomar la decisión de cuánto tiempo se deben presupuestar los recursos para completar la tarea. Para obtener información sobre cómo asociar tareas con horas planificadas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Aplicar conjuntos de recursos a un proyecto y presupuestar recursos en el caso comercial

>[!IMPORTANT]
Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información de presupuestación no sea precisa.

Para aplicar conjuntos de recursos y presupuestar recursos de proyecto en el caso comercial de un proyecto sin conjunto de recursos:

1. Vaya al proyecto para el que desea presupuestar recursos.
1. Clic **Caso comercial** en el panel izquierdo.
1. (Condicional) Si su empresa no tiene una licencia para Workfront Scenario Planner, haga clic en **Editar presupuesto de recursos** en el **Presupuestación de recursos** y continúe con el paso 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Opcional y condicional) Si la información del proyecto se ha publicado a partir de una iniciativa en el Scenario Planner, realice una de las siguientes acciones:

   * Seleccione el Planificador de recursos en la **Elija las horas que se utilizarán para calcular el costo de mano de obra presupuestado del proyecto** y haga clic en **Elija > Editar presupuesto de recursos**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Si el Planificador de escenarios se seleccionó para presupuestar recursos para el proyecto, haga clic en **Cambiar** > **Editar presupuesto de recursos**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Utiliza las horas presupuestadas del proyecto para calcular el costo de mano de obra presupuestado del proyecto.

   El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general del Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Le recomendamos que tome la decisión de usar el Planificador de recursos o el Planificador de escenarios cuando empiece a trabajar en un proyecto. Cambiar con frecuencia entre los dos durante la duración del proyecto puede crear incoherencias en la forma de presupuestar los recursos del proyecto.

1. En el **Seleccionar conjunto de recursos** , especifique uno o varios **Conjuntos de recursos**.

   Debe especificar únicamente conjuntos de recursos que se rellenen con usuarios activos.

   >[!TIP]
   Si el proyecto ya está asociado a conjuntos de recursos, el Planificador de recursos se muestra de forma predeterminada. Para agregar más conjuntos de recursos al proyecto, edite el proyecto. Para obtener información sobre cómo editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clic **Aplicar**.

   Se muestra el Planificador de recursos para el proyecto seleccionado.

   De forma predeterminada, las 20 primeras funciones del puesto asociadas a este proyecto se enumeran en la sección Presupuestación de recursos en orden alfabético. 

   Para obtener más información sobre el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budget_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Opcional y condicional) Expanda las funciones del puesto para ver los usuarios asociados a ellas.

   >[!NOTE]
   Los usuarios activos se muestran en los roles asociados a ellos solo si cumplen los siguientes criterios:
   * Pertenecen a uno de los conjuntos de recursos del proyecto.
   * Tienen horas presupuestadas asignadas a ellos.
   * Están asociados a uno de los roles del proyecto.


    

1. Clic **Hoy** para volver al lapso de tiempo actual.
1. (Opcional) Haga clic en **Semana**, **Mes** o **Trimestre** para mostrar información del proyecto en diferentes lapsos de tiempo.
1. (Opcional) Haga clic en **Horas** menú desplegable y seleccione. **Horas**,**ETC**, o **Coste** para cambiar la forma en que se muestra la información en el Planificador de recursos. Las horas se muestran de forma predeterminada.

1. (Opcional) Haga clic en **Exportar** para exportar el Planificador de recursos a un archivo de Excel.

   >[!NOTE]
   Puede exportar datos de hasta 12 períodos de tiempo a la vez.

1. (Opcional) Haga clic en **Pantalla completa** icono ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) para mostrar el Planificador de recursos en modo de pantalla completa.

1. Actualice el **BDG** (Horas presupuestadas) con valores de hora, ETC o costo para los usuarios, los roles o el proyecto, mediante una de las siguientes acciones:

   * Calcule manualmente la cantidad de horas, los valores de ETC o de costo para los roles, los usuarios o el proyecto.

      O

   * Haga clic en **Opciones** para el proyecto o los roles y seleccione una opción para presupuestar automáticamente las horas de los roles, usuarios o el proyecto.
   Para obtener más información sobre la presupuestación en la vista de proyecto del Planificador de recursos, consulte [Presupuestar recursos en el Planificador de recursos utilizando las vistas Proyecto y Rol](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Puede presupuestar horas, ETC o costos para sus recursos para cualquier lapso de tiempo mostrado en el área de Presupuestación de recursos, independientemente de la cronología del proyecto. Por ejemplo, si desea indicar que los recursos podrían no estar disponibles durante la escala de tiempo del proyecto (cuando estén asociados con horas planificadas), pero podrían estar disponibles durante otro período, puede presupuestarlos para períodos de tiempo en los que las horas planificadas sean cero, si es entonces cuando estarán disponibles para trabajar.

1. (Opcional) Para saber si puede mover las horas presupuestadas, los jornadas completas o los costos a otro lapso de tiempo, haga clic en **Opciones** icono, luego **Ajustar fechas de presupuesto**.

   Para obtener más información sobre el ajuste de fechas presupuestadas, consulte [Ajustar fechas de presupuesto en el Planificador de recursos](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Haga clic en **Guardar**.

   Si tiene tasas de costo por hora asociadas con sus roles, al presupuestar los recursos en el área de Presupuestación de recursos se calcula el **Costo laboral presupuestado** del proyecto. El costo de mano de obra presupuestado se muestra en el área Presupuestación de recursos del caso comercial y en el Resumen del caso comercial.

   >[!TIP]
   El coste se muestra en el caso comercial en la moneda del proyecto.

   La información de presupuesto especificada en el caso comercial también se muestra en el Planificador de recursos.

   Al copiar un proyecto, tiene la opción de copiar también las horas presupuestadas en el nuevo proyecto. Solo se copian las horas presupuestadas en el Planificador de recursos. Para obtener más información, consulte [Copiar un proyecto](../manage-projects/copy-project.md).
