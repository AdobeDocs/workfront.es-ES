---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Descripción general de las áreas del caso empresarial
description: Este artículo describe las áreas del caso empresarial de un proyecto.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 2%

---

# Descripción general de las áreas del caso empresarial

Este artículo describe las áreas del caso empresarial de un proyecto.

Para obtener información sobre cómo crear un caso empresarial para un proyecto, vea [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Adobe Workfront o del grupo debe habilitar todas las secciones del caso empresarial para que sean visibles en el proyecto, excepto la sección Información del proyecto. La sección Información del proyecto está habilitada de forma predeterminada.

Para obtener más información sobre cómo habilitar las áreas del caso empresarial, consulte la sección &quot;Casos comerciales&quot; en  [Configurar preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Las siguientes son áreas del caso empresarial de un proyecto:

* Información del proyecto
* Metas
* Gastos
* Presupuestación de recursos
* Riesgos
* Tarjeta de puntuación
* Formularios personalizados
* Resumen de caso comercial

## Información del proyecto

El administrador de Workfront no puede configurar el área **Información del proyecto** del caso empresarial. Todos los proyectos tienen un área de Información del proyecto en el Caso comercial. 

La sección Información del proyecto del caso empresarial incluye la información básica de un proyecto antes de que el proyecto se haya iniciado.

Considere la posibilidad de editar los campos siguientes:

* **Descripción**: especifica una descripción para el proyecto.
* **Propietario del proyecto**

  De forma predeterminada, el usuario que crea el proyecto también es el Propietario del proyecto. Puede editar este campo e indicar otro usuario activo como propietario del proyecto.

* **Patrocinador del proyecto**

  Considere la posibilidad de agregar a alguien más que no sea el Propietario del proyecto como patrocinador del proyecto. El patrocinador recibe la aprobación del caso empresarial. 

* **Portfolio**: especifique un Portfolio para el proyecto. Debe crear el Portfolio y colocarlo en el estado **Activo** antes de que esté disponible para seleccionarlo en este menú desplegable.

  Para obtener más información sobre portafolios, consulte [descripción general del Portfolio en Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Para obtener más información sobre cómo crear Portfolio, consulte [Crear un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Beneficio planificado**: Calcule el beneficio monetario planificado para su organización cuando se complete este proyecto. Puede ser cualquier cantidad de moneda y debe ser un valor positivo. Por ejemplo, 10 000 $.
* **Estado**: De forma predeterminada, el estado de una solicitud de proyecto se establece en **Idea**.

  Si cambia el estado a cualquier otra cosa que no sea Idea o Planificación, el botón **Enviar** desaparece del área Resumen de caso comercial y ya no puede enviar el caso comercial para su aprobación. 

* **Fecha fija de inicio**: especifique una fecha en la que desee que comience el proyecto.
* **Fecha de finalización fija**: especifique una fecha en la que desee que finalice el proyecto.

  >[!NOTE]
  >
  >Las fechas de inicio y finalización fijas en el caso empresarial no afectan a las fechas de inicio y finalización planificadas del proyecto. Representan las fechas solicitadas por el creador del proyecto para el momento en que el proyecto se desarrollaría de forma ideal. En su lugar, las Fechas planificadas de inicio y finalización planificada del proyecto muestran la cronología planificada para el proyecto, que se basa en las tareas del proyecto.

## Metas

Los objetivos definen los objetivos del proyecto. Esta área está habilitada de forma predeterminada en el caso empresarial, pero el administrador de Workfront puede optar por no mostrarla. Este campo muestra los objetivos en orden de prioridad.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Puede crear objetivos estratégicos para su organización que no estén conectados al caso empresarial individual de un proyecto. Debe tener acceso a las metas de Adobe Workfront para poder crear metas estratégicas. A continuación, puede conectarlos con proyectos fuera de sus casos comerciales. Para obtener información sobre cómo crear metas con Workfront Goals, consulta [Información general sobre Adobe Workfront Goals](../../../workfront-goals/goal-management/wf-goals-overview.md).

Definir los objetivos es opcional para que el proyecto reciba una puntuación en Portfolio Optimizer. Esta sección es la única sección opcional del caso empresarial. Todas las demás secciones del caso empresarial deben completarse antes de que el proyecto se clasifique en Portfolio Optimizer. Puede indicar un nivel de prioridad para una meta a medida que la crea.

Para obtener más información sobre los objetivos, consulte  [Crear metas de caso empresarial](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Gastos

Los gastos representan los costos no laborales en los que se podría incurrir durante la duración de un proyecto. Esta área está habilitada de forma predeterminada en el caso empresarial, pero el administrador de Workfront puede optar por no mostrarla. 

Los gastos que especifique en el caso comercial también se especifican en la pestaña Gastos del proyecto, como Gastos planificados.

Los gastos afectan a los siguientes campos del proyecto:

* Costo presupuestado
* Valor neto

Para obtener más información sobre los costos presupuestados y los valores netos, consulte [Información general sobre los campos financieros de caso empresarial](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obtener más información sobre los gastos, consulte  [Administrar gastos de proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md)

El administrador de Workfront puede configurar tipos de gastos personalizados.

Para obtener más información sobre cómo crear tipos de gastos personalizados, consulte [Crear tipos de gastos personalizados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Presupuestación de recursos

Puede realizar las siguientes acciones en el área de Presupuestación de recursos del caso empresarial:

* Asocie conjuntos de recursos al proyecto.
* Presupuestar los recursos en el nivel de proyecto.

Las horas presupuestadas para los recursos del proyecto se muestran en el área de Presupuestación de recursos del caso empresarial y generan el costo de mano de obra presupuestado del proyecto. Esta área del caso empresarial está habilitada de forma predeterminada.

Para obtener más información acerca de cómo presupuestar recursos para el proyecto en el caso comercial, vea [Presupuesto de recursos en el caso comercial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Tenga en cuenta lo siguiente al ver la sección Presupuestación de recursos del caso empresarial:

* Puede presupuestar la información de recursos aquí con las siguientes herramientas:

   * El Planificador de recursos

     Para obtener más información, consulte [Recursos de presupuesto en el caso comercial con el Planificador de recursos](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * El Scenario Planner , si su empresa ha adquirido una licencia adicional para Adobe Scenario Planner

     Para obtener más información, consulte [Recursos presupuestarios en el caso comercial con Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general sobre el Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

* La información mostrada aquí también se muestra en el Planificador de recursos o el Planificador de escenarios a nivel del sistema. 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Después de presupuestar los recursos, el costo de mano de obra presupuestado del proyecto se muestra en el área de Presupuestación de recursos si los roles están asociados con tasas de costo por hora. El costo de mano de obra presupuestado se muestra en la moneda del proyecto.

  >[!IMPORTANT]
  >
  >El costo de mano de obra presupuestado es el costo asociado con los roles del proyecto y no con los usuarios. La suma de todos los costes laborales presupuestados para los usuarios puede ser igual o no al coste laboral presupuestado de la función asociada con los usuarios. 

  Para obtener más información sobre el costo de mano de obra presupuestado, vea [Información general sobre los campos financieros del caso empresarial](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Para obtener más información sobre cómo crear roles de trabajo y asociar tarifas de costo por hora con ellos, consulte [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Riesgos

Los riesgos son factores que pueden impedir que un proyecto finalice a tiempo o según el presupuesto. Definir estos factores es importante para que el Portfolio gerente o el patrocinador del proyecto tomen una decisión informada sobre la aprobación del proyecto. Esta área está habilitada de forma predeterminada en el caso empresarial, pero el administrador de Workfront puede optar por no mostrarla.

Puede asociar un coste potencial con los riesgos que está definiendo en caso de que se produzcan. El coste de los riesgos de un proyecto afecta al valor neto del proyecto. 

Para obtener más información sobre el valor neto del proyecto, consulte [Información general sobre los campos financieros de caso empresarial](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obtener más información sobre la creación de riesgos, consulte  [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

El administrador de Workfront puede configurar tipos de riesgos personalizados.

Para obtener más información acerca de cómo crear y editar tipos de riesgos personalizados, vea [Editar y crear tipos de riesgos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Tarjeta de puntuación

Los informes de valoración miden la alineación del proyecto. Esta área está habilitada de forma predeterminada en el caso empresarial, pero el administrador de Workfront puede optar por no mostrarla.

Para obtener más información sobre cómo aplicar un cuadro de mandos a un proyecto y generar una puntuación de alineación, vea [Aplicar un cuadro de mandos a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para aplicar un informe de valoración, el administrador de Workfront debe crear uno. El área **informe de valoración** del caso empresarial no se muestra a menos que se cree un informe de valoración.

Para obtener más información sobre la creación de un cuadro de mandos, consulte  [Crear un cuadro de mandos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Formularios personalizados

Puede adjuntar Forms personalizado a un proyecto al definir un caso empresarial. Esta área no está habilitada de manera predeterminada en el caso comercial. El administrador de Workfront debe habilitarlo para mostrarlo en el caso comercial.

Para obtener más información sobre cómo habilitar las áreas del caso empresarial, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar un formulario personalizado, el administrador de Workfront debe crear primero un formulario personalizado.

Para obtener más información sobre cómo crear un formulario personalizado, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

Puede utilizar formularios personalizados para recopilar información adicional que no se muestre en los demás campos del caso empresarial.

Para obtener más información acerca de cómo aplicar un formulario personalizado, vea [Adjuntar un formulario personalizado a un caso empresarial](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Resumen de caso comercial

* [Resumen del caso empresarial](#overview-of-the-business-case-summary)
* [Exportar el caso comercial](#export-the-business-case)

### Descripción general del resumen del caso empresarial {#overview-of-the-business-case-summary}

Puede ver un resumen de las finanzas principales del proyecto y si un proyecto está alineado o no con un informe de valoración en el panel Resumen de caso empresarial, en la esquina superior derecha del caso empresarial

No puede editar el Resumen de caso comercial. Esta es solo una vista rápida del estado del proyecto en relación con los campos financieros y el informe de valoración. \
 

Los siguientes campos se muestran en el Resumen de caso comercial:

* El valor neto del proyecto
* Costo presupuestado del proyecto
* El costo de riesgo potencial
* El Beneficio Planificado
* La puntuación de alineación

Para obtener más información sobre estos campos, consulte [Información general sobre los campos financieros de caso empresarial](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Exportar el caso comercial {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Puede exportar el caso empresarial a un archivo de PDF, en caso de que necesite imprimirlo o adjuntarlo a un mensaje de correo electrónico en un formato más conciso. 

Para obtener más información, vea [Exportar el caso comercial de un proyecto](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
