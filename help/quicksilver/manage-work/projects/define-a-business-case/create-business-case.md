---
navigation-topic: business-case-and-scorecards
title: Creación de un caso empresarial para un proyecto
description: Puede utilizar el caso empresarial para solicitar un proyecto y definir el propósito, el presupuesto y el beneficio potencial del proyecto. El administrador de Portafolios o el patrocinador del proyecto utilizan la información del caso empresarial para analizar y priorizar el proyecto antes de aprobarlo.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 68%

---

# Creación de un caso empresarial para un proyecto

Puede utilizar el caso empresarial para solicitar un proyecto y definir el propósito, el presupuesto y el beneficio potencial del proyecto. El administrador de Portafolios o el patrocinador del proyecto utilizan la información del caso empresarial para analizar y priorizar el proyecto antes de aprobarlo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Proyectos, Datos financieros y Administración de recursos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos superiores en el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Tenga en cuenta lo siguiente al solicitar un proyecto a través de un caso empresarial:

* El administrador de Adobe Workfront o del administrador de grupos debe habilitar las secciones del caso empresarial para que aparezcan en el proyecto.\
  Para obtener información acerca de cómo habilitar las secciones del caso empresarial en el sistema, consulte el artículo [Configurar las preferencias del proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Para obtener información acerca de las áreas del caso empresarial, vea el artículo [Información general de las áreas del caso empresarial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Debe completar todas las áreas del caso empresarial, excepto el área de metas, si desea que el proyecto reciba una puntuación en el Optimizador de portafolios. Completar el área de Metas es opcional. El proyecto recibe una puntuación en el Optimizador de portafolios aunque esta área no esté completada.

  Para obtener información sobre cómo trabajar con cuadros de resultados y con el Optimizador de portafolios, consulte el artículo [Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Creación de un caso empresarial

{{step1-to-projects}}

1. Click **New Project**, then select **Request Project** from the drop-down that appears. The project is created and the **Idea** status is assigned by default.

   >[!CAUTION]
   >
   >Si el estado de Idea se ha eliminado en la instancia de Workfront, el proyecto se coloca en el estado predeterminado para nuevos proyectos, tal como se define en el área Preferencias del proyecto. Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias del proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Enter a name in the project title field.
1. (Optional) Click the **More** icon ![More icon](assets/qs-more-icon-on-an-object.png), then **Attach Template** to create the Work Breakdown Structure of your project.

   O

   Empiece a añadir tareas al proyecto manualmente.

1. (Conditional) If you selected to attach a template, continue attaching the template to the project.
1. In the left panel, click **Business Case**.
1. (Optional) To edit the **Project Info** section, click **Edit Project Info**. 

   For more information about editing the **Project Info** section fields, see the section [Project Info](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) To edit the **Goals** section, click **Edit Goals**.

   For more information about editing the **Goals** section of the Business Case, see the section [Goals](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) To edit the **Expenses** section, click **Edit Expenses**.

   For more information about editing the **Expenses** section of the Business Case, see the section [Expenses](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Click **Edit Resource Budgeting** to budget your resources and obtain the Budgeted Labor Cost associated with the job roles on the project. Para obtener más información, consulte [Recursos de presupuesto en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >La información que se muestra aquí es la misma que la que aparece en las herramientas de presupuestación de recursos en el sistema.

1. (Opcional) Haga clic en **Editar riesgos** para añadir posibles riesgos a este proyecto. Para obtener información acerca de cómo añadir riesgos al caso empresarial, vea la sección [Riesgos](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) en el artículo [Información general sobre las áreas del caso empresarial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Optional) Select a **Scorecard** in the **Add a Scorecard to this Project** drop-down menu.

   Se deben crear cuadros de resultados para poder adjuntarlos a los proyectos.

   Para obtener más información sobre los cuadros de resultados, vea el artículo [Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Opcional) Seleccione un **Formulario personalizado** en el menú desplegable **Formularios personalizados**.

   Se deben crear formularios personalizados para poder adjuntarlos a los proyectos.

   For more information about Custom Forms, see the article [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click **Submit**. El estado del proyecto se cambió a **Solicitado** y se envía para que se apruebe el caso empresarial.

   Para obtener más información acerca de cómo aprobar un caso empresarial, vea el artículo [Aprobar un caso empresarial](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> After completing the Business Case, you can export a copy of it to a .pdf file. For more information about exporting the Business Case to a .pdf file, see [Export the Business Case of a project](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


