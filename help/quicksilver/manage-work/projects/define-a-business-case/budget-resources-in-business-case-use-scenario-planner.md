---
navigation-topic: business-case-and-scorecards
title: Recursos de presupuesto en el caso empresarial con el planificador de escenarios
description: Como parte de la planificación de recursos, puede utilizar el Planificador de escenario de Adobe Workfront para presupuestar las funciones de trabajo necesarias para completar el trabajo en un proyecto al crear el caso empresarial.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Recursos de presupuesto en el caso empresarial con el planificador de escenarios

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Como parte de la planificación de recursos, puede utilizar el Planificador de escenario de Adobe Workfront para presupuestar las funciones de trabajo necesarias para completar el trabajo en un proyecto al crear el caso empresarial.

Para obtener más información sobre cómo crear un caso empresarial, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>La información de la función de trabajo de la iniciativa vinculada al proyecto que se introduce en el Planificador de escenario de nivel de sistema se puede ver en el área de Presupuestación de recursos del caso empresarial del proyecto al publicar la iniciativa. El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

También puede presupuestar recursos en el caso empresarial utilizando el planificador de recursos. Para obtener más información, consulte lo siguiente:

* [Recursos presupuestarios en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Le recomendamos que tome la decisión de usar el Planificador de recursos o el Planificador de escenario cuando empiece a trabajar en un proyecto. A menudo, el cambio entre los dos durante la vida del proyecto puede crear incoherencias en la forma en que se presupuestan los recursos para el proyecto.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Negocios o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para el planificador de escenarios de Adobe Workfront para acceder a las funciones que se describen en este artículo.</p> <p>Para obtener información sobre cómo obtener el planificador de escenarios de Workfront, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar el planificador de escenarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente: </p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Datos financieros</p> </li> 
     <li> <p>Planificador de escenarios </p> </li> 
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

* Cree un plan con el planificador de escenarios.

   Para obtener más información, consulte [Crear y editar planes en el planificador de escenarios](../../../scenario-planner/create-and-edit-plans.md).

* Cree una iniciativa sobre el plan y vincúlela a un proyecto.

   Asegúrese de indicar la información de funciones de trabajo necesaria para la iniciativa y actualizar el proyecto vinculado con esta información.

   Para obtener más información, consulte los siguientes artículos:

   * [Crear y editar iniciativas en el planificador de escenarios](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importar proyectos a planes en el planificador de escenarios](../../../scenario-planner/import-projects-to-plans.md)
   * [Actualizar o crear proyectos publicando iniciativas en el Planificador de escenarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Aunque no son requisitos previos, también se recomienda lo siguiente:

   * Asigne tareas del proyecto a las funciones de trabajo presupuestadas en el Planificador de escenario.
   * Indique el número de horas planificadas para las tareas del proyecto.

      Esto le ayuda a comprender la cantidad de trabajo que una tarea podría necesitar completar, lo que le ayuda a decidir cuánto tiempo se deben presupuestar los recursos para completar la tarea.

      Para obtener información sobre cómo asociar tareas con horas planificadas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Recursos presupuestarios en el caso empresarial utilizando el planificador de escenario para proyectos vinculados a iniciativas

>[!IMPORTANT]
Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información del presupuesto no sea precisa.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Vaya al proyecto cuyos recursos desea presupuestar.

   >[!TIP]
   Se trata de un proyecto vinculado a una iniciativa del Planificador de escenario cuya iniciativa vinculada se haya publicado al menos una vez.

1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. (Condicional) En el **Presupuestación de recursos** , realice una de las siguientes acciones:

   * Si acaba de publicar información del Planificador de escenario, seleccione Planificador de escenario en la **Elija qué horas utilizar para calcular el costo laboral presupuestado del proyecto** en el área Presupuestación de recursos y, a continuación, haga clic en **Choose**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Si el Planificador de recursos se seleccionó anteriormente para presupuestar recursos para el proyecto, haga clic en **Cambiar** > **Planificador de escenario** > **Choose**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront utiliza las horas de función de trabajo necesarias de la iniciativa vinculada para calcular el costo laboral presupuestado y las horas presupuestadas del proyecto. Esta es la opción recomendada. El coste se muestra en el caso empresarial en la moneda del proyecto.

      <!--drafted for Budgeted Hours:
   <span class="preview">Cuando copia un proyecto y selecciona copiar las horas presupuestadas en el nuevo proyecto, las horas presupuestadas con el planificador de escenario no se copian en el nuevo proyecto. Solo se copian las horas presupuestadas en el Planificador de recursos. Para obtener más información, consulte [Copiar un proyecto](../manage-projects/copy-project.md)</span>
—>

   >[!IMPORTANT]
   Cuando se utiliza el Planificador de escenario para presupuestar recursos para el proyecto, el Coste de trabajo presupuestado se muestra en las siguientes áreas de Workfront:
   * Área de presupuestación de recursos del caso empresarial
   * El planificador de escenario a nivel de sistema como el coste personal de la iniciativa vinculada al proyecto. Para obtener más información, consulte [Crear y editar iniciativas en el planificador de escenarios](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Opcional) Haga clic en **Ver en el planificador de escenarios** para abrir el plan que contiene la iniciativa vinculada al proyecto. Se abre el Planificador de escenario en una nueva ficha del explorador.
1. (Opcional) Actualice la información sobre la iniciativa. Para obtener más información, consulte [Crear y editar iniciativas en el planificador de escenarios](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   Debe publicar la iniciativa después de cada cambio en el área de Presupuestación de recursos del proyecto para actualizarla.
