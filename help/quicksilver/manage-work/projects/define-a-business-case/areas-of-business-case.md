---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Información general sobre las áreas del caso empresarial
description: Este artículo describe las áreas del Caso de negocio de un proyecto.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# Información general sobre las áreas del caso empresarial

Este artículo describe las áreas del Caso de negocio de un proyecto.

Para obtener información sobre cómo crear un caso práctico para un proyecto, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Adobe Workfront o el administrador de grupos deben habilitar todas las secciones del caso empresarial antes de que estén visibles en el proyecto, excepto en la sección Información del proyecto . La sección Información del proyecto está activada de forma predeterminada.

Para obtener más información sobre cómo habilitar las áreas del Caso empresarial, consulte la sección &quot;Casos de negocio&quot; en  [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Las siguientes son las áreas del caso empresarial de un proyecto:

* Información del proyecto
* Metas
* Gastos
* Presupuestación de recursos
* Riesgos
* Tarjeta de puntuación
* Formularios personalizados
* Resumen de caso comercial

## Información del proyecto

La variable **Información del proyecto** El administrador de Workfront no puede configurar el área del caso empresarial. Todos los proyectos tienen un área Información del proyecto en el caso empresarial. 

La sección Información del proyecto del caso empresarial incluye la información básica de un proyecto antes de que este se haya iniciado.

Considere la posibilidad de editar los campos siguientes:

* **Descripción**: Especifique una descripción para el proyecto.
* **Propietario del proyecto**

   De forma predeterminada, el usuario que crea el proyecto también es el propietario del proyecto. Puede editar este campo e indicar otro usuario activo como propietario del proyecto.

* **Patrocinador de proyecto**

   Considere la posibilidad de agregar otra persona que no sea el propietario del proyecto como patrocinador del proyecto. El patrocinador recibe la aprobación del caso empresarial. 

* **Portfolio**: Especifique un Portfolio para el proyecto. Debe crear el Portfolio y colocarlo en el estado de **Activo** antes de que esté disponible para seleccionarlo en este menú desplegable.

   Para obtener más información sobre portafolios, consulte [Información general del Portfolio en Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   Para obtener más información sobre la creación de Portfolio, consulte [Crear un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Beneficio planificado**: Calcule cuál es el beneficio monetario que se planea obtener para su organización cuando se complete este proyecto. Puede ser cualquier cantidad de moneda y debe ser un valor positivo. Por ejemplo, 10 000 $.
* **Estado**: De forma predeterminada, el estado de una solicitud de proyecto está establecido en **Idea**.

   Si cambia el estado a cualquier cosa que no sea Idea o Planificación, la variable **Submit** desaparece del área Resumen de casos empresariales y ya no puede enviar el caso empresarial para su aprobación. 

* **Fecha de inicio fija**: Especifique una fecha en la que desee que comience el proyecto.
* **Fecha final fija**: Especifique una fecha en la que desee que finalice el proyecto.

   >[!NOTE]
   >
   >Las fechas de inicio y finalización fijas del caso empresarial no afectan a las fechas de inicio y finalización planificadas del proyecto. Representan las fechas solicitadas por el creador del proyecto para saber cuándo se desarrollaría idealmente el proyecto. En su lugar, las fechas de inicio y finalización planificadas del proyecto muestran el calendario planificado para el proyecto, que se basa en las tareas del proyecto.

## Metas

Los objetivos definen los objetivos del proyecto. Esta área está habilitada de forma predeterminada en el caso de uso, pero es posible que el administrador de Workfront decida no mostrarla. Este campo muestra los objetivos en orden de prioridad.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
Puede crear objetivos estratégicos para su organización que no estén conectados al caso empresarial individual de un proyecto. Debe tener acceso a los objetivos de Adobe Workfront para poder crear objetivos estratégicos. A continuación, puede conectarlos con proyectos fuera de sus Casos de negocio. Para obtener información sobre la creación de objetivos con los objetivos de Workfront, consulte [Información general sobre los objetivos de Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

La definición de los objetivos es opcional para que el proyecto reciba una puntuación en el Optimizador de Portfolio. Esta sección es la única sección opcional del caso empresarial. Todas las demás secciones del caso empresarial deben completarse antes de que el proyecto se clasifique en el optimizador de Portfolio. Puede indicar un nivel de prioridad para un objetivo a medida que lo crea.

Para obtener más información sobre los objetivos, consulte  [Crear objetivos de caso empresarial](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Gastos

Los gastos representan los costos no laborales que podrían incurrir durante la vida de un proyecto. Esta área está habilitada de forma predeterminada en el caso de uso, pero es posible que el administrador de Workfront decida no mostrarla. 

Los gastos que introduzca en el caso de negocio también se introducen en la pestaña Gastos del proyecto, como Gastos planificados.

Los gastos afectan a los siguientes campos del proyecto:

* Costo presupuestado
* Valor neto

Para obtener más información sobre los costos presupuestados y los valores netos, consulte [Información general sobre los campos financieros de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obtener más información sobre los gastos, consulte  [Administrar los gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

El administrador de Workfront puede configurar tipos de gastos personalizados.

Para obtener más información sobre la creación de tipos de gastos personalizados, consulte [Crear tipos de gastos personalizados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Presupuestación de recursos

Puede realizar las siguientes acciones en el área Presupuestación de recursos del caso empresarial:

* Asocie grupos de recursos al proyecto.
* Asigne un presupuesto a los recursos en el nivel de proyecto.

Las horas presupuestadas para los recursos del proyecto se muestran en el área de Presupuesto de Recursos del Caso de Negocio, lo que genera el costo de trabajo presupuestado del proyecto. Esta área del caso empresarial está habilitada de forma predeterminada.

Para obtener más información sobre la presupuestación de recursos para el proyecto en el caso práctico, consulte [Recursos presupuestarios en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Tenga en cuenta lo siguiente al ver la sección Presupuestación de recursos del caso empresarial:

* Puede presupuestar la información de recursos aquí mediante las siguientes herramientas:

   * El planificador de recursos

      Para obtener más información, consulte [Recursos presupuestarios en el caso empresarial utilizando el planificador de recursos](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Planificador de escenario , si su empresa ha adquirido una licencia adicional para el planificador de escenario de Adobe

      Para obtener más información, consulte [Recursos de presupuesto en el caso empresarial con el planificador de escenarios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

* La información mostrada aquí también se muestra en el Planificador de recursos o en el Planificador de escenario a nivel de sistema. 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Después de presupuestar los recursos, el Coste de trabajo presupuestado del proyecto se muestra en el área Presupuestación de recursos si las funciones están asociadas con las tasas de Coste por hora. El Coste de trabajo presupuestado se muestra en la moneda del proyecto.

   >[!IMPORTANT]
   El costo de trabajo presupuestado es el costo asociado con las funciones del proyecto, y no con los usuarios. La suma de todos los costes laborales presupuestados para los usuarios puede o no ser igual al coste laboral presupuestado del puesto de trabajo asociado a los usuarios. 

   Para obtener más información sobre el coste laboral presupuestado, consulte [Información general sobre los campos financieros de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   Para obtener más información sobre la creación de funciones de trabajo y la asociación de tasas de costo por hora con ellas, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Riesgos

Los riesgos son factores que podrían impedir que un proyecto termine a tiempo o con presupuesto. La definición de estos factores es importante para que el administrador de Portfolio o el patrocinador del proyecto tomen una decisión educada sobre la aprobación del proyecto. Esta área está habilitada de forma predeterminada en el caso de uso, pero es posible que el administrador de Workfront decida no mostrarla.

Puede asociar un coste potencial con los riesgos que está definiendo en caso de que se produzcan. El coste de los riesgos en un proyecto afecta al valor neto del proyecto. 

Para obtener más información sobre el valor neto del proyecto, consulte [Información general sobre los campos financieros de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obtener más información sobre la creación de riesgos, consulte  [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

El administrador de Workfront puede configurar tipos de riesgo personalizados.

Para obtener más información sobre la creación y edición de tipos de riesgo personalizados, consulte [Editar y crear tipos de riesgo](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Tarjeta de puntuación

Los informes de valoración miden la alineación del proyecto. Esta área está habilitada de forma predeterminada en el caso de uso, pero es posible que el administrador de Workfront decida no mostrarla.

Para obtener más información sobre la aplicación de un informe de valoración a un proyecto y la generación de una puntuación de alineación, consulte [Aplicar un informe de valoración a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para aplicar un informe de valoración, el administrador de Workfront debe crear uno. La variable **Informe de valoración** El área del caso empresarial no se muestra a menos que se cree un informe de valoración.

Para obtener más información sobre la creación de un informe de valoración, consulte  [Crear un informe de valoración](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Formularios personalizados

Puede adjuntar Forms personalizado a un proyecto al definir un caso empresarial. Esta área no está habilitada de forma predeterminada en el caso de uso. El administrador de Workfront debe habilitarlo para que se muestre en el caso empresarial.

Para obtener más información sobre cómo habilitar las áreas del caso empresarial, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar un formulario personalizado, el administrador de Workfront debe crear primero un formulario personalizado.

Para obtener más información sobre cómo crear un formulario personalizado, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

Puede utilizar formularios personalizados para recopilar información adicional que no se muestra en los demás campos del caso práctico.

Para obtener más información sobre la aplicación de un formulario personalizado, consulte [Adjuntar un formulario personalizado a un caso práctico](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Resumen de caso comercial

* [Resumen del caso empresarial](#overview-of-the-business-case-summary)
* [Exportar el caso empresarial](#export-the-business-case)

### Resumen del caso empresarial {#overview-of-the-business-case-summary}

Puede ver un resumen de las finanzas del proyecto principal y si un proyecto está alineado o no con un informe de valoración en el panel Resumen de casos empresariales , en la esquina superior derecha del caso empresarial .

No puede editar el resumen de casos empresariales. Esta es solo una vista rápida del estado del proyecto en relación con los campos financieros y el informe de valoración. \
 

Los campos siguientes se muestran en el resumen de caso empresarial:

* El valor neto del proyecto
* El costo presupuestado del proyecto
* El costo de riesgo potencial
* El beneficio planeado
* Puntuación de alineación

Para obtener más información sobre estos campos, consulte [Información general sobre los campos financieros de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Exportar el caso empresarial {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Puede exportar el caso empresarial a un archivo PDF, en caso de que necesite imprimirlo o adjuntarlo a un correo electrónico en un formato más conciso. 

Para obtener más información, consulte [Exportar el caso empresarial de un proyecto](../../../manage-work/projects/define-a-business-case/export-business-case.md).

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
