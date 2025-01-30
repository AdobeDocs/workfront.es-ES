---
navigation-topic: business-case-and-scorecards
title: Presupuestar recursos en el caso comercial utilizando el Planificador de recursos
description: Como parte de la planificación de recursos, puede utilizar el Planificador de recursos en el nivel de proyecto para presupuestar los roles de trabajo necesarios para completar el trabajo en un proyecto al crear el caso empresarial.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 16%

---

# Presupuestar recursos en el caso comercial utilizando el Planificador de recursos

<!--Audited: 01/2025-->

Como parte de la planificación de recursos, puede utilizar el Planificador de recursos en el nivel de proyecto para presupuestar los roles de trabajo necesarios para completar el trabajo en un proyecto al crear el caso empresarial.

Para obtener más información sobre cómo crear un caso empresarial, vea [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>La información introducida en el Planificador de recursos de nivel de proyecto también se puede ver en el Planificador de recursos de nivel de sistema. Lo contrario también es cierto. Para obtener información sobre el Planificador de recursos, consulte [Información general sobre el Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

También puede presupuestar recursos en el caso empresarial mediante Adobe Workfront Scenario Planner. Para obtener más información, consulte [Recursos de presupuesto en el caso empresarial con el planificador de escenarios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Requisitos de acceso

Para realizar los pasos de este artículo, debe tener lo siguiente:

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Prime o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: Light o superior</p>
   <p>Actual: revisión o superior</p>

<p><b>IMPORTANTE:</b></p> 
   <p>Nuevo: Debe tener una licencia estándar para modificar la información de presupuesto de recursos. </p> 
   <p>Actual: Debe tener una licencia de planificación para modificar la información de presupuesto de recursos. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a los siguientes elementos: </p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Datos financieros</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar, debe hacer lo siguiente:

* Cumpla todos los requisitos previos para la planificación de recursos en Adobe Workfront. Para obtener más información, consulte [Resumen del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Asociar conjuntos de recursos al proyecto.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >No puede presupuestar recursos asignados a problemas en el caso comercial. Puede presupuestarlos en el Planificador de recursos del sistema. Para obtener más información sobre el Planificador de recursos, consulte [Información general del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Aunque no se trata de un requisito previo, también le recomendamos que indique las horas planificadas para las tareas del proyecto. Esto le ayuda a comprender la cantidad de trabajo que una tarea puede necesitar para completarse, lo que le ayuda a tomar la decisión de cuánto tiempo se deben presupuestar los recursos para completar la tarea. Para obtener información sobre cómo asociar tareas con horas planificadas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Aplicar conjuntos de recursos a un proyecto y presupuestar recursos en el caso comercial

>[!IMPORTANT]
>
>Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información de presupuestación no sea precisa.

Para aplicar conjuntos de recursos y presupuestar recursos de proyecto en el caso comercial de un proyecto sin conjunto de recursos:

1. Vaya al proyecto para el que desea presupuestar recursos.
1. Haga clic en **Caso empresarial** en el panel de la izquierda.
1. (Condicional) Si su compañía no tiene una licencia para el Planificador de escenarios de Workfront, haga clic en **Editar presupuesto de recursos** en la sección **Presupuesto de recursos** y, a continuación, continúe con el paso 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Opcional y condicional) Si la información del proyecto se ha publicado a partir de una iniciativa en el Scenario Planner, realice una de las siguientes acciones:

   * Seleccione Planificador de recursos en el campo **Elija qué horas usar para calcular el costo de mano de obra presupuestado del proyecto** y luego haga clic en **Elegir > Editar presupuesto de recursos**.

     ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Si se seleccionó el Planificador de escenarios para presupuestar recursos para el proyecto, haga clic en **Cambiar** > **Editar presupuesto de recursos**.

     ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   Utiliza las horas presupuestadas del proyecto para calcular el costo de mano de obra presupuestado del proyecto.

   El Planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener más información sobre el Planificador de escenarios de Workfront, consulte [Información general sobre el Planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   >
   >Le recomendamos que tome la decisión de usar el Planificador de recursos o el Planificador de escenarios cuando empiece a trabajar en un proyecto. Cambiar con frecuencia entre los dos durante la duración del proyecto puede crear incoherencias en la forma de presupuestar los recursos del proyecto.

1. En el campo **Seleccionar conjunto de recursos**, especifique uno o varios **conjuntos de recursos**.

   Debe especificar únicamente conjuntos de recursos que se rellenen con usuarios activos.

   >[!TIP]
   >
   >Si el proyecto ya está asociado a conjuntos de recursos, el Planificador de recursos se muestra de forma predeterminada. Para agregar más conjuntos de recursos al proyecto, edite el proyecto. Para obtener información sobre cómo editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Haga clic en **Aplicar**.

   Se muestra el Planificador de recursos para el proyecto seleccionado.

   De forma predeterminada, las 20 primeras funciones del puesto asociadas a este proyecto se enumeran en la sección Presupuestación de recursos en orden alfabético. 

   Para obtener más información sobre el Planificador de recursos, consulte [Información general del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![área_de_presupuestación_de_recursos_BC.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Opcional y condicional) Expanda las funciones del puesto para ver los usuarios asociados a ellas.

   >[!NOTE]
   >
   >Los usuarios activos se muestran en los roles asociados a ellos solo si cumplen los siguientes criterios:
   >
   >   
   >   
   >   * Pertenecen a uno de los conjuntos de recursos del proyecto.
   >   * Tienen horas presupuestadas asignadas a ellos.
   >   * Están asociados a uno de los roles del proyecto.
   >   
   >

    

1. Haga clic en **Hoy** para regresar al lapso de tiempo de hoy.
1. (Opcional) Haga clic en **Semana**, **Mes** o **Trimestre** para mostrar información del proyecto en diferentes lapsos de tiempo.
1. (Opcional) Haga clic en el menú desplegable **Horas** y seleccione **Horas**,**ETC** o **Costo** para cambiar la forma en que se muestra la información en el Planificador de recursos. Las horas se muestran de forma predeterminada.

1. (Opcional) Haga clic en **Exportar** para exportar el Planificador de recursos a un archivo de Excel.

   >[!NOTE]
   >
   >Puede exportar datos de hasta 12 períodos de tiempo a la vez.

1. (Opcional) Haga clic en el icono **Pantalla completa** ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) para mostrar el Planificador de recursos en modo de pantalla completa.

1. Actualice el campo **BDG** (Horas presupuestadas) con valores de hora, ETC o costo para los usuarios, roles o el proyecto mediante uno de los procedimientos siguientes:

   * Calcule manualmente la cantidad de horas, los valores de ETC o de costo para los roles, los usuarios o el proyecto.

     O

   * Haga clic en el icono **Opciones** del proyecto o de los roles y seleccione una opción para presupuestar automáticamente las horas de los roles, los usuarios o el proyecto.

   Para obtener más información acerca de cómo presupuestar en la vista de proyecto del Planificador de recursos, consulte [Presupuesto de recursos en el Planificador de recursos mediante las vistas de proyecto y rol](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   >
   >Puede presupuestar horas, ETC o costos para sus recursos para cualquier lapso de tiempo mostrado en el área de Presupuestación de recursos, independientemente de la cronología del proyecto. Por ejemplo, si desea indicar que los recursos podrían no estar disponibles durante la escala de tiempo del proyecto (cuando estén asociados con horas planificadas), pero podrían estar disponibles durante otro período, puede presupuestarlos para períodos de tiempo en los que las horas planificadas sean cero, si es entonces cuando estarán disponibles para trabajar.

1. (Opcional) Para saber si puede mover las horas, los jornadas completas o los costos presupuestados a otro lapso de tiempo, haga clic en el icono **Opciones** y después en **Ajustar fechas de presupuesto**.

   Para obtener más información acerca del ajuste de fechas presupuestadas, vea [Ajustar fechas de presupuesto en el Planificador de recursos](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Haga clic en **Guardar**.

   Si tiene tasas de costo por hora asociadas con sus roles, al presupuestar los recursos en el área de Presupuestación de recursos se calcula el **Costo de mano de obra presupuestado** del proyecto. El costo de mano de obra presupuestado se muestra en el área Presupuestación de recursos del caso comercial y en el Resumen del caso comercial.

   >[!TIP]
   >
   >El coste se muestra en el caso comercial en la moneda del proyecto.

   La información de presupuesto especificada en el caso comercial también se muestra en el Planificador de recursos.

   Al copiar un proyecto, tiene la opción de copiar también las horas presupuestadas en el nuevo proyecto. Solo se copian las horas presupuestadas en el Planificador de recursos. Para obtener más información, consulte [Copiar un proyecto](../manage-projects/copy-project.md).
