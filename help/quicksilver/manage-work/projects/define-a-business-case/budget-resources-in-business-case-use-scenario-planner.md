---
navigation-topic: business-case-and-scorecards
title: Presupuestar recursos en el caso empresarial con el Scenario Planner
description: Como parte de la planificación de recursos, puede utilizar el Planificador de escenarios de Adobe Workfront para presupuestar las funciones de trabajo necesarias para completar el trabajo en un proyecto al crear el caso empresarial.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Presupuestar recursos en el caso empresarial con el Scenario Planner

Como parte de la planificación de recursos, puede utilizar el Planificador de escenarios de Adobe Workfront para presupuestar las funciones de trabajo necesarias para completar el trabajo en un proyecto al crear el caso empresarial.

Para obtener más información sobre la creación de un caso empresarial, consulte [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>La información de función para la iniciativa vinculada al proyecto que introduzca en el planificador de escenarios a nivel de sistema se puede ver en el área de presupuesto de recursos del caso empresarial del proyecto cuando publica la iniciativa. El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general del Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

También puede presupuestar recursos en el caso comercial utilizando el Planificador de recursos. Para obtener más información, consulte lo siguiente:

* [Recursos de presupuesto en el caso comercial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Le recomendamos que tome la decisión de usar el Planificador de recursos o el Planificador de escenarios cuando empiece a trabajar en un proyecto. Cambiar con frecuencia entre los dos durante la duración del proyecto puede crear incoherencias en la forma de presupuestar los recursos del proyecto.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Empresa o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para el planificador de escenarios de Adobe Workfront a fin de acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre la obtención del Scenario Planner de Workfront, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar el Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente: </p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Datos financieros</p> </li> 
     <li> <p>Planificador de escenarios </p> </li> 
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

* Cree un plan con el Scenario Planner.

   Para obtener más información, consulte [Crear y editar planes en el Scenario Planner](../../../scenario-planner/create-and-edit-plans.md).

* Cree una iniciativa en el plan y vincúlela a un proyecto.

   Asegúrese de indicar la información de funciones del puesto necesaria para la iniciativa y actualizar el proyecto vinculado con esta información.

   Para obtener más información, consulte los siguientes artículos:

   * [Crear y editar iniciativas en el Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importar proyectos a planes en el Scenario Planner](../../../scenario-planner/import-projects-to-plans.md)
   * [Actualizar o crear proyectos publicando iniciativas en el Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

* Aunque estos no son requisitos previos, también recomendamos lo siguiente:

   * Asigne tareas en el proyecto a las funciones presupuestadas en el Scenario Planner.
   * Indique el número de horas planificadas para las tareas del proyecto.

      Esto le ayuda a comprender la cantidad de trabajo que una tarea puede necesitar para completarse, lo que le ayuda a decidir cuánto tiempo se deben presupuestar los recursos para completar la tarea.

      Para obtener información sobre cómo asociar tareas con horas planificadas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Presupuestar recursos en el caso empresarial utilizando el Scenario Planner para proyectos vinculados a iniciativas

>[!IMPORTANT]
Puede presupuestar sus recursos para un período de 15 años. Si se presupuestan recursos para un proyecto con una duración superior a 15 años, es posible que la información de presupuestación no sea precisa.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Vaya al proyecto para el que desea presupuestar recursos.

   >[!TIP]
   Este es un proyecto vinculado a una iniciativa del Scenario Planner cuya iniciativa vinculada se ha publicado al menos una vez.

1. Clic **Caso comercial** en el panel izquierdo.
1. (Condicional) En el **Presupuestación de recursos** , realice una de las siguientes acciones:

   * Si acaba de publicar información desde el Scenario Planner, seleccione Scenario Planner en la **Elija las horas que se utilizarán para calcular el costo de mano de obra presupuestado del proyecto** en el área Presupuestación de recursos y haga clic en **Elegir**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Si el Planificador de recursos se seleccionó anteriormente para presupuestar recursos para el proyecto, haga clic en **Cambiar** > **Planificador de escenarios** > **Elegir**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront utiliza las horas de función requeridas de la iniciativa vinculada para calcular el coste laboral presupuestado y las horas presupuestadas del proyecto. Esta es la opción recomendada. El coste se muestra en el caso comercial en la moneda del proyecto.

      Cuando copia un proyecto y selecciona copiar las horas presupuestadas en el nuevo proyecto, las horas presupuestadas mediante el Scenario Planner no se copian en el nuevo proyecto. Solo se copian las horas presupuestadas en el Planificador de recursos. Para obtener más información, consulte [Copiar un proyecto](../manage-projects/copy-project.md).

      >[!IMPORTANT]
      Cuando utiliza el Planificador de escenarios para presupuestar recursos para el proyecto, el Coste de mano de obra presupuestado se muestra en las siguientes áreas de Workfront:
      * Área de presupuesto de recursos del caso empresarial
      * El planificador de escenarios a nivel de sistema como coste de personas de la iniciativa vinculada al proyecto. Para obtener más información, consulte [Crear y editar iniciativas en el Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Opcional) Haga clic en **Ver en el planificador de escenarios** para abrir el plan que contiene la iniciativa vinculada al proyecto. Se abrirá el Scenario Planner en una nueva pestaña del explorador.
1. (Opcional) Actualice la información sobre la iniciativa. Para obtener más información, consulte [Crear y editar iniciativas en el Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   Debe publicar la iniciativa después de cada cambio para que se actualice el área de Presupuestación de recursos del proyecto.
